# Comparing `tmp/qiskit-ibm-provider-0.6.1.tar.gz` & `tmp/qiskit-ibm-provider-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ibm-provider-0.6.1.tar", last modified: Mon Jun 12 17:47:35 2023, max compression
+gzip compressed data, was "qiskit-ibm-provider-0.6.2.tar", last modified: Tue Jul 25 19:29:49 2023, max compression
```

## Comparing `qiskit-ibm-provider-0.6.1.tar` & `qiskit-ibm-provider-0.6.2.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.724488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.728488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.728488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/client_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.732488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/runtime_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.732488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/program_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.732488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/utils/data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/apiconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/hub_group_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    39657 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    29933 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_backend_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_qubit_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.736488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31784 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/ibm_circuit_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    48877 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/ibm_composite_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/ibm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/job_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/queueinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/sub_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.736488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/backend_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/config_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.736488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/backend_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/gates_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/jobs_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/qubits_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.740488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/proxies/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/proxies/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.740488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.740488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40086 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)    18670 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/value.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/type_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.740488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.740488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.740488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.744488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23938 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.744488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/backend_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/hgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/json_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/qobj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.744488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/device_layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.748488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/error_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/gate_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.728488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.748488 qiskit-ibm-provider-0.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.748488 qiskit-ibm-provider-0.6.1/test/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/e2e/test_real_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/e2e/test_tutorials.py
--rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/ibm_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.752488 qiskit-ibm-provider-0.6.1/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_basic_server_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    40183 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_composite_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_filter_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_ibm_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_ibm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_ibm_job_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_ibm_qasm_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_websocket_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/jobtestcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/proxy_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.752488 qiskit-ibm-provider-0.6.1/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/test/unit/mock/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/mock/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/mock/fake_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    22540 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/test_ibm_job_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/test_ibm_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/test_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/test/unit/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/control_flow_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
--rw-r--r--   0 runner    (1001) docker     (123)    59873 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/test/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/utils/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/ws_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.675955 qiskit-ibm-provider-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-07-25 19:29:49.675955 qiskit-ibm-provider-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.643955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.647955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.647955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/client_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.647955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/runtime_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.651955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/program_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.651955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/utils/data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/apiconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/hub_group_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40123 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29933 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_backend_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_qubit_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.651955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32106 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/ibm_circuit_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48877 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/ibm_composite_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/ibm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/job_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/queueinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/sub_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.655955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/backend_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/config_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.655955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/backend_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/gates_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/jobs_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/qubits_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.655955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/proxies/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/proxies/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.659955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.659955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46038 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18670 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/type_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.659955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.659955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.659955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.659955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23938 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.663955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/backend_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/hgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/json_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/qobj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.663955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/device_layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.663955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/gate_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.643955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-25 19:29:49.675955 qiskit-ibm-provider-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.667955 qiskit-ibm-provider-0.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.667955 qiskit-ibm-provider-0.6.2/test/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/e2e/test_real_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/e2e/test_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/fake_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/ibm_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.671955 qiskit-ibm-provider-0.6.2/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_basic_server_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40183 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_composite_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_filter_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_ibm_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_ibm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_ibm_job_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_ibm_qasm_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_websocket_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/jobtestcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/proxy_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.671955 qiskit-ibm-provider-0.6.2/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.671955 qiskit-ibm-provider-0.6.2/test/unit/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/mock/fake_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/mock/fake_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22540 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/test_ibm_job_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/test_ibm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/test_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.671955 qiskit-ibm-provider-0.6.2/test/unit/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.671955 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.675955 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.675955 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/control_flow_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59873 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.675955 qiskit-ibm-provider-0.6.2/test/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/utils/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/ws_server.py
```

### Comparing `qiskit-ibm-provider-0.6.1/LICENSE.txt` & `qiskit-ibm-provider-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/PKG-INFO` & `qiskit-ibm-provider-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-provider
-Version: 0.6.1
+Version: 0.6.2
 Summary: Qiskit IBM Quantum Provider for accessing the quantum devices and simulators at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-provider
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-provider/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-provider-0.6.1/README.md` & `qiskit-ibm-provider-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/account.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/exceptions.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/management.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/management.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/storage.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/storage.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/auth.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/client_parameters.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/client_parameters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/account.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/auth.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/base.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/runtime.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/runtime_ws.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/runtime_ws.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/version.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/websocket.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/websocket.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/exceptions.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/backend.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/base.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/job.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/program_job.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/program_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/root.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/root.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/runtime.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         if start_session:
             payload["start_session"] = start_session
         if all([hub, group, project]):
             payload["hub"] = hub
             payload["group"] = group
             payload["project"] = project
         data = json.dumps(payload, cls=RuntimeEncoder)
-        return self.session.post(url, data=data).json()
+        return self.session.post(url, data=data, timeout=900).json()
 
     def jobs_get(
         self,
         limit: int = None,
         skip: int = None,
         pending: bool = None,
         program_id: str = None,
```

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/utils/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/utils/data_mapper.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/utils/data_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/session.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/apiconstants.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/apiconstants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/exceptions.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/hub_group_project.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/hub_group_project.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_backend.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -467,14 +467,18 @@
             if dynamic:
                 program_id = QASM3RUNNERPROGRAMID
             else:
                 program_id = QOBJRUNNERPROGRAMID
         else:
             run_config.pop("program_id", None)
 
+        image: Optional[str] = run_config.get("image", None)  # type: ignore
+        if image is not None:
+            image = str(image)
+
         if isinstance(init_circuit, bool):
             warnings.warn(
                 "init_circuit does not accept boolean values. "
                 "A quantum circuit should be passed in instead."
             )
 
         if isinstance(shots, float):
@@ -509,32 +513,35 @@
             run_config_dict["skip_transpilation"] = True
 
         return self._runtime_run(
             program_id=program_id,
             inputs=run_config_dict,
             options=options,
             job_tags=job_tags,
+            image=image,
         )
 
     def _runtime_run(
         self,
         program_id: str,
         inputs: Dict,
         options: Dict,
         job_tags: Optional[List[str]] = None,
+        image: Optional[str] = None,
     ) -> IBMCircuitJob:
         """Runs the runtime program and returns the corresponding job object"""
         hgp_name = self._instance or self.provider._get_hgp().name
         try:
             response = self.provider._runtime_client.program_run(
                 program_id=program_id,
                 backend_name=options["backend"],
                 params=inputs,
                 hgp=hgp_name,
                 job_tags=job_tags,
+                image=image,
             )
         except RequestsApiError as ex:
             raise IBMBackendApiError("Error submitting job: {}".format(str(ex))) from ex
         try:
             job_id = response["id"]
             job = IBMCircuitJob(
                 backend=self,
@@ -816,14 +823,19 @@
                 - If one of the circuits contains more qubits than on the backend."""
         schedule_error_msg = (
             "Class 'Schedule' is no longer supported as an input circuit. "
             "Use 'pulse gates' instead. See `tutorial "
             "https://qiskit.org/documentation/tutorials/circuits_advanced/05_pulse_gates.html` "
             "on how to use pulse gates."
         )
+        if len(circuits) > self._max_circuits:
+            raise IBMBackendValueError(
+                f"Number of circuits, {len(circuits)} exceeds the "
+                f"maximum for this backend, {self._max_circuits})"
+            )
         for circ in circuits:
             if isinstance(circ, Schedule):
                 raise IBMBackendValueError(schedule_error_msg)
             if isinstance(circ, QuantumCircuit):
                 if circ.num_qubits > self._configuration.num_qubits:
                     raise IBMBackendValueError(
                         f"Circuit contains {circ.num_qubits} qubits, "
```

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_backend_service.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_backend_service.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_provider.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_qubit_properties.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_qubit_properties.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/constants.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/exceptions.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/ibm_circuit_job.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/ibm_circuit_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,14 +599,19 @@
             return [circuits]
         return []
 
     def _get_params(self) -> None:
         """Retrieve job parameters"""
         if not self._params:
             with api_to_job_error():
+                if self._provider._runtime_client.job_type(self.job_id()) == "IQX":
+                    raise IBMJobError(
+                        f"{self.job_id()} is a legacy job. Retrieving parameters of legacy "
+                        f"jobs is not supported from qiskit-ibm-provider"
+                    ) from None
                 api_response = self._runtime_client.job_get(self.job_id())
                 self._params = api_response.get("params", {})
 
     def wait_for_final_state(  # pylint: disable=arguments-differ
         self,
         timeout: Optional[float] = None,
     ) -> None:
```

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/ibm_composite_job.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/ibm_composite_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/ibm_job.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/ibm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/job_monitor.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/job_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/queueinfo.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/queueinfo.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/sub_job.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/sub_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/utils.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/backend_info.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/backend_info.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/config_widget.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/config_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/backend_update.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/backend_update.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/constants.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/dashboard.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/utils.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/gates_widget.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/gates_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/jobs_widget.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/jobs_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/qubits_widget.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/qubits_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/proxies/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/proxies/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/proxies/configuration.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/proxies/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/circuits.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/circuits.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 
 import io
 import json
 import struct
 import uuid
 import warnings
 
+from collections import defaultdict
 import numpy as np
 
 from qiskit import circuit as circuit_mod
 from qiskit import extensions
 from qiskit.circuit import library, controlflow, CircuitInstruction
 from qiskit.circuit.classicalregister import ClassicalRegister, Clbit
 from qiskit.circuit.gate import Gate
 from qiskit.circuit.controlledgate import ControlledGate
 from qiskit.circuit.instruction import Instruction
 from qiskit.circuit.quantumcircuit import QuantumCircuit
 from qiskit.circuit.quantumregister import QuantumRegister, Qubit
 from qiskit.extensions import quantum_initializer
 from qiskit.quantum_info.operators import SparsePauliOp
 from qiskit.synthesis import evolution as evo_synth
+from qiskit.transpiler.layout import Layout, TranspileLayout
 from .. import common, formats, type_keys
 from . import value, schedules
 
 
 def _read_header_v2(  # type: ignore[no-untyped-def]
     file_obj, version, vectors, metadata_deserializer=None
 ):
@@ -294,14 +296,15 @@
     else:
         if gate_name in {
             "Initialize",
             "StatePreparation",
             "UCRXGate",
             "UCRYGate",
             "UCRZGate",
+            "DiagonalGate",
         }:
             gate = gate_class(params)
         else:
             if gate_name == "Barrier":
                 params = [len(qargs)]
             elif gate_name in {"BreakLoopOp", "ContinueLoopOp"}:
                 params = [len(qargs), len(cargs)]
@@ -810,14 +813,156 @@
             for bit in reg:
                 bit_indices.append(bitmap.get(bit, -1))
             file_obj.write(struct.pack(REGISTER_ARRAY_PACK, *bit_indices))
 
     return len(in_circ_regs) + len(out_circ_regs)
 
 
+def _write_layout(file_obj, circuit):  # type: ignore[no-untyped-def]
+    if circuit.layout is None:
+        # Write a null header if there is no layout present
+        file_obj.write(struct.pack(formats.LAYOUT_PACK, False, -1, -1, -1, 0))
+        return
+    initial_size = -1
+    input_qubit_mapping = {}
+    initial_layout_array = []
+    extra_registers = defaultdict(list)
+    if circuit.layout.initial_layout is not None:
+        initial_size = len(circuit.layout.initial_layout)
+        layout_mapping = circuit.layout.initial_layout.get_physical_bits()
+        for i in range(circuit.num_qubits):
+            qubit = layout_mapping[i]
+            input_qubit_mapping[qubit] = i
+            if qubit._register is not None or qubit._index is not None:
+                if qubit._register not in circuit.qregs:
+                    extra_registers[qubit._register].append(qubit)
+                initial_layout_array.append((qubit._index, qubit._register))
+            else:
+                initial_layout_array.append((None, None))
+    input_qubit_size = -1
+    input_qubit_mapping_array = []
+    if circuit.layout.input_qubit_mapping is not None:
+        input_qubit_size = len(circuit.layout.input_qubit_mapping)
+        input_qubit_mapping_array = [None] * input_qubit_size
+        layout_mapping = circuit.layout.initial_layout.get_virtual_bits()
+        for qubit, index in circuit.layout.input_qubit_mapping.items():
+            if (
+                getattr(qubit, "_register", None) is not None
+                and getattr(qubit, "_index", None) is not None
+            ):
+                if qubit._register not in circuit.qregs:
+                    extra_registers[qubit._register].append(qubit)
+                input_qubit_mapping_array[index] = layout_mapping[qubit]
+            else:
+                input_qubit_mapping_array[index] = layout_mapping[qubit]
+    final_layout_size = -1
+    final_layout_array = []
+    if circuit.layout.final_layout is not None:
+        final_layout_size = len(circuit.layout.final_layout)
+        final_layout_physical = circuit.layout.final_layout.get_physical_bits()
+        for i in range(circuit.num_qubits):
+            virtual_bit = final_layout_physical[i]
+            final_layout_array.append(circuit.find_bit(virtual_bit).index)
+
+    file_obj.write(
+        struct.pack(
+            formats.LAYOUT_PACK,
+            True,
+            initial_size,
+            input_qubit_size,
+            final_layout_size,
+            len(extra_registers),
+        )
+    )
+    _write_registers(
+        file_obj,
+        list(extra_registers),
+        [x for bits in extra_registers.values() for x in bits],
+    )
+    for index, register in initial_layout_array:
+        reg_name_bytes = (
+            None if register is None else register.name.encode(common.ENCODE)
+        )
+        file_obj.write(
+            struct.pack(
+                formats.INITIAL_LAYOUT_BIT_PACK,
+                -1 if index is None else index,
+                -1 if reg_name_bytes is None else len(reg_name_bytes),
+            )
+        )
+        if reg_name_bytes is not None:
+            file_obj.write(reg_name_bytes)
+    for i in input_qubit_mapping_array:
+        file_obj.write(struct.pack("!I", i))
+    for i in final_layout_array:
+        file_obj.write(struct.pack("!I", i))
+
+
+def _read_layout(file_obj, circuit):  # type: ignore[no-untyped-def]
+    header = formats.LAYOUT._make(
+        struct.unpack(formats.LAYOUT_PACK, file_obj.read(formats.LAYOUT_SIZE))
+    )
+    if not header.exists:
+        return
+    registers = {
+        name: QuantumRegister(len(v[1]), name)
+        for name, v in _read_registers_v4(file_obj, header.extra_registers)["q"].items()
+    }
+    initial_layout = None
+    initial_layout_virtual_bits = []
+    for _ in range(header.initial_layout_size):
+        virtual_bit = formats.INITIAL_LAYOUT_BIT._make(
+            struct.unpack(
+                formats.INITIAL_LAYOUT_BIT_PACK,
+                file_obj.read(formats.INITIAL_LAYOUT_BIT_SIZE),
+            )
+        )
+        if virtual_bit.index == -1 and virtual_bit.register_size == -1:
+            qubit = Qubit()
+        else:
+            register_name = file_obj.read(virtual_bit.register_size).decode(
+                common.ENCODE
+            )
+            if register_name in registers:
+                qubit = registers[register_name][virtual_bit.index]
+            else:
+                register = next(
+                    filter(lambda x, name=register_name: x.name == name, circuit.qregs)
+                )
+                qubit = register[virtual_bit.index]
+        initial_layout_virtual_bits.append(qubit)
+    if initial_layout_virtual_bits:
+        initial_layout = Layout.from_qubit_list(initial_layout_virtual_bits)
+    input_qubit_mapping = None
+    input_qubit_mapping_array = []
+    for _ in range(header.input_mapping_size):
+        input_qubit_mapping_array.append(
+            struct.unpack("!I", file_obj.read(struct.calcsize("!I")))[0]
+        )
+    if input_qubit_mapping_array:
+        input_qubit_mapping = {}
+        physical_bits = initial_layout.get_physical_bits()
+        for index, bit in enumerate(input_qubit_mapping_array):
+            input_qubit_mapping[physical_bits[bit]] = index
+    final_layout = None
+    final_layout_array = []
+    for _ in range(header.final_layout_size):
+        final_layout_array.append(
+            struct.unpack("!I", file_obj.read(struct.calcsize("!I")))[0]
+        )
+
+    if final_layout_array:
+        layout_dict = {
+            circuit.qubits[bit]: index for index, bit in enumerate(final_layout_array)
+        }
+        final_layout = Layout(layout_dict)
+
+    circuit._layout = TranspileLayout(initial_layout, input_qubit_mapping, final_layout)
+
+
 def write_circuit(file_obj, circuit, metadata_serializer=None):  # type: ignore[no-untyped-def]
     """Write a single QuantumCircuit object in the file like object.
 
     Args:
         file_obj (FILE): The file like object to write the circuit data in.
         circuit (QuantumCircuit): The circuit data to write.
         metadata_serializer (JSONEncoder): An optional JSONEncoder class that
@@ -883,14 +1028,15 @@
         file_obj.write(custom_operations_buffer.getvalue())
 
     file_obj.write(instruction_buffer.getvalue())
     instruction_buffer.close()
 
     # Write calibrations
     _write_calibrations(file_obj, circuit.calibrations, metadata_serializer)
+    _write_layout(file_obj, circuit)
 
 
 def read_circuit(file_obj, version, metadata_deserializer=None):  # type: ignore[no-untyped-def]
     """Read a single QuantumCircuit object from the file like object.
 
     Args:
         file_obj (FILE): The file like object to read the circuit data from.
@@ -1016,9 +1162,10 @@
                 f"The ParameterVector: '{vec_name}' is not fully identical to its "
                 "pre-serialization state. Elements "
                 f"{', '.join([str(x) for x in set(range(len(vector))) - initialized_params])} "
                 "in the ParameterVector will be not equal to the pre-serialized ParameterVector "
                 f"as they weren't used in the circuit: {circ.name}",
                 UserWarning,
             )
-
+    if version >= 8:
+        _read_layout(file_obj, circ)
     return circ
```

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/schedules.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/schedules.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/value.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/value.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/common.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 
 import io
 import struct
 
 from . import formats
 
-QPY_VERSION = 7
+QPY_VERSION = 8
 ENCODE = "utf8"
 
 
 def read_generic_typed_data(file_obj):  # type: ignore[no-untyped-def]
     """Read a single data chunk from the file like object.
 
     Args:
```

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/exceptions.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/formats.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/formats.py`

 * *Files 4% similar despite different names*

```diff
@@ -271,7 +271,24 @@
 SEQUENCE_PACK = "!Q"
 SEQUENCE_SIZE = struct.calcsize(SEQUENCE_PACK)
 
 # MAP_ITEM
 MAP_ITEM = namedtuple("MAP_ITEM", ["key_size", "type", "size"])
 MAP_ITEM_PACK = "!H1cH"
 MAP_ITEM_SIZE = struct.calcsize(MAP_ITEM_PACK)
+
+LAYOUT = namedtuple(
+    "LAYOUT",
+    [
+        "exists",
+        "initial_layout_size",
+        "input_mapping_size",
+        "final_layout_size",
+        "extra_registers",
+    ],
+)
+LAYOUT_PACK = "!?iiiI"
+LAYOUT_SIZE = struct.calcsize(LAYOUT_PACK)
+
+INITIAL_LAYOUT_BIT = namedtuple("INITIAL_LAYOUT_BIT", ["index", "register_size"])
+INITIAL_LAYOUT_BIT_PACK = "!ii"
+INITIAL_LAYOUT_BIT_SIZE = struct.calcsize(INITIAL_LAYOUT_BIT_PACK)
```

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/interface.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/interface.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/type_keys.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/type_keys.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/basis/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/plugin.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/plugin.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/backend_decoder.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/backend_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/converters.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/converters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/hgp.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/hgp.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/json.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/json.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/json_decoder.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/json_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,39 +7,39 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Custom JSON decoder."""
-from typing import Dict, Tuple, Union, List, Any, Optional
 import json
 import logging
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import dateutil.parser
+from qiskit.circuit.controlflow import ForLoopOp, IfElseOp, SwitchCaseOp, WhileLoopOp
+from qiskit.circuit.gate import Gate, Instruction
+from qiskit.circuit.library.standard_gates import get_standard_gate_name_mapping
+from qiskit.circuit.parameter import Parameter
 from qiskit.providers.models import (
-    QasmBackendConfiguration,
-    PulseBackendConfiguration,
-    PulseDefaults,
     BackendProperties,
     Command,
+    PulseBackendConfiguration,
+    PulseDefaults,
+    QasmBackendConfiguration,
 )
 from qiskit.providers.models.backendproperties import Gate as GateSchema
-from qiskit.circuit.controlflow import IfElseOp, WhileLoopOp, ForLoopOp
-from qiskit.circuit.gate import Gate, Instruction
-from qiskit.circuit.parameter import Parameter
-from qiskit.circuit.library.standard_gates import get_standard_gate_name_mapping
 from qiskit.pulse.calibration_entries import PulseQobjDef
-from qiskit.transpiler.target import Target, InstructionProperties
-from qiskit.qobj.pulse_qobj import PulseLibraryItem
 from qiskit.qobj.converters.pulse_instruction import QobjToInstructionConverter
+from qiskit.qobj.pulse_qobj import PulseLibraryItem
+from qiskit.transpiler.target import InstructionProperties, Target
 from qiskit.utils import apply_prefix
 
-from .converters import utc_to_local, utc_to_local_all
 from ..ibm_qubit_properties import IBMQubitProperties
+from .converters import utc_to_local, utc_to_local_all
 
 logger = logging.getLogger(__name__)
 
 
 def defaults_from_server_data(defaults: Dict) -> PulseDefaults:
     """Decode pulse defaults data.
 
@@ -107,14 +107,15 @@
 
     # Load Qiskit object representation
     qiskit_inst_mapping = get_standard_gate_name_mapping()
     qiskit_control_flow_mapping = {
         "if_else": IfElseOp,
         "while_loop": WhileLoopOp,
         "for_loop": ForLoopOp,
+        "switch_case": SwitchCaseOp,
     }
 
     in_data = {"num_qubits": configuration.n_qubits}
 
     # Parse global configuration properties
     if hasattr(configuration, "dt"):
         in_data["dt"] = configuration.dt
```

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/json_encoder.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/options.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/qobj_utils.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/qobj_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/utils.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/version.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/colormaps.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/colormaps.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/device_layouts.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/device_layouts.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/exceptions.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/__init__.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/error_map.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/error_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/gate_map.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/gate_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/PKG-INFO` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-provider
-Version: 0.6.1
+Version: 0.6.2
 Summary: Qiskit IBM Quantum Provider for accessing the quantum devices and simulators at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-provider
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-provider/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/SOURCES.txt` & `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/setup.cfg` & `qiskit-ibm-provider-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/setup.py` & `qiskit-ibm-provider-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Setup qiskit_ibm_provider"""
 
 import os
 
 import setuptools
 
 REQUIREMENTS = [
-    "qiskit-terra>=0.24.0",
+    "qiskit-terra>=0.24.2",
     "requests>=2.19",
     "requests-ntlm>=1.1.0",
     "numpy>=1.13",
     "urllib3>=1.21.1",
     "python-dateutil>=2.8.0",
     "websocket-client>=1.5.1",
     "websockets>=10.0",
```

### Comparing `qiskit-ibm-provider-0.6.1/test/__init__.py` & `qiskit-ibm-provider-0.6.2/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/account.py` & `qiskit-ibm-provider-0.6.2/test/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/contextmanagers.py` & `qiskit-ibm-provider-0.6.2/test/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/decorators.py` & `qiskit-ibm-provider-0.6.2/test/decorators.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/e2e/test_real_devices.py` & `qiskit-ibm-provider-0.6.2/test/e2e/test_real_devices.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/e2e/test_tutorials.py` & `qiskit-ibm-provider-0.6.2/test/e2e/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/fake_account_client.py` & `qiskit-ibm-provider-0.6.2/test/fake_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/http_server.py` & `qiskit-ibm-provider-0.6.2/test/http_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/ibm_test_case.py` & `qiskit-ibm-provider-0.6.2/test/ibm_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_account_client.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_backend.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_basic_server_paths.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_basic_server_paths.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_composite_job.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_composite_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_filter_backends.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_filter_backends.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_ibm_integration.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_ibm_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_ibm_job.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_ibm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_ibm_job_attributes.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_ibm_job_attributes.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_ibm_provider.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_ibm_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_ibm_qasm_simulator.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_ibm_qasm_simulator.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_jupyter.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_proxies.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_proxies.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_serialization.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/integration/test_websocket_integration.py` & `qiskit-ibm-provider-0.6.2/test/integration/test_websocket_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/jobtestcase.py` & `qiskit-ibm-provider-0.6.2/test/jobtestcase.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/proxy_server.py` & `qiskit-ibm-provider-0.6.2/test/proxy_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/mock/fake_account_client.py` & `qiskit-ibm-provider-0.6.2/test/unit/mock/fake_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/mock/fake_provider.py` & `qiskit-ibm-provider-0.6.2/test/unit/mock/fake_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/test_account.py` & `qiskit-ibm-provider-0.6.2/test/unit/test_account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/test_backend.py` & `qiskit-ibm-provider-0.6.2/test/unit/test_backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import warnings
 
 from qiskit import transpile, qasm3, QuantumCircuit
 from qiskit.providers.fake_provider import FakeManila
 from qiskit.providers.models import BackendStatus, BackendProperties
 
 from qiskit_ibm_provider.ibm_backend import IBMBackend
+from qiskit_ibm_provider.exceptions import IBMBackendValueError
 
 from ..ibm_test_case import IBMTestCase
 
 
 class TestBackend(IBMTestCase):
     """Tests for IBMBackend class."""
 
@@ -296,31 +297,70 @@
         qasm3_circ = qasm3.dumps(circ, disable_constants=True)
 
         with mock.patch.object(IBMBackend, "_runtime_run") as mock_run:
             backend.run(circuits=qasm3_circ, dynamic=True)
 
         mock_run.assert_called_once()
 
+    def test_runtime_image_selection_submission(self):
+        """Test image selection from runtime"""
+        # pylint: disable=not-context-manager
+
+        backend = self._create_dc_test_backend()
+
+        circ = QuantumCircuit(2, 2)
+        circ.measure(0, 0)
+        with circ.if_test((0, False)):
+            circ.x(1)
+
+        with mock.patch.object(IBMBackend, "_runtime_run") as mock_run:
+            backend.run(circuits=circ, dynamic=True)
+
+        mock_run.assert_called_once()
+
     def test_multi_openqasm3_submission(self):
         """Test submitting multiple openqasm3 strings with dynamic=True"""
         # pylint: disable=not-context-manager
 
         backend = self._create_dc_test_backend()
 
         circ = QuantumCircuit(2, 2)
         circ.measure(0, 0)
         with circ.if_test((0, False)):
             circ.x(1)
 
-        qasm3_circ = qasm3.dumps(circ, disable_constants=True)
-        qasm3_circs = [qasm3_circ, qasm3_circ]
+        image = "test-image"
 
         with mock.patch.object(IBMBackend, "_runtime_run") as mock_run:
-            backend.run(circuits=qasm3_circs, dynamic=True)
+            backend.run(circuits=circ, dynamic=True, image=image)
 
         mock_run.assert_called_once()
+        self.assertEqual(mock_run.call_args.kwargs["image"], image)
 
     def test_deepcopy(self):
         """Test that deepcopy of a backend works properly"""
         backend = self._create_dc_test_backend()
         backend_copy = copy.deepcopy(backend)
         self.assertEqual(backend_copy.name, backend.name)
+
+    def test_too_many_circuits(self):
+        """Test exception when number of circuits exceeds backend._max_circuits"""
+        model_backend = FakeManila()
+        backend = IBMBackend(
+            configuration=model_backend.configuration(),
+            provider=mock.MagicMock(),
+            api_client=None,
+            instance=None,
+        )
+        max_circs = backend.configuration().max_experiments
+
+        circs = []
+        for _ in range(max_circs + 1):
+            circ = QuantumCircuit(1)
+            circ.x(0)
+            circs.append(circ)
+        with self.assertRaises(IBMBackendValueError) as err:
+            backend.run(circs)
+        self.assertIn(
+            f"Number of circuits, {max_circs+1} exceeds the maximum for this backend, {max_circs}",
+            str(err.exception),
+        )
```

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/test_ibm_job_states.py` & `qiskit-ibm-provider-0.6.2/test/unit/test_ibm_job_states.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/test_ibm_logger.py` & `qiskit-ibm-provider-0.6.2/test/unit/test_ibm_logger.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/test_serialization.py` & `qiskit-ibm-provider-0.6.2/test/unit/test_serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/test_websocket.py` & `qiskit-ibm-provider-0.6.2/test/unit/test_websocket.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py` & `qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/control_flow_test_case.py` & `qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/control_flow_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py` & `qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/test_scheduler.py` & `qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/test_utils.py` & `qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/test_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/unit/utils/ws_handler.py` & `qiskit-ibm-provider-0.6.2/test/unit/utils/ws_handler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/utils.py` & `qiskit-ibm-provider-0.6.2/test/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.1/test/ws_server.py` & `qiskit-ibm-provider-0.6.2/test/ws_server.py`

 * *Files identical despite different names*

