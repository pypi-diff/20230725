# Comparing `tmp/ai2_kit-0.5.0.tar.gz` & `tmp/ai2_kit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.5.0.tar", max compression
+gzip compressed data, was "ai2_kit-0.5.1.tar", max compression
```

## Comparing `ai2_kit-0.5.0.tar` & `ai2_kit-0.5.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.5.0/LICENSE
--rw-r--r--   0        0        0     2012 2023-07-21 03:28:16.683182 ai2_kit-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.0/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.5.0/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0      144 2023-06-15 02:12:13.145370 ai2_kit-0.5.0/ai2_kit/algorithm/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9573 2023-06-15 02:12:13.155370 ai2_kit-0.5.0/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc
--rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.5.0/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.0/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0      139 2023-02-14 03:43:41.260120 ai2_kit-0.5.0/ai2_kit/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2243 2023-07-20 03:31:49.016223 ai2_kit-0.5.0/ai2_kit/core/__pycache__/artifact.cpython-39.pyc
--rw-r--r--   0        0        0     5928 2023-07-20 03:31:48.996223 ai2_kit-0.5.0/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc
--rw-r--r--   0        0        0      512 2023-06-15 07:55:24.192005 ai2_kit-0.5.0/ai2_kit/core/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0     7307 2023-07-24 07:57:09.456574 ai2_kit-0.5.0/ai2_kit/core/__pycache__/connector.cpython-39.pyc
--rw-r--r--   0        0        0     9586 2023-07-24 09:28:27.095300 ai2_kit-0.5.0/ai2_kit/core/__pycache__/executor.cpython-39.pyc
--rw-r--r--   0        0        0      894 2023-06-29 05:30:14.695752 ai2_kit-0.5.0/ai2_kit/core/__pycache__/future.cpython-39.pyc
--rw-r--r--   0        0        0     2847 2023-07-20 03:31:48.996223 ai2_kit-0.5.0/ai2_kit/core/__pycache__/job.cpython-39.pyc
--rw-r--r--   0        0        0      436 2023-06-29 05:30:14.695752 ai2_kit-0.5.0/ai2_kit/core/__pycache__/log.cpython-39.pyc
--rw-r--r--   0        0        0    10069 2023-07-21 03:41:53.042985 ai2_kit-0.5.0/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc
--rw-r--r--   0        0        0     3063 2023-07-20 03:31:49.026223 ai2_kit-0.5.0/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc
--rw-r--r--   0        0        0     2611 2023-07-21 03:41:53.282985 ai2_kit-0.5.0/ai2_kit/core/__pycache__/script.cpython-39.pyc
--rw-r--r--   0        0        0     8116 2023-07-24 09:28:27.215300 ai2_kit-0.5.0/ai2_kit/core/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.5.0/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     5745 2023-07-10 01:27:05.779682 ai2_kit-0.5.0/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.5.0/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-07-21 04:37:23.322249 ai2_kit-0.5.0/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     8006 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/core/executor.py
--rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.5.0/ai2_kit/core/future.py
--rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.5.0/ai2_kit/core/job.py
--rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.5.0/ai2_kit/core/log.py
--rw-r--r--   0        0        0     9587 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.5.0/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2363 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/core/script.py
--rw-r--r--   0        0        0     5900 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.0/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0      110 2023-06-15 07:55:24.202005 ai2_kit-0.5.0/ai2_kit/dflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.0/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0      141 2023-02-14 03:43:41.670121 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4566 2023-07-24 09:28:27.615300 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/asap.cpython-39.pyc
--rw-r--r--   0        0        0     2517 2023-06-29 05:30:14.805753 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/cll.cpython-39.pyc
--rw-r--r--   0        0        0     3221 2023-02-23 07:10:20.489990 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/common.cpython-39.pyc
--rw-r--r--   0        0        0     1532 2023-07-24 09:28:27.285300 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/constant.cpython-39.pyc
--rw-r--r--   0        0        0     5609 2023-07-21 03:41:53.572985 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc
--rw-r--r--   0        0        0     5117 2023-07-24 09:28:27.245300 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/data.cpython-39.pyc
--rw-r--r--   0        0        0     6200 2023-06-27 02:27:16.171507 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc
--rw-r--r--   0        0        0     6358 2023-07-21 03:41:53.282985 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc
--rw-r--r--   0        0        0     2519 2023-07-20 03:31:49.026223 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/iface.cpython-39.pyc
--rw-r--r--   0        0        0    12264 2023-07-21 03:41:53.392985 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc
--rw-r--r--   0        0        0     9323 2023-07-24 09:28:27.295300 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc
--rw-r--r--   0        0        0    10687 2023-07-24 09:28:27.305300 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/selector.cpython-39.pyc
--rw-r--r--   0        0        0      538 2023-07-21 03:41:53.862985 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/updater.cpython-39.pyc
--rw-r--r--   0        0        0     3360 2023-07-24 08:47:10.485875 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     6463 2023-07-21 03:41:53.572985 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc
--rw-r--r--   0        0        0     5225 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/domain/asap.py
--rw-r--r--   0        0        0     1805 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     6585 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     5454 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/domain/data.py
--rw-r--r--   0        0        0     7895 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.5.0/ai2_kit/domain/iface.py
--rw-r--r--   0        0        0    17292 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     9046 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/domain/lasp.py
--rw-r--r--   0        0        0    13582 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      186 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     6882 2023-07-24 08:46:11.435884 ai2_kit-0.5.0/ai2_kit/domain/util.py
--rw-r--r--   0        0        0     7678 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/domain/vasp.py
--rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.5.0/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.0/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0      139 2023-06-28 08:15:51.392260 ai2_kit-0.5.0/ai2_kit/tool/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1616 2023-06-28 08:15:51.392260 ai2_kit-0.5.0/ai2_kit/tool/__pycache__/ase.cpython-39.pyc
--rw-r--r--   0        0        0     1039 2023-07-07 01:23:16.068582 ai2_kit-0.5.0/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.0/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0      143 2023-02-14 03:43:41.260120 ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7937 2023-07-24 09:28:27.095300 ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc
--rw-r--r--   0        0        0     5996 2023-06-15 08:55:37.729603 ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc
--rw-r--r--   0        0        0     5966 2023-02-14 03:43:41.260120 ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc
--rw-r--r--   0        0        0     6336 2023-07-20 03:31:49.786223 ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc
--rw-r--r--   0        0        0    10064 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     9135 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0      953 2023-07-24 09:30:29.085274 ai2_kit-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 ai2_kit-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2012 2023-07-21 03:28:16.683182 ai2_kit-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.1/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.5.1/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-15 02:12:13.145370 ai2_kit-0.5.1/ai2_kit/algorithm/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9573 2023-06-15 02:12:13.155370 ai2_kit-0.5.1/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc
+-rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.5.1/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.1/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0      139 2023-02-14 03:43:41.260120 ai2_kit-0.5.1/ai2_kit/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2243 2023-07-20 03:31:49.016223 ai2_kit-0.5.1/ai2_kit/core/__pycache__/artifact.cpython-39.pyc
+-rw-r--r--   0        0        0     5928 2023-07-20 03:31:48.996223 ai2_kit-0.5.1/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc
+-rw-r--r--   0        0        0      512 2023-06-15 07:55:24.192005 ai2_kit-0.5.1/ai2_kit/core/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0     7307 2023-07-24 07:57:09.456574 ai2_kit-0.5.1/ai2_kit/core/__pycache__/connector.cpython-39.pyc
+-rw-r--r--   0        0        0     9586 2023-07-24 09:28:27.095300 ai2_kit-0.5.1/ai2_kit/core/__pycache__/executor.cpython-39.pyc
+-rw-r--r--   0        0        0      894 2023-06-29 05:30:14.695752 ai2_kit-0.5.1/ai2_kit/core/__pycache__/future.cpython-39.pyc
+-rw-r--r--   0        0        0     2847 2023-07-20 03:31:48.996223 ai2_kit-0.5.1/ai2_kit/core/__pycache__/job.cpython-39.pyc
+-rw-r--r--   0        0        0      436 2023-06-29 05:30:14.695752 ai2_kit-0.5.1/ai2_kit/core/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0    10069 2023-07-21 03:41:53.042985 ai2_kit-0.5.1/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc
+-rw-r--r--   0        0        0     3063 2023-07-20 03:31:49.026223 ai2_kit-0.5.1/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc
+-rw-r--r--   0        0        0     2611 2023-07-21 03:41:53.282985 ai2_kit-0.5.1/ai2_kit/core/__pycache__/script.cpython-39.pyc
+-rw-r--r--   0        0        0     8116 2023-07-24 09:28:27.215300 ai2_kit-0.5.1/ai2_kit/core/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.5.1/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     5894 2023-07-25 01:13:41.843210 ai2_kit-0.5.1/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.5.1/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-07-21 04:37:23.322249 ai2_kit-0.5.1/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     8006 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.5.1/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.5.1/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.5.1/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     9587 2023-07-21 01:27:23.144801 ai2_kit-0.5.1/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.5.1/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2363 2023-07-21 01:27:23.144801 ai2_kit-0.5.1/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     5900 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.1/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0      110 2023-06-15 07:55:24.202005 ai2_kit-0.5.1/ai2_kit/dflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.1/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0      141 2023-02-14 03:43:41.670121 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4703 2023-07-25 00:52:37.103514 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/asap.cpython-39.pyc
+-rw-r--r--   0        0        0     2517 2023-06-29 05:30:14.805753 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/cll.cpython-39.pyc
+-rw-r--r--   0        0        0     3221 2023-02-23 07:10:20.489990 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0        0        0     1532 2023-07-24 09:28:27.285300 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/constant.cpython-39.pyc
+-rw-r--r--   0        0        0     5609 2023-07-21 03:41:53.572985 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc
+-rw-r--r--   0        0        0     5117 2023-07-24 09:28:27.245300 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/data.cpython-39.pyc
+-rw-r--r--   0        0        0     6200 2023-06-27 02:27:16.171507 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc
+-rw-r--r--   0        0        0     6358 2023-07-21 03:41:53.282985 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc
+-rw-r--r--   0        0        0     2519 2023-07-20 03:31:49.026223 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/iface.cpython-39.pyc
+-rw-r--r--   0        0        0    12264 2023-07-21 03:41:53.392985 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc
+-rw-r--r--   0        0        0     9323 2023-07-24 09:28:27.295300 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc
+-rw-r--r--   0        0        0    10687 2023-07-24 09:28:27.305300 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/selector.cpython-39.pyc
+-rw-r--r--   0        0        0      538 2023-07-21 03:41:53.862985 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/updater.cpython-39.pyc
+-rw-r--r--   0        0        0     3360 2023-07-24 08:47:10.485875 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     6463 2023-07-21 03:41:53.572985 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc
+-rw-r--r--   0        0        0     5449 2023-07-25 00:53:24.333505 ai2_kit-0.5.1/ai2_kit/domain/asap.py
+-rw-r--r--   0        0        0     1805 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     6585 2023-07-21 01:27:23.144801 ai2_kit-0.5.1/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     5454 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/domain/data.py
+-rw-r--r--   0        0        0     7895 2023-07-21 01:27:23.144801 ai2_kit-0.5.1/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.5.1/ai2_kit/domain/iface.py
+-rw-r--r--   0        0        0    17292 2023-07-25 01:07:27.943305 ai2_kit-0.5.1/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     9046 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/domain/lasp.py
+-rw-r--r--   0        0        0    13582 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      186 2023-07-21 01:27:23.144801 ai2_kit-0.5.1/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     6882 2023-07-24 08:46:11.435884 ai2_kit-0.5.1/ai2_kit/domain/util.py
+-rw-r--r--   0        0        0     7678 2023-07-21 01:27:23.144801 ai2_kit-0.5.1/ai2_kit/domain/vasp.py
+-rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.5.1/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.1/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0      139 2023-06-28 08:15:51.392260 ai2_kit-0.5.1/ai2_kit/tool/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1616 2023-06-28 08:15:51.392260 ai2_kit-0.5.1/ai2_kit/tool/__pycache__/ase.cpython-39.pyc
+-rw-r--r--   0        0        0     1039 2023-07-07 01:23:16.068582 ai2_kit-0.5.1/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.1/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0      143 2023-02-14 03:43:41.260120 ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7937 2023-07-24 09:28:27.095300 ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc
+-rw-r--r--   0        0        0     5996 2023-06-15 08:55:37.729603 ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc
+-rw-r--r--   0        0        0     5966 2023-02-14 03:43:41.260120 ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc
+-rw-r--r--   0        0        0     6336 2023-07-20 03:31:49.786223 ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc
+-rw-r--r--   0        0        0    10064 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     9135 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      953 2023-07-25 01:36:42.212881 ai2_kit-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 ai2_kit-0.5.1/PKG-INFO
```

### Comparing `ai2_kit-0.5.0/LICENSE` & `ai2_kit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/README.md` & `ai2_kit-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.5.1/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/__pycache__/artifact.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/core/__pycache__/artifact.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/__pycache__/cmd.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/core/__pycache__/cmd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/__pycache__/connector.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/core/__pycache__/connector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/__pycache__/executor.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/core/__pycache__/executor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/__pycache__/future.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/core/__pycache__/future.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/__pycache__/job.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/core/__pycache__/job.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/__pycache__/script.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/core/__pycache__/script.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/__pycache__/util.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/core/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/artifact.py` & `ai2_kit-0.5.1/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/checkpoint.py` & `ai2_kit-0.5.1/ai2_kit/core/checkpoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -176,20 +176,23 @@
                     f'Key:        \t{key}',
                     f'Call Site:  \t{value["info"]["call_site"]}',
                     f'Function:   \t{value["info"]["fn_name"]}',
                 ]))
             else:
                 print(key)
 
-    def rm(self, glob_pattern: str, yes=False):
+    def rm(self, glob_pattern: str, yes=False, exclude: Optional[str]=None):
         """remove checkpoint entries with the given pattern"""
         assert _checkpoint_data is not None
 
-        for key in list(_checkpoint_data.keys()):
-            if fnmatch.fnmatch(key, glob_pattern):
-                if yes:
-                    del _checkpoint_data[key]
-                else:
-                    print(f"Delete checkpoint {key}? [y/n]")
-                    if input().lower() == 'y':
-                        del _checkpoint_data[key]
+        keys = [ key for key in _checkpoint_data.keys() if fnmatch.fnmatch(key, glob_pattern) ]
+        if exclude is not None:
+            keys = [ key for key in keys if not fnmatch.fnmatch(key, exclude) ]
+
+        for key in keys:
+            if not yes:
+                print(f"Delete checkpoint {key}? [y/n]")
+                if input().lower() != 'y':
+                    continue
+            del _checkpoint_data[key]
+            print(f"Delete checkpoint {key}")
         _dump_checkpoint()
```

### Comparing `ai2_kit-0.5.0/ai2_kit/core/connector.py` & `ai2_kit-0.5.1/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/executor.py` & `ai2_kit-0.5.1/ai2_kit/core/executor.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/job.py` & `ai2_kit-0.5.1/ai2_kit/core/job.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/queue_system.py` & `ai2_kit-0.5.1/ai2_kit/core/queue_system.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/resource_manager.py` & `ai2_kit-0.5.1/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/script.py` & `ai2_kit-0.5.1/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/core/util.py` & `ai2_kit-0.5.1/ai2_kit/core/util.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/asap.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/asap.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Jul 24 09:25:32 2023 UTC, .py size: 5225 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,286 +1,294 @@
-00000000: 610d 0d0a 0000 0000 8c43 be64 6914 0000  a........C.di...
+00000000: 610d 0d0a 0000 0000 d01c bf64 f514 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6400  d.l.m.Z.m.Z...d.
-00000080: 6407 6c0e 6d0f 5a0f 0100 6400 6408 6c10  d.l.m.Z...d.d.l.
-00000090: 5a11 6409 640a 8400 5a12 6512 8300 5c04  Z.d.d...Z.e...\.
-000000a0: 5a13 5a14 5a15 5a16 6408 5300 290b e900  Z.Z.Z.Z.d.S.)...
-000000b0: 0000 0029 01da 0741 5341 5058 595a 2902  ...)...ASAPXYZ).
-000000c0: da0f 636c 7573 7465 725f 7072 6f63 6573  ..cluster_proces
-000000d0: 73da 0b73 6574 5f72 6564 7563 6572 2901  s..set_reducer).
-000000e0: da14 756e 6976 6572 7361 6c5f 736f 6170  ..universal_soap
-000000f0: 5f68 7970 6572 2901 da14 756e 6976 6572  _hyper)...univer
-00000100: 7361 6c5f 6163 7366 5f68 7970 6572 2901  sal_acsf_hyper).
-00000110: da12 4469 6d65 6e73 696f 6e5f 5265 6475  ..Dimension_Redu
-00000120: 6365 7273 2902 da07 4c41 494f 5f44 42da  cers)...LAIO_DB.
-00000130: 0a73 6b6c 6561 726e 5f44 4229 01da 0563  .sklearn_DB)...c
-00000140: 6469 7374 4e63 0000 0000 0000 0000 0000  distNc..........
-00000150: 0000 0400 0000 0500 0000 0300 0000 73b0  ..............s.
-00000160: 0000 0064 2074 0074 0164 049c 0287 0266  ...d t.t.d.....f
-00000170: 0164 0564 0684 0d7d 0074 0074 0164 049c  .d.d...}.t.t.d..
-00000180: 0287 0087 0466 0264 0764 0884 0c89 0274  .....f.d.d.....t
-00000190: 0074 0164 099c 0264 0a64 0b84 0489 0474  .t.d...d.d.....t
-000001a0: 0074 0164 099c 0264 0c64 0d84 0489 0074  .t.d...d.d.....t
-000001b0: 026a 0374 0164 0e9c 0264 0f64 1084 047d  .j.t.d...d.d...}
-000001c0: 0164 2174 026a 0364 149c 0164 1564 1684  .d!t.j.d...d.d..
-000001d0: 0589 0164 1764 1884 0089 0374 026a 0374  ...d.d.....t.j.t
-000001e0: 0164 199c 0287 0187 0366 0264 1a64 1b84  .d.......f.d.d..
-000001f0: 0c7d 0264 2274 0074 026a 0364 1d9c 0264  .}.d"t.t.j.d...d
-00000200: 1e64 1f84 057d 037c 007c 017c 027c 0366  .d...}.|.|.|.|.f
-00000210: 0453 0029 234e 46e9 0400 0000 fa11 2e2f  .S.)#NF......../
-00000220: 6173 6170 2d64 6573 6372 6970 746f 7229  asap-descriptor)
-00000230: 02da 0761 7361 7078 797a da07 7365 7474  ...asapxyz..sett
-00000240: 696e 6763 0500 0000 0000 0000 0000 0000  ingc............
-00000250: 0800 0000 0500 0000 1300 0000 7358 0000  ............sX..
-00000260: 0088 007c 007c 0183 027d 057c 006a 007c  ...|.|...}.|.j.|
-00000270: 057c 027c 0364 018d 0301 007c 00a0 017c  .|.|.d.....|...|
-00000280: 04a1 0101 007c 00a0 0274 037c 05a0 04a1  .....|...t.|....
-00000290: 0083 01a1 017d 067c 0272 4c7c 00a0 0574  .....}.|.rL|...t
-000002a0: 037c 05a0 04a1 0083 01a1 016e 0264 007d  .|.........n.d.}
-000002b0: 077c 067c 0766 0253 0029 024e 2903 da0e  .|.|.f.S.).N)...
-000002c0: 6465 7363 5f73 7065 635f 6469 6374 da0b  desc_spec_dict..
-000002d0: 6b65 6570 5f61 746f 6d69 63da 096e 5f70  keep_atomic..n_p
-000002e0: 726f 6365 7373 2906 da1a 636f 6d70 7574  rocess)...comput
-000002f0: 655f 676c 6f62 616c 5f64 6573 6372 6970  e_global_descrip
-00000300: 746f 7273 da0a 7361 7665 5f73 7461 7465  tors..save_state
-00000310: da1a 6665 7463 685f 636f 6d70 7574 6564  ..fetch_computed
-00000320: 5f64 6573 6372 6970 746f 7273 da04 6c69  _descriptors..li
-00000330: 7374 da04 6b65 7973 da21 6665 7463 685f  st..keys.!fetch_
-00000340: 636f 6d70 7574 6564 5f61 746f 6d69 635f  computed_atomic_
-00000350: 6465 7363 7269 7074 6f72 7329 0872 0d00  descriptors).r..
-00000360: 0000 720e 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00000370: 00da 0b70 6174 685f 7072 6566 6978 da0f  ...path_prefix..
-00000380: 6465 7363 7269 7074 6f72 5f73 7065 63da  descriptor_spec.
-00000390: 1267 6c6f 6261 6c5f 6465 7363 7269 7074  .global_descript
-000003a0: 6f72 73da 1261 746f 6d69 635f 6465 7363  ors..atomic_desc
-000003b0: 7269 7074 6f72 7329 01da 1367 6574 5f64  riptors)...get_d
-000003c0: 6573 6372 6970 746f 725f 7370 6563 a900  escriptor_spec..
-000003d0: fa2e 2f68 6f6d 652f 6865 6e72 792f 7372  ../home/henry/sr
-000003e0: 632f 6169 322d 6b69 742f 6169 325f 6b69  c/ai2-kit/ai2_ki
-000003f0: 742f 646f 6d61 696e 2f61 7361 702e 7079  t/domain/asap.py
-00000400: da0e 6765 745f 6465 7363 7269 7074 6f72  ..get_descriptor
-00000410: 0f00 0000 7314 0000 0000 020a 0104 0102  ....s...........
-00000420: 0102 0102 fd06 050a 0212 011a 017a 315f  .............z1_
-00000430: 5f65 7870 6f72 745f 7265 6d6f 7465 5f66  _export_remote_f
-00000440: 756e 6374 696f 6e73 2e3c 6c6f 6361 6c73  unctions.<locals
-00000450: 3e2e 6765 745f 6465 7363 7269 7074 6f72  >.get_descriptor
-00000460: 6302 0000 0000 0000 0000 0000 000a 0000  c...............
-00000470: 0006 0000 0013 0000 0073 b800 0000 6401  .........s....d.
-00000480: 5c02 7d02 7d03 6402 4400 5d20 7d04 7c01  \.}.}.d.D.] }.|.
-00000490: a000 7c04 6400 a102 7d03 7c03 6400 7501  ..|.d...}.|.d.u.
-000004a0: 720c 7c04 7d02 0100 7136 710c 7401 6403  r.|.}...q6q.t.d.
-000004b0: 8301 8201 7c02 6404 6b02 724a 6404 6405  ....|.d.k.rJd.d.
-000004c0: 6406 6901 6901 5300 7402 7403 7c03 6407  d.i.i.S.t.t.|.d.
-000004d0: 1900 7c03 6408 1900 7c03 6409 1900 8303  ..|.d...|.d.....
-000004e0: 8301 7d05 7c02 640a 6b02 727a 8800 7c00  ..}.|.d.k.rz..|.
-000004f0: 7c03 8302 7d06 6e12 7c02 640b 6b02 728c  |...}.n.|.d.k.r.
-00000500: 8801 7c00 7c03 8302 7d06 6900 7d07 7c06  ..|.|...}.i.}.|.
-00000510: a004 a100 4400 5d1a 5c02 7d08 7d09 7c08  ....D.].\.}.}.|.
-00000520: 7c09 6901 7c05 640c 9c02 7c07 7c08 3c00  |.i.|.d...|.|.<.
-00000530: 7198 7c07 5300 290d 4e29 024e 4e29 03da  q.|.S.).N).NN)..
-00000540: 0473 6f61 70da 0461 6373 66da 0263 6d7a  .soap..acsf..cmz
-00000550: 1755 6e6b 6e6f 776e 2064 6573 6372 6970  .Unknown descrip
-00000560: 746f 7220 7479 7065 7222 0000 00da 0474  tor typer".....t
-00000570: 7970 65da 0243 4dda 0c72 6564 7563 6572  ype..CM..reducer
-00000580: 5f74 7970 65da 0c65 6c65 6d65 6e74 5f77  _type..element_w
-00000590: 6973 65da 047a 6574 6172 2100 0000 7220  ise..zetar!...r 
-000005a0: 0000 0029 02da 1161 746f 6d69 635f 6465  ...)...atomic_de
-000005b0: 7363 7269 7074 6f72 da10 7265 6475 6365  scriptor..reduce
-000005c0: 725f 6675 6e63 7469 6f6e 2905 da03 6765  r_function)...ge
-000005d0: 74da 0a56 616c 7565 4572 726f 72da 0464  t..ValueError..d
-000005e0: 6963 7472 0400 0000 da05 6974 656d 7329  ictr......items)
-000005f0: 0a72 0d00 0000 720e 0000 005a 0f64 6573  .r....r....Z.des
-00000600: 6372 6970 746f 725f 7479 7065 da06 7061  criptor_type..pa
-00000610: 7261 6d73 da03 6b65 79da 0c72 6564 7563  rams..key..reduc
-00000620: 6572 5f73 7065 63da 1661 746f 6d69 635f  er_spec..atomic_
-00000630: 6465 7363 7269 7074 6f72 5f73 7065 6372  descriptor_specr
-00000640: 1900 0000 da01 6bda 0176 2902 da1f 6765  ......k..v)...ge
-00000650: 745f 6163 7366 5f61 746f 6d69 635f 6465  t_acsf_atomic_de
-00000660: 7363 7269 7074 6f72 5f73 7065 63da 1f67  scriptor_spec..g
-00000670: 6574 5f73 6f61 705f 6174 6f6d 6963 5f64  et_soap_atomic_d
-00000680: 6573 6372 6970 746f 725f 7370 6563 721d  escriptor_specr.
-00000690: 0000 0072 1e00 0000 721c 0000 001e 0000  ...r....r.......
-000006a0: 0073 3000 0000 0001 0801 0801 0c01 0801  .s0.............
-000006b0: 0401 0602 0803 0801 0c02 0401 0601 0601  ................
-000006c0: 06fd 0606 0801 0c01 0801 0a02 0401 1002  ................
-000006d0: 0601 02fe 0c04 7a36 5f5f 6578 706f 7274  ......z6__export
-000006e0: 5f72 656d 6f74 655f 6675 6e63 7469 6f6e  _remote_function
-000006f0: 732e 3c6c 6f63 616c 733e 2e67 6574 5f64  s.<locals>.get_d
-00000700: 6573 6372 6970 746f 725f 7370 6563 2902  escriptor_spec).
-00000710: 720d 0000 0072 2e00 0000 6302 0000 0000  r....r....c.....
-00000720: 0000 0000 0000 0005 0000 0007 0000 0053  ...............S
-00000730: 0000 0073 7a00 0000 7c01 6401 1900 7d02  ...sz...|.d...}.
-00000740: 7c02 6400 7500 7236 6402 6403 7c01 6404  |.d.u.r6d.d.|.d.
-00000750: 1900 7c01 6405 1900 7c01 6406 1900 7c01  ..|.d...|.d...|.
-00000760: 6407 1900 6408 9c05 6901 7d03 6e12 7400  d...d...i.}.n.t.
-00000770: 7c00 a001 a100 7c02 6409 640a 8d03 7d03  |.....|.d.d...}.
-00000780: 7c03 a002 a100 4400 5d24 7d04 7c01 640b  |.....D.]$}.|.d.
-00000790: 1900 7c03 7c04 1900 640b 3c00 7c01 640c  ..|.|...d.<.|.d.
-000007a0: 1900 7c03 7c04 1900 640c 3c00 7150 7c03  ..|.|...d.<.qP|.
-000007b0: 5300 290d 4eda 0670 7265 7365 745a 0573  S.).N..presetZ.s
-000007c0: 6f61 7031 da04 534f 4150 da05 725f 6375  oap1..SOAP..r_cu
-000007d0: 74da 056e 5f6d 6178 da05 6c5f 6d61 78da  t..n_max..l_max.
-000007e0: 0573 6967 6d61 2905 7223 0000 00da 0663  .sigma).r#.....c
-000007f0: 7574 6f66 66da 016e da01 6cda 1361 746f  utoff..n..l..ato
-00000800: 6d5f 6761 7573 7369 616e 5f77 6964 7468  m_gaussian_width
-00000810: 46a9 01da 0464 756d 70da 0372 6266 da09  F....dump..rbf..
-00000820: 6372 6f73 736f 7665 7229 0372 0500 0000  crossover).r....
-00000830: da12 6765 745f 676c 6f62 616c 5f73 7065  ..get_global_spe
-00000840: 6369 6573 7216 0000 0029 0572 0d00 0000  ciesr....).r....
-00000850: 722e 0000 0072 3600 0000 7231 0000 0072  r....r6...r1...r
-00000860: 3200 0000 721d 0000 0072 1d00 0000 721e  2...r....r....r.
-00000870: 0000 0072 3500 0000 4000 0000 731e 0000  ...r5...@...s...
-00000880: 0000 0108 0108 0202 0102 0106 0106 0106  ................
-00000890: 0106 fb04 ff06 0a12 020c 0110 0112 027a  ...............z
-000008a0: 425f 5f65 7870 6f72 745f 7265 6d6f 7465  B__export_remote
-000008b0: 5f66 756e 6374 696f 6e73 2e3c 6c6f 6361  _functions.<loca
-000008c0: 6c73 3e2e 6765 745f 736f 6170 5f61 746f  ls>.get_soap_ato
-000008d0: 6d69 635f 6465 7363 7269 7074 6f72 5f73  mic_descriptor_s
-000008e0: 7065 6363 0200 0000 0000 0000 0000 0000  pecc............
-000008f0: 0400 0000 0500 0000 5300 0000 732e 0000  ........S...s...
-00000900: 007c 0164 0119 007d 027c 0264 0075 0072  .|.d...}.|.d.u.r
-00000910: 187c 0164 0219 006e 027c 027d 0374 007c  .|.d...n.|.}.t.|
-00000920: 00a0 01a1 007c 0364 0364 048d 0353 0029  .....|.d.d...S.)
-00000930: 054e 7236 0000 0072 3800 0000 4672 4000  .Nr6...r8...Fr@.
-00000940: 0000 2902 7206 0000 0072 4400 0000 2904  ..).r....rD...).
-00000950: 720d 0000 0072 2e00 0000 7236 0000 005a  r....r....r6...Z
-00000960: 0b66 6163 7366 5f70 6172 616d 721d 0000  .facsf_paramr...
-00000970: 0072 1d00 0000 721e 0000 0072 3400 0000  .r....r....r4...
-00000980: 5600 0000 7306 0000 0000 0108 0114 017a  V...s..........z
-00000990: 425f 5f65 7870 6f72 745f 7265 6d6f 7465  B__export_remote
-000009a0: 5f66 756e 6374 696f 6e73 2e3c 6c6f 6361  _functions.<loca
-000009b0: 6c73 3e2e 6765 745f 6163 7366 5f61 746f  ls>.get_acsf_ato
-000009c0: 6d69 635f 6465 7363 7269 7074 6f72 5f73  mic_descriptor_s
-000009d0: 7065 6329 02da 0b64 6573 6372 6970 746f  pec)...descripto
-000009e0: 7273 720e 0000 0063 0200 0000 0000 0000  rsr....c........
-000009f0: 0000 0000 0400 0000 0300 0000 5300 0000  ............S...
-00000a00: 7316 0000 0074 007c 0183 017d 027c 02a0  s....t.|...}.|..
-00000a10: 017c 00a1 017d 037c 0353 00a9 014e 2902  .|...}.|.S...N).
-00000a20: 7207 0000 00da 0d66 6974 5f74 7261 6e73  r......fit_trans
-00000a30: 666f 726d 2904 7245 0000 0072 0e00 0000  form).rE...r....
-00000a40: da07 7265 6475 6365 72da 1372 6564 7563  ..reducer..reduc
-00000a50: 6564 5f64 6573 6372 6970 746f 7273 721d  ed_descriptorsr.
-00000a60: 0000 0072 1d00 0000 721e 0000 00da 1072  ...r....r......r
-00000a70: 6564 7563 655f 6469 6d65 6e73 696f 6e5c  educe_dimension\
-00000a80: 0000 0073 0600 0000 0001 0801 0a01 7a33  ...s..........z3
-00000a90: 5f5f 6578 706f 7274 5f72 656d 6f74 655f  __export_remote_
-00000aa0: 6675 6e63 7469 6f6e 732e 3c6c 6f63 616c  functions.<local
-00000ab0: 733e 2e72 6564 7563 655f 6469 6d65 6e73  s>.reduce_dimens
-00000ac0: 696f 6eda 0965 7563 6c69 6465 616e e902  ion..euclidean..
-00000ad0: 0000 00e9 3200 0000 2901 da0a 6465 7363  ....2...)...desc
-00000ae0: 7269 7074 6f72 6305 0000 0000 0000 0000  riptorc.........
-00000af0: 0000 0007 0000 0006 0000 0053 0000 0073  ...........S...s
-00000b00: 5800 0000 7c02 6400 7500 724a 7400 7c00  X...|.d.u.rJt.|.
-00000b10: 8301 7d05 7c00 7401 6a02 6a03 7c05 7404  ..}.|.t.j.j.|.t.
-00000b20: 7c05 7c04 8302 6401 6402 8d03 1900 7d06  |.|...d.d.....}.
-00000b30: 7401 a005 7406 7c06 7c00 7c01 8303 7404  t...t.|.|.|...t.
-00000b40: 6403 7c05 1b00 6404 8302 a102 7d02 7407  d.|...d.....}.t.
-00000b50: 7c02 7c03 7c01 6405 8d03 5300 2906 4e46  |.|.|.d...S.).NF
-00000b60: 2901 da07 7265 706c 6163 6567 0000 0000  )...replaceg....
-00000b70: 0040 8f40 e964 0000 0029 015a 0a6d 6574  .@.@.d...).Z.met
-00000b80: 7269 6374 7970 6529 08da 036c 656e da02  rictype)...len..
-00000b90: 6e70 da06 7261 6e64 6f6d da06 6368 6f69  np..random..choi
-00000ba0: 6365 da03 6d69 6eda 0a70 6572 6365 6e74  ce..min..percent
-00000bb0: 696c 6572 0a00 0000 7209 0000 0029 0772  iler....r....).r
-00000bc0: 4e00 0000 da06 6d65 7472 6963 da03 6570  N.....metric..ep
-00000bd0: 735a 0b6d 696e 5f73 616d 706c 6573 5a0b  sZ.min_samplesZ.
-00000be0: 6576 616c 5f73 616d 706c 6572 3d00 0000  eval_sampler=...
-00000bf0: da06 7361 6d70 6c65 721d 0000 0072 1d00  ..sampler....r..
-00000c00: 0000 721e 0000 00da 1267 6574 5f64 6273  ..r......get_dbs
-00000c10: 6361 6e5f 7472 6169 6e65 7262 0000 0073  can_trainerb...s
-00000c20: 0a00 0000 0001 0801 0801 1c02 1e01 7a35  ..............z5
-00000c30: 5f5f 6578 706f 7274 5f72 656d 6f74 655f  __export_remote_
-00000c40: 6675 6e63 7469 6f6e 732e 3c6c 6f63 616c  functions.<local
-00000c50: 733e 2e67 6574 5f64 6273 6361 6e5f 7472  s>.get_dbscan_tr
-00000c60: 6169 6e65 7263 0000 0000 0000 0000 0000  ainerc..........
-00000c70: 0000 0100 0000 0400 0000 5b00 0000 730e  ..........[...s.
-00000c80: 0000 0074 0066 0069 007c 00a4 018e 0153  ...t.f.i.|.....S
-00000c90: 0072 4600 0000 2901 7208 0000 0029 01da  .rF...).r....)..
-00000ca0: 066b 7761 7267 7372 1d00 0000 721d 0000  .kwargsr....r...
-00000cb0: 0072 1e00 0000 da13 6765 745f 6c61 696f  .r......get_laio
-00000cc0: 5f64 625f 7472 6169 6e65 726b 0000 0073  _db_trainerk...s
-00000cd0: 0200 0000 0001 7a36 5f5f 6578 706f 7274  ......z6__export
-00000ce0: 5f72 656d 6f74 655f 6675 6e63 7469 6f6e  _remote_function
-00000cf0: 732e 3c6c 6f63 616c 733e 2e67 6574 5f6c  s.<locals>.get_l
-00000d00: 6169 6f5f 6462 5f74 7261 696e 6572 2902  aio_db_trainer).
-00000d10: 724e 0000 0072 0e00 0000 6302 0000 0000  rN...r....c.....
-00000d20: 0000 0000 0000 0004 0000 0004 0000 0013  ................
-00000d30: 0000 0073 5200 0000 7c01 a000 6401 6400  ...sR...|...d.d.
-00000d40: a102 7d02 7c02 6400 7501 7224 8800 7c00  ..}.|.d.u.r$..|.
-00000d50: 6601 6900 7c02 a401 8e01 5300 7c01 a000  f.i.|.....S.|...
-00000d60: 6402 6400 a102 7d03 7c03 6400 7501 7246  d.d...}.|.d.u.rF
-00000d70: 8801 6600 6900 7c03 a401 8e01 5300 7401  ..f.i.|.....S.t.
-00000d80: 6403 8301 8201 6400 5300 2904 4eda 0664  d.....d.S.).N..d
-00000d90: 6273 6361 6e5a 066c 6169 6f64 627a 1455  bscanZ.laiodbz.U
-00000da0: 6e6b 6e6f 776e 2074 7261 696e 6572 2074  nknown trainer t
-00000db0: 7970 6529 0272 2a00 0000 722b 0000 0029  ype).r*...r+...)
-00000dc0: 0472 4e00 0000 720e 0000 005a 0e64 6273  .rN...r....Z.dbs
-00000dd0: 6361 6e5f 7365 7474 696e 675a 0e6c 6169  can_settingZ.lai
-00000de0: 6f64 625f 7365 7474 696e 6729 0272 5a00  odb_setting).rZ.
-00000df0: 0000 725c 0000 0072 1d00 0000 721e 0000  ..r\...r....r...
-00000e00: 00da 0b67 6574 5f74 7261 696e 6572 6f00  ...get_trainero.
-00000e10: 0000 730e 0000 0000 010c 0108 0110 010c  ..s.............
-00000e20: 0108 010e 017a 2e5f 5f65 7870 6f72 745f  .....z.__export_
-00000e30: 7265 6d6f 7465 5f66 756e 6374 696f 6e73  remote_functions
-00000e40: 2e3c 6c6f 6361 6c73 3e2e 6765 745f 7472  .<locals>.get_tr
-00000e50: 6169 6e65 72fa 0e2e 2f61 7361 702d 636c  ainer.../asap-cl
-00000e60: 7573 7465 7229 0272 0d00 0000 7245 0000  uster).r....rE..
-00000e70: 0063 0400 0000 0000 0000 0000 0000 0900  .c..............
-00000e80: 0000 0500 0000 5300 0000 734e 0000 007c  ......S...sN...|
-00000e90: 0364 0164 0164 029c 037d 0474 007c 007c  .d.d.d...}.t.|.|
-00000ea0: 027c 017c 0483 047d 0569 007d 0674 01a0  .|.|...}.i.}.t..
-00000eb0: 0274 037c 0583 01a1 017d 0774 047c 0583  .t.|.....}.t.|..
-00000ec0: 0144 005d 147d 087c 077c 057c 086b 0219  .D.].}.|.|.|.k..
-00000ed0: 007c 067c 083c 0071 347c 0653 0029 034e  .|.|.<.q4|.S.).N
-00000ee0: 4629 03da 0670 7265 6669 785a 0773 6176  F)...prefixZ.sav
-00000ef0: 6578 797a da07 7361 7665 7478 7429 0572  exyz..savetxt).r
-00000f00: 0300 0000 7252 0000 00da 0661 7261 6e67  ....rR.....arang
-00000f10: 6572 5100 0000 da03 7365 7429 0972 0d00  erQ.....set).r..
-00000f20: 0000 7245 0000 00da 0774 7261 696e 6572  ..rE.....trainer
-00000f30: 7218 0000 00da 076f 7074 696f 6e73 da06  r......options..
-00000f40: 6c61 6265 6c73 da06 6772 6f75 7073 da05  labels..groups..
-00000f50: 696e 6465 78da 056c 6162 656c 721d 0000  index..labelr...
-00000f60: 0072 1d00 0000 721e 0000 00da 0b67 6574  .r....r......get
-00000f70: 5f63 6c75 7374 6572 7900 0000 7314 0000  _clustery...s...
-00000f80: 0000 0202 0102 0102 fd06 050e 0204 010e  ................
-00000f90: 010c 0112 017a 2e5f 5f65 7870 6f72 745f  .....z.__export_
-00000fa0: 7265 6d6f 7465 5f66 756e 6374 696f 6e73  remote_functions
-00000fb0: 2e3c 6c6f 6361 6c73 3e2e 6765 745f 636c  .<locals>.get_cl
-00000fc0: 7573 7465 7229 0346 720b 0000 0072 0c00  uster).Fr....r..
-00000fd0: 0000 2904 724b 0000 004e 724c 0000 0072  ..).rK...NrL...r
-00000fe0: 4d00 0000 2901 725f 0000 0029 0472 0200  M...).r_...).r..
-00000ff0: 0000 722c 0000 0072 5200 0000 da07 6e64  ..r,...rR.....nd
-00001000: 6172 7261 7929 0472 1f00 0000 724a 0000  array).r....rJ..
-00001010: 0072 5e00 0000 726a 0000 0072 1d00 0000  .r^...rj...r....
-00001020: 2905 7234 0000 0072 5a00 0000 721c 0000  ).r4...rZ...r...
-00001030: 0072 5c00 0000 7235 0000 0072 1e00 0000  .r\...r5...r....
-00001040: da19 5f5f 6578 706f 7274 5f72 656d 6f74  ..__export_remot
-00001050: 655f 6675 6e63 7469 6f6e 730d 0000 0073  e_functions....s
-00001060: 1c00 0000 0002 160f 1622 1016 1006 1206  ........."......
-00001070: 1209 0804 180a 140f 0201 0201 0201 02fc  ................
-00001080: 726c 0000 0029 17da 1061 7361 706c 6962  rl...)...asaplib
-00001090: 2e64 6174 612e 7879 7a72 0200 0000 5a15  .data.xyzr....Z.
-000010a0: 6173 6170 6c69 622e 636c 692e 6675 6e63  asaplib.cli.func
-000010b0: 5f61 7361 7072 0300 0000 7204 0000 005a  _asapr....r....Z
-000010c0: 1961 7361 706c 6962 2e68 7970 6572 732e  .asaplib.hypers.
-000010d0: 6879 7065 725f 736f 6170 7205 0000 005a  hyper_soapr....Z
-000010e0: 1961 7361 706c 6962 2e68 7970 6572 732e  .asaplib.hypers.
-000010f0: 6879 7065 725f 6163 7366 7206 0000 005a  hyper_acsfr....Z
-00001100: 1d61 7361 706c 6962 2e72 6564 7563 6564  .asaplib.reduced
-00001110: 696d 2e64 696d 5f72 6564 7563 6572 7207  im.dim_reducerr.
-00001120: 0000 005a 1e61 7361 706c 6962 2e63 6c75  ...Z.asaplib.clu
-00001130: 7374 6572 2e6d 6c5f 636c 7573 7465 725f  ster.ml_cluster_
-00001140: 6669 7472 0800 0000 7209 0000 00da 1673  fitr....r......s
-00001150: 6369 7079 2e73 7061 7469 616c 2e64 6973  cipy.spatial.dis
-00001160: 7461 6e63 6572 0a00 0000 da05 6e75 6d70  tancer......nump
-00001170: 7972 5200 0000 726c 0000 0072 1f00 0000  yrR...rl...r....
-00001180: 724a 0000 0072 5e00 0000 726a 0000 0072  rJ...r^...rj...r
-00001190: 1d00 0000 721d 0000 0072 1d00 0000 721e  ....r....r....r.
-000011a0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000011b0: 0073 2000 0000 0c01 1001 0c01 0c01 0c01  .s .............
-000011c0: 1002 0c02 0803 087f 0008 04fb 0201 0201  ................
-000011d0: 0201 0201 02fc                           ......
+00000020: 0004 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6500 6a03 6403 6502 6404 8d02 0100  ..e.j.d.e.d.....
+00000050: 6400 6405 6c04 6d05 5a05 0100 6400 6406  d.d.l.m.Z...d.d.
+00000060: 6c06 6d07 5a07 6d08 5a08 0100 6400 6407  l.m.Z.m.Z...d.d.
+00000070: 6c09 6d0a 5a0a 0100 6400 6408 6c0b 6d0c  l.m.Z...d.d.l.m.
+00000080: 5a0c 0100 6400 6409 6c0d 6d0e 5a0e 0100  Z...d.d.l.m.Z...
+00000090: 6400 640a 6c0f 6d10 5a10 6d11 5a11 0100  d.d.l.m.Z.m.Z...
+000000a0: 6400 640b 6c12 6d13 5a13 0100 6400 6401  d.d.l.m.Z...d.d.
+000000b0: 6c14 5a15 640c 640d 8400 5a16 6516 8300  l.Z.d.d...Z.e...
+000000c0: 5c04 5a17 5a18 5a19 5a1a 6401 5300 290e  \.Z.Z.Z.Z.d.S.).
+000000d0: e900 0000 004e 2901 da17 4e75 6d62 6144  .....N)...NumbaD
+000000e0: 6570 7265 6361 7469 6f6e 5761 726e 696e  eprecationWarnin
+000000f0: 67da 0669 676e 6f72 6529 01da 0863 6174  g..ignore)...cat
+00000100: 6567 6f72 7929 01da 0741 5341 5058 595a  egory)...ASAPXYZ
+00000110: 2902 da0f 636c 7573 7465 725f 7072 6f63  )...cluster_proc
+00000120: 6573 73da 0b73 6574 5f72 6564 7563 6572  ess..set_reducer
+00000130: 2901 da14 756e 6976 6572 7361 6c5f 736f  )...universal_so
+00000140: 6170 5f68 7970 6572 2901 da14 756e 6976  ap_hyper)...univ
+00000150: 6572 7361 6c5f 6163 7366 5f68 7970 6572  ersal_acsf_hyper
+00000160: 2901 da12 4469 6d65 6e73 696f 6e5f 5265  )...Dimension_Re
+00000170: 6475 6365 7273 2902 da07 4c41 494f 5f44  ducers)...LAIO_D
+00000180: 42da 0a73 6b6c 6561 726e 5f44 4229 01da  B..sklearn_DB)..
+00000190: 0563 6469 7374 6300 0000 0000 0000 0000  .cdistc.........
+000001a0: 0000 0004 0000 0005 0000 0003 0000 0073  ...............s
+000001b0: b000 0000 6420 7400 7401 6404 9c02 8702  ....d t.t.d.....
+000001c0: 6601 6405 6406 840d 7d00 7400 7401 6404  f.d.d...}.t.t.d.
+000001d0: 9c02 8700 8704 6602 6407 6408 840c 8902  ......f.d.d.....
+000001e0: 7400 7401 6409 9c02 640a 640b 8404 8904  t.t.d...d.d.....
+000001f0: 7400 7401 6409 9c02 640c 640d 8404 8900  t.t.d...d.d.....
+00000200: 7402 6a03 7401 640e 9c02 640f 6410 8404  t.j.t.d...d.d...
+00000210: 7d01 6421 7402 6a03 6414 9c01 6415 6416  }.d!t.j.d...d.d.
+00000220: 8405 8901 6417 6418 8400 8903 7402 6a03  ....d.d.....t.j.
+00000230: 7401 6419 9c02 8701 8703 6602 641a 641b  t.d.......f.d.d.
+00000240: 840c 7d02 6422 7400 7402 6a03 641d 9c02  ..}.d"t.t.j.d...
+00000250: 641e 641f 8405 7d03 7c00 7c01 7c02 7c03  d.d...}.|.|.|.|.
+00000260: 6604 5300 2923 4e46 e904 0000 00fa 112e  f.S.)#NF........
+00000270: 2f61 7361 702d 6465 7363 7269 7074 6f72  /asap-descriptor
+00000280: 2902 da07 6173 6170 7879 7ada 0773 6574  )...asapxyz..set
+00000290: 7469 6e67 6305 0000 0000 0000 0000 0000  tingc...........
+000002a0: 0008 0000 0005 0000 0013 0000 0073 5800  .............sX.
+000002b0: 0000 8800 7c00 7c01 8302 7d05 7c00 6a00  ....|.|...}.|.j.
+000002c0: 7c05 7c02 7c03 6401 8d03 0100 7c00 a001  |.|.|.d.....|...
+000002d0: 7c04 a101 0100 7c00 a002 7403 7c05 a004  |.....|...t.|...
+000002e0: a100 8301 a101 7d06 7c02 724c 7c00 a005  ......}.|.rL|...
+000002f0: 7403 7c05 a004 a100 8301 a101 6e02 6400  t.|.........n.d.
+00000300: 7d07 7c06 7c07 6602 5300 2902 4e29 03da  }.|.|.f.S.).N)..
+00000310: 0e64 6573 635f 7370 6563 5f64 6963 74da  .desc_spec_dict.
+00000320: 0b6b 6565 705f 6174 6f6d 6963 da09 6e5f  .keep_atomic..n_
+00000330: 7072 6f63 6573 7329 06da 1a63 6f6d 7075  process)...compu
+00000340: 7465 5f67 6c6f 6261 6c5f 6465 7363 7269  te_global_descri
+00000350: 7074 6f72 73da 0a73 6176 655f 7374 6174  ptors..save_stat
+00000360: 65da 1a66 6574 6368 5f63 6f6d 7075 7465  e..fetch_compute
+00000370: 645f 6465 7363 7269 7074 6f72 73da 046c  d_descriptors..l
+00000380: 6973 74da 046b 6579 73da 2166 6574 6368  ist..keys.!fetch
+00000390: 5f63 6f6d 7075 7465 645f 6174 6f6d 6963  _computed_atomic
+000003a0: 5f64 6573 6372 6970 746f 7273 2908 7210  _descriptors).r.
+000003b0: 0000 0072 1100 0000 7213 0000 0072 1400  ...r....r....r..
+000003c0: 0000 da0b 7061 7468 5f70 7265 6669 78da  ....path_prefix.
+000003d0: 0f64 6573 6372 6970 746f 725f 7370 6563  .descriptor_spec
+000003e0: da12 676c 6f62 616c 5f64 6573 6372 6970  ..global_descrip
+000003f0: 746f 7273 da12 6174 6f6d 6963 5f64 6573  tors..atomic_des
+00000400: 6372 6970 746f 7273 2901 da13 6765 745f  criptors)...get_
+00000410: 6465 7363 7269 7074 6f72 5f73 7065 63a9  descriptor_spec.
+00000420: 00fa 2e2f 686f 6d65 2f68 656e 7279 2f73  .../home/henry/s
+00000430: 7263 2f61 6932 2d6b 6974 2f61 6932 5f6b  rc/ai2-kit/ai2_k
+00000440: 6974 2f64 6f6d 6169 6e2f 6173 6170 2e70  it/domain/asap.p
+00000450: 79da 0e67 6574 5f64 6573 6372 6970 746f  y..get_descripto
+00000460: 7214 0000 0073 1400 0000 0002 0a01 0401  r....s..........
+00000470: 0201 0201 02fd 0605 0a02 1201 1a01 7a31  ..............z1
+00000480: 5f5f 6578 706f 7274 5f72 656d 6f74 655f  __export_remote_
+00000490: 6675 6e63 7469 6f6e 732e 3c6c 6f63 616c  functions.<local
+000004a0: 733e 2e67 6574 5f64 6573 6372 6970 746f  s>.get_descripto
+000004b0: 7263 0200 0000 0000 0000 0000 0000 0a00  rc..............
+000004c0: 0000 0600 0000 1300 0000 73b8 0000 0064  ..........s....d
+000004d0: 015c 027d 027d 0364 0244 005d 207d 047c  .\.}.}.d.D.] }.|
+000004e0: 01a0 007c 0464 00a1 027d 037c 0364 0075  ...|.d...}.|.d.u
+000004f0: 0172 0c7c 047d 0201 0071 3671 0c74 0164  .r.|.}...q6q.t.d
+00000500: 0383 0182 017c 0264 046b 0272 4a64 0464  .....|.d.k.rJd.d
+00000510: 0564 0669 0169 0153 0074 0274 037c 0364  .d.i.i.S.t.t.|.d
+00000520: 0719 007c 0364 0819 007c 0364 0919 0083  ...|.d...|.d....
+00000530: 0383 017d 057c 0264 0a6b 0272 7a88 007c  ...}.|.d.k.rz..|
+00000540: 007c 0383 027d 066e 127c 0264 0b6b 0272  .|...}.n.|.d.k.r
+00000550: 8c88 017c 007c 0383 027d 0669 007d 077c  ...|.|...}.i.}.|
+00000560: 06a0 04a1 0044 005d 1a5c 027d 087d 097c  .....D.].\.}.}.|
+00000570: 087c 0969 017c 0564 0c9c 027c 077c 083c  .|.i.|.d...|.|.<
+00000580: 0071 987c 0753 0029 0d4e 2902 4e4e 2903  .q.|.S.).N).NN).
+00000590: da04 736f 6170 da04 6163 7366 da02 636d  ..soap..acsf..cm
+000005a0: 7a17 556e 6b6e 6f77 6e20 6465 7363 7269  z.Unknown descri
+000005b0: 7074 6f72 2074 7970 6572 2500 0000 da04  ptor typer%.....
+000005c0: 7479 7065 da02 434d da0c 7265 6475 6365  type..CM..reduce
+000005d0: 725f 7479 7065 da0c 656c 656d 656e 745f  r_type..element_
+000005e0: 7769 7365 da04 7a65 7461 7224 0000 0072  wise..zetar$...r
+000005f0: 2300 0000 2902 da11 6174 6f6d 6963 5f64  #...)...atomic_d
+00000600: 6573 6372 6970 746f 72da 1072 6564 7563  escriptor..reduc
+00000610: 6572 5f66 756e 6374 696f 6e29 05da 0367  er_function)...g
+00000620: 6574 da0a 5661 6c75 6545 7272 6f72 da04  et..ValueError..
+00000630: 6469 6374 7207 0000 00da 0569 7465 6d73  dictr......items
+00000640: 290a 7210 0000 0072 1100 0000 5a0f 6465  ).r....r....Z.de
+00000650: 7363 7269 7074 6f72 5f74 7970 65da 0670  scriptor_type..p
+00000660: 6172 616d 73da 036b 6579 da0c 7265 6475  arams..key..redu
+00000670: 6365 725f 7370 6563 da16 6174 6f6d 6963  cer_spec..atomic
+00000680: 5f64 6573 6372 6970 746f 725f 7370 6563  _descriptor_spec
+00000690: 721c 0000 00da 016b da01 7629 02da 1f67  r......k..v)...g
+000006a0: 6574 5f61 6373 665f 6174 6f6d 6963 5f64  et_acsf_atomic_d
+000006b0: 6573 6372 6970 746f 725f 7370 6563 da1f  escriptor_spec..
+000006c0: 6765 745f 736f 6170 5f61 746f 6d69 635f  get_soap_atomic_
+000006d0: 6465 7363 7269 7074 6f72 5f73 7065 6372  descriptor_specr
+000006e0: 2000 0000 7221 0000 0072 1f00 0000 2300   ...r!...r....#.
+000006f0: 0000 7330 0000 0000 0108 0108 010c 0108  ..s0............
+00000700: 0104 0106 0208 0308 010c 0204 0106 0106  ................
+00000710: 0106 fd06 0608 010c 0108 010a 0204 0110  ................
+00000720: 0206 0102 fe0c 047a 365f 5f65 7870 6f72  .......z6__expor
+00000730: 745f 7265 6d6f 7465 5f66 756e 6374 696f  t_remote_functio
+00000740: 6e73 2e3c 6c6f 6361 6c73 3e2e 6765 745f  ns.<locals>.get_
+00000750: 6465 7363 7269 7074 6f72 5f73 7065 6329  descriptor_spec)
+00000760: 0272 1000 0000 7231 0000 0063 0200 0000  .r....r1...c....
+00000770: 0000 0000 0000 0000 0500 0000 0700 0000  ................
+00000780: 5300 0000 737a 0000 007c 0164 0119 007d  S...sz...|.d...}
+00000790: 027c 0264 0075 0072 3664 0264 037c 0164  .|.d.u.r6d.d.|.d
+000007a0: 0419 007c 0164 0519 007c 0164 0619 007c  ...|.d...|.d...|
+000007b0: 0164 0719 0064 089c 0569 017d 036e 1274  .d...d...i.}.n.t
+000007c0: 007c 00a0 01a1 007c 0264 0964 0a8d 037d  .|.....|.d.d...}
+000007d0: 037c 03a0 02a1 0044 005d 247d 047c 0164  .|.....D.]$}.|.d
+000007e0: 0b19 007c 037c 0419 0064 0b3c 007c 0164  ...|.|...d.<.|.d
+000007f0: 0c19 007c 037c 0419 0064 0c3c 0071 507c  ...|.|...d.<.qP|
+00000800: 0353 0029 0d4e da06 7072 6573 6574 5a05  .S.).N..presetZ.
+00000810: 736f 6170 31da 0453 4f41 50da 0572 5f63  soap1..SOAP..r_c
+00000820: 7574 da05 6e5f 6d61 78da 056c 5f6d 6178  ut..n_max..l_max
+00000830: da05 7369 676d 6129 0572 2600 0000 da06  ..sigma).r&.....
+00000840: 6375 746f 6666 da01 6eda 016c da13 6174  cutoff..n..l..at
+00000850: 6f6d 5f67 6175 7373 6961 6e5f 7769 6474  om_gaussian_widt
+00000860: 6846 a901 da04 6475 6d70 da03 7262 66da  hF....dump..rbf.
+00000870: 0963 726f 7373 6f76 6572 2903 7208 0000  .crossover).r...
+00000880: 00da 1267 6574 5f67 6c6f 6261 6c5f 7370  ...get_global_sp
+00000890: 6563 6965 7372 1900 0000 2905 7210 0000  eciesr....).r...
+000008a0: 0072 3100 0000 7239 0000 0072 3400 0000  .r1...r9...r4...
+000008b0: 7235 0000 0072 2000 0000 7220 0000 0072  r5...r ...r ...r
+000008c0: 2100 0000 7238 0000 0045 0000 0073 1e00  !...r8...E...s..
+000008d0: 0000 0001 0801 0802 0201 0201 0601 0601  ................
+000008e0: 0601 06fb 04ff 060a 1202 0c01 1001 1202  ................
+000008f0: 7a42 5f5f 6578 706f 7274 5f72 656d 6f74  zB__export_remot
+00000900: 655f 6675 6e63 7469 6f6e 732e 3c6c 6f63  e_functions.<loc
+00000910: 616c 733e 2e67 6574 5f73 6f61 705f 6174  als>.get_soap_at
+00000920: 6f6d 6963 5f64 6573 6372 6970 746f 725f  omic_descriptor_
+00000930: 7370 6563 6302 0000 0000 0000 0000 0000  specc...........
+00000940: 0004 0000 0005 0000 0053 0000 0073 2e00  .........S...s..
+00000950: 0000 7c01 6401 1900 7d02 7c02 6400 7500  ..|.d...}.|.d.u.
+00000960: 7218 7c01 6402 1900 6e02 7c02 7d03 7400  r.|.d...n.|.}.t.
+00000970: 7c00 a001 a100 7c03 6403 6404 8d03 5300  |.....|.d.d...S.
+00000980: 2905 4e72 3900 0000 723b 0000 0046 7243  ).Nr9...r;...FrC
+00000990: 0000 0029 0272 0900 0000 7247 0000 0029  ...).r....rG...)
+000009a0: 0472 1000 0000 7231 0000 0072 3900 0000  .r....r1...r9...
+000009b0: 5a0b 6661 6373 665f 7061 7261 6d72 2000  Z.facsf_paramr .
+000009c0: 0000 7220 0000 0072 2100 0000 7237 0000  ..r ...r!...r7..
+000009d0: 005b 0000 0073 0600 0000 0001 0801 1401  .[...s..........
+000009e0: 7a42 5f5f 6578 706f 7274 5f72 656d 6f74  zB__export_remot
+000009f0: 655f 6675 6e63 7469 6f6e 732e 3c6c 6f63  e_functions.<loc
+00000a00: 616c 733e 2e67 6574 5f61 6373 665f 6174  als>.get_acsf_at
+00000a10: 6f6d 6963 5f64 6573 6372 6970 746f 725f  omic_descriptor_
+00000a20: 7370 6563 2902 da0b 6465 7363 7269 7074  spec)...descript
+00000a30: 6f72 7372 1100 0000 6302 0000 0000 0000  orsr....c.......
+00000a40: 0000 0000 0004 0000 0003 0000 0053 0000  .............S..
+00000a50: 0073 1600 0000 7400 7c01 8301 7d02 7c02  .s....t.|...}.|.
+00000a60: a001 7c00 a101 7d03 7c03 5300 a901 4e29  ..|...}.|.S...N)
+00000a70: 0272 0a00 0000 da0d 6669 745f 7472 616e  .r......fit_tran
+00000a80: 7366 6f72 6d29 0472 4800 0000 7211 0000  sform).rH...r...
+00000a90: 00da 0772 6564 7563 6572 da13 7265 6475  ...reducer..redu
+00000aa0: 6365 645f 6465 7363 7269 7074 6f72 7372  ced_descriptorsr
+00000ab0: 2000 0000 7220 0000 0072 2100 0000 da10   ...r ...r!.....
+00000ac0: 7265 6475 6365 5f64 696d 656e 7369 6f6e  reduce_dimension
+00000ad0: 6100 0000 7306 0000 0000 0108 010a 017a  a...s..........z
+00000ae0: 335f 5f65 7870 6f72 745f 7265 6d6f 7465  3__export_remote
+00000af0: 5f66 756e 6374 696f 6e73 2e3c 6c6f 6361  _functions.<loca
+00000b00: 6c73 3e2e 7265 6475 6365 5f64 696d 656e  ls>.reduce_dimen
+00000b10: 7369 6f6e da09 6575 636c 6964 6561 6ee9  sion..euclidean.
+00000b20: 0200 0000 e932 0000 0029 01da 0a64 6573  .....2...)...des
+00000b30: 6372 6970 746f 7263 0500 0000 0000 0000  criptorc........
+00000b40: 0000 0000 0700 0000 0600 0000 5300 0000  ............S...
+00000b50: 7358 0000 007c 0264 0075 0072 4a74 007c  sX...|.d.u.rJt.|
+00000b60: 0083 017d 057c 0074 016a 026a 037c 0574  ...}.|.t.j.j.|.t
+00000b70: 047c 057c 0483 0264 0164 028d 0319 007d  .|.|...d.d.....}
+00000b80: 0674 01a0 0574 067c 067c 007c 0183 0374  .t...t.|.|.|...t
+00000b90: 0464 037c 051b 0064 0483 02a1 027d 0274  .d.|...d.....}.t
+00000ba0: 077c 027c 037c 0164 058d 0353 0029 064e  .|.|.|.d...S.).N
+00000bb0: 4629 01da 0772 6570 6c61 6365 6700 0000  F)...replaceg...
+00000bc0: 0000 408f 40e9 6400 0000 2901 5a0a 6d65  ..@.@.d...).Z.me
+00000bd0: 7472 6963 7479 7065 2908 da03 6c65 6eda  trictype)...len.
+00000be0: 026e 70da 0672 616e 646f 6dda 0663 686f  .np..random..cho
+00000bf0: 6963 65da 036d 696e da0a 7065 7263 656e  ice..min..percen
+00000c00: 7469 6c65 720d 0000 0072 0c00 0000 2907  tiler....r....).
+00000c10: 7251 0000 00da 066d 6574 7269 63da 0365  rQ.....metric..e
+00000c20: 7073 5a0b 6d69 6e5f 7361 6d70 6c65 735a  psZ.min_samplesZ
+00000c30: 0b65 7661 6c5f 7361 6d70 6c65 7240 0000  .eval_sampler@..
+00000c40: 00da 0673 616d 706c 6572 2000 0000 7220  ...sampler ...r 
+00000c50: 0000 0072 2100 0000 da12 6765 745f 6462  ...r!.....get_db
+00000c60: 7363 616e 5f74 7261 696e 6572 6700 0000  scan_trainerg...
+00000c70: 730a 0000 0000 0108 0108 011c 021e 017a  s..............z
+00000c80: 355f 5f65 7870 6f72 745f 7265 6d6f 7465  5__export_remote
+00000c90: 5f66 756e 6374 696f 6e73 2e3c 6c6f 6361  _functions.<loca
+00000ca0: 6c73 3e2e 6765 745f 6462 7363 616e 5f74  ls>.get_dbscan_t
+00000cb0: 7261 696e 6572 6300 0000 0000 0000 0000  rainerc.........
+00000cc0: 0000 0001 0000 0004 0000 005b 0000 0073  ...........[...s
+00000cd0: 0e00 0000 7400 6600 6900 7c00 a401 8e01  ....t.f.i.|.....
+00000ce0: 5300 7249 0000 0029 0172 0b00 0000 2901  S.rI...).r....).
+00000cf0: da06 6b77 6172 6773 7220 0000 0072 2000  ..kwargsr ...r .
+00000d00: 0000 7221 0000 00da 1367 6574 5f6c 6169  ..r!.....get_lai
+00000d10: 6f5f 6462 5f74 7261 696e 6572 7000 0000  o_db_trainerp...
+00000d20: 7302 0000 0000 017a 365f 5f65 7870 6f72  s......z6__expor
+00000d30: 745f 7265 6d6f 7465 5f66 756e 6374 696f  t_remote_functio
+00000d40: 6e73 2e3c 6c6f 6361 6c73 3e2e 6765 745f  ns.<locals>.get_
+00000d50: 6c61 696f 5f64 625f 7472 6169 6e65 7229  laio_db_trainer)
+00000d60: 0272 5100 0000 7211 0000 0063 0200 0000  .rQ...r....c....
+00000d70: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00000d80: 1300 0000 7352 0000 007c 01a0 0064 0164  ....sR...|...d.d
+00000d90: 00a1 027d 027c 0264 0075 0172 2488 007c  ...}.|.d.u.r$..|
+00000da0: 0066 0169 007c 02a4 018e 0153 007c 01a0  .f.i.|.....S.|..
+00000db0: 0064 0264 00a1 027d 037c 0364 0075 0172  .d.d...}.|.d.u.r
+00000dc0: 4688 0166 0069 007c 03a4 018e 0153 0074  F..f.i.|.....S.t
+00000dd0: 0164 0383 0182 0164 0053 0029 044e da06  .d.....d.S.).N..
+00000de0: 6462 7363 616e 5a06 6c61 696f 6462 7a14  dbscanZ.laiodbz.
+00000df0: 556e 6b6e 6f77 6e20 7472 6169 6e65 7220  Unknown trainer 
+00000e00: 7479 7065 2902 722d 0000 0072 2e00 0000  type).r-...r....
+00000e10: 2904 7251 0000 0072 1100 0000 5a0e 6462  ).rQ...r....Z.db
+00000e20: 7363 616e 5f73 6574 7469 6e67 5a0e 6c61  scan_settingZ.la
+00000e30: 696f 6462 5f73 6574 7469 6e67 2902 725d  iodb_setting).r]
+00000e40: 0000 0072 5f00 0000 7220 0000 0072 2100  ...r_...r ...r!.
+00000e50: 0000 da0b 6765 745f 7472 6169 6e65 7274  ....get_trainert
+00000e60: 0000 0073 0e00 0000 0001 0c01 0801 1001  ...s............
+00000e70: 0c01 0801 0e01 7a2e 5f5f 6578 706f 7274  ......z.__export
+00000e80: 5f72 656d 6f74 655f 6675 6e63 7469 6f6e  _remote_function
+00000e90: 732e 3c6c 6f63 616c 733e 2e67 6574 5f74  s.<locals>.get_t
+00000ea0: 7261 696e 6572 fa0e 2e2f 6173 6170 2d63  rainer.../asap-c
+00000eb0: 6c75 7374 6572 2902 7210 0000 0072 4800  luster).r....rH.
+00000ec0: 0000 6304 0000 0000 0000 0000 0000 0009  ..c.............
+00000ed0: 0000 0005 0000 0053 0000 0073 4e00 0000  .......S...sN...
+00000ee0: 7c03 6401 6401 6402 9c03 7d04 7400 7c00  |.d.d.d...}.t.|.
+00000ef0: 7c02 7c01 7c04 8304 7d05 6900 7d06 7401  |.|.|...}.i.}.t.
+00000f00: a002 7403 7c05 8301 a101 7d07 7404 7c05  ..t.|.....}.t.|.
+00000f10: 8301 4400 5d14 7d08 7c07 7c05 7c08 6b02  ..D.].}.|.|.|.k.
+00000f20: 1900 7c06 7c08 3c00 7134 7c06 5300 2903  ..|.|.<.q4|.S.).
+00000f30: 4e46 2903 da06 7072 6566 6978 5a07 7361  NF)...prefixZ.sa
+00000f40: 7665 7879 7ada 0773 6176 6574 7874 2905  vexyz..savetxt).
+00000f50: 7206 0000 0072 5500 0000 da06 6172 616e  r....rU.....aran
+00000f60: 6765 7254 0000 00da 0373 6574 2909 7210  gerT.....set).r.
+00000f70: 0000 0072 4800 0000 da07 7472 6169 6e65  ...rH.....traine
+00000f80: 7272 1b00 0000 da07 6f70 7469 6f6e 73da  rr......options.
+00000f90: 066c 6162 656c 73da 0667 726f 7570 73da  .labels..groups.
+00000fa0: 0569 6e64 6578 da05 6c61 6265 6c72 2000  .index..labelr .
+00000fb0: 0000 7220 0000 0072 2100 0000 da0b 6765  ..r ...r!.....ge
+00000fc0: 745f 636c 7573 7465 727e 0000 0073 1400  t_cluster~...s..
+00000fd0: 0000 0002 0201 0201 02fd 0605 0e02 0401  ................
+00000fe0: 0e01 0c01 1201 7a2e 5f5f 6578 706f 7274  ......z.__export
+00000ff0: 5f72 656d 6f74 655f 6675 6e63 7469 6f6e  _remote_function
+00001000: 732e 3c6c 6f63 616c 733e 2e67 6574 5f63  s.<locals>.get_c
+00001010: 6c75 7374 6572 2903 4672 0e00 0000 720f  luster).Fr....r.
+00001020: 0000 0029 0472 4e00 0000 4e72 4f00 0000  ...).rN...NrO...
+00001030: 7250 0000 0029 0172 6200 0000 2904 7205  rP...).rb...).r.
+00001040: 0000 0072 2f00 0000 7255 0000 00da 076e  ...r/...rU.....n
+00001050: 6461 7272 6179 2904 7222 0000 0072 4d00  darray).r"...rM.
+00001060: 0000 7261 0000 0072 6d00 0000 7220 0000  ..ra...rm...r ..
+00001070: 0029 0572 3700 0000 725d 0000 0072 1f00  .).r7...r]...r..
+00001080: 0000 725f 0000 0072 3800 0000 7221 0000  ..r_...r8...r!..
+00001090: 00da 195f 5f65 7870 6f72 745f 7265 6d6f  ...__export_remo
+000010a0: 7465 5f66 756e 6374 696f 6e73 1200 0000  te_functions....
+000010b0: 731c 0000 0000 0216 0f16 2210 1610 0612  s.........".....
+000010c0: 0612 0908 0418 0a14 0f02 0102 0102 0102  ................
+000010d0: fc72 6f00 0000 291b da08 7761 726e 696e  .ro...)...warnin
+000010e0: 6773 5a11 6e75 6d62 612e 636f 7265 2e65  gsZ.numba.core.e
+000010f0: 7272 6f72 7372 0200 0000 da0e 6669 6c74  rrorsr......filt
+00001100: 6572 7761 726e 696e 6773 da10 6173 6170  erwarnings..asap
+00001110: 6c69 622e 6461 7461 2e78 797a 7205 0000  lib.data.xyzr...
+00001120: 005a 1561 7361 706c 6962 2e63 6c69 2e66  .Z.asaplib.cli.f
+00001130: 756e 635f 6173 6170 7206 0000 0072 0700  unc_asapr....r..
+00001140: 0000 5a19 6173 6170 6c69 622e 6879 7065  ..Z.asaplib.hype
+00001150: 7273 2e68 7970 6572 5f73 6f61 7072 0800  rs.hyper_soapr..
+00001160: 0000 5a19 6173 6170 6c69 622e 6879 7065  ..Z.asaplib.hype
+00001170: 7273 2e68 7970 6572 5f61 6373 6672 0900  rs.hyper_acsfr..
+00001180: 0000 5a1d 6173 6170 6c69 622e 7265 6475  ..Z.asaplib.redu
+00001190: 6365 6469 6d2e 6469 6d5f 7265 6475 6365  cedim.dim_reduce
+000011a0: 7272 0a00 0000 5a1e 6173 6170 6c69 622e  rr....Z.asaplib.
+000011b0: 636c 7573 7465 722e 6d6c 5f63 6c75 7374  cluster.ml_clust
+000011c0: 6572 5f66 6974 720b 0000 0072 0c00 0000  er_fitr....r....
+000011d0: da16 7363 6970 792e 7370 6174 6961 6c2e  ..scipy.spatial.
+000011e0: 6469 7374 616e 6365 720d 0000 00da 056e  distancer......n
+000011f0: 756d 7079 7255 0000 0072 6f00 0000 7222  umpyrU...ro...r"
+00001200: 0000 0072 4d00 0000 7261 0000 0072 6d00  ...rM...ra...rm.
+00001210: 0000 7220 0000 0072 2000 0000 7220 0000  ..r ...r ...r ..
+00001220: 0072 2100 0000 da08 3c6d 6f64 756c 653e  .r!.....<module>
+00001230: 0100 0000 7326 0000 0008 010c 010e 020c  ....s&..........
+00001240: 0110 010c 010c 010c 0110 020c 0208 0408  ................
+00001250: 7f00 0804 fb02 0102 0102 0102 0102 fc    ...............
```

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/cll.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/cll.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/common.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/constant.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/constant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/data.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/data.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/iface.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/iface.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/selector.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/selector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/updater.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/updater.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/util.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/asap.py` & `ai2_kit-0.5.1/ai2_kit/domain/asap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# Suppress numba warning of umap.
+# Ref: https://github.com/lmcinnes/umap/issues/252
+from numba.core.errors import NumbaDeprecationWarning
+import warnings
+warnings.filterwarnings("ignore", category=NumbaDeprecationWarning)
+
 from asaplib.data.xyz import ASAPXYZ
 from asaplib.cli.func_asap import cluster_process, set_reducer
 from asaplib.hypers.hyper_soap import universal_soap_hyper
 from asaplib.hypers.hyper_acsf import universal_acsf_hyper
 from asaplib.reducedim.dim_reducer import Dimension_Reducers
 from asaplib.cluster.ml_cluster_fit import LAIO_DB, sklearn_DB
```

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/constant.py` & `ai2_kit-0.5.1/ai2_kit/domain/constant.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/cp2k.py` & `ai2_kit-0.5.1/ai2_kit/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/data.py` & `ai2_kit-0.5.1/ai2_kit/domain/data.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/deepmd.py` & `ai2_kit-0.5.1/ai2_kit/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/iface.py` & `ai2_kit-0.5.1/ai2_kit/domain/iface.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/lammps.py` & `ai2_kit-0.5.1/ai2_kit/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/lasp.py` & `ai2_kit-0.5.1/ai2_kit/domain/lasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/selector.py` & `ai2_kit-0.5.1/ai2_kit/domain/selector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/util.py` & `ai2_kit-0.5.1/ai2_kit/domain/util.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/domain/vasp.py` & `ai2_kit-0.5.1/ai2_kit/domain/vasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/main.py` & `ai2_kit-0.5.1/ai2_kit/main.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/tool/__pycache__/ase.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/tool/__pycache__/ase.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/tool/ase.py` & `ai2_kit-0.5.1/ai2_kit/tool/ase.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc` & `ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.5.1/ai2_kit/workflow/cll_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.5.1/ai2_kit/workflow/fep_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.0/pyproject.toml` & `ai2_kit-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.5.0"
+version = "0.5.1"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ai2_kit-0.5.0/PKG-INFO` & `ai2_kit-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

