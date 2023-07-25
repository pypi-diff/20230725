# Comparing `tmp/ai2_kit-0.5.1.tar.gz` & `tmp/ai2_kit-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.5.1.tar", max compression
+gzip compressed data, was "ai2_kit-0.5.2.tar", max compression
```

## Comparing `ai2_kit-0.5.1.tar` & `ai2_kit-0.5.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.5.1/LICENSE
--rw-r--r--   0        0        0     2012 2023-07-21 03:28:16.683182 ai2_kit-0.5.1/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.1/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.5.1/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0      144 2023-06-15 02:12:13.145370 ai2_kit-0.5.1/ai2_kit/algorithm/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9573 2023-06-15 02:12:13.155370 ai2_kit-0.5.1/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc
--rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.5.1/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.1/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0      139 2023-02-14 03:43:41.260120 ai2_kit-0.5.1/ai2_kit/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2243 2023-07-20 03:31:49.016223 ai2_kit-0.5.1/ai2_kit/core/__pycache__/artifact.cpython-39.pyc
--rw-r--r--   0        0        0     5928 2023-07-20 03:31:48.996223 ai2_kit-0.5.1/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc
--rw-r--r--   0        0        0      512 2023-06-15 07:55:24.192005 ai2_kit-0.5.1/ai2_kit/core/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0     7307 2023-07-24 07:57:09.456574 ai2_kit-0.5.1/ai2_kit/core/__pycache__/connector.cpython-39.pyc
--rw-r--r--   0        0        0     9586 2023-07-24 09:28:27.095300 ai2_kit-0.5.1/ai2_kit/core/__pycache__/executor.cpython-39.pyc
--rw-r--r--   0        0        0      894 2023-06-29 05:30:14.695752 ai2_kit-0.5.1/ai2_kit/core/__pycache__/future.cpython-39.pyc
--rw-r--r--   0        0        0     2847 2023-07-20 03:31:48.996223 ai2_kit-0.5.1/ai2_kit/core/__pycache__/job.cpython-39.pyc
--rw-r--r--   0        0        0      436 2023-06-29 05:30:14.695752 ai2_kit-0.5.1/ai2_kit/core/__pycache__/log.cpython-39.pyc
--rw-r--r--   0        0        0    10069 2023-07-21 03:41:53.042985 ai2_kit-0.5.1/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc
--rw-r--r--   0        0        0     3063 2023-07-20 03:31:49.026223 ai2_kit-0.5.1/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc
--rw-r--r--   0        0        0     2611 2023-07-21 03:41:53.282985 ai2_kit-0.5.1/ai2_kit/core/__pycache__/script.cpython-39.pyc
--rw-r--r--   0        0        0     8116 2023-07-24 09:28:27.215300 ai2_kit-0.5.1/ai2_kit/core/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.5.1/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     5894 2023-07-25 01:13:41.843210 ai2_kit-0.5.1/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.5.1/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-07-21 04:37:23.322249 ai2_kit-0.5.1/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     8006 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/core/executor.py
--rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.5.1/ai2_kit/core/future.py
--rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.5.1/ai2_kit/core/job.py
--rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.5.1/ai2_kit/core/log.py
--rw-r--r--   0        0        0     9587 2023-07-21 01:27:23.144801 ai2_kit-0.5.1/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.5.1/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2363 2023-07-21 01:27:23.144801 ai2_kit-0.5.1/ai2_kit/core/script.py
--rw-r--r--   0        0        0     5900 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.1/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0      110 2023-06-15 07:55:24.202005 ai2_kit-0.5.1/ai2_kit/dflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.1/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0      141 2023-02-14 03:43:41.670121 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4703 2023-07-25 00:52:37.103514 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/asap.cpython-39.pyc
--rw-r--r--   0        0        0     2517 2023-06-29 05:30:14.805753 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/cll.cpython-39.pyc
--rw-r--r--   0        0        0     3221 2023-02-23 07:10:20.489990 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/common.cpython-39.pyc
--rw-r--r--   0        0        0     1532 2023-07-24 09:28:27.285300 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/constant.cpython-39.pyc
--rw-r--r--   0        0        0     5609 2023-07-21 03:41:53.572985 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc
--rw-r--r--   0        0        0     5117 2023-07-24 09:28:27.245300 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/data.cpython-39.pyc
--rw-r--r--   0        0        0     6200 2023-06-27 02:27:16.171507 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc
--rw-r--r--   0        0        0     6358 2023-07-21 03:41:53.282985 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc
--rw-r--r--   0        0        0     2519 2023-07-20 03:31:49.026223 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/iface.cpython-39.pyc
--rw-r--r--   0        0        0    12264 2023-07-21 03:41:53.392985 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc
--rw-r--r--   0        0        0     9323 2023-07-24 09:28:27.295300 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc
--rw-r--r--   0        0        0    10687 2023-07-24 09:28:27.305300 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/selector.cpython-39.pyc
--rw-r--r--   0        0        0      538 2023-07-21 03:41:53.862985 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/updater.cpython-39.pyc
--rw-r--r--   0        0        0     3360 2023-07-24 08:47:10.485875 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     6463 2023-07-21 03:41:53.572985 ai2_kit-0.5.1/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc
--rw-r--r--   0        0        0     5449 2023-07-25 00:53:24.333505 ai2_kit-0.5.1/ai2_kit/domain/asap.py
--rw-r--r--   0        0        0     1805 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     6585 2023-07-21 01:27:23.144801 ai2_kit-0.5.1/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     5454 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/domain/data.py
--rw-r--r--   0        0        0     7895 2023-07-21 01:27:23.144801 ai2_kit-0.5.1/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.5.1/ai2_kit/domain/iface.py
--rw-r--r--   0        0        0    17292 2023-07-25 01:07:27.943305 ai2_kit-0.5.1/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     9046 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/domain/lasp.py
--rw-r--r--   0        0        0    13582 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      186 2023-07-21 01:27:23.144801 ai2_kit-0.5.1/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     6882 2023-07-24 08:46:11.435884 ai2_kit-0.5.1/ai2_kit/domain/util.py
--rw-r--r--   0        0        0     7678 2023-07-21 01:27:23.144801 ai2_kit-0.5.1/ai2_kit/domain/vasp.py
--rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.5.1/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.1/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0      139 2023-06-28 08:15:51.392260 ai2_kit-0.5.1/ai2_kit/tool/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1616 2023-06-28 08:15:51.392260 ai2_kit-0.5.1/ai2_kit/tool/__pycache__/ase.cpython-39.pyc
--rw-r--r--   0        0        0     1039 2023-07-07 01:23:16.068582 ai2_kit-0.5.1/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.1/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0      143 2023-02-14 03:43:41.260120 ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7937 2023-07-24 09:28:27.095300 ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc
--rw-r--r--   0        0        0     5996 2023-06-15 08:55:37.729603 ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc
--rw-r--r--   0        0        0     5966 2023-02-14 03:43:41.260120 ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc
--rw-r--r--   0        0        0     6336 2023-07-20 03:31:49.786223 ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc
--rw-r--r--   0        0        0    10064 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     9135 2023-07-24 09:25:32.885347 ai2_kit-0.5.1/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0      953 2023-07-25 01:36:42.212881 ai2_kit-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 ai2_kit-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2012 2023-07-21 03:28:16.683182 ai2_kit-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.2/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.5.2/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-15 02:12:13.145370 ai2_kit-0.5.2/ai2_kit/algorithm/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9573 2023-06-15 02:12:13.155370 ai2_kit-0.5.2/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc
+-rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.5.2/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.2/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0      139 2023-02-14 03:43:41.260120 ai2_kit-0.5.2/ai2_kit/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2243 2023-07-20 03:31:49.016223 ai2_kit-0.5.2/ai2_kit/core/__pycache__/artifact.cpython-39.pyc
+-rw-r--r--   0        0        0     5928 2023-07-20 03:31:48.996223 ai2_kit-0.5.2/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc
+-rw-r--r--   0        0        0      512 2023-06-15 07:55:24.192005 ai2_kit-0.5.2/ai2_kit/core/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0     7307 2023-07-24 07:57:09.456574 ai2_kit-0.5.2/ai2_kit/core/__pycache__/connector.cpython-39.pyc
+-rw-r--r--   0        0        0     9586 2023-07-24 09:28:27.095300 ai2_kit-0.5.2/ai2_kit/core/__pycache__/executor.cpython-39.pyc
+-rw-r--r--   0        0        0      894 2023-06-29 05:30:14.695752 ai2_kit-0.5.2/ai2_kit/core/__pycache__/future.cpython-39.pyc
+-rw-r--r--   0        0        0     2847 2023-07-20 03:31:48.996223 ai2_kit-0.5.2/ai2_kit/core/__pycache__/job.cpython-39.pyc
+-rw-r--r--   0        0        0      436 2023-06-29 05:30:14.695752 ai2_kit-0.5.2/ai2_kit/core/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0    10069 2023-07-21 03:41:53.042985 ai2_kit-0.5.2/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc
+-rw-r--r--   0        0        0     3063 2023-07-20 03:31:49.026223 ai2_kit-0.5.2/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc
+-rw-r--r--   0        0        0     2611 2023-07-21 03:41:53.282985 ai2_kit-0.5.2/ai2_kit/core/__pycache__/script.cpython-39.pyc
+-rw-r--r--   0        0        0     8116 2023-07-24 09:28:27.215300 ai2_kit-0.5.2/ai2_kit/core/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.5.2/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     5894 2023-07-25 01:13:41.843210 ai2_kit-0.5.2/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.5.2/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-07-21 04:37:23.322249 ai2_kit-0.5.2/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     8006 2023-07-24 09:25:32.885347 ai2_kit-0.5.2/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.5.2/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.5.2/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.5.2/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     9587 2023-07-21 01:27:23.144801 ai2_kit-0.5.2/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.5.2/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2363 2023-07-21 01:27:23.144801 ai2_kit-0.5.2/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     5900 2023-07-24 09:25:32.885347 ai2_kit-0.5.2/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.2/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0      110 2023-06-15 07:55:24.202005 ai2_kit-0.5.2/ai2_kit/dflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.2/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0      141 2023-02-14 03:43:41.670121 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4703 2023-07-25 00:52:37.103514 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/asap.cpython-39.pyc
+-rw-r--r--   0        0        0     2517 2023-06-29 05:30:14.805753 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/cll.cpython-39.pyc
+-rw-r--r--   0        0        0     3221 2023-02-23 07:10:20.489990 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0        0        0     1532 2023-07-24 09:28:27.285300 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/constant.cpython-39.pyc
+-rw-r--r--   0        0        0     5609 2023-07-21 03:41:53.572985 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc
+-rw-r--r--   0        0        0     5117 2023-07-24 09:28:27.245300 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/data.cpython-39.pyc
+-rw-r--r--   0        0        0     6200 2023-06-27 02:27:16.171507 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc
+-rw-r--r--   0        0        0     6358 2023-07-21 03:41:53.282985 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc
+-rw-r--r--   0        0        0     2519 2023-07-20 03:31:49.026223 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/iface.cpython-39.pyc
+-rw-r--r--   0        0        0    12264 2023-07-21 03:41:53.392985 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc
+-rw-r--r--   0        0        0     9323 2023-07-24 09:28:27.295300 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc
+-rw-r--r--   0        0        0    10687 2023-07-24 09:28:27.305300 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/selector.cpython-39.pyc
+-rw-r--r--   0        0        0      538 2023-07-21 03:41:53.862985 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/updater.cpython-39.pyc
+-rw-r--r--   0        0        0     3360 2023-07-24 08:47:10.485875 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     6463 2023-07-21 03:41:53.572985 ai2_kit-0.5.2/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc
+-rw-r--r--   0        0        0     5449 2023-07-25 00:53:24.333505 ai2_kit-0.5.2/ai2_kit/domain/asap.py
+-rw-r--r--   0        0        0     1805 2023-07-24 09:25:32.885347 ai2_kit-0.5.2/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     6585 2023-07-21 01:27:23.144801 ai2_kit-0.5.2/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     5454 2023-07-24 09:25:32.885347 ai2_kit-0.5.2/ai2_kit/domain/data.py
+-rw-r--r--   0        0        0     7895 2023-07-25 02:20:46.132275 ai2_kit-0.5.2/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.5.2/ai2_kit/domain/iface.py
+-rw-r--r--   0        0        0    17292 2023-07-25 01:07:27.943305 ai2_kit-0.5.2/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     9046 2023-07-24 09:25:32.885347 ai2_kit-0.5.2/ai2_kit/domain/lasp.py
+-rw-r--r--   0        0        0    13582 2023-07-24 09:25:32.885347 ai2_kit-0.5.2/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      186 2023-07-21 01:27:23.144801 ai2_kit-0.5.2/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     6882 2023-07-24 08:46:11.435884 ai2_kit-0.5.2/ai2_kit/domain/util.py
+-rw-r--r--   0        0        0     7759 2023-07-25 02:20:48.862274 ai2_kit-0.5.2/ai2_kit/domain/vasp.py
+-rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.5.2/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.2/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0      139 2023-06-28 08:15:51.392260 ai2_kit-0.5.2/ai2_kit/tool/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1616 2023-06-28 08:15:51.392260 ai2_kit-0.5.2/ai2_kit/tool/__pycache__/ase.cpython-39.pyc
+-rw-r--r--   0        0        0     1039 2023-07-07 01:23:16.068582 ai2_kit-0.5.2/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.2/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0      143 2023-02-14 03:43:41.260120 ai2_kit-0.5.2/ai2_kit/workflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7937 2023-07-24 09:28:27.095300 ai2_kit-0.5.2/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc
+-rw-r--r--   0        0        0     5996 2023-06-15 08:55:37.729603 ai2_kit-0.5.2/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc
+-rw-r--r--   0        0        0     5966 2023-02-14 03:43:41.260120 ai2_kit-0.5.2/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc
+-rw-r--r--   0        0        0     6336 2023-07-20 03:31:49.786223 ai2_kit-0.5.2/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc
+-rw-r--r--   0        0        0    10064 2023-07-24 09:25:32.885347 ai2_kit-0.5.2/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     9135 2023-07-24 09:25:32.885347 ai2_kit-0.5.2/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      953 2023-07-25 02:21:11.212269 ai2_kit-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 ai2_kit-0.5.2/PKG-INFO
```

### Comparing `ai2_kit-0.5.1/LICENSE` & `ai2_kit-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/README.md` & `ai2_kit-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.5.2/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/__pycache__/artifact.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/core/__pycache__/artifact.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/__pycache__/cmd.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/core/__pycache__/cmd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/__pycache__/connector.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/core/__pycache__/connector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/__pycache__/executor.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/core/__pycache__/executor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/__pycache__/future.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/core/__pycache__/future.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/__pycache__/job.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/core/__pycache__/job.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/__pycache__/script.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/core/__pycache__/script.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/__pycache__/util.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/core/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/artifact.py` & `ai2_kit-0.5.2/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/checkpoint.py` & `ai2_kit-0.5.2/ai2_kit/core/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/connector.py` & `ai2_kit-0.5.2/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/executor.py` & `ai2_kit-0.5.2/ai2_kit/core/executor.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/job.py` & `ai2_kit-0.5.2/ai2_kit/core/job.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/queue_system.py` & `ai2_kit-0.5.2/ai2_kit/core/queue_system.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/resource_manager.py` & `ai2_kit-0.5.2/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/script.py` & `ai2_kit-0.5.2/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/core/util.py` & `ai2_kit-0.5.2/ai2_kit/core/util.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/asap.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/asap.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/cll.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/cll.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/common.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/constant.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/constant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/data.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/data.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/iface.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/iface.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/selector.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/selector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/updater.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/updater.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/util.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/asap.py` & `ai2_kit-0.5.2/ai2_kit/domain/asap.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/constant.py` & `ai2_kit-0.5.2/ai2_kit/domain/constant.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/cp2k.py` & `ai2_kit-0.5.2/ai2_kit/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/data.py` & `ai2_kit-0.5.2/ai2_kit/domain/data.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/deepmd.py` & `ai2_kit-0.5.2/ai2_kit/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/iface.py` & `ai2_kit-0.5.2/ai2_kit/domain/iface.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/lammps.py` & `ai2_kit-0.5.2/ai2_kit/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/lasp.py` & `ai2_kit-0.5.2/ai2_kit/domain/lasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/selector.py` & `ai2_kit-0.5.2/ai2_kit/domain/selector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/util.py` & `ai2_kit-0.5.2/ai2_kit/domain/util.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/domain/vasp.py` & `ai2_kit-0.5.2/ai2_kit/domain/vasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,20 +181,21 @@
             input_data = dict_nested_get(
                 file, ['attrs', 'vasp', 'input_data'], input_data # type: ignore
             )
             incar = Incar.from_dict(input_data)
             incar.write_file(os.path.join(task_dir, 'INCAR'))
 
             # create POSCAR
-            elements_all = atoms.get_chemical_symbols()
+            atoms = atoms[atoms.numbers.argsort()]
+            elements_all = atoms.get_chemical_symbols() # type: ignore
             elements = [
                 item[0] for item in _symbol_count_from_symbols(elements_all)
             ]
             ase.io.write(
-                os.path.join(task_dir, 'POSCAR'), atoms, format='vasp'
+                os.path.join(task_dir, 'POSCAR'), atoms, format='vasp' # type: ignore
             )
 
             # create POTCAR
             with open(os.path.join(task_dir, 'POTCAR'), 'w') as out_file:
                 for element in elements:
                     with open(potcar_source[element], 'r') as in_file:
                         out_file.write(in_file.read())
```

### Comparing `ai2_kit-0.5.1/ai2_kit/main.py` & `ai2_kit-0.5.2/ai2_kit/main.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/tool/__pycache__/ase.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/tool/__pycache__/ase.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/tool/ase.py` & `ai2_kit-0.5.2/ai2_kit/tool/ase.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc` & `ai2_kit-0.5.2/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.5.2/ai2_kit/workflow/cll_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.5.2/ai2_kit/workflow/fep_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.1/pyproject.toml` & `ai2_kit-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ai2_kit-0.5.1/PKG-INFO` & `ai2_kit-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

