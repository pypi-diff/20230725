# Comparing `tmp/lava_nc-0.7.0.post2.tar.gz` & `tmp/lava_nc-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lava_nc-0.7.0.post2.tar", max compression
+gzip compressed data, was "lava_nc-0.8.0.tar", max compression
```

## Comparing `lava_nc-0.7.0.post2.tar` & `lava_nc-0.8.0.tar`

### file list

```diff
@@ -1,225 +1,263 @@
--rw-r--r--   0        0        0      333 2023-05-03 16:57:46.490211 lava_nc-0.7.0.post2/LICENSE
--rw-r--r--   0        0        0     4767 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/pyproject.toml
--rw-r--r--   0        0        0    26529 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/LICENSE
--rw-r--r--   0        0        0     5550 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/builders/channel_builder.py
--rw-r--r--   0        0        0     4236 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/builders/interfaces.py
--rw-r--r--   0        0        0    15527 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/builders/py_builder.py
--rw-r--r--   0        0        0     4937 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/builders/runtimeservice_builder.py
--rw-r--r--   0        0        0     4607 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/channel_map.py
--rw-r--r--   0        0        0     1372 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/channels/interfaces.py
--rw-r--r--   0        0        0    10521 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/channels/pypychannel.py
--rw-r--r--   0        0        0    35450 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/compiler.py
--rw-r--r--   0        0        0    44872 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/compiler_graphs.py
--rw-r--r--   0        0        0     1550 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/compiler_utils.py
--rw-r--r--   0        0        0      573 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/exceptions.py
--rw-r--r--   0        0        0     1778 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/executable.py
--rw-r--r--   0        0        0      721 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/mappable_interface.py
--rw-r--r--   0        0        0     7583 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/mapper.py
--rw-r--r--   0        0        0     2250 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/node.py
--rw-r--r--   0        0        0      514 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/address.py
--rw-r--r--   0        0        0    10380 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/channel_builders_factory.py
--rw-r--r--   0        0        0     2390 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/channel_map_updater.py
--rw-r--r--   0        0        0      696 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/constants.py
--rw-r--r--   0        0        0      769 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/exceptions.py
--rw-r--r--   0        0        0     2086 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/interfaces.py
--rw-r--r--   0        0        0     7543 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/py/pyproc_compiler.py
--rw-r--r--   0        0        0     4153 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/utils.py
--rw-r--r--   0        0        0     5711 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/compiler/var_model.py
--rw-r--r--   0        0        0     1525 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/LICENSE
--rw-r--r--   0        0        0     1613 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/callback_fx.py
--rw-r--r--   0        0        0     6408 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/decorator.py
--rw-r--r--   0        0        0     1999 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/learning/constants.py
--rw-r--r--   0        0        0    23198 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/learning/learning_rule.py
--rw-r--r--   0        0        0    12270 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/learning/learning_rule_applier.py
--rw-r--r--   0        0        0    23302 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/learning/product_series.py
--rw-r--r--   0        0        0     4603 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/learning/random.py
--rw-r--r--   0        0        0      685 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/learning/string_symbols.py
--rw-r--r--   0        0        0    23789 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/learning/symbolic_equation.py
--rw-r--r--   0        0        0     2068 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/learning/utils.py
--rw-r--r--   0        0        0     1084 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/model/interfaces.py
--rw-r--r--   0        0        0     5193 2023-05-03 16:57:46.494211 lava_nc-0.7.0.post2/src/lava/magma/core/model/model.py
--rw-r--r--   0        0        0    52944 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/model/py/connection.py
--rw-r--r--   0        0        0    25160 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/model/py/model.py
--rw-r--r--   0        0        0     3100 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/model/py/neuron.py
--rw-r--r--   0        0        0    36060 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/model/py/ports.py
--rw-r--r--   0        0        0      458 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/model/py/type.py
--rw-r--r--   0        0        0      352 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/model/spike_type.py
--rw-r--r--   0        0        0     2914 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/model/sub/model.py
--rw-r--r--   0        0        0     3781 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/process/connection.py
--rw-r--r--   0        0        0     2285 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/process/interfaces.py
--rw-r--r--   0        0        0      194 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/process/message_interface_enum.py
--rw-r--r--   0        0        0     1690 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/process/neuron.py
--rw-r--r--   0        0        0     2763 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/process/ports/exceptions.py
--rw-r--r--   0        0        0    38136 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/process/ports/ports.py
--rw-r--r--   0        0        0      459 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/process/ports/reduce_ops.py
--rw-r--r--   0        0        0    23800 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/process/process.py
--rw-r--r--   0        0        0     7993 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/process/variable.py
--rw-r--r--   0        0        0     3767 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/resources.py
--rw-r--r--   0        0        0     1502 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/run_conditions.py
--rw-r--r--   0        0        0    22433 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/run_configs.py
--rw-r--r--   0        0        0     1506 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/sync/domain.py
--rw-r--r--   0        0        0     1107 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/sync/protocol.py
--rw-r--r--   0        0        0     1523 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/sync/protocols/async_protocol.py
--rw-r--r--   0        0        0     4386 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/core/sync/protocols/loihi_protocol.py
--rw-r--r--   0        0        0    26529 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/runtime/LICENSE
--rw-r--r--   0        0        0      720 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/runtime/message_infrastructure/factory.py
--rw-r--r--   0        0        0     1790 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/runtime/message_infrastructure/message_infrastructure_interface.py
--rw-r--r--   0        0        0     4385 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/runtime/message_infrastructure/multiprocessing.py
--rw-r--r--   0        0        0     1452 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/runtime/message_infrastructure/nx.py
--rw-r--r--   0        0        0     1005 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/runtime/message_infrastructure/shared_memory_manager.py
--rw-r--r--   0        0        0     2439 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/runtime/mgmt_token_enums.py
--rw-r--r--   0        0        0    22602 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/runtime/runtime.py
--rw-r--r--   0        0        0     8310 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/runtime/runtime_services/channel_broker/channel_broker.py
--rw-r--r--   0        0        0     1324 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/runtime/runtime_services/enums.py
--rw-r--r--   0        0        0     1159 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/runtime/runtime_services/interfaces.py
--rw-r--r--   0        0        0    22607 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/magma/runtime/runtime_services/runtime_service.py
--rw-r--r--   0        0        0     1525 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/LICENSE
--rw-r--r--   0        0        0     2934 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/conv/models.py
--rw-r--r--   0        0        0     5954 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/conv/process.py
--rw-r--r--   0        0        0    16042 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/conv/utils.py
--rw-r--r--   0        0        0    14321 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/dense/models.py
--rw-r--r--   0        0        0    11177 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/dense/process.py
--rw-r--r--   0        0        0      236 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/io/__init__.py
--rw-r--r--   0        0        0     7532 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/io/dataloader.py
--rw-r--r--   0        0        0     9449 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/io/encoder.py
--rw-r--r--   0        0        0     2740 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/io/reset.py
--rw-r--r--   0        0        0     4831 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/io/sink.py
--rw-r--r--   0        0        0     2020 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/io/source.py
--rw-r--r--   0        0        0     3083 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/learning_rules/r_stdp_learning_rule.py
--rw-r--r--   0        0        0     1991 2023-05-03 16:57:46.498211 lava_nc-0.7.0.post2/src/lava/proc/learning_rules/stdp_learning_rule.py
--rw-r--r--   0        0        0    18980 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/lif/models.py
--rw-r--r--   0        0        0    12911 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/lif/process.py
--rw-r--r--   0        0        0     2646 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/monitor/models.py
--rw-r--r--   0        0        0    11074 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/monitor/process.py
--rw-r--r--   0        0        0     1074 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/receiver/models.py
--rw-r--r--   0        0        0     1082 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/receiver/process.py
--rw-r--r--   0        0        0     5997 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/rf/models.py
--rw-r--r--   0        0        0     3591 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/rf/process.py
--rw-r--r--   0        0        0     2464 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/rf_iz/models.py
--rw-r--r--   0        0        0      181 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/rf_iz/process.py
--rw-r--r--   0        0        0     9115 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/sdn/models.py
--rw-r--r--   0        0        0     7382 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/sdn/process.py
--rw-r--r--   0        0        0     1431 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/spiker/models.py
--rw-r--r--   0        0        0     1461 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/proc/spiker/process.py
--rw-r--r--   0        0        0     1525 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/utils/LICENSE
--rw-r--r--   0        0        0     4282 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/utils/dataloader/mnist.py
--rw-r--r--   0        0        0     3254 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/utils/plots.py
--rw-r--r--   0        0        0     1466 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/utils/profiler.py
--rw-r--r--   0        0        0     1868 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/utils/system.py
--rw-r--r--   0        0        0     7911 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/src/lava/utils/weightutils.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/builders/__init__.py
--rw-r--r--   0        0        0    20945 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/builders/test_builder.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/channels/__init__.py
--rw-r--r--   0        0        0     5130 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/channels/test_pypychannel.py
--rw-r--r--   0        0        0      113 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/subcompilers/__init__.py
--rw-r--r--   0        0        0      113 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/subcompilers/py/__init__.py
--rw-r--r--   0        0        0     8989 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/subcompilers/py/test_pyproc_compiler.py
--rw-r--r--   0        0        0    18797 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/subcompilers/test_channel_builders_factory.py
--rw-r--r--   0        0        0     3741 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/subcompilers/test_channel_map_updater.py
--rw-r--r--   0        0        0     2168 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/test_channel_builder.py
--rw-r--r--   0        0        0     5376 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/test_channel_map.py
--rw-r--r--   0        0        0    30646 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/test_compiler.py
--rw-r--r--   0        0        0     2048 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/compiler/test_node.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/learning/__init__.py
--rw-r--r--   0        0        0    50548 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/learning/test_learning_rule.py
--rw-r--r--   0        0        0     5470 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/learning/test_learning_rule_applier.py
--rw-r--r--   0        0        0    12737 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/learning/test_product_series.py
--rw-r--r--   0        0        0     1905 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/learning/test_random.py
--rw-r--r--   0        0        0    18180 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/learning/test_symbolic_equation.py
--rw-r--r--   0        0        0     2230 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/learning/test_utils.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/model/py/__init__.py
--rw-r--r--   0        0        0     5870 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/model/py/test_model.py
--rw-r--r--   0        0        0     6898 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/model/py/test_ports.py
--rw-r--r--   0        0        0     9117 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/model/test_decorators.py
--rw-r--r--   0        0        0     1552 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/model/test_sub_model.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/process/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/process/ports/__init__.py
--rw-r--r--   0        0        0    21231 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/process/ports/test_ports.py
--rw-r--r--   0        0        0    34827 2023-05-03 16:57:46.502211 lava_nc-0.7.0.post2/tests/lava/magma/core/process/ports/test_virtual_ports_in_process.py
--rw-r--r--   0        0        0     1377 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/core/process/test_lif_dense_lif.py
--rw-r--r--   0        0        0    12308 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/core/process/test_process.py
--rw-r--r--   0        0        0     4635 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/core/process/test_variable.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/__init__.py
--rw-r--r--   0        0        0     3675 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_async_protocol.py
--rw-r--r--   0        0        0     5783 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_context_manager.py
--rw-r--r--   0        0        0     5174 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_exception_handling.py
--rw-r--r--   0        0        0     2038 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_get_set_non_determinism.py
--rw-r--r--   0        0        0     7469 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_get_set_var.py
--rw-r--r--   0        0        0    10583 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_io_ports.py
--rw-r--r--   0        0        0     1216 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_leakage.py
--rw-r--r--   0        0        0     2238 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_loihi_protocol.py
--rw-r--r--   0        0        0     3661 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_loihi_with_async_protocol.py
--rw-r--r--   0        0        0     6682 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_pause_requested_from_model.py
--rw-r--r--   0        0        0    14794 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_ref_var_ports.py
--rw-r--r--   0        0        0     3822 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_run_continuously_and_pause.py
--rw-r--r--   0        0        0     2829 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_runtime.py
--rw-r--r--   0        0        0     2903 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_runtime_service.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/proc/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.506212 lava_nc-0.7.0.post2/tests/lava/proc/conv/__init__.py
--rw-r--r--   0        0        0   559366 2023-05-03 16:57:46.510212 lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_0.npz
--rw-r--r--   0        0        0   590766 2023-05-03 16:57:46.514212 lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_1.npz
--rw-r--r--   0        0        0   956638 2023-05-03 16:57:46.522212 lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_2.npz
--rw-r--r--   0        0        0    68302 2023-05-03 16:57:46.522212 lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_3.npz
--rw-r--r--   0        0        0   185142 2023-05-03 16:57:46.522212 lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_4.npz
--rw-r--r--   0        0        0   409190 2023-05-03 16:57:46.526212 lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_5.npz
--rw-r--r--   0        0        0  1888366 2023-05-03 16:57:46.542213 lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_6.npz
--rw-r--r--   0        0        0  1790434 2023-05-03 16:57:46.554213 lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_7.npz
--rw-r--r--   0        0        0   714214 2023-05-03 16:57:46.558214 lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_8.npz
--rw-r--r--   0        0        0   670702 2023-05-03 16:57:46.562214 lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_9.npz
--rw-r--r--   0        0        0      999 2023-05-03 16:57:46.562214 lava_nc-0.7.0.post2/tests/lava/proc/conv/test_process.py
--rw-r--r--   0        0        0     7343 2023-05-03 16:57:46.562214 lava_nc-0.7.0.post2/tests/lava/proc/conv/test_utils.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.562214 lava_nc-0.7.0.post2/tests/lava/proc/dense/__init__.py
--rw-r--r--   0        0        0    53052 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/dense/test_learning.py
--rw-r--r--   0        0        0    47972 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/dense/test_models.py
--rw-r--r--   0        0        0     3666 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/dense/test_process.py
--rw-r--r--   0        0        0    24791 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/dense/test_stdp_sim.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/io/__init__.py
--rw-r--r--   0        0        0     7309 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/io/test_dataloader.py
--rw-r--r--   0        0        0     2001 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/io/test_source_sink.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/lif/__init__.py
--rw-r--r--   0        0        0    38490 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/lif/test_models.py
--rw-r--r--   0        0        0     2213 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/lif/test_process.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/monitor/__init__.py
--rw-r--r--   0        0        0    12959 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/monitor/test_monitors.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/rf/__init__.py
--rw-r--r--   0        0        0     9354 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/rf/test_models.py
--rw-r--r--   0        0        0      868 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/rf/test_process.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/rf_iz/__init__.py
--rw-r--r--   0        0        0     3563 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/rf_iz/test_models.py
--rw-r--r--   0        0        0      901 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/rf_iz/test_process.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/sdn/__init__.py
--rw-r--r--   0        0        0     7800 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/sdn/test_models.py
--rw-r--r--   0        0        0     1457 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/sdn/test_process.py
--rw-r--r--   0        0        0     1710 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/proc/spiker/test_models.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/test_utils/__init__.py
--rw-r--r--   0        0        0     1525 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/test_utils/utils.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/tutorials/__init__.py
--rw-r--r--   0        0        0     9340 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/tutorials/test_tutorials.py
--rw-r--r--   0        0        0        0 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/utils/__init__.py
--rw-r--r--   0        0        0     2165 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/utils/test_plots.py
--rw-r--r--   0        0        0    15761 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tests/lava/utils/test_weightutils.py
--rw-r--r--   0        0        0     1525 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tutorials/LICENSE
--rw-r--r--   0        0        0     9985 2023-05-03 16:57:46.566214 lava_nc-0.7.0.post2/tutorials/end_to_end/convert_params.py
--rw-r--r--   0        0        0   220767 2023-05-03 16:57:46.590215 lava_nc-0.7.0.post2/tutorials/end_to_end/mnist_pretrained.npy
--rw-r--r--   0        0        0   276563 2023-05-03 16:57:46.590215 lava_nc-0.7.0.post2/tutorials/end_to_end/tutorial00_tour_through_lava.ipynb
--rw-r--r--   0        0        0    24427 2023-05-03 16:57:46.590215 lava_nc-0.7.0.post2/tutorials/end_to_end/tutorial01_mnist_digit_classification.ipynb
--rw-r--r--   0        0        0  1170553 2023-05-03 16:57:46.602215 lava_nc-0.7.0.post2/tutorials/end_to_end/tutorial02_excitatory_inhibitory_network.ipynb
--rw-r--r--   0        0        0   566145 2023-05-03 16:57:46.606215 lava_nc-0.7.0.post2/tutorials/in_depth/three_factor_learning/tutorial01_Reward_Modulated_STDP.ipynb
--rw-r--r--   0        0        0    10117 2023-05-03 16:57:46.606215 lava_nc-0.7.0.post2/tutorials/in_depth/three_factor_learning/utils.py
--rw-r--r--   0        0        0     6552 2023-05-03 16:57:46.606215 lava_nc-0.7.0.post2/tutorials/in_depth/tutorial01_installing_lava.ipynb
--rw-r--r--   0        0        0    16399 2023-05-03 16:57:46.606215 lava_nc-0.7.0.post2/tutorials/in_depth/tutorial02_processes.ipynb
--rw-r--r--   0        0        0    15539 2023-05-03 16:57:46.606215 lava_nc-0.7.0.post2/tutorials/in_depth/tutorial03_process_models.ipynb
--rw-r--r--   0        0        0    14366 2023-05-03 16:57:46.606215 lava_nc-0.7.0.post2/tutorials/in_depth/tutorial04_execution.ipynb
--rw-r--r--   0        0        0    13442 2023-05-03 16:57:46.606215 lava_nc-0.7.0.post2/tutorials/in_depth/tutorial05_connect_processes.ipynb
--rw-r--r--   0        0        0    21815 2023-05-03 16:57:46.606215 lava_nc-0.7.0.post2/tutorials/in_depth/tutorial06_hierarchical_processes.ipynb
--rw-r--r--   0        0        0    12809 2023-05-03 16:57:46.606215 lava_nc-0.7.0.post2/tutorials/in_depth/tutorial07_remote_memory_access.ipynb
--rw-r--r--   0        0        0    73297 2023-05-03 16:57:46.606215 lava_nc-0.7.0.post2/tutorials/in_depth/tutorial08_stdp.ipynb
--rw-r--r--   0        0        0   137711 2023-05-03 16:57:46.606215 lava_nc-0.7.0.post2/tutorials/in_depth/tutorial09_custom_learning_rules.ipynb
--rw-r--r--   0        0        0   222561 2023-05-03 16:57:46.610215 lava_nc-0.7.0.post2/tutorials/in_depth/tutorial10_sigma_delta_neurons.ipynb
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 lava_nc-0.7.0.post2/PKG-INFO
+-rw-r--r--   0        0        0      333 2023-07-25 06:40:19.509229 lava_nc-0.8.0/LICENSE
+-rw-r--r--   0        0        0     8687 2023-07-25 06:40:19.509229 lava_nc-0.8.0/README.md
+-rw-r--r--   0        0        0     4785 2023-07-25 06:40:19.509229 lava_nc-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    26529 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/LICENSE
+-rw-r--r--   0        0        0     5537 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/builders/channel_builder.py
+-rw-r--r--   0        0        0     4210 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/builders/interfaces.py
+-rw-r--r--   0        0        0    15815 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/builders/py_builder.py
+-rw-r--r--   0        0        0     4937 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/builders/runtimeservice_builder.py
+-rw-r--r--   0        0        0     4607 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/channel_map.py
+-rw-r--r--   0        0        0     1372 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/channels/interfaces.py
+-rw-r--r--   0        0        0    10930 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/channels/pypychannel.py
+-rw-r--r--   0        0        0    35594 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/compiler.py
+-rw-r--r--   0        0        0    44862 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/compiler_graphs.py
+-rw-r--r--   0        0        0     1550 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/compiler_utils.py
+-rw-r--r--   0        0        0      573 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/exceptions.py
+-rw-r--r--   0        0        0     1847 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/executable.py
+-rw-r--r--   0        0        0      721 2023-07-25 06:40:19.509229 lava_nc-0.8.0/src/lava/magma/compiler/mappable_interface.py
+-rw-r--r--   0        0        0     7533 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/compiler/mapper.py
+-rw-r--r--   0        0        0     2269 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/compiler/node.py
+-rw-r--r--   0        0        0      514 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/address.py
+-rw-r--r--   0        0        0    10344 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/channel_builders_factory.py
+-rw-r--r--   0        0        0     2390 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/channel_map_updater.py
+-rw-r--r--   0        0        0      696 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/constants.py
+-rw-r--r--   0        0        0      769 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/exceptions.py
+-rw-r--r--   0        0        0     2060 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/interfaces.py
+-rw-r--r--   0        0        0     7543 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/py/pyproc_compiler.py
+-rw-r--r--   0        0        0     4135 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/compiler/utils.py
+-rw-r--r--   0        0        0     5751 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/compiler/var_model.py
+-rw-r--r--   0        0        0     1525 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/LICENSE
+-rw-r--r--   0        0        0     2620 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/callback_fx.py
+-rw-r--r--   0        0        0     6408 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/decorator.py
+-rw-r--r--   0        0        0     2046 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/learning/constants.py
+-rw-r--r--   0        0        0    23198 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/learning/learning_rule.py
+-rw-r--r--   0        0        0    12270 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/learning/learning_rule_applier.py
+-rw-r--r--   0        0        0    23302 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/learning/product_series.py
+-rw-r--r--   0        0        0     4603 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/learning/random.py
+-rw-r--r--   0        0        0      685 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/learning/string_symbols.py
+-rw-r--r--   0        0        0    23794 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/learning/symbolic_equation.py
+-rw-r--r--   0        0        0     2054 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/learning/utils.py
+-rw-r--r--   0        0        0     1071 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/model/interfaces.py
+-rw-r--r--   0        0        0     5193 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/model/model.py
+-rw-r--r--   0        0        0    54857 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/model/py/connection.py
+-rw-r--r--   0        0        0    25994 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/model/py/model.py
+-rw-r--r--   0        0        0     3100 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/model/py/neuron.py
+-rw-r--r--   0        0        0    36047 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/model/py/ports.py
+-rw-r--r--   0        0        0      458 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/model/py/type.py
+-rw-r--r--   0        0        0      352 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/model/spike_type.py
+-rw-r--r--   0        0        0     2914 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/model/sub/model.py
+-rw-r--r--   0        0        0     3781 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/process/connection.py
+-rw-r--r--   0        0        0     2285 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/process/interfaces.py
+-rw-r--r--   0        0        0      194 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/process/message_interface_enum.py
+-rw-r--r--   0        0        0     1690 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/process/neuron.py
+-rw-r--r--   0        0        0     2763 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/process/ports/exceptions.py
+-rw-r--r--   0        0        0    37774 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/process/ports/ports.py
+-rw-r--r--   0        0        0      439 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/process/ports/reduce_ops.py
+-rw-r--r--   0        0        0    24952 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/process/process.py
+-rw-r--r--   0        0        0     9124 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/process/variable.py
+-rw-r--r--   0        0        0     3605 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/resources.py
+-rw-r--r--   0        0        0     1502 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/run_conditions.py
+-rw-r--r--   0        0        0    22435 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/run_configs.py
+-rw-r--r--   0        0        0     1506 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/sync/domain.py
+-rw-r--r--   0        0        0     1107 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/sync/protocol.py
+-rw-r--r--   0        0        0     1523 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/sync/protocols/async_protocol.py
+-rw-r--r--   0        0        0     4386 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/core/sync/protocols/loihi_protocol.py
+-rw-r--r--   0        0        0    26529 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/runtime/LICENSE
+-rw-r--r--   0        0        0      718 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/runtime/message_infrastructure/factory.py
+-rw-r--r--   0        0        0     1635 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/runtime/message_infrastructure/message_infrastructure_interface.py
+-rw-r--r--   0        0        0     4385 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/runtime/message_infrastructure/multiprocessing.py
+-rw-r--r--   0        0        0     1400 2023-07-25 06:40:19.513229 lava_nc-0.8.0/src/lava/magma/runtime/message_infrastructure/nx.py
+-rw-r--r--   0        0        0     1005 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/magma/runtime/message_infrastructure/shared_memory_manager.py
+-rw-r--r--   0        0        0     2440 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/magma/runtime/mgmt_token_enums.py
+-rw-r--r--   0        0        0    22811 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/magma/runtime/runtime.py
+-rw-r--r--   0        0        0     8253 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/magma/runtime/runtime_services/channel_broker/channel_broker.py
+-rw-r--r--   0        0        0     1324 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/magma/runtime/runtime_services/enums.py
+-rw-r--r--   0        0        0     1159 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/magma/runtime/runtime_services/interfaces.py
+-rw-r--r--   0        0        0    22589 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/magma/runtime/runtime_services/runtime_service.py
+-rw-r--r--   0        0        0     1525 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/LICENSE
+-rw-r--r--   0        0        0     2648 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/clp/novelty_detector/models.py
+-rw-r--r--   0        0        0     1710 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/clp/novelty_detector/process.py
+-rw-r--r--   0        0        0     6473 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/clp/nsm/models.py
+-rw-r--r--   0        0        0     3582 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/clp/nsm/process.py
+-rw-r--r--   0        0        0     4781 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/clp/prototype_lif/models.py
+-rw-r--r--   0        0        0     1750 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/clp/prototype_lif/process.py
+-rw-r--r--   0        0        0     2934 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/conv/models.py
+-rw-r--r--   0        0        0     5954 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/conv/process.py
+-rw-r--r--   0        0        0    16043 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/conv/utils.py
+-rw-r--r--   0        0        0    14858 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/dense/models.py
+-rw-r--r--   0        0        0    11223 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/dense/process.py
+-rw-r--r--   0        0        0      236 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/io/__init__.py
+-rw-r--r--   0        0        0     7532 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/io/dataloader.py
+-rw-r--r--   0        0        0     9397 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/io/encoder.py
+-rw-r--r--   0        0        0     4902 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/io/extractor.py
+-rw-r--r--   0        0        0     5053 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/io/injector.py
+-rw-r--r--   0        0        0     2740 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/io/reset.py
+-rw-r--r--   0        0        0     4831 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/io/sink.py
+-rw-r--r--   0        0        0     2020 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/io/source.py
+-rw-r--r--   0        0        0     8248 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/io/utils.py
+-rw-r--r--   0        0        0     3083 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/learning_rules/r_stdp_learning_rule.py
+-rw-r--r--   0        0        0     1991 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/learning_rules/stdp_learning_rule.py
+-rw-r--r--   0        0        0    21063 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/lif/models.py
+-rw-r--r--   0        0        0    15487 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/lif/process.py
+-rw-r--r--   0        0        0     2646 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/monitor/models.py
+-rw-r--r--   0        0        0    10813 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/monitor/process.py
+-rw-r--r--   0        0        0     1074 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/receiver/models.py
+-rw-r--r--   0        0        0     1082 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/receiver/process.py
+-rw-r--r--   0        0        0     5997 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/rf/models.py
+-rw-r--r--   0        0        0     3591 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/rf/process.py
+-rw-r--r--   0        0        0     2464 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/rf_iz/models.py
+-rw-r--r--   0        0        0      181 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/rf_iz/process.py
+-rw-r--r--   0        0        0     9115 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/sdn/models.py
+-rw-r--r--   0        0        0     7382 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/sdn/process.py
+-rw-r--r--   0        0        0    15919 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/sparse/models.py
+-rw-r--r--   0        0        0    11530 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/sparse/process.py
+-rw-r--r--   0        0        0     1421 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/spiker/models.py
+-rw-r--r--   0        0        0     1461 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/proc/spiker/process.py
+-rw-r--r--   0        0        0     1525 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/utils/LICENSE
+-rw-r--r--   0        0        0     4360 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/utils/dataloader/mnist.py
+-rw-r--r--   0        0        0     3973 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/utils/loihi.py
+-rw-r--r--   0        0        0     3254 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/utils/plots.py
+-rw-r--r--   0        0        0     1466 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/utils/profiler.py
+-rw-r--r--   0        0        0     4484 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/utils/serialization.py
+-rw-r--r--   0        0        0     7010 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/utils/slurm.py
+-rw-r--r--   0        0        0      772 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/utils/sparse.py
+-rw-r--r--   0        0        0     2577 2023-07-25 06:40:19.517229 lava_nc-0.8.0/src/lava/utils/system.py
+-rw-r--r--   0        0        0     8544 2023-07-25 06:40:19.521230 lava_nc-0.8.0/src/lava/utils/weightutils.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/builders/__init__.py
+-rw-r--r--   0        0        0    20945 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/builders/test_builder.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/channels/__init__.py
+-rw-r--r--   0        0        0     5130 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/channels/test_pypychannel.py
+-rw-r--r--   0        0        0      113 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/subcompilers/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/subcompilers/py/__init__.py
+-rw-r--r--   0        0        0     8975 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/subcompilers/py/test_pyproc_compiler.py
+-rw-r--r--   0        0        0    18475 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/subcompilers/test_channel_builders_factory.py
+-rw-r--r--   0        0        0     3741 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/subcompilers/test_channel_map_updater.py
+-rw-r--r--   0        0        0     2168 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/test_channel_builder.py
+-rw-r--r--   0        0        0     5366 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/test_channel_map.py
+-rw-r--r--   0        0        0    30496 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/test_compiler.py
+-rw-r--r--   0        0        0     2038 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/compiler/test_node.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/learning/__init__.py
+-rw-r--r--   0        0        0    49958 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/learning/test_learning_rule.py
+-rw-r--r--   0        0        0     5470 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/learning/test_learning_rule_applier.py
+-rw-r--r--   0        0        0    12737 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/learning/test_product_series.py
+-rw-r--r--   0        0        0     1886 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/learning/test_random.py
+-rw-r--r--   0        0        0    18180 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/learning/test_symbolic_equation.py
+-rw-r--r--   0        0        0     2230 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/learning/test_utils.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/model/py/__init__.py
+-rw-r--r--   0        0        0     5850 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/model/py/test_model.py
+-rw-r--r--   0        0        0     6898 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/model/py/test_ports.py
+-rw-r--r--   0        0        0     9326 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/model/test_decorators.py
+-rw-r--r--   0        0        0     1552 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/model/test_sub_model.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/process/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/process/ports/__init__.py
+-rw-r--r--   0        0        0    21782 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/process/ports/test_ports.py
+-rw-r--r--   0        0        0    34827 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/process/ports/test_virtual_ports_in_process.py
+-rw-r--r--   0        0        0     1327 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/process/test_lif_dense_lif.py
+-rw-r--r--   0        0        0    13934 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/process/test_process.py
+-rw-r--r--   0        0        0     4635 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/core/process/test_variable.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/__init__.py
+-rw-r--r--   0        0        0     3607 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_async_protocol.py
+-rw-r--r--   0        0        0     5783 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_context_manager.py
+-rw-r--r--   0        0        0     5174 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_exception_handling.py
+-rw-r--r--   0        0        0     2038 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_get_set_non_determinism.py
+-rw-r--r--   0        0        0     7469 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_get_set_var.py
+-rw-r--r--   0        0        0    10583 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_io_ports.py
+-rw-r--r--   0        0        0     1216 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_leakage.py
+-rw-r--r--   0        0        0     2238 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_loihi_protocol.py
+-rw-r--r--   0        0        0     3672 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_loihi_with_async_protocol.py
+-rw-r--r--   0        0        0     6682 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_pause_requested_from_model.py
+-rw-r--r--   0        0        0    14794 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_ref_var_ports.py
+-rw-r--r--   0        0        0     3822 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_run_continuously_and_pause.py
+-rw-r--r--   0        0        0     2938 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_runtime.py
+-rw-r--r--   0        0        0     2903 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/magma/runtime/test_runtime_service.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/proc/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/proc/clp/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.521230 lava_nc-0.8.0/tests/lava/proc/clp/integration/__init__.py
+-rw-r--r--   0        0        0    21963 2023-07-25 06:40:19.525230 lava_nc-0.8.0/tests/lava/proc/clp/integration/test_clp_one_shot.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.525230 lava_nc-0.8.0/tests/lava/proc/clp/novelty_detector/__init__.py
+-rw-r--r--   0        0        0     4075 2023-07-25 06:40:19.525230 lava_nc-0.8.0/tests/lava/proc/clp/novelty_detector/test_models.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.525230 lava_nc-0.8.0/tests/lava/proc/clp/nsm/__init__.py
+-rw-r--r--   0        0        0     7818 2023-07-25 06:40:19.525230 lava_nc-0.8.0/tests/lava/proc/clp/nsm/test_nsm.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.525230 lava_nc-0.8.0/tests/lava/proc/clp/prototype_lif/__init__.py
+-rw-r--r--   0        0        0     8495 2023-07-25 06:40:19.525230 lava_nc-0.8.0/tests/lava/proc/clp/prototype_lif/test_models.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.525230 lava_nc-0.8.0/tests/lava/proc/conv/__init__.py
+-rw-r--r--   0        0        0   559366 2023-07-25 06:40:19.529230 lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_0.npz
+-rw-r--r--   0        0        0   590766 2023-07-25 06:40:19.533230 lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_1.npz
+-rw-r--r--   0        0        0   956638 2023-07-25 06:40:19.537231 lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_2.npz
+-rw-r--r--   0        0        0    68302 2023-07-25 06:40:19.541231 lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_3.npz
+-rw-r--r--   0        0        0   185142 2023-07-25 06:40:19.541231 lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_4.npz
+-rw-r--r--   0        0        0   409190 2023-07-25 06:40:19.545231 lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_5.npz
+-rw-r--r--   0        0        0  1888366 2023-07-25 06:40:19.557232 lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_6.npz
+-rw-r--r--   0        0        0  1790434 2023-07-25 06:40:19.573234 lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_7.npz
+-rw-r--r--   0        0        0   714214 2023-07-25 06:40:19.577234 lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_8.npz
+-rw-r--r--   0        0        0   670702 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_9.npz
+-rw-r--r--   0        0        0      999 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/conv/test_process.py
+-rw-r--r--   0        0        0     7354 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/conv/test_utils.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/dense/__init__.py
+-rw-r--r--   0        0        0    53114 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/dense/test_learning.py
+-rw-r--r--   0        0        0    47978 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/dense/test_models.py
+-rw-r--r--   0        0        0     3666 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/dense/test_process.py
+-rw-r--r--   0        0        0    24791 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/dense/test_stdp_sim.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/io/__init__.py
+-rw-r--r--   0        0        0     7315 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/io/test_dataloader.py
+-rw-r--r--   0        0        0    19371 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/io/test_extractor.py
+-rw-r--r--   0        0        0    20367 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/io/test_injector.py
+-rw-r--r--   0        0        0     2008 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/io/test_source_sink.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/lif/__init__.py
+-rw-r--r--   0        0        0    39788 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/lif/test_models.py
+-rw-r--r--   0        0        0     2213 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/lif/test_process.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/monitor/__init__.py
+-rw-r--r--   0        0        0    12959 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/monitor/test_monitors.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/rf/__init__.py
+-rw-r--r--   0        0        0     9377 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/rf/test_models.py
+-rw-r--r--   0        0        0      868 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/rf/test_process.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/rf_iz/__init__.py
+-rw-r--r--   0        0        0     3575 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/rf_iz/test_models.py
+-rw-r--r--   0        0        0      901 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/rf_iz/test_process.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/sdn/__init__.py
+-rw-r--r--   0        0        0     7832 2023-07-25 06:40:19.581234 lava_nc-0.8.0/tests/lava/proc/sdn/test_models.py
+-rw-r--r--   0        0        0     1457 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/proc/sdn/test_process.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/proc/sparse/__init__.py
+-rw-r--r--   0        0        0    57243 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/proc/sparse/test_models.py
+-rw-r--r--   0        0        0     3887 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/proc/sparse/test_process.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/proc/spiker/__init__.py
+-rw-r--r--   0        0        0     1696 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/proc/spiker/test_models.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/test_utils/__init__.py
+-rw-r--r--   0        0        0     1547 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/test_utils/utils.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/tutorials/__init__.py
+-rw-r--r--   0        0        0     9812 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/tutorials/test_tutorials.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/utils/__init__.py
+-rw-r--r--   0        0        0     7293 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/utils/test_loihi.py
+-rw-r--r--   0        0        0     2160 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/utils/test_plots.py
+-rw-r--r--   0        0        0     6046 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/utils/test_serialization.py
+-rw-r--r--   0        0        0    11140 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/utils/test_slurm.py
+-rw-r--r--   0        0        0    15761 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tests/lava/utils/test_weightutils.py
+-rw-r--r--   0        0        0     1525 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tutorials/LICENSE
+-rw-r--r--   0        0        0    10009 2023-07-25 06:40:19.585235 lava_nc-0.8.0/tutorials/end_to_end/convert_params.py
+-rw-r--r--   0        0        0   220767 2023-07-25 06:40:19.605236 lava_nc-0.8.0/tutorials/end_to_end/mnist_pretrained.npy
+-rw-r--r--   0        0        0   274771 2023-07-25 06:40:19.609237 lava_nc-0.8.0/tutorials/end_to_end/tutorial00_tour_through_lava.ipynb
+-rw-r--r--   0        0        0    23948 2023-07-25 06:40:19.609237 lava_nc-0.8.0/tutorials/end_to_end/tutorial01_mnist_digit_classification.ipynb
+-rw-r--r--   0        0        0  1170553 2023-07-25 06:40:19.617237 lava_nc-0.8.0/tutorials/end_to_end/tutorial02_excitatory_inhibitory_network.ipynb
+-rw-r--r--   0        0        0    10438 2023-07-25 06:40:19.617237 lava_nc-0.8.0/tutorials/in_depth/clp/clp.py
+-rw-r--r--   0        0        0   462884 2023-07-25 06:40:19.621238 lava_nc-0.8.0/tutorials/in_depth/clp/tutorial01_one-shot_learning_with_novelty_detection.ipynb
+-rw-r--r--   0        0        0     8365 2023-07-25 06:40:19.621238 lava_nc-0.8.0/tutorials/in_depth/clp/utils.py
+-rw-r--r--   0        0        0   566145 2023-07-25 06:40:19.625238 lava_nc-0.8.0/tutorials/in_depth/three_factor_learning/tutorial01_Reward_Modulated_STDP.ipynb
+-rw-r--r--   0        0        0     9676 2023-07-25 06:40:19.625238 lava_nc-0.8.0/tutorials/in_depth/three_factor_learning/utils.py
+-rw-r--r--   0        0        0     6552 2023-07-25 06:40:19.625238 lava_nc-0.8.0/tutorials/in_depth/tutorial01_installing_lava.ipynb
+-rw-r--r--   0        0        0    16399 2023-07-25 06:40:19.625238 lava_nc-0.8.0/tutorials/in_depth/tutorial02_processes.ipynb
+-rw-r--r--   0        0        0    15539 2023-07-25 06:40:19.625238 lava_nc-0.8.0/tutorials/in_depth/tutorial03_process_models.ipynb
+-rw-r--r--   0        0        0    14366 2023-07-25 06:40:19.625238 lava_nc-0.8.0/tutorials/in_depth/tutorial04_execution.ipynb
+-rw-r--r--   0        0        0    13442 2023-07-25 06:40:19.625238 lava_nc-0.8.0/tutorials/in_depth/tutorial05_connect_processes.ipynb
+-rw-r--r--   0        0        0    21815 2023-07-25 06:40:19.625238 lava_nc-0.8.0/tutorials/in_depth/tutorial06_hierarchical_processes.ipynb
+-rw-r--r--   0        0        0    12809 2023-07-25 06:40:19.625238 lava_nc-0.8.0/tutorials/in_depth/tutorial07_remote_memory_access.ipynb
+-rw-r--r--   0        0        0    73297 2023-07-25 06:40:19.625238 lava_nc-0.8.0/tutorials/in_depth/tutorial08_stdp.ipynb
+-rw-r--r--   0        0        0   137711 2023-07-25 06:40:19.625238 lava_nc-0.8.0/tutorials/in_depth/tutorial09_custom_learning_rules.ipynb
+-rw-r--r--   0        0        0   222561 2023-07-25 06:40:19.629238 lava_nc-0.8.0/tutorials/in_depth/tutorial10_sigma_delta_neurons.ipynb
+-rw-r--r--   0        0        0     9974 2023-07-25 06:40:19.629238 lava_nc-0.8.0/tutorials/in_depth/tutorial11_serialization.ipynb
+-rw-r--r--   0        0        0    10429 1970-01-01 00:00:00.000000 lava_nc-0.8.0/PKG-INFO
```

### Comparing `lava_nc-0.7.0.post2/pyproject.toml` & `lava_nc-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 [tool.poetry]
 name = "lava-nc"
 packages = [
     {include = "lava", from = "src"},
     {include = "tests"}
 ]
 include = ["tutorials"]
-version = "0.7.0.post2"
+version = "0.8.0"
+readme = "README.md"
 description = "A Software Framework for Neuromorphic Computing"
 homepage = "https://lava-nc.org/"
 repository = "https://github.com/lava-nc/lava"
 authors = [ 
     "Intel's Neuromorphic Computing Lab and the open source community <lava@intel.com>"
 ]
 license = "(BSD-3-Clause), (LGPL-2.1-or-later)"
@@ -43,18 +44,18 @@
 "Questions and Answers" = "https://github.com/lava-nc/lava/discussions/categories/q-a"
 "Frequently Asked Questions" = "https://github.com/lava-nc/lava/wiki/Frequently-Asked-Questions-(FAQ)"
 "Discussions" = "https://github.com/lava-nc/lava/discussions"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 
-numpy = "^1.22.2"
-scipy = "^1.8.0"
+numpy = "^1.24.4"
+scipy = "^1.10.1"
 networkx = "<=2.8.7"
-asteval = "^0.9.27"
+asteval = "^0.9.31"
 
 [tool.poetry.dev-dependencies]
 bandit = "1.7.4"
 coverage = "^6.3.2"
 darglint = "^1.8.1"
 flake8 = "^4.0.1"
 flake8-bandit = "^3.0.0"
@@ -166,17 +167,17 @@
 # flake8-isort = ["+*"]
 # flake8-mutable = ["+*"]
 # flake8-pytest-style = ["+*"]
 # flake8-spellcheck = ["-*"]
 # mccabe = ["+*"]
 # pep8-naming = ["+*"]
 # pyflakes = ["+*"]
-# pylint = ["+*"]
+pylint = ["+*"]
 
 pycodestyle = ["+*", "-W503", "-E203"]
-pyflakes = ["-*"]                           # Disable temporarily until lint fix is pushed
-pylint = ["-*"]                             # Disable temporarily until lint fix is pushed
+# pyflakes = ["-*"]                           # Disable temporarily until lint fix is pushed
+# pylint = ["-*"]                             # Disable temporarily until lint fix is pushed
 
 [tool.flakeheaven.exceptions."tests/"]
 pycodestyle = ["-F401"]                     # Disable a check
 flake8-bandit = ["-S101"]                   # Ignore asserts for tests
 pyflakes = ["-*"]                           # Disable a plugin
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/LICENSE` & `lava_nc-0.8.0/src/lava/magma/compiler/LICENSE`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/builders/channel_builder.py` & `lava_nc-0.8.0/src/lava/magma/compiler/builders/channel_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,8 +186,7 @@
             Channel
 
         Raises
         ------
         Exception
             Can't build channel of type specified
         """
-        pass
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/builders/interfaces.py` & `lava_nc-0.8.0/src/lava/magma/compiler/builders/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,25 +10,23 @@
 
 class AbstractBuilder(ABC):
     """Builders interface for building processes in a given backend."""
 
     @abstractmethod
     def build(self):
         """Build the actual process."""
-        pass
 
 
 class ResourceAddress(ABC):
     pass
 
 
 class Resource(ABC):
     def write(self, hw: ty.Any):
         """Given hw, write this compiled resource"""
-        pass
 
 
 class CompiledResource(Resource):
     """Signifies a compiled resource held by the builder. Must be
     serializable if the builder is being serialized after compilation
     before mapping"""
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/builders/py_builder.py` & `lava_nc-0.8.0/src/lava/magma/compiler/builders/py_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: LGPL 2.1 or later
 # See: https://spdx.org/licenses/
 
 import typing as ty
 
 import numpy as np
+from scipy.sparse import csr_matrix
 from lava.magma.compiler.builders.interfaces import AbstractProcessBuilder
 
 from lava.magma.compiler.channels.interfaces import AbstractCspPort
 from lava.magma.compiler.channels.pypychannel import CspRecvPort, CspSendPort
 from lava.magma.compiler.utils import (
     PortInitializer,
     VarInitializer,
@@ -398,14 +399,20 @@
             # Build variable
             lt = self._get_lava_type(name)
             if issubclass(lt.cls, np.ndarray):
                 var = lt.cls(v.shape, lt.d_type)
                 var[:] = v.value
             elif issubclass(lt.cls, (int, float, str)):
                 var = v.value
+            elif issubclass(lt.cls, (csr_matrix)):
+                if isinstance(v.value, int):
+                    var = csr_matrix(v.shape, dtype=lt.d_type)
+                    var[:] = v.value
+                else:
+                    var = v.value
             else:
                 raise NotImplementedError(
                     "Cannot initiliaze variable "
                     "datatype, \
                     only subclasses of int, float and str are \
                     supported"
                 )
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/builders/runtimeservice_builder.py` & `lava_nc-0.8.0/src/lava/magma/compiler/builders/runtimeservice_builder.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/channel_map.py` & `lava_nc-0.8.0/src/lava/magma/compiler/channel_map.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/channels/interfaces.py` & `lava_nc-0.8.0/src/lava/magma/compiler/channels/interfaces.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/channels/pypychannel.py` & `lava_nc-0.8.0/src/lava/magma/compiler/channels/pypychannel.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 import typing as ty
 from dataclasses import dataclass
 from multiprocessing import Semaphore
 from queue import Queue, Empty
 from threading import BoundedSemaphore, Condition, Thread
 from time import time
+from scipy.sparse import csr_matrix
+from lava.utils.sparse import find
+
 
 import numpy as np
 from lava.magma.compiler.channels.interfaces import (
     Channel,
     AbstractCspSendPort,
     AbstractCspRecvPort,
 )
@@ -55,15 +58,15 @@
         self._req = req
         self._ack = ack
         self._size = size
         self._idx = 0
         self._done = False
         self._array = []
         self._semaphore = None
-        self.observer = None
+        self.observer: ty.Optional[ty.Callable[[], ty.Any]] = None
         self.thread = None
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
@@ -121,14 +124,18 @@
 
     def send(self, data):
         """
         Send data on the channel. May block if the channel is already full.
         """
         if data.shape != self._shape:
             raise AssertionError(f"{data.shape=} {self._shape=} Mismatch")
+
+        if isinstance(data, csr_matrix):
+            data = find(data, explicit_zeros=True)[2]
+
         self._semaphore.acquire()
         self._array[self._idx][:] = data[:]
         self._idx = (self._idx + 1) % self._size
         self._req.release()
 
     def join(self):
         if not self._done:
@@ -199,15 +206,15 @@
         self._size = size
         self._req = req
         self._ack = ack
         self._idx = 0
         self._done = False
         self._array = []
         self._queue = None
-        self.observer = None
+        self.observer: ty.Optional[ty.Callable[[], ty.Any]] = None
         self.thread = None
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
@@ -300,34 +307,38 @@
         """Instantiates CspSelector object and class attributes"""
         self._cv = Condition()
 
     def _changed(self):
         with self._cv:
             self._cv.notify_all()
 
-    def _set_observer(self, channel_actions, observer):
+    @staticmethod
+    def _set_observer(
+            channel_actions: ty.Tuple,
+            observer: ty.Union[ty.Callable[[], ty.Any], None]) -> None:
         for channel, _ in channel_actions:
             channel.observer = observer
 
     def select(
             self,
-            *args: ty.Tuple[
-                ty.Union[CspSendPort, CspRecvPort], ty.Callable[[], ty.Any]
+            *channel_actions: ty.Tuple[
+                ty.Union[CspSendPort, CspRecvPort],
+                ty.Callable[[], ty.Any]
             ],
-    ):
+    ) -> None:
         """
         Wait for any channel to become ready, then execute the corresponding
         callable and return the result.
         """
         with self._cv:
-            self._set_observer(args, self._changed)
+            self._set_observer(channel_actions, self._changed)
             while True:
-                for channel, action in args:
+                for channel, action in channel_actions:
                     if channel.probe():
-                        self._set_observer(args, None)
+                        self._set_observer(channel_actions, None)
                         return action()
                 self._cv.wait()
 
 
 class PyPyChannel(Channel):
     """Helper class to create the set of send and recv port and encapsulate
     them inside a common structure. We call this a PyPyChannel"""
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/compiler.py` & `lava_nc-0.8.0/src/lava/magma/compiler/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,19 +124,21 @@
         executable : Executable
             An instance of an Executable that contains all required Builders.
         """
         # Group and sort all Processes connected to 'process' into a list of
         # ProcGroups.
         proc_group_digraph = ProcGroupDiGraphs(process, run_cfg)
         proc_groups: ty.List[ProcGroup] = proc_group_digraph.get_proc_groups()
+        # Get a flattened list of all AbstractProcesses
+        process_list = list(itertools.chain.from_iterable(proc_groups))
         channel_map = ChannelMap.from_proc_groups(proc_groups)
         proc_builders, channel_map = self._compile_proc_groups(
             proc_groups, channel_map
         )
-        py_builders, c_builders, nc_builders = split_proc_builders_by_type(
+        _, c_builders, nc_builders = split_proc_builders_by_type(
             proc_builders
         )
 
         node_configs = self._create_node_cfgs(proc_groups)
         sync_domains, node_to_sync_domain_dict = self._create_sync_domains(
             proc_groups, run_cfg, node_configs, self.log
         )
@@ -157,14 +159,15 @@
         )
         sync_channel_builders = self._create_sync_channel_builders(
             runtime_service_builders
         )
 
         # Package all Builders and NodeConfigs into an Executable.
         executable = Executable(
+            process_list,
             proc_builders,
             channel_builders,
             node_configs,
             sync_domains,
             runtime_service_builders,
             sync_channel_builders,
         )
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/compiler_graphs.py` & `lava_nc-0.8.0/src/lava/magma/compiler/compiler_graphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import importlib
 import importlib.util as import_utils
 import inspect
 import itertools
 import os
 import pkgutil
-import re
 import sys
 import types
 import typing as ty
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from enum import Enum, auto
 import warnings
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/compiler_utils.py` & `lava_nc-0.8.0/src/lava/magma/compiler/compiler_utils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/exceptions.py` & `lava_nc-0.8.0/src/lava/magma/compiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/executable.py` & `lava_nc-0.8.0/src/lava/magma/compiler/executable.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,20 @@
     processes for the various nodes in the system and channel configurations.
     An Executable should be serializable so it can be saved and loaded at a
     later point.
     """
     # py_builders: ty.Dict[AbstractProcess, NcProcessBuilder]
     # c_builders: ty.Dict[AbstractProcess, CProcessBuilder]
     # nc_builders: ty.Dict[AbstractProcess, PyProcessBuilder]
+    process_list: ty.List[AbstractProcess]  # All leaf processes, flat list.
     proc_builders: ty.Dict[AbstractProcess, 'AbstractProcessBuilder']
     channel_builders: ty.List[ChannelBuilderMp]
     node_configs: ty.List[NodeConfig]
     sync_domains: ty.List[SyncDomain]
     runtime_service_builders: ty.Optional[ty.Dict[SyncDomain,
                                                   RuntimeServiceBuilder]] = None
     sync_channel_builders: ty.Optional[
         ty.Iterable[AbstractChannelBuilder]] = None
 
     def assign_runtime_to_all_processes(self, runtime):
-        for p in self.proc_builders.keys():
+        for p in self.process_list:
             p.runtime = runtime
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/mappable_interface.py` & `lava_nc-0.8.0/src/lava/magma/compiler/mappable_interface.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/mapper.py` & `lava_nc-0.8.0/src/lava/magma/compiler/mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         is done. It maps logical addresses to virtual addresses.
 
         Parameters
         ----------
         executable: Compiled Executable
 
         """
-        py_builders, c_builders, nc_builders = split_proc_builders_by_type(
+        _, c_builders, nc_builders = split_proc_builders_by_type(
             executable.proc_builders)
         # Iterate over all the ncbuilder and map them
         for ncb in nc_builders.values():
             if isinstance(ncb.compiled_resources[0],
                           N3LogicalNeuroCore):
                 num_cores = NUM_VIRTUAL_CORES_L3
             else:
@@ -120,15 +120,14 @@
             ports = {**cb.c_ports, **cb.ref_ports}
             # Iterate over all the ports
             for port in ports:
                 # Iterate over channel map to find its corresponding
                 # src or dst and its initializers
                 for port_pair in channel_map:
                     src = port_pair.src
-                    dst = port_pair.dst
                     # Checking if the initializers are same
                     if channel_map[port_pair].src_port_initializer == ports[
                             port]:
                         var_model = channel_map[
                             port_pair].dst_port_initializer.var_model
                         # Checking to see if its ConvInVarModel or not
                         if hasattr(var_model, "address"):
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/node.py` & `lava_nc-0.8.0/src/lava/magma/compiler/node.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (C) 2021-22 Intel Corporation
 # SPDX-License-Identifier: LGPL 2.1 or later
 # See: https://spdx.org/licenses/
 
 from __future__ import annotations
 
-import typing
 import typing as ty
 from collections import UserList, OrderedDict
 
 if ty.TYPE_CHECKING:
     from lava.magma.core.process.process import AbstractProcess
 from lava.magma.core.resources import AbstractNode
 from lava.magma.compiler.var_model import AbstractVarModel
@@ -23,15 +22,15 @@
 
     def __init__(
         self,
         node_type: ty.Type[AbstractNode],
         processes: ty.List[AbstractProcess],
     ):
         self.id: int = -1
-        self.node_type: typing.Type[AbstractNode] = node_type
+        self.node_type: ty.Type[AbstractNode] = node_type
         self.processes = processes
 
     def add_process(self, process: AbstractProcess):
         self.processes.append(process)
 
     def __str__(self):
         return f"{self.id=} {self.node_type=} {self.processes=}"
@@ -53,15 +52,15 @@
 
     def __str__(self):
         result = []
         result.append(f"{self._node_ctr=}")
         result.append(str(self.node_map))
         return "\n".join(result)
 
-    def append(self, node: Node):
+    def append(self, node: Node):  # pylint: disable=arguments-renamed
         """Appends a new node to the NodeConfig."""
         node.id = self._node_ctr
         self._node_ctr += 1
         super().append(node)
         for p in node.processes:
             self.node_map[p] = node
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/address.py` & `lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/address.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/channel_builders_factory.py` & `lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/channel_builders_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,18 +102,18 @@
                     dst_pt_init,
                 )
                 channel_builders.append(channel_builder)
             if ch_type in [ChannelType.PyC, ChannelType.CPy]:
                 src_pt_init.connected_port_type = LoihiConnectedPortType.C_PY
                 dst_pt_init.connected_port_type = LoihiConnectedPortType.C_PY
                 if ch_type is ChannelType.PyC:
-                    p_port, c_port = src_port, dst_port
+                    p_port = src_port
                     pi = dst_pt_init
                 else:
-                    c_port, p_port = src_port, dst_port
+                    p_port = dst_port
                     pi = src_pt_init
                 lt = getattr(p_port.process.model_class, p_port.name).cls
                 if lt in [PyInPort.VEC_DENSE, PyOutPort.VEC_DENSE]:
                     pi.connected_port_encoding_type = \
                         LoihiConnectedPortEncodingType.VEC_DENSE
                 elif lt in [PyInPort.SCALAR_DENSE, PyOutPort.SCALAR_DENSE]:
                     pi.connected_port_encoding_type = \
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/channel_map_updater.py` & `lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/channel_map_updater.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/constants.py` & `lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/constants.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/exceptions.py` & `lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/exceptions.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/interfaces.py` & `lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,20 @@
     Processes, whose ProcessModels can be executed on the same type of
     backend."""
 
     @abstractmethod
     def compile(self, channel_map: ChannelMap) -> ChannelMap:
         """Partitions all Processes in the SubCompiler's ProcGroup onto the
         available resources."""
-        pass
 
     @abstractmethod
     def get_builders(
         self, channel_map: ChannelMap
     ) -> ty.Tuple[ty.Dict[AbstractProcess, AbstractProcessBuilder], ChannelMap]:
         """After compilation, creates and returns builders for all Processes."""
-        pass
 
 
 class SubCompiler(AbstractSubCompiler):
     def __init__(
         self,
         proc_group: ty.Optional[ProcGroup],
         compile_config: ty.Optional[ty.Dict[str, ty.Any]] = None,
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/subcompilers/py/pyproc_compiler.py` & `lava_nc-0.8.0/src/lava/magma/compiler/subcompilers/py/pyproc_compiler.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/utils.py` & `lava_nc-0.8.0/src/lava/magma/compiler/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,26 +125,24 @@
         = None
     spike_type: ty.Optional[SpikeType] = None
 
 
 @dataclass
 class LoihiInPortInitializer(LoihiIOPortInitializer):
     """Port Initializer for a InPort for C/NC Models"""
-    pass
 
 
 @dataclass
 class LoihiCInPortInitializer(LoihiIOPortInitializer):
     embedded_core = 0
     embedded_counters = None
 
 
 @dataclass
 class LoihiOutPortInitializer(LoihiIOPortInitializer):
     """Port Initializer for a OutPort for C/NC Models"""
-    pass
 
 
 @dataclass
 class LoihiVarPortInitializer(LoihiPortInitializer):
     # This address needs to be defined based on var model
     pass
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/compiler/var_model.py` & `lava_nc-0.8.0/src/lava/magma/compiler/var_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 
     def __post_init__(self, var: Var) -> None:
         if var is not None:
             self.var_id: int = var.id
             self.name: str = var.name
             self.shape: ty.Tuple[int, ...] = var.shape
             self.proc_id: int = var.process.id
+            self.dtype = type(var.init)
 
 
 @dataclass
 class PyVarModel(AbstractVarModel):
     pass
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/LICENSE` & `lava_nc-0.8.0/src/lava/magma/core/LICENSE`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/decorator.py` & `lava_nc-0.8.0/src/lava/magma/core/decorator.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/learning/constants.py` & `lava_nc-0.8.0/src/lava/magma/core/learning/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (C) 2021-23 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
-from enum import IntEnum, auto
+from enum import IntEnum
 import lava.magma.core.learning.string_symbols as str_symbols
 
 # ---------------------------------------------------------------------------
 # Width constants (only for fixed-point implementation)
 # Width of epoch time
 W_EPOCH_TIME = 6
 
@@ -85,11 +85,12 @@
     str_symbols.Y1: 0,
     str_symbols.Y2: 1,
     str_symbols.Y3: 2
 }
 
 
 class GradedSpikeCfg(IntEnum):
-    USE_REGULAR_IMPULSE = auto()
-    OVERWRITE = auto()
-    ADD_WITH_SATURATION = auto()
-    ADD_WITHOUT_SATURATION = auto()
+    # Do not change the values below as they determine hardware behavior
+    USE_REGULAR_IMPULSE = 0
+    OVERWRITE = 1
+    ADD_WITH_SATURATION = 2
+    ADD_WITHOUT_SATURATION = 3
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/learning/learning_rule.py` & `lava_nc-0.8.0/src/lava/magma/core/learning/learning_rule.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/learning/learning_rule_applier.py` & `lava_nc-0.8.0/src/lava/magma/core/learning/learning_rule_applier.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/learning/product_series.py` & `lava_nc-0.8.0/src/lava/magma/core/learning/product_series.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/learning/random.py` & `lava_nc-0.8.0/src/lava/magma/core/learning/random.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/learning/string_symbols.py` & `lava_nc-0.8.0/src/lava/magma/core/learning/string_symbols.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/learning/symbolic_equation.py` & `lava_nc-0.8.0/src/lava/magma/core/learning/symbolic_equation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Copyright (C) 2021-22 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import re
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 import typing as ty
 import ast
 
 import lava.magma.core.learning.string_symbols as str_symbols
 
 
-class Symbol(object):
+class Symbol(ABC):
     """Super class for all possible symbols."""
 
     def __init__(self, expr: ty.Optional[str] = "") -> None:
         """Initialize a Symbol.
 
         Parameters
         ----------
@@ -46,16 +46,17 @@
         self._expr = expr
 
     @abstractmethod
     def __str__(self):
         pass
 
     @staticmethod
-    def find_expr(expr: str, reg_expr: str, symbol: "Symbol") \
-            -> ty.Tuple[ty.Optional["Symbol"], str]:
+    def find_expr(expr: str,
+                  reg_expr: str,
+                  symbol: "Symbol") -> ty.Tuple[ty.Optional["Symbol"], str]:
         """Factory method for creating symbols.
 
         Matches an expression to a regular expression and if there is a match,
         return a symbol of the matching part of the expression
         as well as the rest of the expression.
 
         Parameters
@@ -128,15 +129,14 @@
         res = res + "]"
 
         return res
 
 
 class Operator(Symbol):
     """Abstract super class for operator Symbols."""
-    pass
 
 
 class Addition(Operator):
     """Symbol representing the addition operator."""
 
     @staticmethod
     def find(expr: str) -> ty.Tuple[ty.Optional["Addition"], str]:
@@ -227,16 +227,14 @@
     def __str__(self):
         return "Multiplication(" + self._expr + ")"
 
 
 class FactorSym(Symbol):
     """Abstract super class for factor Symbols."""
 
-    pass
-
 
 class Dependency(FactorSym):
     """Abstract super class for dependency Symbols."""
 
 
 class X0(Dependency):
     """Symbol representing the x0 dependency."""
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/learning/utils.py` & `lava_nc-0.8.0/src/lava/magma/core/learning/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (C) 2021-22 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import numpy as np
 import typing as ty
-import struct
 
 
 def stochastic_round(values: np.ndarray,
                      random_numbers: ty.Union[int, float, np.ndarray],
                      probabilities: np.ndarray) -> np.ndarray:
     """Stochastically add 1 to an ndarray at location where random numbers are
     less than given probabilities.
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/model/interfaces.py` & `lava_nc-0.8.0/src/lava/magma/core/model/interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         """Returns the shape of the port"""
         return self._shape
 
     @property
     @abstractmethod
     def csp_ports(self) -> ty.List[AbstractCspPort]:
         """Returns all csp ports of the port."""
-        pass
 
     def start(self):
         """Start all csp ports."""
         for csp_port in self.csp_ports:
             csp_port.start()
 
     def join(self):
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/model/model.py` & `lava_nc-0.8.0/src/lava/magma/core/model/model.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/model/py/connection.py` & `lava_nc-0.8.0/src/lava/magma/core/model/py/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (C) 2021-23 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 from abc import abstractmethod
+from lava.utils.sparse import find
 import numpy as np
 import typing
+from scipy.sparse import csr_matrix
 
 from lava.magma.core.learning.learning_rule import (
     LoihiLearningRule,
     Loihi2FLearningRule,
     Loihi3FLearningRule,
 )
 from lava.magma.core.model.py.ports import PyInPort
@@ -301,15 +303,15 @@
     @abstractmethod
     def _create_learning_rule_applier(
             self, product_series: ProductSeries
     ) -> AbstractLearningRuleApplier:
         pass
 
     @abstractmethod
-    def _init_randoms(self):
+    def _init_randoms(self) -> None:
         pass
 
     @property
     def _x_traces(self) -> np.ndarray:
         """Get x traces.
 
         Returns
@@ -823,19 +825,20 @@
         y_taus = self._y_taus
 
         # get spike times
         t_spike_x = self.tx
         t_spike_y = self.ty
 
         # most naive algorithm to decay traces
-        x_traces_history = np.full((t_epoch + 1,) + x_traces.shape, np.nan,
+        x_traces_history = np.full((t_epoch + 1,) + x_traces.shape, 0,
                                    dtype=int)
         x_traces_history[0] = x_traces
-        y_traces_history = np.full((t_epoch + 1,) + y_traces.shape, np.nan,
+        y_traces_history = np.full((t_epoch + 1,) + y_traces.shape, 0,
                                    dtype=int)
+
         y_traces_history[0] = y_traces
 
         for t in range(1, t_epoch + 1):
             x_traces_history[t][x_taus != 0] = self._decay_trace(
                 x_traces_history[t - 1][x_taus != 0],
                 1,
                 x_taus[x_taus != 0][:, np.newaxis],
@@ -938,29 +941,37 @@
         learning rule."""
         applier_args = self._extract_applier_args(
             x_traces_history, y_traces_history
         )
 
         for syn_var_name, lr_applier in self._learning_rule_appliers.items():
             syn_var = getattr(self, syn_var_name).copy()
-            syn_var = np.left_shift(
-                syn_var, W_ACCUMULATOR_S - W_SYN_VAR_S[syn_var_name]
-            )
-            syn_var = lr_applier.apply(syn_var, **applier_args)
+            shift = W_ACCUMULATOR_S - W_SYN_VAR_S[syn_var_name]
+            if isinstance(syn_var, csr_matrix):
+                syn_var.data = syn_var.data << shift
+                dst, src, _ = find(syn_var, explicit_zeros=True)
+                syn_var[dst, src] = lr_applier.apply(syn_var,
+                                                     **applier_args)[dst, src]
+            else:
+                syn_var = syn_var << shift
+                syn_var = lr_applier.apply(syn_var, **applier_args)
+
             syn_var = self._saturate_synaptic_variable_accumulator(
                 syn_var_name, syn_var
             )
             syn_var = self._stochastic_round_synaptic_variable(
                 syn_var_name,
                 syn_var,
                 self._conn_var_random.random_stochastic_round,
             )
-            syn_var = np.right_shift(
-                syn_var, W_ACCUMULATOR_S - W_SYN_VAR_S[syn_var_name]
-            )
+
+            if isinstance(syn_var, csr_matrix):
+                syn_var.data = syn_var.data >> shift
+            else:
+                syn_var = syn_var >> shift
 
             syn_var = self._saturate_synaptic_variable(syn_var_name, syn_var)
             setattr(self, syn_var_name, syn_var)
 
     def _extract_applier_args(
         self, x_traces_history: np.ndarray, y_traces_history: np.ndarray
     ) -> dict:
@@ -1011,133 +1022,157 @@
             x_traces_history, y_traces_history
         )
         applier_args.update(evaluated_traces)
 
         return applier_args
 
     def _saturate_synaptic_variable_accumulator(
-            self, synaptic_variable_name: str,
-            synaptic_variable_values: np.ndarray
-    ) -> np.ndarray:
+            self, syn_var_name: str,
+            syn_var_values: typing.Union[np.ndarray, csr_matrix]
+    ) -> typing.Union[np.ndarray, csr_matrix]:
         """Saturate synaptic variable accumulator.
 
         Checks that sign is valid.
 
         Parameters
         ----------
-        synaptic_variable_name: str
+        syn_var_name: str
             Synaptic variable name.
-        synaptic_variable_values: ndarray
+        syn_var_values: ndarray, csr_matrix
             Synaptic variable values to saturate.
 
         Returns
         ----------
-        result : ndarray
+        result : ndarray, csr_matrix
             Saturated synaptic variable values.
         """
         # Weights
-        if synaptic_variable_name == "weights":
+        if syn_var_name == "weights":
             if self.sign_mode == SignMode.MIXED:
-                return synaptic_variable_values
+                return syn_var_values
             elif self.sign_mode == SignMode.EXCITATORY:
-                return np.maximum(0, synaptic_variable_values)
+                return np.maximum(0, syn_var_values)
             elif self.sign_mode == SignMode.INHIBITORY:
-                return np.minimum(0, synaptic_variable_values)
+                return np.minimum(0, syn_var_values)
         # Delays
-        elif synaptic_variable_name == "tag_2":
-            return np.maximum(0, synaptic_variable_values)
+        elif syn_var_name == "tag_2":
+            if isinstance(syn_var_values, csr_matrix):
+                syn_var_values.data[syn_var_values.data < 0] = 0
+                return syn_var_values
+            return np.maximum(0, syn_var_values)
         # Tags
-        elif synaptic_variable_name == "tag_1":
-            return synaptic_variable_values
+        elif syn_var_name == "tag_1":
+            return syn_var_values
         else:
             raise ValueError(
-                f"synaptic_variable_name can be 'weights', "
+                f"syn_var_name can be 'weights', "
                 f"'tag_1', or 'tag_2'."
-                f"Got {synaptic_variable_name=}."
+                f"Got {syn_var_name=}."
             )
 
     @staticmethod
     def _stochastic_round_synaptic_variable(
-        synaptic_variable_name: str,
-        synaptic_variable_values: np.ndarray,
+        syn_var_name: str,
+        syn_var_values: typing.Union[np.ndarray, csr_matrix],
         random: float,
-    ) -> np.ndarray:
+    ) -> typing.Union[np.ndarray, csr_matrix]:
         """Stochastically round synaptic variable after learning rule
         application.
 
         Parameters
         ----------
-        synaptic_variable_name: str
+        syn_var_name: str
             Synaptic variable name.
-        synaptic_variable_values: ndarray
+        syn_var_values: ndarray, csr_matrix
             Synaptic variable values to stochastically round.
 
         Returns
         ----------
-        result : ndarray
+        result : ndarray, csr_matrix
             Stochastically rounded synaptic variable values.
         """
-        exp_mant = 2 ** (W_ACCUMULATOR_U - W_SYN_VAR_U[synaptic_variable_name])
+        exp_mant = 2 ** (W_ACCUMULATOR_U - W_SYN_VAR_U[syn_var_name])
 
-        integer_part = synaptic_variable_values / exp_mant
+        if isinstance(syn_var_values, csr_matrix):
+            integer_part = syn_var_values.data / exp_mant
+        else:
+            integer_part = syn_var_values / exp_mant
         fractional_part = integer_part % 1
 
         integer_part = np.floor(integer_part)
         integer_part = stochastic_round(integer_part, random, fractional_part)
-        result = (integer_part * exp_mant).astype(
-            synaptic_variable_values.dtype
-        )
 
-        return result
+        if isinstance(syn_var_values, csr_matrix):
+            syn_var_values.data = (integer_part
+                                   * exp_mant).astype(syn_var_values.dtype)
+            return syn_var_values
+        else:
+            return (integer_part * exp_mant).astype(
+                syn_var_values.dtype
+            )
 
     def _saturate_synaptic_variable(
-            self, synaptic_variable_name: str,
-            synaptic_variable_values: np.ndarray
+            self, syn_var_name: str,
+            syn_var_val: typing.Union[np.ndarray, csr_matrix]
     ) -> np.ndarray:
         """Saturate synaptic variable.
 
         Checks that synaptic variable values is between bounds set by
         the hardware.
 
         Parameters
         ----------
-        synaptic_variable_name: str
+        syn_var_name: str
             Synaptic variable name.
-        synaptic_variable_values: ndarray
+        syn_var_val: ndarray, csr_matrix
             Synaptic variable values to saturate.
 
         Returns
         ----------
-        result : ndarray
+        result : ndarray, csr_matrix
             Saturated synaptic variable values.
         """
+
         # Weights
-        if synaptic_variable_name == "weights":
+        if syn_var_name == "weights":
             return clip_weights(
-                synaptic_variable_values,
+                syn_var_val,
                 sign_mode=self.sign_mode,
                 num_bits=W_WEIGHTS_U,
             )
         # Delays
-        elif synaptic_variable_name == "tag_2":
+        elif syn_var_name == "tag_2":
+            if isinstance(syn_var_val, csr_matrix):
+                _min = -(2 ** W_TAG_2_U) - 1
+                _max = (2 ** W_TAG_2_U) - 1
+                syn_var_val.data[syn_var_val.data < _min] = _min
+                syn_var_val.data[syn_var_val.data > _max] = _max
+                return syn_var_val
+
             return np.clip(
-                synaptic_variable_values, a_min=0, a_max=2 ** W_TAG_2_U - 1
+                syn_var_val, a_min=0, a_max=2 ** W_TAG_2_U - 1
             )
         # Tags
-        elif synaptic_variable_name == "tag_1":
+        elif syn_var_name == "tag_1":
+            if isinstance(syn_var_val, csr_matrix):
+                _min = -(2 ** W_TAG_1_U) - 1
+                _max = (2 ** W_TAG_1_U) - 1
+                syn_var_val.data[syn_var_val.data < _min] = _min
+                syn_var_val.data[syn_var_val.data > _max] = _max
+                return syn_var_val
             return np.clip(
-                synaptic_variable_values,
+                syn_var_val,
                 a_min=-(2 ** W_TAG_1_U) - 1,
                 a_max=2 ** W_TAG_1_U - 1,
             )
         else:
             raise ValueError(
-                f"synaptic_variable_name can be 'weights', "
+                f"syn_var_name can be 'weights', "
                 f"'tag_1', or 'tag_2'."
-                f"Got {synaptic_variable_name=}."
+                f"Got {syn_var_name=}."
             )
 
 
 class LearningConnectionModelFloat(PyLearningConnection):
     """Floating-point implementation of the Connection Process.
 
     This ProcessModel constitutes a behavioral implementation of Loihi synapses
@@ -1419,15 +1454,20 @@
         learning rule."""
         applier_args = self._extract_applier_args(
             x_traces_history, y_traces_history
         )
 
         for syn_var_name, lr_applier in self._learning_rule_appliers.items():
             syn_var = getattr(self, syn_var_name).copy()
-            syn_var = lr_applier.apply(syn_var, **applier_args)
+            if (isinstance(syn_var, csr_matrix)):
+                dst, src, _ = find(syn_var, explicit_zeros=True)
+                syn_var[dst, src] = lr_applier.apply(syn_var,
+                                                     **applier_args)[dst, src]
+            else:
+                syn_var = lr_applier.apply(syn_var, **applier_args)
             syn_var = self._saturate_synaptic_variable(syn_var_name, syn_var)
             setattr(self, syn_var_name, syn_var)
 
     def _extract_applier_args(
         self, x_traces_history: np.ndarray, y_traces_history: np.ndarray
     ) -> dict:
         """Extracts arguments for the LearningRuleApplierFloat.
@@ -1507,14 +1547,20 @@
                 return np.maximum(0, synaptic_variable_values)
             elif self.sign_mode == SignMode.INHIBITORY:
                 return np.minimum(0, synaptic_variable_values)
         # Delays
         elif synaptic_variable_name == "tag_1":
             return synaptic_variable_values
         elif synaptic_variable_name == "tag_2":
+            if isinstance(synaptic_variable_values, csr_matrix):
+                synaptic_variable_values[synaptic_variable_values < 0] = 0
+                return synaptic_variable_values
             return np.maximum(0, synaptic_variable_values)
         else:
             raise ValueError(
                 f"synaptic_variable_name can be 'weights', "
                 f"'tag_1', or 'tag_2'."
                 f"Got {synaptic_variable_name=}."
             )
+
+    def _init_randoms(self) -> None:
+        pass
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/model/py/model.py` & `lava_nc-0.8.0/src/lava/magma/core/model/py/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright (C) 2021-22 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import typing as ty
 from abc import ABC, abstractmethod
 import logging
+from lava.utils.sparse import find
 import numpy as np
+from scipy.sparse import csr_matrix
 import platform
 
 from lava.magma.compiler.channels.pypychannel import (
     CspSendPort,
     CspRecvPort,
     CspSelector,
 )
@@ -121,14 +123,20 @@
         elif isinstance(var, np.ndarray):
             # FIXME: send a whole vector (also runtime_service.py)
             var_iter = np.nditer(var, order="C")
             num_items: np.int32 = np.prod(var.shape)
             data_port.send(enum_to_np(num_items))
             for value in var_iter:
                 data_port.send(enum_to_np(value, np.float64))
+        elif isinstance(var, csr_matrix):
+            _, _, values = find(var, explicit_zeros=True)
+            num_items = var.data.size
+            data_port.send(enum_to_np(num_items))
+            for value in values:
+                data_port.send(enum_to_np(value, np.float64))
         elif isinstance(var, str):
             encoded_str = list(var.encode("ascii"))
             data_port.send(enum_to_np(len(encoded_str)))
             for ch in encoded_str:
                 data_port.send(enum_to_np(ch, d_type=np.int32))
 
     def _set_var(self):
@@ -157,26 +165,38 @@
             # Set data one by one
             for i in var_iter:
                 if num_items == 0:
                     break
                 num_items -= 1
                 i[...] = data_port.recv()[0]
             self.process_to_service.send(MGMT_RESPONSE.SET_COMPLETE)
+        elif isinstance(var, csr_matrix):
+            # First item is number of items
+            num_items = int(data_port.recv()[0])
+
+            buffer = np.empty(num_items)
+            # Set data one by one
+            for i in range(num_items):
+                buffer[i] = data_port.recv()[0]
+            dst, src, _ = find(var)
+            var = csr_matrix((buffer, (dst, src)), var.shape)
+            setattr(self, var_name, var)
+
+            self.process_to_service.send(MGMT_RESPONSE.SET_COMPLETE)
         elif isinstance(var, str):
             # First item is number of items
             num_items = int(data_port.recv()[0])
 
             s = []
             for i in range(num_items):
                 s.append(int(data_port.recv()[0]))  # decode string from ascii
 
             s = bytes(s).decode("ascii")
             setattr(self, var_name, s)
             self.process_to_service.send(MGMT_RESPONSE.SET_COMPLETE)
-
         else:
             self.process_to_service.send(MGMT_RESPONSE.ERROR)
             raise RuntimeError("Unsupported type")
 
         # notify PM that Vars have been changed
         self.on_var_update()
 
@@ -218,30 +238,28 @@
             self._action = self._selector.select(*self._channel_actions)
 
     @abstractmethod
     def add_ports_for_polling(self):
         """
         Add various ports to poll for communication on ports
         """
-        pass
 
     def join(self):
         """
         Wait for all the ports to shutdown.
         """
         self.service_to_process.join()
         self.process_to_service.join()
         for p in self.py_ports:
             p.join()
 
     def on_var_update(self):
         """This method is called if a Var is updated. It
         can be used as callback function to calculate dependent
         changes."""
-        pass
 
 
 class PyLoihiProcessModel(AbstractPyProcessModel):
     """
     ProcessModel to simulate a Process on Loihi using CPU.
 
     The PyLoihiProcessModel implements the same phases of execution as the
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/model/py/neuron.py` & `lava_nc-0.8.0/src/lava/magma/core/model/py/neuron.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/model/py/ports.py` & `lava_nc-0.8.0/src/lava/magma/core/model/py/ports.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         connected PyPorts. The CSP Port is the low level interface of the
         backend messaging infrastructure which is used to send and receive data.
 
         Returns
         -------
         A list of all CSP Ports connected to the PyPort.
         """
-        pass
 
 
 class AbstractPyIOPort(AbstractPyPort):
     """Abstract class of an input/output Port implemented in python.
 
     A PyIOPort can either be an input or an output Port and is the common
     abstraction of PyInPort/PyOutPort.
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/model/sub/model.py` & `lava_nc-0.8.0/src/lava/magma/core/model/sub/model.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/process/connection.py` & `lava_nc-0.8.0/src/lava/magma/core/process/connection.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/process/interfaces.py` & `lava_nc-0.8.0/src/lava/magma/core/process/interfaces.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/process/neuron.py` & `lava_nc-0.8.0/src/lava/magma/core/process/neuron.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/process/ports/exceptions.py` & `lava_nc-0.8.0/src/lava/magma/core/process/ports/exceptions.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/process/ports/ports.py` & `lava_nc-0.8.0/src/lava/magma/core/process/ports/ports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (C) 2021-22 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
+from __future__ import annotations
 import typing as ty
 from abc import ABC, abstractmethod
 import math
 import numpy as np
 import functools as ft
 
 from lava.magma.core.process.interfaces import AbstractProcessMember
@@ -379,45 +380,37 @@
 
 class AbstractIOPort(AbstractPort):
     """Abstract base class for InPorts and OutPorts.
     This class needs no implementation and only serves to establish a clear
     type hierarchy needed for validating connections.
     """
 
-    pass
-
 
 class AbstractRVPort(AbstractPort):
     """Abstract base class for RefPorts and VarPorts.
     This class needs no implementation and only serves to establish a clear
     type hierarchy needed for validating connections.
     """
 
-    pass
-
 
 class AbstractSrcPort(ABC):
     """Interface for source ports such as OutPorts and RefPorts from which
     connections originate.
     This class needs no implementation and only serves to establish a clear
     type hierarchy needed for validating connections.
     """
 
-    pass
-
 
 class AbstractDstPort(ABC):
     """Interface for destination ports such as InPorts and VarPorts in which
     connections terminate.
     This class needs no implementation and only serves to establish a clear
     type hierarchy needed for validating connections.
     """
 
-    pass
-
 
 class OutPort(AbstractIOPort, AbstractSrcPort):
     """Output ports are members of a Lava Process and can be connected to
     other ports to facilitate sending of messages via channels.
 
     OutPorts connect to other InPorts of peer processes or to other OutPorts of
     processes that contain this OutPort's parent process as a sub process.
@@ -631,28 +624,30 @@
         self.connect(var_ports)
 
     def get_dst_vars(self) -> ty.List[Var]:
         """Returns destination Vars this RefPort is connected to."""
         return [ty.cast(VarPort, p).var for p in self.get_dst_ports()]
 
     @staticmethod
-    def create_implicit_var_port(var: Var) -> "ImplicitVarPort":
+    def create_implicit_var_port(var: Var) -> ImplicitVarPort:
         """Creates and returns an ImplicitVarPort for the given Var."""
         # Create a VarPort to wrap Var
         vp = ImplicitVarPort(var)
         # Propagate name and parent process of Var to VarPort
         vp.name = "_" + var.name + "_implicit_port"
         if var.process is not None:
             # Only assign when parent process is already assigned
             vp.process = var.process
             # VarPort name could shadow existing attribute
             if hasattr(var.process, vp.name):
-                raise AssertionError(
-                    "Name of implicit VarPort might conflict"
-                    " with existing attribute.")
+                name = str(vp.name)
+                name_suffix = 1
+                while hasattr(var.process, vp.name):
+                    vp.name = name + "_" + str(name_suffix)
+                    name_suffix += 1
             setattr(var.process, vp.name, vp)
             var.process.var_ports.add_members({vp.name: vp})
 
         return vp
 
 
 class VarPort(AbstractRVPort, AbstractDstPort):
@@ -745,15 +740,17 @@
                         p.process.__class__.__name__, p.name))
         self._connect_backward(to_list(ports), AbstractRVPort)
 
 
 class ImplicitVarPort(VarPort):
     """Sub class for VarPort to identify implicitly created VarPorts when
     a RefPort connects directly to a Var."""
-    pass
+
+    def __init__(self, var: Var) -> None:
+        super().__init__(var)
 
 
 class AbstractVirtualPort(AbstractPort):
     """Abstract base class interface for any type of port that merely serves
     to transform the properties of a user-defined port."""
 
     @property
@@ -822,15 +819,15 @@
     port before connecting to another port.
     It is used by the compiler to map the indices of the underlying
     tensor-valued data array from the derived to the new shape."""
 
     def __init__(self,
                  new_shape: ty.Tuple[int, ...],
                  old_shape: ty.Tuple[int, ...]):
-        AbstractPort.__init__(self, new_shape)
+        super().__init__(new_shape)
         self.old_shape = old_shape
 
     def get_transform_func_fwd(self) -> ft.partial:
         """Returns a function pointer that implements the forward (fwd)
         transformation of the ReshapePort, which reshapes incoming data to
         a new shape (the shape of the destination Process).
 
@@ -857,15 +854,15 @@
     ports along given axis into a new port before connecting to another port.
     The shape of all concatenated ports outside of the concatenation
     dimension must be the same.
     It is used by the compiler to map the indices of the underlying
     tensor-valued data array from the derived to the new shape."""
 
     def __init__(self, ports: ty.List[AbstractPort], axis: int):
-        AbstractPort.__init__(self, self._get_new_shape(ports, axis))
+        super().__init__(self._get_new_shape(ports, axis))
         self._connect_backward(
             ports, AbstractPort, assert_same_shape=False, assert_same_type=True
         )
         self.concat_axis = axis
 
     @staticmethod
     def _get_new_shape(ports: ty.List[AbstractPort], axis):
@@ -912,15 +909,15 @@
         out_port.transpose([3, 1, 2]).connect(in_port)
     """
 
     def __init__(self,
                  new_shape: ty.Tuple[int, ...],
                  axes: ty.Tuple[int, ...]):
         self.axes = axes
-        AbstractPort.__init__(self, new_shape)
+        super().__init__(new_shape)
 
     def get_transform_func_fwd(self) -> ft.partial:
         """Returns a function pointer that implements the forward (fwd)
         transformation of the TransposePort, which transposes (permutes)
         incoming data according to a specific order of axes (to match the
         destination Process).
 
@@ -937,22 +934,7 @@
         source Process).
 
         Returns
         -------
         function_pointer : functools.partial
             a function pointer that can be applied to incoming data"""
         return ft.partial(np.transpose, axes=np.argsort(self.axes))
-
-
-class ReIndexPort(AbstractVirtualPort):
-    """A ReIndexPort is a virtual port that allows to re-index the elements
-    of a port before connecting to another port.
-    It is used by the compiler to map the indices of the underlying
-    tensor-valued data array from the derived to the new shape.
-
-    Example:
-        out_port = OutPort((2, 2))
-        in_port = InPort((2, 2))
-        out_port.reindex([3, 1, 0, 2]).connect(in_port)
-    """
-
-    pass
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/process/process.py` & `lava_nc-0.8.0/src/lava/magma/core/process/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from lava.magma.core.process.message_interface_enum import ActorType
 from lava.magma.core.process.ports.ports import \
     InPort, OutPort, RefPort, VarPort
 from lava.magma.core.process.variable import Var
 from lava.magma.core.run_conditions import AbstractRunCondition
 from lava.magma.core.run_configs import RunConfig
 from lava.magma.runtime.runtime import Runtime
-from lava.magma.runtime.runtime_services.enums import LoihiVersion
 
 if ty.TYPE_CHECKING:
     from lava.magma.core.model.model import AbstractProcessModel
 
 
 class ProcessPostInitCaller(type):
     """Metaclass for AbstractProcess that overwrites __call__() in order to
@@ -219,15 +218,14 @@
         """On destruction, terminate Runtime automatically to
         free compute resources.
         """
         self.stop()
 
     def __enter__(self):
         """Executed when Process enters a "with" block of a context manager."""
-        pass
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """Stop the runtime when exiting "with" block of a context manager."""
         self.stop()
 
     def _post_init(self):
         """Called after __init__() method of any sub class via
@@ -279,15 +277,15 @@
     @runtime.setter
     def runtime(self, value):
         """Returns current Runtime or None if no Runtime exists."""
         self._runtime = value
 
     def register_sub_procs(self, procs: ty.Dict[str, AbstractProcess]):
         """Registers other processes as sub processes of this process."""
-        for name, p in procs.items():
+        for p in procs.values():
             if not isinstance(p, AbstractProcess):
                 raise AssertionError
             p.parent_proc = self
         self.procs.add_members(procs)
 
     def validate_var_aliases(self):
         """Validates that any aliased Var is a member of a Process that is a
@@ -326,39 +324,63 @@
         - stop() terminates execution and releases control of all
           involved compute nodes.
 
         If a run has been suspended by either pause() or a RunCondition
         being no longer satisfied, run() can be called again to resume
         execution from the current state.
 
+        NOTE: run_cfg will be ignored when re-running a previously compiled
+        process.
+
         Parameters
         ----------
         condition : AbstractRunCondition
             Specifies for how long to run the Process.
         run_cfg : RunConfig, optional
             Used by the compiler to select a ProcessModel for each Process.
             Must be provided when Processes have to be compiled, can be
             omitted otherwise.
         compile_config: Dict[str, Any], optional
             Configuration options for the Compiler and SubCompilers.
         """
         if not self._runtime:
             if not run_cfg:
-                raise ValueError("The Processes that are to be executed have "
-                                 "not been compiled yet. This requires that a"
-                                 "RunConfig is passed to the run() method.")
+                raise ValueError("run_cfg must not be None when calling"
+                                 " Process.run() unless the process has already"
+                                 " been compiled.")
+            self.create_runtime(run_cfg=run_cfg, compile_config=compile_config)
+        self._runtime.start(condition)
 
-            executable = self.compile(run_cfg, compile_config)
-            self._runtime = Runtime(executable,
-                                    ActorType.MultiProcessing,
-                                    loglevel=self._log_config.level)
-            executable.assign_runtime_to_all_processes(self._runtime)
-            self._runtime.initialize()
+    def create_runtime(self, run_cfg: ty.Optional[RunConfig] = None,
+                       executable: ty.Optional[Executable] = None,
+                       compile_config:
+                       ty.Optional[ty.Dict[str, ty.Any]] = None):
+        """Creates a runtime for this process and all connected processes by
+        compiling the process to an executable and assigning that executable to
+        the process and connected processes.
 
-        self._runtime.start(condition)
+        See Process.run() for information on Process blocking, which must be
+        specified in the run_cfg passed to create_runtime.
+
+        Parameters
+        ----------
+        run_cfg : RunConfig, optional
+            Used by the compiler to select a ProcessModel for each Process.
+            Must be provided when Processes have to be compiled, can be
+            omitted otherwise.
+        compile_config: Dict[str, Any], optional
+            Configuration options for the Compiler and SubCompilers.
+        """
+        if executable is None:
+            executable = self.compile(run_cfg, compile_config)
+        self._runtime = Runtime(executable,
+                                ActorType.MultiProcessing,
+                                loglevel=self._log_config.level)
+        executable.assign_runtime_to_all_processes(self._runtime)
+        self._runtime.initialize()
 
     def compile(self,
                 run_cfg: RunConfig,
                 compile_config: ty.Optional[ty.Dict[str, ty.Any]] = None
                 ) -> Executable:
         """Compiles this and any process connected to this process and
         returns the resulting Executable that can either be serialized or
@@ -588,7 +610,13 @@
 
     def __next__(self):
         self._iterator += 1
         if self._iterator < len(self.members):
             return getattr(self, self.member_names[self._iterator])
         self._iterator = -1
         raise StopIteration
+
+    def __getstate__(self):
+        return self.__dict__
+
+    def __setstate__(self, d):
+        self.__dict__ = d
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/process/variable.py` & `lava_nc-0.8.0/src/lava/magma/core/process/variable.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (C) 2021-22 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import typing as ty
 import numpy as np
-
+from scipy.sparse import csr_matrix, spmatrix
+from lava.utils.sparse import find
 from lava.magma.core.process.interfaces import (
     AbstractProcessMember,
     IdGeneratorSingleton,
 )
 
 
 class Var(AbstractProcessMember):
@@ -122,44 +123,65 @@
                     f"'{other_proc.name}::{other_proc.__class__.__name__}' "
                     f"must be a member of a process that is a strict sub "
                     f"process of the aliasing Var's '{self.name}' in process "
                     f"'{self.process.name}::{self.process.__class__.__name__}'"
                     f"."
                 )
 
-    def set(self, value: ty.Union[np.ndarray, str], idx: np.ndarray = None):
+    def set(self,
+            value: ty.Union[np.ndarray, str, spmatrix],
+            idx: np.ndarray = None):
         """Sets value of Var. If this Var aliases another Var, then set(..) is
         delegated to aliased Var."""
         if self.aliased_var is not None:
             self.aliased_var.set(value, idx)
         else:
             if self.process.runtime:
                 # encode if var is str
                 if isinstance(value, str):
                     value = np.array(
                         list(value.encode("ascii")), dtype=np.int32
                     )
+                elif isinstance(value, spmatrix):
+                    value = value.tocsr()
+                    init_dst, init_src, init_val = find(self.init,
+                                                        explicit_zeros=True)
+                    dst, src, val = find(value, explicit_zeros=True)
+                    if value.shape != self.init.shape or \
+                            np.any(init_dst != dst) or \
+                            np.any(init_src != src) or \
+                            len(val) != len(init_val):
+                        raise ValueError("Indices and number of non-zero "
+                                         "elements must stay equal when using"
+                                         "set on a sparse matrix.")
+                    value = val
+
                 self.process.runtime.set_var(self.id, value, idx)
             else:
                 raise ValueError(
                     "No Runtime available yet. Cannot set new 'Var' without "
                     "Runtime."
                 )
 
     def get(self, idx: np.ndarray = None) -> np.ndarray:
         """Gets and returns value of Var. If this Var aliases another Var,
         then get() is delegated to aliased Var."""
         if self.aliased_var is not None:
             return self.aliased_var.get(idx)
         else:
-            if self.process.runtime:
+            if self.process and self.process.runtime:
                 buffer = self.process.runtime.get_var(self.id, idx)
                 if isinstance(self.init, str):
                     # decode if var is string
                     return bytes(buffer.astype(int).tolist()).decode("ascii")
+                if isinstance(self.init, csr_matrix):
+                    dst, src, _ = find(self.init)
+
+                    ret = csr_matrix((buffer, (dst, src)), self.init.shape)
+                    return ret
                 else:
                     return buffer
             else:
                 return self.init
 
     def __repr__(self):
         return (
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/run_conditions.py` & `lava_nc-0.8.0/src/lava/magma/core/run_conditions.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/run_configs.py` & `lava_nc-0.8.0/src/lava/magma/core/run_configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,19 +75,17 @@
             for sd in custom_sync_domains:
                 if not isinstance(sd, SyncDomain):
                     raise AssertionError("Expected list of SyncDomains.")
             self.custom_sync_domains += custom_sync_domains
 
     def exclude_nodes(self, nodes: ty.List[AbstractNode]):
         """Excludes given nodes from consideration by compiler."""
-        pass
 
     def require_nodes(self, nodes: ty.List[AbstractNode]):
         """Requires that compiler maps processes to given nodes."""
-        pass
 
     def select(self,
                process: AbstractProcess,
                proc_model: ty.List[ty.Type[AbstractProcessModel]]) \
             -> ty.Type[AbstractProcessModel]:
         pass
 
@@ -164,54 +162,55 @@
         self.select_tag = select_tag
         self.select_sub_proc_model = select_sub_proc_model
         self.exception_proc_model_map = exception_proc_model_map
         if not exception_proc_model_map:
             self.exception_proc_model_map = {}
 
     def select(self,
-               proc: AbstractProcess,
+               process: AbstractProcess,
                proc_models: ty.List[ty.Type[AbstractProcessModel]]) \
             -> ty.Type[AbstractProcessModel]:
         """
         Selects an appropriate ProcessModel from a list of ProcessModels for
         a Process, based on user requests.
 
         Parameters
         ----------
-        proc: AbstractProcess
+        process: AbstractProcess
             Process for which ProcessModel is selected
         proc_models: List[AbstractProcessModel]
             List of ProcessModels to select from
 
         Returns
         -------
         Selected ProcessModel class
         """
         num_pm = len(proc_models)
         # Case 0: No ProcessModels exist:
         # ------------------------------
         # Raise error
         if num_pm == 0:
-            raise AssertionError(f"[{self.__class__.__qualname__}]: No "
-                                 f"ProcessModels exist for Process "
-                                 f"{proc.name}::{proc.__class__.__qualname__}.")
+            raise AssertionError(
+                f"[{self.__class__.__qualname__}]: No ProcessModels exist for "
+                f"Process {process.name}::{process.__class__.__qualname__}."
+            )
 
         # Required modules and helper functions
         from lava.magma.core.model.sub.model import AbstractSubProcessModel
 
         def _issubpm(pm: ty.Type[AbstractProcessModel]) -> bool:
             """Checks if input ProcessModel is a SubProcessModel"""
             return issubclass(pm, AbstractSubProcessModel)
 
         # Case 1: Exceptions in a dict:
         # ----------------------------
         # We will simply return the ProcessModel class associated with a
         # Process class in the exceptions dictionary
-        if proc.__class__ in self.exception_proc_model_map:
-            return self.exception_proc_model_map[proc.__class__]
+        if process.__class__ in self.exception_proc_model_map:
+            return self.exception_proc_model_map[process.__class__]
 
         # Case 2: Only 1 PM found:
         # -----------------------
         # Assumption: User doesn't care about the type: Sub or HW-specific.
         if num_pm == 1:
             # If type of the PM is neither Sub nor HW-supported, raise error
             if not (_issubpm(proc_models[0]) or self._is_hw_supported(
@@ -243,16 +242,16 @@
                         return proc_models[0]
                     else:
                         # We did not find the tag that user provided in tags
                         raise AssertionError(
                             f"[{self.__class__.__qualname__}]: No "
                             f"ProcessModels found with tag "
                             f"'{self.select_tag}' for Process "
-                            f"{proc.name}::"
-                            f"{proc.__class__.__qualname__}.")
+                            f"{process.name}::"
+                            f"{process.__class__.__qualname__}.")
 
         # Case 3: Multiple PMs exist:
         # --------------------------
         # Collect indices of Sub and HW-specific PMs:
         sub_pm_idxs = [idx for idx, pm in enumerate(proc_models) if
                        _issubpm(pm)]
         leaf_pm_idxs = self._order_according_to_resources(proc_models)
@@ -265,67 +264,69 @@
             if len(sub_pm_idxs) == 1:
                 return proc_models[sub_pm_idxs[0]]
             # Case 3a(ii): User didn't provide select_tag:
             # -------------------------------------------
             # Assumption: User doesn't care about tags. We return the first
             # SubProcessModel found
             if self.select_tag is None:
-                self.log.info(f"[{self.__class__.__qualname__}]: Using the"
-                              f" first SubProcessModel "
-                              f"{proc_models[sub_pm_idxs[0]].__qualname__} "
-                              f"available for Process "
-                              f"{proc.name}::{proc.__class__.__qualname__}.")
+                self.log.info(
+                    f"[{self.__class__.__qualname__}]: Using the first "
+                    f"SubProcessModel "
+                    f"{proc_models[sub_pm_idxs[0]].__qualname__} "
+                    f"available for Process "
+                    f"{process.name}::{process.__class__.__qualname__}."
+                )
                 return proc_models[sub_pm_idxs[0]]
             # Case 3a(iii): User asked for a specific tag:
             # -------------------------------------------
             else:
                 # Collect indices of all SubPMs with select_tag
                 valid_sub_pm_idxs = \
                     [idx for idx in sub_pm_idxs
                      if self.select_tag in proc_models[sub_pm_idxs[idx]].tags]
                 if len(valid_sub_pm_idxs) == 0:
                     raise AssertionError(f"[{self.__class__.__qualname__}]: No "
                                          f"ProcessModels found with tag "
                                          f"{self.select_tag} for Process "
-                                         f"{proc.name}::"
-                                         f"{proc.__class__.__qualname__}.")
+                                         f"{process.name}::"
+                                         f"{process.__class__.__qualname__}.")
                 return proc_models[valid_sub_pm_idxs[0]]
         # Case 3b: User didn't ask for SubProcessModel:
         # --------------------------------------------
         # Raise error if no HW-specific ProcessModels exist
         if len(leaf_pm_idxs) == 0:
             raise AssertionError(f"[{self.__class__.__qualname__}]: "
                                  f"No hardware-specific ProcessModels were "
-                                 f"found for Process {proc.name}::"
-                                 f"{proc.__class__.__qualname__}. "
+                                 f"found for Process {process.name}::"
+                                 f"{process.__class__.__qualname__}. "
                                  f"Try setting select_sub_proc_model=True.")
         # Case 3b(i): User didn't provide select_tag:
         # ------------------------------------------
         # Assumption: User doesn't care about tags. We return the first
         # HW-specific ProcessModel found
         if self.select_tag is None:
             self.log.info(f"[{self.__class__.__qualname__}]: Using the first "
                           f"Hardware-specific ProcessModel "
                           f"{proc_models[leaf_pm_idxs[0]].__qualname__} "
                           f"available for Process "
-                          f"{proc.name}::{proc.__class__.__qualname__}.")
+                          f"{process.name}::{process.__class__.__qualname__}.")
             return proc_models[leaf_pm_idxs[0]]
         # Case 3b(ii): User asked for a specific tag:
         # ------------------------------------------
         else:
             # Collect indices of all HW-specific PMs with select_tag
             valid_leaf_pm_idxs = \
                 [idx for idx in leaf_pm_idxs
                  if self.select_tag in proc_models[idx].tags]
             if len(valid_leaf_pm_idxs) == 0:
                 raise AssertionError(f"[{self.__class__.__qualname__}]: No "
                                      f"ProcessModels found with tag "
                                      f"'{self.select_tag}' for Process "
-                                     f"{proc.name}::"
-                                     f"{proc.__class__.__qualname__}.")
+                                     f"{process.name}::"
+                                     f"{process.__class__.__qualname__}.")
             return proc_models[valid_leaf_pm_idxs[0]]
 
     def _is_hw_supported(self, pm: ty.Type[AbstractProcessModel]) -> bool:
         """Checks if the process models is a PyProcModel"""
         return issubclass(pm, AbstractPyProcessModel)
 
     def _order_according_to_resources(self, proc_models: ty.List[ty.Type[
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/sync/domain.py` & `lava_nc-0.8.0/src/lava/magma/core/sync/domain.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/sync/protocol.py` & `lava_nc-0.8.0/src/lava/magma/core/sync/protocol.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/sync/protocols/async_protocol.py` & `lava_nc-0.8.0/src/lava/magma/core/sync/protocols/async_protocol.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/core/sync/protocols/loihi_protocol.py` & `lava_nc-0.8.0/src/lava/magma/core/sync/protocols/loihi_protocol.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/runtime/LICENSE` & `lava_nc-0.8.0/src/lava/magma/runtime/LICENSE`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/runtime/message_infrastructure/factory.py` & `lava_nc-0.8.0/src/lava/magma/runtime/message_infrastructure/factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # SPDX-License-Identifier: LGPL 2.1 or later
 # See: https://spdx.org/licenses/
 
 from lava.magma.core.process.message_interface_enum import ActorType
 from lava.magma.runtime.message_infrastructure.multiprocessing import \
     MultiProcessing
 
-"""Factory class to create the messaging infrastructure"""
-
 
 class MessageInfrastructureFactory:
-    """Creates the message infrastructure instance based on type"""
+    """Factory class to create the messaging infrastructure"""
+
     @staticmethod
     def create(factory_type: ActorType):
-        """type of actor framework being chosen"""
+        """Creates the message infrastructure instance based on type
+        of actor framework being chosen."""
         if factory_type == ActorType.MultiProcessing:
             return MultiProcessing()
         else:
             raise Exception("Unsupported factory_type")
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/runtime/message_infrastructure/message_infrastructure_interface.py` & `lava_nc-0.8.0/src/lava/magma/runtime/message_infrastructure/message_infrastructure_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,44 +9,37 @@
     from lava.magma.compiler.builders.runtimeservice_builder import \
         RuntimeServiceBuilder
 from abc import ABC, abstractmethod
 
 from lava.magma.compiler.channels.interfaces import ChannelType, Channel
 from lava.magma.core.sync.domain import SyncDomain
 
-"""A Message Infrastructure Interface which can create actors which would
-participate in message passing/exchange, start and stop them as well as
-declare the underlying Channel Infrastructure Class to be used for message
-passing implementation."""
-
 
 class MessageInfrastructureInterface(ABC):
-    """Interface to provide the ability to create actors which can
-    communicate via message passing"""
+    """A Message Infrastructure Interface which can create actors which would
+    participate in message passing/exchange, start and stop them as well as
+    declare the underlying Channel Infrastructure Class to be used for message
+    passing implementation."""
+
     @abstractmethod
     def start(self):
         """Starts the messaging infrastructure"""
-        pass
 
     @abstractmethod
     def stop(self):
         """Stops the messaging infrastructure"""
-        pass
 
     @abstractmethod
     def build_actor(self, target_fn: ty.Callable, builder: ty.Union[
         ty.Dict['AbstractProcess', 'PyProcessBuilder'], ty.Dict[
             SyncDomain, 'RuntimeServiceBuilder']]):
         """Given a target_fn starts a system process"""
-        pass
 
     @property
     @abstractmethod
     def actors(self) -> ty.List[ty.Any]:
         """Returns a list of actors"""
-        pass
 
     @abstractmethod
     def channel_class(self, channel_type: ChannelType) -> ty.Type[Channel]:
         """Given the Channel Type, Return the Channel Implementation to
         be used during execution"""
-        pass
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/runtime/message_infrastructure/multiprocessing.py` & `lava_nc-0.8.0/src/lava/magma/runtime/message_infrastructure/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/runtime/message_infrastructure/nx.py` & `lava_nc-0.8.0/src/lava/magma/runtime/message_infrastructure/nx.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,29 +13,25 @@
 
 class NxBoardMsgInterface(MessageInfrastructureInterface):
     """Implements message passing using nx board"""
 
     @property
     def actors(self):
         """Returns a list of actors"""
-        pass
 
     def start(self):
         """Starts the shared memory manager"""
-        pass
 
     def build_actor(self, target_fn: ty.Callable, builder: ty.Union[
         ty.Dict['AbstractProcess', 'PyProcessBuilder'], ty.Dict[
             SyncDomain, 'RuntimeServiceBuilder']]) -> ty.Any:
         """Given a target_fn starts a system (os) process"""
-        pass
 
     def stop(self):
         """Stops the shared memory manager"""
-        pass
 
     def channel_class(self, channel_type: ChannelType) -> ty.Type[ChannelType]:
         """Given a channel type, returns the shared memory based class
         implementation for the same."""
         if channel_type == ChannelType.CNc:
             return CNcChannel
         elif channel_type == ChannelType.NcC:
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/runtime/message_infrastructure/shared_memory_manager.py` & `lava_nc-0.8.0/src/lava/magma/runtime/message_infrastructure/shared_memory_manager.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/runtime/mgmt_token_enums.py` & `lava_nc-0.8.0/src/lava/magma/runtime/mgmt_token_enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (C) 2021-22 Intel Corporation
 # SPDX-License-Identifier: LGPL 2.1 or later
 # See: https://spdx.org/licenses/
 
+"""Defines message tokens for Actions (Commands) and Responses. Also defines
+helper functions to convert scalar values to these message tokens."""
+
 import typing as ty
 import numpy as np
 
-"""Defines message tokens for Actions (Commands) and Responses. Also defines
-helper functions to convert scalar values to these message tokens"""
-
 
 def enum_to_np(value: ty.Union[int, float],
                d_type: type = np.float64) -> np.array:
     """
     Helper function to convert an int (or EnumInt) or a float to a single value
     np array so as to pass it via the message passing framework. The dtype of
     the np array is specified by d_type with the default of np.int32.
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/runtime/runtime.py` & `lava_nc-0.8.0/src/lava/magma/runtime/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 # See: https://spdx.org/licenses/
 
 from __future__ import annotations
 
 import logging
 import sys
 import traceback
-import typing
 import typing as ty
 
 import numpy as np
-from lava.magma.compiler.channels.pypychannel import CspRecvPort, CspSendPort
+from scipy.sparse import csr_matrix
 from lava.magma.compiler.var_model import AbstractVarModel, LoihiSynapseVarModel
 from lava.magma.core.process.message_interface_enum import ActorType
 from lava.magma.runtime.message_infrastructure.factory import \
     MessageInfrastructureFactory
 from lava.magma.runtime.message_infrastructure. \
     message_infrastructure_interface import \
     MessageInfrastructureInterface
@@ -110,29 +109,30 @@
 
     def __init__(self,
                  exe: Executable,
                  message_infrastructure_type: ActorType,
                  loglevel: int = logging.WARNING):
         self.log = logging.getLogger(__name__)
         self.log.setLevel(loglevel)
-        self._run_cond: typing.Optional[AbstractRunCondition] = None
+        self._run_cond: ty.Optional[AbstractRunCondition] = None
         self._executable: Executable = exe
 
         self._messaging_infrastructure_type: ActorType = \
             message_infrastructure_type
         self._messaging_infrastructure: \
             ty.Optional[MessageInfrastructureInterface] = None
         self._is_initialized: bool = False
         self._is_running: bool = False
         self._is_started: bool = False
         self._req_paused: bool = False
         self._req_stop: bool = False
         self.runtime_to_service: ty.Iterable[CspSendPort] = []
         self.service_to_runtime: ty.Iterable[CspRecvPort] = []
         self._open_ports: ty.List[AbstractCspPort] = []
+        self.num_steps: int = 0
 
     def __del__(self):
         """On destruction, terminate Runtime automatically to
         free compute resources.
         """
         if self._is_started:
             self.stop()
@@ -505,14 +505,23 @@
             req_port.send(MGMT_COMMAND.GET_DATA)
             req_port.send(enum_to_np(model_id))
             req_port.send(enum_to_np(var_id))
 
             # 2. Receive Data [NUM_ITEMS, DATA1, DATA2, ...]
             data_port: CspRecvPort = self.service_to_runtime[runtime_srv_id]
             num_items: int = int(data_port.recv()[0].item())
+
+            if ev.dtype == csr_matrix:
+                buffer = np.zeros(num_items)
+
+                for i in range(num_items):
+                    buffer[i] = data_port.recv()[0]
+
+                return buffer[idx] if idx else buffer
+
             buffer: np.ndarray = np.zeros((1, np.prod(ev.shape)))
             for i in range(num_items):
                 buffer[0, i] = data_port.recv()[0]
 
             # 3. Reshape result and return
             reshape_order = 'F' if isinstance(
                 ev, LoihiSynapseVarModel) else 'C'
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/runtime/runtime_services/channel_broker/channel_broker.py` & `lava_nc-0.8.0/src/lava/magma/runtime/runtime_services/channel_broker/channel_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from lava.magma.runtime.message_infrastructure.shared_memory_manager import (
     SharedMemoryManager,
 )
 
 try:
     from nxcore.arch.base.nxboard import NxBoard
     from nxcore.graph.channel import Channel
-    from nxcore.graph.processes.phase_enums import Phase
     from nxcore.graph.processes.embedded.embedded_snip import EmbeddedSnip
 except ImportError:
     class NxBoard:
         pass
 
     class Channel:
         pass
```

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/runtime/runtime_services/enums.py` & `lava_nc-0.8.0/src/lava/magma/runtime/runtime_services/enums.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/runtime/runtime_services/interfaces.py` & `lava_nc-0.8.0/src/lava/magma/runtime/runtime_services/interfaces.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/magma/runtime/runtime_services/runtime_service.py` & `lava_nc-0.8.0/src/lava/magma/runtime/runtime_services/runtime_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,33 @@
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: LGPL 2.1 or later
 # See: https://spdx.org/licenses/
 
+"""The RuntimeService interface is responsible for
+coordinating the execution of a group of process models belonging to a common
+synchronization domain. The domain will follow a SyncProtocol or will be
+asynchronous. The processes and their corresponding process models are
+selected by the Runtime dependent on the RunConfiguration assigned at the
+start of execution. For each group of processes which follow the same
+protocol and execute on the same node, the Runtime creates a RuntimeService.
+Each RuntimeService coordinates all actions and commands from the Runtime,
+transmitting them to the processes under its management and
+returning action and command responses back to Runtime.
+
+RuntimeService Types:
+
+PyRuntimeService: (Abstract Class) Coordinates process models executing on
+   the CPU and written in Python.
+   Concrete Implementations:
+    a. LoihiPyRuntimeService: Coordinates process models executing on
+       the CPU and written in Python and following the LoihiProtocol.
+    b. AsyncPyRuntimeService: Coordinates process models executing on
+       the CPU and written in Python and following the AsyncProtocol.
+"""
+
 import logging
 import typing as ty
 from abc import abstractmethod
 
 import numpy as np
 
 from lava.magma.compiler.channels.pypychannel import (
@@ -21,36 +43,14 @@
     MGMT_COMMAND,
 )
 
 from lava.magma.runtime.runtime_services.enums import LoihiPhase
 from lava.magma.runtime.runtime_services.interfaces import \
     AbstractRuntimeService
 
-"""The RuntimeService interface is responsible for
-coordinating the execution of a group of process models belonging to a common
-synchronization domain. The domain will follow a SyncProtocol or will be
-asynchronous. The processes and their corresponding process models are
-selected by the Runtime dependent on the RunConfiguration assigned at the
-start of execution. For each group of processes which follow the same
-protocol and execute on the same node, the Runtime creates a RuntimeService.
-Each RuntimeService coordinates all actions and commands from the Runtime,
- transmitting them to the the processes under it's managment and
-returning action and command responses back to Runtime.
-
-RuntimeService Types:
-
-PyRuntimeService: (Abstract Class) Coordinates process models executing on
-   the CPU and written in Python.
-   Concrete Implementations:
-    a. LoihiPyRuntimeService: Coordinates process models executing on
-       the CPU and written in Python and following the LoihiProtocol.
-    b. AsyncPyRuntimeService: Coordinates process models executing on
-       the CPU and written in Python and following the AsyncProtocol.
-"""
-
 
 class PyRuntimeService(AbstractRuntimeService):
     """Abstract RuntimeService for Python, it provides base methods
     for start and run. It is not meant to instantiated directly
     but used by inheritance
     """
 
@@ -74,15 +74,14 @@
         self.run()
 
     @abstractmethod
     def run(self):
         """Override this method to implement the runtime service. The run
         method is invoked upon start which called when the execution is
         started by the runtime."""
-        pass
 
     def join(self):
         """Stop the necessary channels to coordinate with runtime and group
         of processes this RuntimeService is managing"""
         self.runtime_to_service.join()
         self.service_to_runtime.join()
 
@@ -94,30 +93,30 @@
         """Relays data received from ProcessModel given by model id  to the
         runtime"""
         process_idx = self.model_ids.index(model_id)
         data_recv_port = self.process_to_service[process_idx]
         data_relay_port = self.service_to_runtime
         num_items = data_recv_port.recv()
         data_relay_port.send(num_items)
-        for i in range(int(num_items[0])):
+        for _ in range(int(num_items[0])):
             value = data_recv_port.recv()
             data_relay_port.send(value)
 
     def _relay_to_pm_data_given_model_id(self, model_id: int) -> MGMT_RESPONSE:
         """Relays data received from the runtime to the ProcessModel given by
         the model id."""
         process_idx = self.model_ids.index(model_id)
         data_recv_port = self.runtime_to_service
         data_relay_port = self.service_to_process[process_idx]
         resp_port = self.process_to_service[process_idx]
         # Receive and relay number of items
         num_items = data_recv_port.recv()
         data_relay_port.send(num_items)
         # Receive and relay data1, data2, ...
-        for i in range(int(num_items[0].item())):
+        for _ in range(int(num_items[0].item())):
             data_relay_port.send(data_recv_port.recv())
         rsp = resp_port.recv()
         return rsp
 
     def _send_pm_req_given_model_id(self, model_id: int, *requests):
         """Sends requests to a ProcessModel given by the model id."""
         process_idx = self.model_ids.index(model_id)
```

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/LICENSE` & `lava_nc-0.8.0/src/lava/proc/LICENSE`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/conv/models.py` & `lava_nc-0.8.0/src/lava/proc/conv/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/conv/process.py` & `lava_nc-0.8.0/src/lava/proc/conv/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/conv/utils.py` & `lava_nc-0.8.0/src/lava/proc/conv/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,26 +153,26 @@
             f'Found output y dimension (={y_out}) to be less than 1.'
             f'Check your convolution sizes.'
         )
 
     return x_out, y_out, out_channels
 
 
-def conv(input: np.ndarray,
+def conv(input_: np.ndarray,
          weight: np.ndarray,
          kernel_size: Tuple[int, int],
          stride: Tuple[int, int],
          padding: Tuple[int, int],
          dilation: Tuple[int, int],
          groups: int) -> np.ndarray:
     """Convolution implementation
 
     Parameters
     ----------
-    input : 3 dimensional np array
+    input_ : 3 dimensional np array
         convolution input.
     weight : 4 dimensional np array
         convolution kernel weight.
     kernel_size : 2 element tuple, list, or array
         convolution kernel size in XY/WH format.
     stride : 2 element tuple, list, or array
         convolution stride in XY/WH format.
@@ -188,49 +188,49 @@
     3 dimensional np array
         convolution output
     """
     if TORCH_IS_AVAILABLE:
         # with torch.no_grad():  # this seems to cause problems
         output = F.conv2d(
             torch.unsqueeze(  # torch expects a batch dimension NCHW
-                torch.FloatTensor(input.transpose([2, 1, 0])),
+                torch.FloatTensor(input_.transpose([2, 1, 0])),
                 dim=0,
             ),
             torch.FloatTensor(
                 # torch actually does correlation
                 # so flipping the spatial dimension of weight
                 # copy() is needed because
                 # torch cannot handle negative stride
                 weight[:, ::-1, ::-1].transpose([0, 3, 2, 1]).copy()
             ),
-            stride=stride[::-1].tolist(),
-            padding=padding[::-1].tolist(),
-            dilation=dilation[::-1].tolist(),
+            stride=list(stride[::-1]),
+            padding=list(padding[::-1]),
+            dilation=list(dilation[::-1]),
             groups=groups
         )[0].cpu().data.numpy().transpose([2, 1, 0])
     else:
         output = conv_scipy(
-            input, weight, kernel_size, stride, padding, dilation, groups
+            input_, weight, kernel_size, stride, padding, dilation, groups
         )
 
     return output.astype(weight.dtype)
 
 
-def conv_scipy(input: np.ndarray,
+def conv_scipy(input_: np.ndarray,
                weight: np.ndarray,
                kernel_size: Tuple[int, int],
                stride: Tuple[int, int],
                padding: Tuple[int, int],
                dilation: Tuple[int, int],
                groups: int) -> np.ndarray:
     """Scipy based implementation of convolution
 
     Parameters
     ----------
-    input : 3 dimensional np array
+    input_ : 3 dimensional np array
         convolution input.
     weight : 4 dimensional np array
         convolution kernel weight.
     kernel_size : 2 element tuple, list, or array
         convolution kernel size in XY/WH format.
     stride : 2 element tuple, list, or array
         convolution stride in XY/WH format.
@@ -242,15 +242,15 @@
         number of convolution groups.
 
     Returns
     -------
     3 dimensional np array
         convolution output
     """
-    input_shape = input.shape
+    input_shape = input_.shape
     output = np.zeros(
         output_shape(
             input_shape, weight.shape[0],
             kernel_size, stride, padding, dilation
         )
     )
 
@@ -259,32 +259,32 @@
         dilation[0] * (kernel_size[0] - 1) + 1,
         dilation[1] * (kernel_size[1] - 1) + 1,
         weight.shape[-1]
     ])
     dilated_weight[:, ::dilation[0], ::dilation[1], :] = weight
 
     input_padded = np.pad(
-        input,
+        input_,
         ((padding[0], padding[0]), (padding[1], padding[1]), (0, 0)),
         mode='constant',
     )
 
-    if input.shape[-1] % groups != 0:
+    if input_.shape[-1] % groups != 0:
         raise Exception(
             f'Expected number of in_channels to be divisible by group.'
             f'Found {weight.shape[3] = } and {groups = }.'
         )
     if output.shape[-1] % groups != 0:
         raise Exception(
             f'Expected number of out_channels to be divisible by group.'
             f'Found {weight.shape[0] = } and {groups = }.'
         )
 
     k_grp = output.shape[2] // groups
-    c_grp = input.shape[2] // groups
+    c_grp = input_.shape[2] // groups
     for g in range(groups):
         for k in range(k_grp):
             for c in range(c_grp):
                 temp = signal.convolve2d(
                     input_padded[:, :, c + g * c_grp],
                     dilated_weight[k + g * k_grp, :, :, c],
                     mode='valid'
```

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/dense/models.py` & `lava_nc-0.8.0/src/lava/proc/dense/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,17 +68,18 @@
     weights: np.ndarray = LavaPyType(np.ndarray, np.int32, precision=8)
     num_message_bits: np.ndarray = LavaPyType(np.ndarray, int, precision=5)
 
     def __init__(self, proc_params):
         super().__init__(proc_params)
         # Flag to determine whether weights have already been scaled.
         self.weights_set = False
+        self.weight_exp: int = self.proc_params.get("weight_exp", 0)
 
     def run_spk(self):
-        self.weight_exp: int = self.proc_params.get("weight_exp", 0)
+        self.weight_exp = self.proc_params.get("weight_exp", 0)
 
         # Since this Process has no learning, weights are assumed to be static
         # and only require scaling on the first timestep of run_spk().
         if not self.weights_set:
             num_weight_bits: int = self.proc_params.get("num_weight_bits", 8)
             sign_mode: SignMode = self.proc_params.get("sign_mode") \
                 or determine_sign_mode(self.weights)
@@ -143,17 +144,17 @@
 
 
 @implements(proc=LearningDense, protocol=LoihiProtocol)
 @requires(CPU)
 @tag("bit_approximate_loihi", "fixed_pt")
 class PyLearningDenseModelBitApproximate(
         LearningConnectionModelBitApproximate, AbstractPyDenseModelBitAcc):
-    """Implementation of Conn Process with Dense synaptic connections that is
-    bit-accurate with Loihi's hardware implementation of Dense, which means,
-    it mimics Loihi behaviour bit-by-bit.
+    """Implementation of Conn Process with Dense synaptic connections that
+    uses similar constraints as Loihi's hardware implementation of dense
+    connectivity but does not reproduce Loihi bit-by-bit.
     """
 
     def __init__(self, proc_params):
         super().__init__(proc_params)
         # Flag to determine whether weights have already been scaled.
         self.num_weight_bits: int = self.proc_params.get("num_weight_bits", 8)
 
@@ -190,47 +191,57 @@
         self.recv_traces(s_in)
 
 
 class AbstractPyDelayDenseModel(PyLoihiProcessModel):
     """Abstract Conn Process with Dense synaptic connections which incorporates
     delays into the Conn Process.
     """
+    weights: np.ndarray = None
+    delays: np.ndarray = None
+    a_buff: np.ndarray = None
+
+    def calc_act(self, s_in) -> np.ndarray:
+        """
+        Calculate the activation matrix based on s_in by performing
+        delay_wgts * s_in.
+        """
+        # First calculating the activations through delay_wgts * s_in
+        # This matrix is then summed across each row to get the
+        # activations to the output neurons for different delays.
+        # This activation vector is reshaped to a matrix of the form
+        # (n_flat_output_neurons * (max_delay + 1), n_flat_output_neurons)
+        #  which is then transposed to get the activation matrix.
+        return np.reshape(
+            np.sum(self.get_delay_wgts_mat(self.weights,
+                                           self.delays) * s_in, axis=1),
+            (np.max(self.delays) + 1, self.weights.shape[0])).T
 
     @staticmethod
-    def get_del_wgts(weights, delays) -> np.ndarray:
+    def get_delay_wgts_mat(weights, delays) -> np.ndarray:
         """
-        Use self.weights and self.delays to create a matrix where the
-        weights are separated by delay. Returns 2D matrix of form
+        Create a matrix where the synaptic weights are separated
+        by their corresponding delays. The first matrix contains all the
+        weights, where the delay is equal to zero. The second matrix
+        contains all the weights, where the delay is equal to one and so on.
+        These matrices are then stacked together vertically.
+
+        Returns 2D matrix of form
         (num_flat_output_neurons * max_delay + 1, num_flat_input_neurons) where
-        del_wgts[
+        delay_wgts[
             k * num_flat_output_neurons : (k + 1) * num_flat_output_neurons, :
         ]
         contains the weights for all connections with a delay equal to k.
         This allows for the updating of the activation buffer and updating
         weights.
         """
         return np.vstack([
             np.where(delays == k, weights, 0)
             for k in range(np.max(delays) + 1)
         ])
 
-    def calc_act(self, s_in) -> np.ndarray:
-        """
-        Calculate the activations by performing del_wgts * s_in. This matrix
-        is then summed across each row to get the activations to the output
-        neurons for different delays. This activation vector is reshaped to a
-        matrix of the form
-        (n_flat_output_neurons * (max_delay + 1), n_flat_output_neurons)
-        which is then transposed to get the activation matrix.
-        """
-        return np.reshape(
-            np.sum(self.get_del_wgts(self.weights,
-                                     self.delays) * s_in, axis=1),
-            (np.max(self.delays) + 1, self.weights.shape[0])).T
-
     def update_act(self, s_in):
         """
         Updates the activations for the connection.
         Clears first column of a_buff and rolls them to the last column.
         Finally, calculates the activations for the current time step and adds
         them to a_buff.
         This order of operations ensures that delays of 0 correspond to
@@ -259,15 +270,15 @@
     weights: np.ndarray = LavaPyType(np.ndarray, float)
     # delays is a 2D matrix of form (num_flat_output_neurons,
     # num_flat_input_neurons) in C-order (row major).
     delays: np.ndarray = LavaPyType(np.ndarray, int)
     num_message_bits: np.ndarray = LavaPyType(np.ndarray, int, precision=5)
 
     def run_spk(self):
-        # The a_out sent on a each timestep is a buffered value from dendritic
+        # The a_out sent on each timestep is a buffered value from dendritic
         # accumulation at timestep t-1. This prevents deadlocking in
         # networks with recurrent connectivity structures.
         self.a_out.send(self.a_buff[:, 0])
         if self.num_message_bits.item() > 0:
             s_in = self.s_in.recv()
         else:
             s_in = self.s_in.recv().astype(bool)
```

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/dense/process.py` & `lava_nc-0.8.0/src/lava/proc/dense/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,25 +228,26 @@
             weights = weights * (2 ** w_scale)
 
         num_message_bits : int, optional
             Determines whether the Dense Process deals with the incoming
             spikes as binary spikes (num_message_bits = 0) or as graded
             spikes (num_message_bits > 0). Default is 0.
         """
+        if max_delay == 0:
+            max_delay = int(np.max(delays))
 
         super().__init__(weights=weights,
                          num_message_bits=num_message_bits,
                          name=name,
                          log_config=log_config,
+                         max_delay=max_delay,
                          **kwargs)
 
         self._validate_delays(weights, delays)
         shape = weights.shape
-        if max_delay == 0:
-            max_delay = int(np.max(delays))
 
         # Variables
         self.delays = Var(shape=shape, init=delays)
         self.a_buff = Var(shape=(shape[0], max_delay + 1) , init=0)
 
     @staticmethod
     def _validate_delays(weights: np.ndarray, delays: np.ndarray) -> None:
```

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/io/dataloader.py` & `lava_nc-0.8.0/src/lava/proc/io/dataloader.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/io/encoder.py` & `lava_nc-0.8.0/src/lava/proc/io/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from lava.magma.core.process.variable import Var
 from lava.magma.core.sync.protocols.loihi_protocol import LoihiProtocol
 from lava.magma.core.model.py.ports import PyInPort, PyOutPort
 from lava.magma.core.model.py.type import LavaPyType
 from lava.magma.core.resources import HostCPU
 from lava.magma.core.decorator import implements, requires, tag
 from lava.magma.core.model.py.model import PyLoihiProcessModel
-from lava.proc.sdn.models import AbstractDeltaModel
 
 
 @unique
 class Compression(Enum):
     """Enumeration of message compression mode.
 
     Attributes
```

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/io/reset.py` & `lava_nc-0.8.0/src/lava/proc/io/reset.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/io/sink.py` & `lava_nc-0.8.0/src/lava/proc/io/sink.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/io/source.py` & `lava_nc-0.8.0/src/lava/proc/io/source.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/learning_rules/r_stdp_learning_rule.py` & `lava_nc-0.8.0/src/lava/proc/learning_rules/r_stdp_learning_rule.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/learning_rules/stdp_learning_rule.py` & `lava_nc-0.8.0/src/lava/proc/learning_rules/stdp_learning_rule.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/lif/models.py` & `lava_nc-0.8.0/src/lava/proc/lif/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Copyright (C) 2021-22 Intel Corporation
+# Copyright (C) 2021-23 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
+from lava.magma.core.model.py.neuron import (
+    LearningNeuronModelFloat,
+    LearningNeuronModelFixed,
+)
 import numpy as np
 from lava.magma.core.sync.protocols.loihi_protocol import LoihiProtocol
 from lava.magma.core.model.py.ports import PyInPort, PyOutPort
 from lava.magma.core.model.py.type import LavaPyType
 from lava.magma.core.resources import CPU
 from lava.magma.core.decorator import implements, requires, tag
 from lava.magma.core.model.py.model import PyLoihiProcessModel
-from lava.proc.lif.process import LIF, LIFReset, TernaryLIF, LearningLIF
-
-from lava.magma.core.model.py.neuron import (
-    LearningNeuronModelFloat,
-    LearningNeuronModelFixed,
-)
+from lava.proc.lif.process import (LIF, LIFReset, TernaryLIF, LearningLIF,
+                                   LIFRefractory)
 
 
 class AbstractPyLifModelFloat(PyLoihiProcessModel):
     """Abstract implementation of floating point precision
     leaky-integrate-and-fire neuron model.
 
     Specific implementations inherit from here.
@@ -445,14 +445,68 @@
         s_out = self.spiking_activation()
 
         # Reset voltage of spiked neurons to 0
         self.reset_voltage(spike_vector=s_out)
         self.s_out.send(s_out)
 
 
+@implements(proc=LIFRefractory, protocol=LoihiProtocol)
+@requires(CPU)
+@tag("floating_pt")
+class PyLifRefractoryModelFloat(AbstractPyLifModelFloat):
+    """Implementation of Leaky-Integrate-and-Fire neural process with
+    refractory period in floating point precision.
+    """
+
+    s_out: PyOutPort = LavaPyType(PyOutPort.VEC_DENSE, float)
+    vth: float = LavaPyType(float, float)
+    refractory_period_end: np.ndarray = LavaPyType(np.ndarray, int)
+
+    def __init__(self, proc_params):
+        super(PyLifRefractoryModelFloat, self).__init__(proc_params)
+        self.refractory_period = proc_params["refractory_period"]
+
+    def spiking_activation(self):
+        """Spiking activation function for LIF Refractory."""
+        return self.v > self.vth
+
+    def subthr_dynamics(self, activation_in: np.ndarray):
+        """Sub-threshold dynamics of current and voltage variables for
+        all refractory LIF models. This is where the 'leaky integration'
+        happens.
+        """
+        self.u[:] = self.u * (1 - self.du)
+        self.u[:] += activation_in
+        non_refractory = self.refractory_period_end < self.time_step
+        self.v[non_refractory] = (self.v[non_refractory] * (
+            (1 - self.dv) + self.u[non_refractory])
+            + self.bias_mant[non_refractory])
+
+    def process_spikes(self, spike_vector: np.ndarray):
+        self.refractory_period_end[spike_vector] = (self.time_step
+                                                    + self.refractory_period)
+        super().reset_voltage(spike_vector)
+
+    def run_spk(self):
+        """The run function that performs the actual computation during
+        execution orchestrated by a PyLoihiProcessModel using the
+        LoihiProtocol.
+        """
+        # Receive synaptic input
+        a_in_data = self.a_in.recv()
+
+        self.subthr_dynamics(activation_in=a_in_data)
+
+        s_out = self.spiking_activation()
+
+        # Reset voltage of spiked neurons to 0
+        self.process_spikes(spike_vector=s_out)
+        self.s_out.send(s_out)
+
+
 @implements(proc=LearningLIF, protocol=LoihiProtocol)
 @requires(CPU)
 @tag("bit_accurate_loihi", "fixed_pt")
 class PyLearningLIFModelFixed(
     LearningNeuronModelFixed, AbstractPyLifModelFixed
 ):
     """Implementation of Leaky-Integrate-and-Fire neural
```

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/lif/process.py` & `lava_nc-0.8.0/src/lava/proc/lif/process.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-23 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import numpy as np
 import typing as ty
 
-from lava.magma.core.learning.learning_rule import (
-    LoihiLearningRule,
-    Loihi2FLearningRule,
-)
+from lava.magma.core.learning.learning_rule import Loihi2FLearningRule
 from lava.magma.core.process.process import LogConfig, AbstractProcess
 from lava.magma.core.process.variable import Var
 from lava.magma.core.process.ports.ports import InPort, OutPort
 from lava.magma.core.process.neuron import LearningNeuronProcess
 
 
 class AbstractLIF(AbstractProcess):
@@ -343,7 +340,79 @@
         if reset_interval < 1:
             raise ValueError("Reset interval must be > 0.")
         if reset_offset < 0:
             raise ValueError("Reset offset must be positive.")
 
         self.proc_params["reset_interval"] = reset_interval
         self.proc_params["reset_offset"] = reset_offset
+
+
+class LIFRefractory(LIF):
+
+    """Leaky-Integrate-and-Fire (LIF) process with refractory period.
+
+    Parameters
+    ----------
+    shape : tuple(int)
+        Number and topology of LIF neurons.
+    u : float, list, numpy.ndarray, optional
+        Initial value of the neurons' current.
+    v : float, list, numpy.ndarray, optional
+        Initial value of the neurons' voltage (membrane potential).
+    du : float, optional
+        Inverse of decay time-constant for current decay. Currently, only a
+        single decay can be set for the entire population of neurons.
+    dv : float, optional
+        Inverse of decay time-constant for voltage decay. Currently, only a
+        single decay can be set for the entire population of neurons.
+    bias_mant : float, list, numpy.ndarray, optional
+        Mantissa part of neuron bias.
+    bias_exp : float, list, numpy.ndarray, optional
+        Exponent part of neuron bias, if needed. Mostly for fixed point
+        implementations. Ignored for floating point implementations.
+    vth : float, optional
+        Neuron threshold voltage, exceeding which, the neuron will spike.
+        Currently, only a single threshold can be set for the entire
+        population of neurons.
+    refractory_period : int, optional
+        The interval of the refractory period. 1 timestep by default.
+
+
+    See Also
+    --------
+    lava.proc.lif.process.LIF: 'Regular' leaky-integrate-and-fire neuron for
+    documentation on rest of the behavior.
+    """
+
+    def __init__(
+        self,
+        *,
+        shape: ty.Tuple[int, ...],
+        u: ty.Optional[ty.Union[float, list, np.ndarray]] = 0,
+        v: ty.Optional[ty.Union[float, list, np.ndarray]] = 0,
+        du: ty.Optional[float] = 0,
+        dv: ty.Optional[float] = 0,
+        bias_mant: ty.Optional[ty.Union[float, list, np.ndarray]] = 0,
+        bias_exp: ty.Optional[ty.Union[float, list, np.ndarray]] = 0,
+        vth: ty.Optional[float] = 10,
+        refractory_period: ty.Optional[int] = 1,
+        name: ty.Optional[str] = None,
+        log_config: ty.Optional[LogConfig] = None,
+    ) -> None:
+        super().__init__(
+            shape=shape,
+            u=u,
+            v=v,
+            du=du,
+            dv=dv,
+            bias_mant=bias_mant,
+            bias_exp=bias_exp,
+            vth=vth,
+            name=name,
+            log_config=log_config,
+        )
+
+        if refractory_period < 1:
+            raise ValueError("Refractory period must be > 0.")
+
+        self.proc_params["refractory_period"] = refractory_period
+        self.refractory_period_end = Var(shape=shape, init=0)
```

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/monitor/models.py` & `lava_nc-0.8.0/src/lava/proc/monitor/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/monitor/process.py` & `lava_nc-0.8.0/src/lava/proc/monitor/process.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (C) 2021-22 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
-import matplotlib.pyplot as plt
 from lava.magma.core.process.process import AbstractProcess
 from lava.magma.core.process.variable import Var
 from lava.magma.core.process.ports.ports import InPort, OutPort, RefPort
 
 
 class Monitor(AbstractProcess):
     """
@@ -127,31 +126,27 @@
             a Var or OutPort of some process to be monitored.
         num_steps: int
             The number of steps the target Var/OutPort should be monitored.
         """
         # Create names for Ports/Vars to be created in Monitor process for
         # probing purposes. Names are given incrementally each time probe(..)
         # method is called.
-        self.new_ref_port_name = "ref_port_" + \
-                                 str(self.proc_params["n_ref_ports"])
-        self.new_var_read_name = "var_read_" + \
-                                 str(self.proc_params["n_ref_ports"])
-        self.new_in_port_name = "in_port_" + \
-                                str(self.proc_params["n_in_ports"])
-        self.new_out_read_name = "out_read_" + \
-                                 str(self.proc_params["n_in_ports"])
+        new_ref_port_name = f"ref_port_{self.proc_params['n_ref_ports']}"
+        new_var_read_name = f"var_read_{self.proc_params['n_ref_ports']}"
+        new_in_port_name = f"in_port_{self.proc_params['n_in_ports']}"
+        new_out_read_name = f"out_read_{self.proc_params['n_in_ports']}"
 
         # Create and set new Refport and corresponding Var to store data
-        setattr(self, self.new_ref_port_name, RefPort(shape=target.shape))
-        setattr(self, self.new_var_read_name,
+        setattr(self, new_ref_port_name, RefPort(shape=target.shape))
+        setattr(self, new_var_read_name,
                 Var(shape=(num_steps,) + target.shape, init=0))
 
         # Create and set new InPort and corresponding Var to store data
-        setattr(self, self.new_in_port_name, InPort(shape=target.shape))
-        setattr(self, self.new_out_read_name,
+        setattr(self, new_in_port_name, InPort(shape=target.shape))
+        setattr(self, new_out_read_name,
                 Var(shape=(num_steps,) + target.shape, init=0))
 
         # Add the names of new RefPort and Var_read name to proc_params dict
         self.proc_params["RefPorts"].append(self.new_ref_port_name)
         self.proc_params["VarsData1"].append(self.new_var_read_name)
 
         # Add the names of new RefPort and Var_read name to proc_params dict
@@ -175,32 +170,32 @@
         if isinstance(target, Var):
 
             # Update id for the next use of probe(..) method
             n_ref_ports = self.proc_params["n_ref_ports"]
             self.proc_params.overwrite("n_ref_ports", n_ref_ports + 1)
 
             # Connect newly created Refport to the var to be monitored
-            getattr(self, self.new_ref_port_name).connect_var(target)
+            getattr(self, new_ref_port_name).connect_var(target)
 
             # Add the name of probed Var and its process to the target_names
-            self.target_names[self.new_var_read_name] = [target.process.name,
-                                                         target.name]
+            self.target_names[new_var_read_name] = [target.process.name,
+                                                    target.name]
         # If target to be monitored is an OutPort
         elif isinstance(target, OutPort):
 
             # Update id for the next use of probe(..) method
             n_in_ports = self.proc_params["n_in_ports"]
             self.proc_params.overwrite("n_in_ports", n_in_ports + 1)
 
             # Connect newly created InPort from the OutPort to be monitored
-            getattr(self, self.new_in_port_name).connect_from(target)
+            getattr(self, new_in_port_name).connect_from(target)
 
             # Add the name of OutPort and its process to the target_names
-            self.target_names[self.new_out_read_name] = [target.process.name,
-                                                         target.name]
+            self.target_names[new_out_read_name] = [target.process.name,
+                                                    target.name]
 
         # If target is an InPort raise a Type error, as monitoring InPorts is
         # not supported yet
         else:
             raise TypeError("Non-supported probe target: type {}"
                             .format(target))
```

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/receiver/models.py` & `lava_nc-0.8.0/src/lava/proc/receiver/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/receiver/process.py` & `lava_nc-0.8.0/src/lava/proc/receiver/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/rf/models.py` & `lava_nc-0.8.0/src/lava/proc/rf/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/rf/process.py` & `lava_nc-0.8.0/src/lava/proc/rf/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/rf_iz/models.py` & `lava_nc-0.8.0/src/lava/proc/rf_iz/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/sdn/models.py` & `lava_nc-0.8.0/src/lava/proc/sdn/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/sdn/process.py` & `lava_nc-0.8.0/src/lava/proc/sdn/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/spiker/models.py` & `lava_nc-0.8.0/src/lava/proc/spiker/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import numpy as np
 from lava.magma.core.decorator import implements, requires
 from lava.magma.core.model.py.model import PyLoihiProcessModel
-from lava.magma.core.model.py.ports import PyInPort, PyOutPort
+from lava.magma.core.model.py.ports import PyOutPort
 from lava.magma.core.model.py.type import LavaPyType
 from lava.magma.core.resources import CPU
 from lava.magma.core.sync.protocols.loihi_protocol import LoihiProtocol
 
 from lava.proc.spiker.process import Spiker
```

### Comparing `lava_nc-0.7.0.post2/src/lava/proc/spiker/process.py` & `lava_nc-0.8.0/src/lava/proc/spiker/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/utils/LICENSE` & `lava_nc-0.8.0/src/lava/utils/LICENSE`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/utils/dataloader/mnist.py` & `lava_nc-0.8.0/src/lava/utils/dataloader/mnist.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,16 @@
                         # Disabling security lint because we are using hardcoded
                         # URLs specified above
                         res = urllib.request.urlopen(url)  # nosec # noqa
                         with open(os.path.join(path, file), "wb") as f:
                             f.write(res.read())
                         break
                     else:
-                        raise "Url does not start with http"
+                        raise ValueError(f"Specified URL ({url}) does not "
+                                         "start with 'http'.")
                 except urllib.error.URLError as exception:
                     err = exception
                     continue
             else:
                 print("Failed to download mnist dataset")
                 raise err
```

### Comparing `lava_nc-0.7.0.post2/src/lava/utils/plots.py` & `lava_nc-0.8.0/src/lava/utils/plots.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/utils/profiler.py` & `lava_nc-0.8.0/src/lava/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/src/lava/utils/weightutils.py` & `lava_nc-0.8.0/src/lava/utils/weightutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import numpy as np
+from scipy.sparse import spmatrix
 import typing as ty
 from enum import Enum, unique
 from dataclasses import dataclass
 
 
 @unique
 class SignMode(Enum):
@@ -40,28 +41,28 @@
         sign_mode = SignMode.MIXED
 
     return sign_mode
 
 
 @dataclass
 class OptimizedWeights:
-    weights: np.ndarray
+    weights: ty.Union[np.ndarray, spmatrix]
     num_weight_bits: int
     weight_exp: int
 
 
 def optimize_weight_bits(
-        weights: np.ndarray,
+        weights: ty.Union[np.ndarray, spmatrix],
         sign_mode: SignMode,
         loihi2: ty.Optional[bool] = False) -> OptimizedWeights:
     """Optimizes the weight matrix to best fit in Loihi's synapse.
 
     Parameters
     ----------
-    weights : np.ndarray
+    weights : np.ndarray, spmatrix
         Standard 8-bit signed weight matrix.
     sign_mode : SignMode
         Determines whether the weights are purely excitatory, inhibitory,
         or mixed sign.
     loihi2 : bool, optional
         Flag to optimize for Loihi 2. By default False.
 
@@ -71,51 +72,54 @@
         An object that wraps the optimized weight matrix and weight parameters.
     """
     _validate_weights(weights, sign_mode)
 
     weight_exp = _determine_weight_exp(weights, sign_mode)
     num_weight_bits = _determine_num_weight_bits(weights, weight_exp, sign_mode)
 
-    weights = np.left_shift(weights.astype(np.int32), int(-weight_exp))
+    if isinstance(weights, np.ndarray):
+        weights = weights.astype(np.int32) << int(-weight_exp)
+    elif isinstance(weights, spmatrix):
+        weights.data = weights.data.astype(np.int32) << int(-weight_exp)
 
     if loihi2:
-        weights = weights // (1 << (8 - num_weight_bits))
+        weights = (weights / (1 << (8 - num_weight_bits))).astype(np.int32)
         if sign_mode == SignMode.MIXED:
-            weights = weights // 2
+            weights = (weights / 2).astype(np.int32)
 
-    optimized_weights = OptimizedWeights(weights=weights.astype(int),
+    optimized_weights = OptimizedWeights(weights=weights,
                                          num_weight_bits=num_weight_bits,
                                          weight_exp=weight_exp)
     return optimized_weights
 
 
-def _validate_weights(weights: np.ndarray,
+def _validate_weights(weights: ty.Union[np.ndarray, spmatrix],
                       sign_mode: SignMode) -> None:
     """Validate the weight values against the given sign mode.
 
     Parameters
     ----------
-    weights : numpy.ndarray
+    weights : numpy.ndarray, spmatrix
         Weight matrix
     sign_mode : SignMode
         Sign mode specified for the weight matrix
     """
     mixed_flag = int(sign_mode == SignMode.MIXED)
     excitatory_flag = int(sign_mode == SignMode.EXCITATORY)
     inhibitory_flag = int(sign_mode == SignMode.INHIBITORY)
 
     min_weight = (-2 ** 8) * (mixed_flag + inhibitory_flag)
     min_weight += inhibitory_flag
     max_weight = (2 ** 8 - 1) * (mixed_flag + excitatory_flag)
 
-    if np.any(weights > max_weight) or np.any(weights < min_weight):
+    if weights.max() > max_weight or weights.min() < min_weight:
         raise ValueError(f"weights have to be between {min_weight} and "
                          f"{max_weight} for {sign_mode=}. Got "
-                         f"weights between {np.min(weights)} and "
-                         f"{np.max(weights)}.")
+                         f"weights between {weights.min()} and "
+                         f"{weights.max()}.")
 
 
 def _determine_weight_exp(weights: np.ndarray,
                           sign_mode: SignMode) -> int:
     """Determines the weight exponent to be used to optimally represent the
     given weight values and sign mode on Loihi.
 
@@ -193,24 +197,25 @@
         n -= 1
 
     num_weight_bits = 8 + weight_exp - n
 
     return num_weight_bits
 
 
-def truncate_weights(weights: np.ndarray,
+def truncate_weights(weights: ty.Union[np.ndarray, spmatrix],
                      sign_mode: SignMode,
                      num_weight_bits: int,
-                     max_num_weight_bits: ty.Optional[int] = 8) -> np.ndarray:
+                     max_num_weight_bits: ty.Optional[int] = 8
+                     ) -> ty.Union[np.ndarray, spmatrix]:
     """Truncate the least significant bits of the weight matrix given the
     sign mode and number of weight bits.
 
     Parameters
     ----------
-    weights : numpy.ndarray
+    weights : numpy.ndarray, spmatrix
         Weight matrix that is to be truncated.
     sign_mode : SignMode
         Sign mode to use for truncation. See SignMode class for the
         correct values.
     num_weight_bits : int
         Number of bits to use for the weight matrix.
     max_num_weight_bits : int, optional
@@ -218,62 +223,68 @@
         is 8.
 
     Returns
     -------
     numpy.ndarray
         Truncated weight matrix.
     """
-    weights = np.copy(weights).astype(np.int32)
+    weights = weights.copy().astype(np.int32)
 
     if sign_mode == SignMode.INHIBITORY:
         weights = -weights
 
     mixed_flag = int(sign_mode == SignMode.MIXED)
     num_truncate_bits = max_num_weight_bits - num_weight_bits + mixed_flag
 
-    truncated_weights = np.left_shift(
-        np.right_shift(weights, num_truncate_bits),
-        num_truncate_bits).astype(np.int32)
+    if isinstance(weights, np.ndarray):
+        weights = (weights >> num_truncate_bits) << num_truncate_bits
+    elif isinstance(weights, spmatrix):
+        weights.data = (weights.data >> num_truncate_bits) << num_truncate_bits
+        weights.eliminate_zeros()
 
     if sign_mode == SignMode.INHIBITORY:
-        truncated_weights = -truncated_weights
+        weights = -weights
 
-    return truncated_weights
+    return weights
 
 
-def clip_weights(weights: np.ndarray,
+def clip_weights(weights: ty.Union[np.ndarray, spmatrix],
                  sign_mode: SignMode,
-                 num_bits: int) -> np.ndarray:
+                 num_bits: int) -> ty.Union[np.ndarray, spmatrix]:
     """Truncate the least significant bits of the weight matrix given the
     sign mode and number of weight bits.
 
     Parameters
     ----------
-    weights : numpy.ndarray
+    weights : numpy.ndarray, spmatrix
         Weight matrix that is to be truncated.
     sign_mode : SignMode
         Sign mode to use for truncation.
     num_bits : int
         Number of bits to use to clip the weights to.
 
     Returns
     -------
     numpy.ndarray
         Truncated weight matrix.
     """
-    weights = np.copy(weights).astype(np.int32)
+    weights = weights.copy().astype(np.int32)
 
     mixed_flag = int(sign_mode == SignMode.MIXED)
     inhibitory_flag = int(sign_mode == SignMode.INHIBITORY)
 
     if inhibitory_flag:
         weights = -weights
 
     min_wgt = (-2 ** num_bits) * mixed_flag
     max_wgt = 2 ** num_bits - 1
 
-    clipped_weights = np.clip(weights, min_wgt, max_wgt)
+    if isinstance(weights, np.ndarray):
+        weights = np.clip(weights, min_wgt, max_wgt)
+    elif isinstance(weights, spmatrix):
+        weights[weights > max_wgt] = max_wgt
+        weights[weights < min_wgt] = min_wgt
 
     if inhibitory_flag:
-        clipped_weights = -clipped_weights
+        weights = -weights
 
-    return clipped_weights
+    return weights
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/compiler/builders/test_builder.py` & `lava_nc-0.8.0/tests/lava/magma/compiler/builders/test_builder.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/compiler/channels/test_pypychannel.py` & `lava_nc-0.8.0/tests/lava/magma/compiler/channels/test_pypychannel.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/compiler/subcompilers/py/test_pyproc_compiler.py` & `lava_nc-0.8.0/tests/lava/magma/compiler/subcompilers/py/test_pyproc_compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         self.out = OutPort(shape=(1,))
         self.some_var = Var((10,), init=10)
         self.var_port = VarPort(self.some_var)
 
 
 class MockRuntimeService:
     __name__ = "MockRuntimeService"
-    pass
 
 
 # Define minimal Protocol to be implemented.
 class ProtocolA(AbstractSyncProtocol):
     @property
     def runtime_service(self):
         return {CPU: MockRuntimeService()}
@@ -120,15 +119,15 @@
             proc_group=proc_group, compile_config=self.compile_config
         )
         py_proc_compiler.compile(channel_map)
         builders, channel_map = py_proc_compiler.get_builders(channel_map)
 
         # There should be three PyProcessBuilders...
         self.assertEqual(len(builders), 3)
-        for proc, builder in builders.items():
+        for builder in builders.values():
             self.assertIsInstance(builder, PyProcessBuilder)
         # ... one for each Process.
         b1 = ty.cast(PyProcessBuilder, builders[p1])
         b2 = ty.cast(PyProcessBuilder, builders[p2])
         b3 = ty.cast(PyProcessBuilder, builders[p3])
 
         # ProcA builders only have PortInitializers for 'inp' and 'out'...
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/compiler/subcompilers/test_channel_builders_factory.py` & `lava_nc-0.8.0/tests/lava/magma/compiler/subcompilers/test_channel_builders_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 # Copyright (C) 2021-22 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
-from enum import Enum
 import logging
 import typing as ty
 import unittest
 from unittest.mock import Mock
 
-import numpy as np
 from lava.magma.compiler.builders.channel_builder import ChannelBuilderMp
 from lava.magma.compiler.channel_map import ChannelMap, Payload, PortPair
 from lava.magma.compiler.channels.interfaces import ChannelType
 from lava.magma.compiler.compiler_graphs import ProcGroupDiGraphs
 from lava.magma.compiler.subcompilers.channel_builders_factory import \
     ChannelBuildersFactory
 from lava.magma.compiler.utils import LoihiPortInitializer, PortInitializer
-from lava.magma.compiler.var_model import LoihiAddress, LoihiVarModel
 from lava.magma.core.decorator import implements, requires
-from lava.magma.core.model.model import AbstractProcessModel
 from lava.magma.core.model.interfaces import AbstractPortImplementation
 from lava.magma.core.model.py.model import AbstractPyProcessModel
 from lava.magma.core.model.py.ports import (PyInPort, PyOutPort, PyRefPort,
                                             PyVarPort)
 from lava.magma.core.model.py.type import LavaPyType
 from lava.magma.core.model.sub.model import AbstractSubProcessModel
 from lava.magma.core.process.ports.ports import (AbstractPort, InPort, OutPort,
                                                  RefPort, VarPort)
 from lava.magma.core.process.ports.reduce_ops import ReduceSum
 from lava.magma.core.process.process import AbstractProcess
 from lava.magma.core.process.variable import Var
-from lava.magma.core.resources import CPU, LMT, NeuroCore
+from lava.magma.core.resources import CPU
 from lava.magma.core.run_configs import RunConfig
 from lava.magma.core.sync.protocol import AbstractSyncProtocol
 
 
 # A minimal process (A) with an InPort, OutPort and RefPort
 class ProcA(AbstractProcess):
     def __init__(self, **kwargs):
@@ -63,15 +59,14 @@
         # Use ReduceOp to allow for multiple input connections
         self.inp = InPort(shape=(1,), reduce_op=ReduceSum)
         self.out = OutPort(shape=(1,))
 
 
 class MockRuntimeService:
     __name__ = "MockRuntimeService"
-    pass
 
 
 # Define minimal Protocol to be implemented
 class ProtocolA(AbstractSyncProtocol):
     @property
     def runtime_service(self):
         return {CPU: MockRuntimeService()}
@@ -149,23 +144,22 @@
         )
         self.select_sub_proc_model = select_sub_proc_model
         self.select_lmt = select_lmt
 
     def select(self, proc, proc_models):
         py_proc_model = None
         sub_proc_model = None
-        c_proc_model = None
+
         # Find PyProcModel or SubProcModel
         for pm in proc_models:
             if issubclass(pm, AbstractSubProcessModel):
                 sub_proc_model = pm
             if issubclass(pm, AbstractPyProcessModel):
                 py_proc_model = pm
         # Make selection
-
         if self.select_sub_proc_model and sub_proc_model:
             return sub_proc_model
         if py_proc_model and not self.select_lmt:
             return py_proc_model
         else:
             raise AssertionError("No legal ProcessModel found.")
 
@@ -353,17 +347,14 @@
 
         # Create channel builders
         channel_map = ChannelMap.from_proc_groups([proc_group])
         PortInitializerFactory.set_initializers_on_channel_map(channel_map)
         channel_builders = self.factory.from_channel_map(channel_map, self.cfg)
 
         # This should result in 5 channel builders (one for each arrow above)
-        from lava.magma.compiler.builders.channel_builder import \
-            ChannelBuilderMp
-
         self.assertEqual(len(channel_builders), 5)
         for cb in channel_builders:
             self.assertIsInstance(cb, ChannelBuilderMp)
 
         # Each channel builder should connect its source and destination
         # process and port
         # Let's check the first one in detail
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/compiler/subcompilers/test_channel_map_updater.py` & `lava_nc-0.8.0/tests/lava/magma/compiler/subcompilers/test_channel_map_updater.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/compiler/test_channel_builder.py` & `lava_nc-0.8.0/tests/lava/magma/compiler/test_channel_builder.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/compiler/test_channel_map.py` & `lava_nc-0.8.0/tests/lava/magma/compiler/test_channel_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         self.inp = InPort(shape=(1,), reduce_op=ReduceSum)
         self.out = OutPort(shape=(1,))
         self.ref = RefPort(shape=(10,))
 
 
 class MockRuntimeService:
     __name__ = "MockRuntimeService"
-    pass
 
 
 # Define minimal Protocol to be implemented
 class ProtocolA(AbstractSyncProtocol):
     @property
     def runtime_service(self):
         return {CPU: MockRuntimeService()}
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/compiler/test_compiler.py` & `lava_nc-0.8.0/tests/lava/magma/compiler/test_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         # Use ReduceOp to allow for multiple input connections
         self.inp = InPort(shape=(1,), reduce_op=ReduceSum)
         self.out = OutPort(shape=(1,))
 
 
 class MockRuntimeService:
     __name__ = "MockRuntimeService"
-    pass
 
 
 # Define minimal Protocol to be implemented
 class ProtocolA(AbstractSyncProtocol):
     @property
     def runtime_service(self):
         return {CPU: MockRuntimeService()}
@@ -432,17 +431,14 @@
 
     def test_extract_proc_builders(self) -> None:
         """Tests whether the Executable is populated with the correct Builder
         instances."""
         # Create some mock Processes.
         proc1 = Mock(spec_set=AbstractProcess)
         proc2 = Mock(spec_set=AbstractProcess)
-        proc3 = Mock(spec_set=AbstractProcess)
-        proc4 = Mock(spec_set=AbstractProcess)
-        proc5 = Mock(spec_set=AbstractProcess)
 
         # Create some Builders.
         py_builder1 = PyProcessBuilder(AbstractPyProcessModel, 0)
         py_builder2 = PyProcessBuilder(AbstractPyProcessModel, 0)
 
         # Create mock SubCompilers, covering each type (Py, C, Nc).
         # Each SubCompiler has a get_builders() method that returns a mapping
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/compiler/test_node.py` & `lava_nc-0.8.0/tests/lava/magma/compiler/test_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from lava.magma.core.resources import HeadNode, Loihi1System, Loihi2System
 from lava.magma.compiler.node import Node, NodeConfig
 
 
 class MockProcess(AbstractProcess):
     """A mock process"""
 
-    pass
-
 
 class TestNode(unittest.TestCase):
     def test_node_creation(self):
         """Tests Node creation"""
         node1: Node = Node(node_type=HeadNode, processes=[])
         self.assertEqual(node1.node_type, HeadNode)
         self.assertEqual(len(node1.processes), 0)
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/learning/test_learning_rule.py` & `lava_nc-0.8.0/tests/lava/magma/core/learning/test_learning_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,38 +3,23 @@
 # See: https://spdx.org/licenses/
 
 import unittest
 import numpy as np
 
 from lava.magma.core.learning.learning_rule import (
     LoihiLearningRule,
-    Loihi2FLearningRule,
-    Loihi3FLearningRule,
+    Loihi2FLearningRule
 )
 from lava.magma.core.learning.product_series import ProductSeries
 from lava.magma.core.run_conditions import RunSteps
 from lava.magma.core.run_configs import Loihi2SimCfg
-from lava.proc.lif.process import LIF, LearningLIF
+from lava.proc.lif.process import LIF
 from lava.proc.dense.process import LearningDense, Dense
 from lava.proc.monitor.process import Monitor
 from lava.proc.io.source import RingBuffer as SpikeIn
-from lava.magma.core.model.py.neuron import (
-    LearningNeuronModelFloat,
-    LearningNeuronModelFixed,
-)
-from lava.magma.core.sync.protocols.loihi_protocol import LoihiProtocol
-from lava.magma.core.model.py.ports import PyInPort, PyOutPort
-from lava.magma.core.model.py.type import LavaPyType
-from lava.magma.core.resources import CPU
-from lava.magma.core.decorator import implements, requires, tag
-from lava.proc.lif.models import (
-    AbstractPyLifModelFloat,
-    AbstractPyLifModelFixed,
-)
-from lava.proc.io.source import RingBuffer as SpikeIn
 
 
 def create_network(
     size,
     num_steps,
     t_spike,
     learning_rule,
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/learning/test_learning_rule_applier.py` & `lava_nc-0.8.0/tests/lava/magma/core/learning/test_learning_rule_applier.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/learning/test_product_series.py` & `lava_nc-0.8.0/tests/lava/magma/core/learning/test_product_series.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/learning/test_random.py` & `lava_nc-0.8.0/tests/lava/magma/core/learning/test_random.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright (C) 2021-22 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import unittest
-import numpy as np
 
 from lava.magma.core.learning.random import TraceRandom, ConnVarRandom
 
 
 class TestTraceRandom(unittest.TestCase):
     def test_init(self) -> None:
         """Tests creating a valid TraceRandom object."""
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/learning/test_symbolic_equation.py` & `lava_nc-0.8.0/tests/lava/magma/core/learning/test_symbolic_equation.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/learning/test_utils.py` & `lava_nc-0.8.0/tests/lava/magma/core/learning/test_utils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/model/py/test_model.py` & `lava_nc-0.8.0/tests/lava/magma/core/model/py/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from lava.magma.core.run_conditions import RunSteps
 from lava.magma.core.run_configs import Loihi2SimCfg
 from lava.magma.core.sync.protocols.async_protocol import AsyncProtocol
 from lava.magma.core.model.py.model import (
     PyLoihiProcessModel, PyLoihiModelToPyAsyncModel
 )
 
-from lava.proc import io
 from lava.proc.lif.process import LIF
 from lava.proc.sdn.process import SigmaDelta
 from lava.proc.dense.process import Dense
 
 from lava.proc.lif.models import PyLifModelFloat, PyLifModelBitAcc
 from lava.proc.sdn.models import PySigmaDeltaModelFixed
 from lava.proc.dense.models import PyDenseModelFloat
@@ -123,34 +122,34 @@
                         'state_exp': 6}
         output_params = {'shape': (out_size,),
                          'vth': 2,
                          'spike_exp': 6,
                          'state_exp': 6}
         dense_params = {'weights': weights, 'num_message_bits': 16}
 
-        input = SigmaDelta(**input_params)
+        input_ = SigmaDelta(**input_params)
         output = SigmaDelta(**output_params)
         dense = Dense(**dense_params)
-        input.s_out.connect(dense.s_in)
+        input_.s_out.connect(dense.s_in)
         dense.a_out.connect(output.a_in)
 
         run_cnd = RunSteps(num_steps=2)
         # simply run the pyproc model
         output.run(condition=run_cnd,
                    run_cfg=Loihi2SimCfg(select_tag='fixed_pt'))
         sigma_gt = output.sigma.get()
         output.stop()
 
         # Run the same network in async mode.
-        # Currently we don't allow the same process to run twice
+        # Currently, we don't allow the same process to run twice
         # Copy the model used for pyproc model
-        input = SigmaDelta(**input_params)
+        input_ = SigmaDelta(**input_params)
         output = SigmaDelta(**output_params)
         dense = Dense(**dense_params)
-        input.s_out.connect(dense.s_in)
+        input_.s_out.connect(dense.s_in)
         dense.a_out.connect(output.a_in)
 
         output.run(condition=run_cnd,
                    run_cfg=CustomRunConfig(select_tag='fixed_pt'))
         sigma = output.sigma.get()
         output.stop()
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/model/py/test_ports.py` & `lava_nc-0.8.0/tests/lava/magma/core/model/py/test_ports.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/model/test_decorators.py` & `lava_nc-0.8.0/tests/lava/magma/core/model/test_decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,29 +44,29 @@
         # Define minimal Protocol to be implemented
         class TestProtocol(AbstractSyncProtocol):
             pass
 
         # We must pass a class, not an instance or anything else
         with self.assertRaises(TypeError):
             @implements(proc=TestProc(), protocol=TestProtocol)  # type: ignore
-            class TestModel(AbstractProcessModel):  # type: ignore
+            class TestModel(AbstractProcessModel):  # pylint: disable=W0612
                 def run(self):
                     pass
 
         # Same for 'protocol'
         with self.assertRaises(TypeError):
             @implements(proc=TestProc, protocol=TestProtocol())  # type: ignore
-            class TestModel2(AbstractProcessModel):
+            class TestModel2(AbstractProcessModel):  # pylint: disable=W0612
                 def run(self):
                     pass
 
         # And we can only decorate a subclass of 'AbstractProcessModel'
         with self.assertRaises(AssertionError):
             @implements(proc=TestProc, protocol=TestProtocol)
-            class TestProcess2(AbstractProcess):
+            class TestProcess2(AbstractProcess):  # pylint: disable=W0612
                 pass
 
     def test_implements_subclassing(self):
         """Check that 'implements' can also only be called on sub classes."""
 
         # Define minimal Process to be implemented
         class TestProc(AbstractProcess):
@@ -121,15 +121,15 @@
             def run(self):
                 pass
 
         # Attempting to overwrite either of the 'proc' or 'protocol'
         # attributes must fail
         with self.assertRaises(AssertionError):
             @implements(protocol=TestProtocol2)
-            class SubTestModel(TestModel):
+            class SubTestModel(TestModel):  # pylint: disable=W0612
                 pass
 
     def test_requires(self):
         """Checks 'requires' decorator."""
 
         # Define minimal ProcModel that requires a single 'AbstractResource'
         @requires(CPU)
@@ -186,23 +186,23 @@
 
     def test_requires_failing(self):
         """Checks failing 'requires' usage."""
 
         # We must decorate a ProcessModel and nothing else:
         with self.assertRaises(AssertionError):
             @requires(CPU)
-            class Something(AbstractProcess):
+            class Something(AbstractProcess):  # pylint: disable=W0612
                 pass
 
         # We must decorate a ProcessModel with an 'AbstractResource' class
         # and nothing else
         with self.assertRaises(TypeError):
 
             @requires(CPU())  # type: ignore
-            class TestModel(AbstractProcessModel):
+            class TestModel(AbstractProcessModel):  # pylint: disable=W0612
                 def run(self):
                     pass
 
     def test_tags(self):
         """Checks 'tag' decorator"""
         # Define minimal ProcModel and tag it
         @tag('keyword1', 'keyword2')
@@ -237,26 +237,26 @@
 
     def test_tags_failing(self):
         """Checks if 'tag' decorator fails appropriately"""
 
         # Only decorating ProcessModels is allowed
         with self.assertRaises(AssertionError):
             @tag('some-tag')
-            class SomeClass(AbstractProcess):
+            class SomeClass(AbstractProcess):  # pylint: disable=W0612
                 pass
 
         # Tags should be just comma-separated keywords
         with self.assertRaises(AssertionError):
             @tag('keyword1', ['keyword2', 'keyword3'])
-            class TestModel2(AbstractProcessModel):
+            class TestModel2(AbstractProcessModel):  # pylint: disable=W0612
                 def run(self):
                     pass
 
         # Tags should be just comma-separated keywords
         with self.assertRaises(AssertionError):
             @tag('tag1', [['tag2'], 'tag4'])
-            class SomeOtherClass(AbstractProcess):
+            class SomeOtherClass(AbstractProcess):  # pylint: disable=W0612
                 pass
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/model/test_sub_model.py` & `lava_nc-0.8.0/tests/lava/magma/core/model/test_sub_model.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/process/ports/test_ports.py` & `lava_nc-0.8.0/tests/lava/magma/core/process/ports/test_ports.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,15 +286,16 @@
         # In this case, the VarPort inherits its name and parent process from
         # the Var it wraps
         self.assertEqual(vp.name, "_" + v.name + "_implicit_port")
         self.assertEqual(vp.process, v.process)
 
     def test_connect_RefPort_to_Var_process_conflict(self):
         """Checks connecting RefPort implicitly to Var, with registered
-        processes and conflicting names. -> AssertionError"""
+        processes and conflicting names. -> adding _k with k=1,2,3... to
+        the name."""
 
         # Create a mock parent process
         class VarProcess(AbstractProcess):
             # Attribute is named like our implicit VarPort after creation
             _existing_attr_implicit_port = None
 
         # Create a Var and RefPort...
@@ -303,17 +304,29 @@
 
         # ...register a process for the Var and name it so it conflicts with
         # the attribute of VarProcess (very unlikely to happen)
         v.process = VarProcess()
         v.name = "existing_attr"
 
         # ... and connect it directly via connect_var(..)
-        # The naming conflict should raise an AssertionError
-        with self.assertRaises(AssertionError):
-            rp.connect_var(v)
+        rp.connect_var(v)
+
+        # This has the same effect as connecting a RefPort explicitly via a
+        # VarPort to a Var...
+        self.assertEqual(rp.get_dst_vars(), [v])
+        # ... but still creates a VarPort implicitly
+        vp = rp.get_dst_ports()[0]
+        self.assertIsInstance(vp, VarPort)
+        # ... which wraps the original Var
+        self.assertEqual(vp.var, v)
+
+        # In this case, the VarPort inherits its name and parent process from
+        # the Var it wraps + _implicit_port + _k with k=1,2,3...
+        self.assertEqual(vp.name, "_" + v.name + "_implicit_port" + "_1")
+        self.assertEqual(vp.process, v.process)
 
     @unittest.skip("Currently not supported")
     def test_connect_RefPort_to_many_Vars(self):
         """Checks that RefPort can be connected to many Vars."""
 
         # We can have multiple Vars...
         v1 = Var((1, 2, 3))
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/process/ports/test_virtual_ports_in_process.py` & `lava_nc-0.8.0/tests/lava/magma/core/process/ports/test_virtual_ports_in_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/process/test_process.py` & `lava_nc-0.8.0/tests/lava/magma/core/process/test_process.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,38 +2,59 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import logging
 import unittest
 from unittest.mock import Mock, seal
 import typing as ty
+from lava.magma.compiler.executable import Executable
+from lava.magma.core.decorator import implements, requires
+from lava.magma.core.sync.protocols.loihi_protocol import LoihiProtocol
+from lava.magma.core.model.py.model import PyLoihiProcessModel
 
 from lava.magma.core.process.ports.ports import (
     InPort,
     OutPort,
     RefPort,
     VarPort,
 )
 from lava.magma.core.process.process import (
     AbstractProcess,
     Collection,
     ProcessServer, LogConfig, ProcessParameters,
 )
 from lava.magma.core.model.model import AbstractProcessModel
 from lava.magma.core.process.variable import Var
+from lava.magma.core.resources import CPU
 from lava.magma.core.run_conditions import RunSteps
+from lava.magma.core.run_configs import RunConfig
+from lava.magma.runtime.runtime import Runtime
 
 
 class MinimalProcess(AbstractProcess):
     """The most minimal process has no Vars or Ports."""
 
     def __init__(self, name: ty.Optional[str] = None):
         super().__init__(name=name)
 
 
+@implements(proc=MinimalProcess, protocol=LoihiProtocol)
+@requires(CPU)
+class MinimalPyProcessModel(PyLoihiProcessModel):
+    pass
+
+
+class MinimalRunConfig(RunConfig):
+    def __init__(self):
+        super().__init__(custom_sync_domains=None, loglevel=logging.WARNING)
+
+    def select(self, proc, proc_models):
+        return proc_models[0]
+
+
 class TestCollection(unittest.TestCase):
     def setUp(self):
         """Reset ProcessServer before each test."""
         ProcessServer().reset_server()
 
     def test_constuctor(self):
         """Check that Collection can be constructed."""
@@ -255,21 +276,43 @@
         self.assertFalse(yet_another_proc.is_sub_proc_of(proc1))
 
 
 class TestProcess(unittest.TestCase):
     def test_model_property(self) -> None:
         """Tests whether the ProcessModel of a Process can be obtained
         through a property method."""
-
         p = MinimalProcess()
         p._model_class = Mock(spec_set=AbstractProcessModel)
         seal(p._model_class)
-
         self.assertIsInstance(p.model_class, AbstractProcessModel)
 
+    def test_compile(self) -> None:
+        """Test whether compile creates an executable which is ready
+        to build the process model for a simple process."""
+        p = MinimalProcess()
+        run_cfg = MinimalRunConfig()
+        e = p.compile(run_cfg)
+        self.assertIsInstance(e, Executable)
+        self.assertEqual(len(e.proc_builders), 1)
+
+    def test_create_runtime(self) -> None:
+        """Tests the create_runtime method."""
+        p = MinimalProcess()
+        self.assertIsNone(p.runtime)
+        run_cfg = MinimalRunConfig()
+        p.create_runtime(run_cfg)
+        r = p.runtime
+        self.assertIsInstance(r, Runtime)
+        self.assertTrue(r._is_initialized)
+        self.assertFalse(r._is_started)
+        self.assertFalse(r._is_running)
+        # HACK: Need to fix Issue #716 to avoid this.
+        p.run(condition=RunSteps(1), run_cfg=run_cfg)
+        p.stop()
+
     def test_run_without_run_config_raises_error(self) -> None:
         """Tests whether an error is raised when run() is called on
         uncompiled Processes without specifying a RunConfig."""
         p = MinimalProcess()
         condition = RunSteps(200)
         with self.assertRaises(ValueError):
             p.run(condition=condition)
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/core/process/test_variable.py` & `lava_nc-0.8.0/tests/lava/magma/core/process/test_variable.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_async_protocol.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_async_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,46 +65,46 @@
 
 class TestProcess(unittest.TestCase):
     def test_async_process_model(self):
         """
         Verifies the working of Asynchronous Process
         """
         process = AsyncProcess1(shape=(2, 2))
-        simple_sync_domain = SyncDomain("simple", AsyncProtocol(), [process])
+        _ = SyncDomain("simple", AsyncProtocol(), [process])
         process.run(condition=RunContinuous(), run_cfg=Loihi2SimCfg())
         process.stop()
 
     def test_async_process_model_pause(self):
         """
         Verifies the working of Asynchronous Process, pause should have
         effect
         """
         process = AsyncProcess1(shape=(2, 2))
-        simple_sync_domain = SyncDomain("simple", AsyncProtocol(), [process])
+        _ = SyncDomain("simple", AsyncProtocol(), [process])
         process.run(condition=RunContinuous(), run_cfg=Loihi2SimCfg())
         process.pause()
         process.stop()
 
     def test_async_process_num_steps(self):
         """
         Verifies the working of Asynchronous Process, numsteps should be
         implicitly passed as num_steps for the process.
         """
         process = AsyncProcess2(shape=(2, 2))
-        simple_sync_domain = SyncDomain("simple", AsyncProtocol(), [process])
+        _ = SyncDomain("simple", AsyncProtocol(), [process])
         process.run(condition=RunSteps(num_steps=10), run_cfg=Loihi2SimCfg())
         process.stop()
 
     def test_async_process_get(self):
         """
         Verifies the working of Asynchronous Process, get should get the value
         of the variable after run finishes.
         """
         process = AsyncProcess2(shape=(2, 2))
-        simple_sync_domain = SyncDomain("simple", AsyncProtocol(), [process])
+        _ = SyncDomain("simple", AsyncProtocol(), [process])
         process.run(condition=RunSteps(num_steps=10), run_cfg=Loihi2SimCfg())
         print(process.u.get())
         process.stop()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_context_manager.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_exception_handling.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_exception_handling.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_get_set_non_determinism.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_get_set_non_determinism.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self.changed[0] = False
 
 
 class TestNonDeterminismUpdate(unittest.TestCase):
     def test_non_determinism_update(self):
         nb_runs = 10000
         demo_process = DemoProcess(nb_runs=nb_runs)
-        for i in range(nb_runs):
+        for _ in range(nb_runs):
             demo_process.run(condition=RunSteps(num_steps=1),
                              run_cfg=Loihi1SimCfg())
 
             demo_process.changed.set(np.array([True]))
 
             # Uncomment this, test will pass
             # Comment this, test will probably fail
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_get_set_var.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_get_set_var.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_io_ports.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_io_ports.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_leakage.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_leakage.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_loihi_protocol.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_loihi_protocol.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_loihi_with_async_protocol.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_loihi_with_async_protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,14 @@
 from lava.magma.core.process.variable import Var
 from lava.magma.core.resources import CPU
 from lava.magma.core.run_conditions import RunSteps
 from lava.magma.core.run_configs import Loihi2SimCfg
 from lava.magma.core.sync.protocols.async_protocol import AsyncProtocol
 from lava.magma.core.sync.protocols.loihi_protocol import LoihiProtocol
 
-"""
-This test checks if Process with Loihi Protocol works properly with
-process with Async Protocol.
-"""
-
 
 class AsyncProcessDest(AbstractProcess):
     def __init__(self, **kwargs):
         super().__init__()
         shape = kwargs["shape"]
         self.in_port = InPort(shape=shape)
 
@@ -88,14 +83,18 @@
 
     def run_spk(self):
         var = self.in_port.recv()
         self.out_port.send(var)
 
 
 class TestProcess(unittest.TestCase):
+    """This test checks if Process with Loihi Protocol works properly with
+    process with Async Protocol.
+    """
+
     def test_async_with_loihi_protocol(self):
         """
         Test is to send the data to AsyncProcessSrc from AsyncProcessSrc via
         LoihiProcess.
         AsyncProcessSrc -- > LoihiProcess --> AsyncProcessSrc
         """
         shape = (2,)
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_pause_requested_from_model.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_pause_requested_from_model.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_ref_var_ports.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_ref_var_ports.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_run_continuously_and_pause.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_run_continuously_and_pause.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_runtime.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
         expected_type: ty.Type = Runtime
         self.assertIsInstance(
             runtime, expected_type,
             f"Expected type {expected_type} doesn't match {(type(runtime))}")
 
     def test_executable_node_config_assertion(self):
         """Tests runtime constructions with expected constraints"""
-        exe: Executable = Executable(proc_builders={},
+        exe: Executable = Executable(process_list=[],
+                                     proc_builders={},
                                      channel_builders=[],
                                      node_configs=[],
                                      sync_domains=[])
 
         runtime1: Runtime = Runtime(exe, ActorType.MultiProcessing)
         runtime1.initialize()
 
@@ -41,15 +42,16 @@
         runtime2.initialize()
         expected_type: ty.Type = Runtime
         self.assertIsInstance(
             runtime2, expected_type,
             f"Expected type {expected_type} doesn't match {(type(runtime2))}")
         runtime2.stop()
 
-        exe1: Executable = Executable(proc_builders={},
+        exe1: Executable = Executable(process_list=[],
+                                      proc_builders={},
                                       channel_builders=[],
                                       node_configs=[],
                                       sync_domains=[])
         node1: Node = Node(Loihi2System, [])
         exe1.node_configs.append(NodeConfig([node1]))
         runtime3: Runtime = Runtime(exe1, ActorType.MultiProcessing)
         runtime3.initialize(0)
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/magma/runtime/test_runtime_service.py` & `lava_nc-0.8.0/tests/lava/magma/runtime/test_runtime_service.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_0.npz` & `lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_0.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_1.npz` & `lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_1.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_2.npz` & `lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_2.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_3.npz` & `lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_3.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_4.npz` & `lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_4.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_5.npz` & `lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_5.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_6.npz` & `lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_6.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_7.npz` & `lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_7.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_8.npz` & `lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_8.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/conv/ground_truth/gt_conv_paris_9.npz` & `lava_nc-0.8.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_9.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/conv/test_process.py` & `lava_nc-0.8.0/tests/lava/proc/conv/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/conv/test_utils.py` & `lava_nc-0.8.0/tests/lava/proc/conv/test_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,48 +14,47 @@
     compare = True
     # in this case, the test compares against torch ground truth
 else:
     compare = False
     # in this case, the test only checks for error during
     # utils.conv calculation
 
-np.random.seed(8534)
-
 
 class TestConv(unittest.TestCase):
     def test_conv(self) -> None:
         """Test convolution implementation"""
+        prng = np.random.RandomState(8534)
         for _ in range(10):  # testing with 10 random combinations
-            groups = np.random.randint(4) + 1
-            in_channels = (np.random.randint(8) + 1) * groups
-            out_channels = (np.random.randint(8) + 1) * groups
-            kernel_size = np.random.randint([9, 9]) + 1
-            stride = np.random.randint([5, 5]) + 1
-            padding = np.random.randint([5, 5])
-            dilation = np.random.randint([4, 4]) + 1
+            groups = prng.randint(4) + 1
+            in_channels = (prng.randint(8) + 1) * groups
+            out_channels = (prng.randint(8) + 1) * groups
+            kernel_size = prng.randint([9, 9]) + 1
+            stride = prng.randint([5, 5]) + 1
+            padding = prng.randint([5, 5])
+            dilation = prng.randint([4, 4]) + 1
             weight_dims = [out_channels,
                            kernel_size[0], kernel_size[1],
                            in_channels // groups]
-            weights = np.random.randint(256, size=weight_dims) - 128
-            input = np.random.random(
+            weights = prng.randint(256, size=weight_dims) - 128
+            input_ = prng.random(
                 (
                     # input needs to be a certain size
                     # to make sure the output dimension is never negative
-                    np.random.randint([128, 128]) + kernel_size * dilation
+                    prng.randint([128, 128]) + kernel_size * dilation
                 ).tolist()
                 + [in_channels]
             )
 
-            out = utils.conv_scipy(input, weights, kernel_size,
+            out = utils.conv_scipy(input_, weights, kernel_size,
                                    stride, padding, dilation, groups)
 
             if compare:  # if torch is available, compare against it.
                 out_gt = F.conv2d(
                     torch.unsqueeze(  # torch expects a batch dimension NCHW
-                        torch.FloatTensor(input.transpose([2, 1, 0])),
+                        torch.FloatTensor(input_.transpose([2, 1, 0])),
                         dim=0,
                     ),
                     torch.FloatTensor(
                         # torch acutally does correlation
                         # so flipping the spatial dimension of weight
                         # copy() is needed because
                         # torch cannot handle negative stride
@@ -66,15 +65,15 @@
                     dilation=dilation[::-1].tolist(),
                     groups=groups
                 )[0].cpu().data.numpy().transpose([2, 1, 0])
 
                 error = np.abs(out - out_gt).mean()
                 if error >= 1e-3:  # small eps to account for float/double calc
                     # Setting failed! Print out the dimensions for debugging.
-                    print(f'{input.shape=}')
+                    print(f'{input_.shape=}')
                     print(f'{weights.shape=}')
                     print(f'{kernel_size=}')
                     print(f'{stride=}')
                     print(f'{padding=}')
                     print(f'{dilation=}')
                     print(f'{groups=}')
                     print(f'{out.shape=}')
@@ -85,14 +84,15 @@
                     f'Found\n'
                     f'{out.flatten()[:50] = }\n'
                     f'{out_gt.flatten()[:50] = }\n'
                 )
 
     def test_conv_saved_data(self) -> None:
         """Test convolution implementation against saved data."""
+        prng = np.random.RandomState(8534)
         for i in range(10):  # testing with 10 random combinations
             gt_data = np.load(os.path.dirname(os.path.abspath(__file__))
                               + f'/ground_truth/gt_conv_paris_{i}.npz')
             out = utils.conv_scipy(gt_data['input'],
                                    gt_data['weights'],
                                    gt_data['kernel_size'],
                                    gt_data['stride'],
@@ -107,31 +107,32 @@
                 f'Found\n'
                 f'{out.flatten()[:50] = }\n'
                 f'{out_gt.flatten()[:50] = }\n'
             )
 
     def test_conv_to_sparse(self) -> None:
         """Tests translation of a conv to a sparse layer"""
+        prng = np.random.RandomState(8534)
         for _ in range(10):
-            groups = np.random.randint(4) + 1
-            in_channels = (np.random.randint(4) + 1) * groups
-            out_channels = (np.random.randint(8) + 1) * groups
-            kernel_size = np.random.randint([5, 5]) + 1
-            stride = np.random.randint([2, 2]) + 1
-            padding = np.random.randint([2, 2])
-            dilation = np.random.randint([2, 2]) + 1
+            groups = prng.randint(4) + 1
+            in_channels = (prng.randint(4) + 1) * groups
+            out_channels = (prng.randint(8) + 1) * groups
+            kernel_size = prng.randint([5, 5]) + 1
+            stride = prng.randint([2, 2]) + 1
+            padding = prng.randint([2, 2])
+            dilation = prng.randint([2, 2]) + 1
             weight_dims = [out_channels,
                            kernel_size[0], kernel_size[1],
                            in_channels // groups]
-            weights = np.random.randint(256, size=weight_dims) - 128
-            input = np.random.random(
+            weights = prng.randint(256, size=weight_dims) - 128
+            input = prng.random(
                 (
                     # input needs to be a certain size
                     # to make sure the output dimension is never negative
-                    np.random.randint([16, 16]) + kernel_size * dilation
+                    prng.randint([16, 16]) + kernel_size * dilation
                 ).tolist()
                 + [in_channels]
             )
 
             output_gt = utils.conv_scipy(input, weights, kernel_size,
                                          stride, padding, dilation, groups)
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/dense/test_learning.py` & `lava_nc-0.8.0/tests/lava/proc/dense/test_learning.py`

 * *Files 1% similar despite different names*

```diff
@@ -693,16 +693,17 @@
         dw=y0 * x1 learning rule."""
 
         num_steps = 5
 
         learning_rule_cnd = "y0"
         graded_spike_cfg = GradedSpikeCfg.USE_REGULAR_IMPULSE
 
-        pre_ring_buffer, learning_dense, _ = \
-            self.create_network(num_steps, learning_rule_cnd, graded_spike_cfg)
+        pre_ring_buffer, dense, _ = self.create_network(num_steps,
+                                                        learning_rule_cnd,
+                                                        graded_spike_cfg)
 
         # x1 updates with decayed regular impulse, at the end of the epoch
         expected_x1_data = [0.0, 0.0, 0.0, 14.0, 14.0]
         # x2 updates with decayed regular impulse, at the end of the epoch
         expected_x2_data = [0.0, 0.0, 0.0, 16.0, 16.0]
         # weight update at the end of the epoch = value of x1 at post-spike time
         # i.e 1 time step after pre-spike time, hence the decay
@@ -710,17 +711,17 @@
         x1_data = []
         x2_data = []
         wgt_data = []
         for _ in range(num_steps):
             pre_ring_buffer.run(condition=self._run_cnd,
                                 run_cfg=self._run_cfg)
 
-            x1_data.append(learning_dense.x1.get()[0])
-            x2_data.append(learning_dense.x2.get()[0])
-            wgt_data.append(learning_dense.weights.get()[0, 0])
+            x1_data.append(dense.x1.get()[0])
+            x2_data.append(dense.x2.get()[0])
+            wgt_data.append(dense.weights.get()[0, 0])
 
         pre_ring_buffer.stop()
 
         np.testing.assert_almost_equal(x1_data, expected_x1_data)
         np.testing.assert_almost_equal(x2_data, expected_x2_data)
         np.testing.assert_almost_equal(wgt_data, expected_wgt_data)
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/dense/test_models.py` & `lava_nc-0.8.0/tests/lava/proc/dense/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,15 +564,15 @@
         """"""
         shape = (3, 4)
         weights = np.zeros(shape, dtype=float)
         weights[2, 2] = 1
         delays = np.zeros(shape, dtype=int)
         delays[2, 2] = 2
         max_delay = np.max(delays)
-        wgt_dly = AbstractPyDelayDenseModel.get_del_wgts(weights, delays)
+        wgt_dly = AbstractPyDelayDenseModel.get_delay_wgts_mat(weights, delays)
         # Expected shape is maximum delay=2 + 1 = 3 times first dimension of
         # original shape (3, 4) => (9, 4)
         expected_shape = ((max_delay + 1) * 3, 4)
         self.assertTrue(np.shape(wgt_dly) == expected_shape)
         # Expected matrix stacks n zero matrices of original shape of the
         # weights matrix vertically to create the wgt_dly matrix. n being the
         # maximum delay in the delay matrix.
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/dense/test_process.py` & `lava_nc-0.8.0/tests/lava/proc/dense/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/dense/test_stdp_sim.py` & `lava_nc-0.8.0/tests/lava/proc/dense/test_stdp_sim.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/io/test_dataloader.py` & `lava_nc-0.8.0/tests/lava/proc/io/test_dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,27 @@
 class DummyDataset:
     def __init__(self, shape: tuple) -> None:
         self.shape = shape
 
     def __len__(self) -> int:
         return 10
 
-    def __getitem__(self, id: int) -> Tuple[np.ndarray, int]:
-        data = np.arange(np.prod(self.shape)).reshape(self.shape) + id
+    def __getitem__(self, id_: int) -> Tuple[np.ndarray, int]:
+        data = np.arange(np.prod(self.shape)).reshape(self.shape) + id_
         data = data % np.prod(self.shape)
-        label = id
+        label = id_
         return data, label
 
 
 class SpikeDataset(DummyDataset):
-    def __getitem__(self, id: int) -> Tuple[np.ndarray, int]:
-        data = np.arange(np.prod(self.shape)).reshape(self.shape[::-1]) + id
+    def __getitem__(self, id_: int) -> Tuple[np.ndarray, int]:
+        data = np.arange(np.prod(self.shape)).reshape(self.shape[::-1]) + id_
         data = data.transpose(np.arange(len(self.shape))[::-1]) % 13
         data = data >= 10
-        label = id
+        label = id_
         return data, label
 
 
 class DummyProc(AbstractProcess):
     def __init__(self, shape: tuple) -> None:
         super().__init__()
         self.state = Var(shape=shape, init=np.zeros(shape))
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/io/test_source_sink.py` & `lava_nc-0.8.0/tests/lava/proc/io/test_source_sink.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,27 +34,27 @@
 class TestSendReceive(unittest.TestCase):
     """Tests for all SendProces and ReceiveProcess."""
 
     def test_source_sink(self) -> None:
         """Test whatever is being sent form source is received at sink."""
         num_steps = 10
         shape = (64, 64, 16)
-        input = np.random.randint(256, size=shape + (num_steps,))
-        input -= 128
+        input_ = np.random.randint(256, size=shape + (num_steps,))
+        input_ -= 128
         # input = 0.5 * input
 
-        source = SendProcess(data=input)
+        source = SendProcess(data=input_)
         sink = ReceiveProcess(shape=shape, buffer=num_steps)
         source.out_ports.s_out.connect(sink.in_ports.a_in)
 
         run_condition = RunSteps(num_steps=num_steps)
         run_config = TestRunConfig(select_tag='floating_pt')
         sink.run(condition=run_condition, run_cfg=run_config)
         output = sink.data.get()
         sink.stop()
 
         self.assertTrue(
-            np.all(output == input),
+            np.all(output == input_),
             f'Input and Ouptut do not match.\n'
-            f'{output[output!=input]=}\n'
-            f'{input[output!=input] =}\n'
+            f'{output[output!=input_]=}\n'
+            f'{input_[output!=input_] =}\n'
         )
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/lif/test_models.py` & `lava_nc-0.8.0/tests/lava/proc/lif/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# Copyright (C) 2021-22 Intel Corporation
+# Copyright (C) 2021-23 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import unittest
 import numpy as np
+from numpy.testing import assert_almost_equal
 
 from lava.magma.core.decorator import implements, requires, tag
 from lava.magma.core.model.py.model import PyLoihiProcessModel
 from lava.magma.core.model.py.ports import PyOutPort, PyInPort
 from lava.magma.core.model.py.type import LavaPyType
 from lava.magma.core.process.ports.ports import OutPort, InPort
 from lava.magma.core.process.process import AbstractProcess
 from lava.magma.core.process.variable import Var
 from lava.magma.core.resources import CPU
-from lava.magma.core.run_configs import Loihi1SimCfg, Loihi2SimCfg, RunConfig
+from lava.magma.core.run_configs import Loihi2SimCfg, RunConfig
 from lava.magma.core.run_conditions import RunSteps
 from lava.magma.core.sync.protocols.loihi_protocol import LoihiProtocol
-from lava.proc.lif.process import LIF, LIFReset, TernaryLIF
+from lava.proc.lif.process import LIF, LIFReset, TernaryLIF, LIFRefractory
 from lava.proc import io
 
 
 class LifRunConfig(RunConfig):
     """Run configuration selects appropriate LIF ProcessModel based on tag:
     floating point precision or Loihi bit-accurate fixed point precision"""
     def __init__(self, custom_sync_domains=None, select_tag='fixed_pt'):
@@ -240,15 +241,15 @@
         sps.s_out.connect(lif.a_in)
         lif.s_out.connect(spr.s_in)
         # Configure to run 1 step at a time
         rcnd = RunSteps(num_steps=1)
         rcfg = LifRunConfig(select_tag='floating_pt')
         lif_v = []
         # Run 1 timestep at a time and collect state variable u
-        for j in range(num_steps):
+        for _ in range(num_steps):
             lif.run(condition=rcnd, run_cfg=rcfg)
             lif_v.append(lif.v.get()[0])
         lif.stop()
         # Gold standard for testing: voltage decay of 0.5 should integrate
         # the voltage from 128. to 255., with steps of 64., 32., 16., etc.
         expected_v_timeseries = [128., 192., 224., 240., 248., 252., 254., 255.]
         self.assertListEqual(expected_v_timeseries, lif_v)
@@ -389,15 +390,14 @@
         self.assertListEqual(expected_v_timeseries, lif_v)
         self.assertListEqual(expected_float_v, lif_v_float.tolist())
 
     def test_bitacc_pm_scaling_of_bias(self):
         """
         Tests fixed point LIF ProcessModel's scaling of threshold.
         """
-        num_steps = 1
         bias_mant = 2 ** 12 - 1
         bias_exp = 5
         # Set up high threshold and high bias current to check for potential
         # overflow in effective bias in single neuron.
         lif = LIF(shape=(1,),
                   du=0,
                   dv=0,
@@ -821,7 +821,41 @@
         dt = (1 + np.arange(num_steps - reset_offset + 1) % 4).reshape(1, -1)
         v_gt_post = (1 + np.arange(num_neurons)).reshape(-1, 1) * dt
 
         self.assertTrue(np.array_equal(u[:, :reset_offset - 1], u_gt_pre))
         self.assertTrue(np.array_equal(u[:, reset_offset - 1:], u_gt_post))
         self.assertTrue(np.array_equal(v[:, :reset_offset - 1], v_gt_pre))
         self.assertTrue(np.array_equal(v[:, reset_offset - 1:], v_gt_post))
+
+
+class TestLIFRefractory(unittest.TestCase):
+    """Test LIF Refractory process model"""
+
+    def test_float_model(self):
+        """Test float model"""
+        num_neurons = 2
+        num_steps = 8
+        refractory_period = 1
+
+        # Two neurons with different biases
+        lif_refractory = LIFRefractory(shape=(num_neurons,),
+                                       u=np.arange(num_neurons),
+                                       bias_mant=np.arange(num_neurons) + 1,
+                                       bias_exp=np.ones(
+                                           (num_neurons,), dtype=float),
+                                       vth=4.,
+                                       refractory_period=refractory_period)
+
+        v_logger = io.sink.Read(buffer=num_steps)
+        v_logger.connect_var(lif_refractory.v)
+
+        lif_refractory.run(condition=RunSteps(num_steps),
+                           run_cfg=Loihi2SimCfg(select_tag="floating_pt"))
+
+        v = v_logger.data.get()
+        lif_refractory.stop()
+
+        # Voltage is expected to remain at reset level for two time steps
+        v_expected = np.array([[1, 2, 3, 4, 0, 0, 1, 2],
+                               [2, 0, 0, 2, 0, 0, 2, 0]], dtype=float)
+
+        assert_almost_equal(v, v_expected)
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/lif/test_process.py` & `lava_nc-0.8.0/tests/lava/proc/lif/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/monitor/test_monitors.py` & `lava_nc-0.8.0/tests/lava/proc/monitor/test_monitors.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/rf/test_models.py` & `lava_nc-0.8.0/tests/lava/proc/rf/test_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,23 +63,23 @@
 class TestrfProcessModels(unittest.TestCase):
     """Tests for RF Process Model"""
 
     def run_test(
         self,
         period: float,
         alpha: float,
-        input: np.ndarray,
+        input_: np.ndarray,
         state_exp: int = 0,
         decay_bits: int = 0,
         vth: float = 1,
         tag: str = 'floating_pt',
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
-        input = np.int32(input.reshape(1, -1))
-        num_steps = input.size
-        source = io.source.RingBuffer(data=input)
+        input_ = np.int32(input_.reshape(1, -1))
+        num_steps = input_.size
+        source = io.source.RingBuffer(data=input_)
         rf = RF(shape=(1,),
                 period=period,
                 alpha=alpha,
                 vth=vth,
                 state_exp=state_exp,
                 decay_bits=decay_bits)
 
@@ -98,27 +98,27 @@
         sink.run(condition=run_condition, run_cfg=run_config)
 
         s_out = sink.data.get()
         real = real_monitor.get_data()[rf.name]["real"]
         imag = imag_monitor.get_data()[rf.name]["imag"]
         rf.stop()
 
-        return input, real, imag, s_out
+        return input_, real, imag, s_out
 
     def test_float_no_decay(self):
         """Verify that a neuron with no voltage decay spikes
             periodicaly due a single input pulse
         """
         period = 10
         alpha = 0
 
         num_steps = 100
-        input = np.zeros(num_steps)
-        input[0] = 1.1  # spike at first timestep
-        _, _, _, s_out = self.run_test(period, alpha, input)
+        input_ = np.zeros(num_steps)
+        input_[0] = 1.1  # spike at first timestep
+        _, _, _, s_out = self.run_test(period, alpha, input_)
 
         # observe differences in spike times
         spike_idx = np.argwhere(s_out[0, :])
         s_diffs = [j - i for i, j in zip(spike_idx[:-1], spike_idx[1:])]
 
         # Ensure correct spike count
         self.assertTrue((num_steps - 1) / period, s_out.size)
@@ -130,17 +130,17 @@
            voltage should match the alpha parameter at the real peaks.
         """
         period = 10
         alpha = .07
         vth = 1.1
 
         num_steps = 100
-        input = np.zeros(num_steps)
-        input[0] = 1  # spike at first timestep
-        _, real, _, _ = self.run_test(period, alpha, input, vth=vth)
+        input_ = np.zeros(num_steps)
+        input_[0] = 1  # spike at first timestep
+        _, real, _, _ = self.run_test(period, alpha, input_, vth=vth)
 
         ideal_real = np.round((1 - alpha)**np.arange(num_steps), 6)
         round_real = np.round(real.flatten(), 6)
         self.assertListEqual(round_real.tolist()[0:num_steps:period],
                              ideal_real.tolist()[0:num_steps:period])
 
     def test_fixed_pm_no_decay(self):
@@ -151,33 +151,33 @@
         alpha = 0
         vth = .5  # choose a low voltage threshold to achieve repeat spiking
         decay_bits = 12
         state_exp = 6
         period = 10
 
         num_steps = 100
-        input = np.zeros(num_steps)
-        input[0] = 1  # spike at first timestep
+        input_ = np.zeros(num_steps)
+        input_[0] = 1  # spike at first timestep
 
-        _, _, _, s_out = self.run_test(period, alpha, input, vth=vth,
+        _, _, _, s_out = self.run_test(period, alpha, input_, vth=vth,
                                        state_exp=state_exp,
                                        decay_bits=decay_bits,
                                        tag="fixed_pt")
 
         # real, imag voltages
         sin_decay = (1 - alpha) * np.sin(np.pi * 2 * 1 / period)
         cos_decay = (1 - alpha) * np.cos(np.pi * 2 * 1 / period)
 
         # scale decays
         sin_decay = int(sin_decay * (1 << decay_bits))
         cos_decay = int(cos_decay * (1 << decay_bits))
 
         # Run Test RF Dynamics
         real, imag = rf_dynamics(0, 0, sin_decay, cos_decay,
-                                 input * (1 << state_exp),
+                                 input_ * (1 << state_exp),
                                  np.zeros(num_steps),
                                  decay_bits)
 
         # spiking function needs time delayed imaginary voltage
         old_imag = np.zeros(num_steps)
         old_imag[1:num_steps] = imag[:num_steps - 1]
         expected_spikes = (real >= (vth * (1 << state_exp))) \
@@ -193,33 +193,33 @@
         alpha = .05
         vth = .5  # choose a low voltage threshold to achieve repeat spiking
         decay_bits = 12
         state_exp = 6
         period = 10
 
         num_steps = 100
-        input = np.zeros(num_steps)
-        input[0] = 2  # spike at first timestep
+        input_ = np.zeros(num_steps)
+        input_[0] = 2  # spike at first timestep
 
-        _, _, _, s_out = self.run_test(period, alpha, input, vth=vth,
+        _, _, _, s_out = self.run_test(period, alpha, input_, vth=vth,
                                        state_exp=state_exp,
                                        decay_bits=decay_bits,
                                        tag="fixed_pt")
 
         # real, imag voltages
         sin_decay = (1 - alpha) * np.sin(np.pi * 2 * 1 / period)
         cos_decay = (1 - alpha) * np.cos(np.pi * 2 * 1 / period)
 
         # scale decays
         sin_decay = int(sin_decay * (1 << decay_bits))
         cos_decay = int(cos_decay * (1 << decay_bits))
 
         # Run Test RF Dynamics
         real, imag = rf_dynamics(0, 0, sin_decay, cos_decay,
-                                 input * (1 << state_exp),
+                                 input_ * (1 << state_exp),
                                  np.zeros(num_steps),
                                  decay_bits)
 
         # spiking function needs time delayed imaginary voltage
         old_imag = np.zeros(num_steps)
         old_imag[1:num_steps] = imag[:num_steps - 1]
         expected_spikes = (real >= (vth * (1 << state_exp))) \
@@ -244,20 +244,20 @@
         # sin_decay * (1 << state_exp) < (1 << decay_bits)
         period = np.ceil(np.pi * 2
                          / (np.arcsin(1 / ((1 << state_exp) * (1 - alpha)))))
         cos_decay = (1 - alpha) * np.cos(np.pi * 2 * 1 / period)
         cos_decay = int(cos_decay * (1 << decay_bits))
 
         num_steps = 100
-        input = np.zeros(num_steps)
-        input[0] = 1  # spike at first timestep
+        input_ = np.zeros(num_steps)
+        input_[0] = 1  # spike at first timestep
         decay_bits = 12
         state_exp = 6
 
-        _, real, _, _ = self.run_test(period, alpha, input, vth=vth,
+        _, real, _, _ = self.run_test(period, alpha, input_, vth=vth,
                                       state_exp=state_exp,
                                       decay_bits=decay_bits,
                                       tag="fixed_pt")
 
         # Repeatedly decay real voltage
         voltage = np.int32(1 * (1 << state_exp))
         ideal_real = []
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/rf/test_process.py` & `lava_nc-0.8.0/tests/lava/proc/rf/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/rf_iz/test_models.py` & `lava_nc-0.8.0/tests/lava/proc/rf_iz/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 class Testrf_izProcessModels(unittest.TestCase):
     """Tests for RF Process Model"""
 
     def run_test(
         self,
         period: float,
         alpha: float,
-        input: np.ndarray,
+        input_: np.ndarray,
         state_exp: int = 0,
         decay_bits: int = 0,
         vth: float = 1,
         tag: str = 'floating_pt',
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
-        input = input.reshape(1, -1)
-        num_steps = input.size
-        source = io.source.RingBuffer(data=input)
+        input_ = input_.reshape(1, -1)
+        num_steps = input_.size
+        source = io.source.RingBuffer(data=input_)
         rf = RF_IZ(shape=(1,),
                    period=period,
                    alpha=alpha,
                    vth=vth,
                    state_exp=state_exp,
                    decay_bits=decay_bits)
 
@@ -51,27 +51,27 @@
         rf.run(condition=run_condition, run_cfg=run_config)
 
         s_out = sink.data.get()
         real = real_monitor.get_data()[rf.name]["real"]
         imag = imag_monitor.get_data()[rf.name]["imag"]
         rf.stop()
 
-        return input, real, imag, s_out
+        return input_, real, imag, s_out
 
     def test_float_reset(self):
         """Ensure that spikes events are followed by proper rf_iz reset
         """
         period = 10
         alpha = .07
         eps = 1e-5
 
         num_steps = 100
-        input = np.zeros(num_steps)
-        input[[0, 10, 20]] = 1  # Will ensure 3 spikes
-        _, real, imag, s_out = self.run_test(period, alpha, input)
+        input_ = np.zeros(num_steps)
+        input_[[0, 10, 20]] = 1  # Will ensure 3 spikes
+        _, real, imag, s_out = self.run_test(period, alpha, input_)
         s_out = s_out.flatten() == 1  # change to bool
         self.assertGreaterEqual(s_out.sum(), 1)  # ensure network is spiking
         self.assertListEqual(real.flatten()[s_out].tolist(),
                              [0] * np.sum(s_out))
         self.assertListEqual(imag.flatten()[s_out].tolist(),
                              [1 - eps] * np.sum(s_out))
 
@@ -80,17 +80,17 @@
            for fixed point implementation
         """
         period = 10
         alpha = .07
         eps = 1  # in fixed point 1 is the smallest value we can have
         state_exp = 6
         num_steps = 100
-        input = np.zeros(num_steps)
-        input[[0, 10, 20]] = 1  # Will ensure 3 spikes
-        _, real, imag, s_out = self.run_test(period, alpha, input,
+        input_ = np.zeros(num_steps)
+        input_[[0, 10, 20]] = 1  # Will ensure 3 spikes
+        _, real, imag, s_out = self.run_test(period, alpha, input_,
                                              tag="fixed_pt",
                                              state_exp=state_exp,
                                              decay_bits=12)
         s_out = s_out.flatten() == 1  # change to bool
         self.assertGreaterEqual(s_out.sum(), 1)  # ensure network is spiking
         self.assertListEqual(real.flatten()[s_out].tolist(),
                              [0] * np.sum(s_out))
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/rf_iz/test_process.py` & `lava_nc-0.8.0/tests/lava/proc/rf_iz/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/sdn/test_models.py` & `lava_nc-0.8.0/tests/lava/proc/sdn/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,61 +20,61 @@
     """Tests for sigma decoding"""
 
     def run_test(
         self,
         num_steps: int,
         tag: str = 'fixed_pt'
     ) -> Tuple[np.ndarray, np.ndarray]:
-        input = np.sin(0.1 * np.arange(num_steps).reshape(1, -1))
+        input_ = np.sin(0.1 * np.arange(num_steps).reshape(1, -1))
         if tag == 'fixed_pt':
-            input *= (1 << 12)
-            input = input.astype(int)
-        input[:, 1:] -= input[:, :-1]
+            input_ *= (1 << 12)
+            input_ = input_.astype(int)
+        input_[:, 1:] -= input_[:, :-1]
 
-        source = io.source.RingBuffer(data=input)
+        source = io.source.RingBuffer(data=input_)
         sigma = Sigma(shape=(1,))
         sink = io.sink.RingBuffer(shape=sigma.shape, buffer=num_steps)
 
         source.s_out.connect(sigma.a_in)
         sigma.s_out.connect(sink.a_in)
 
         run_condition = RunSteps(num_steps=num_steps)
         run_config = Loihi1SimCfg(select_tag=tag)
 
         sigma.run(condition=run_condition, run_cfg=run_config)
         output = sink.data.get()
         sigma.stop()
 
-        return input, output
+        return input_, output
 
     def test_sigma_decoding_fixed(self) -> None:
         """Test sigma decoding with cumulative sum."""
         num_steps = 100
 
-        input, output = self.run_test(
+        input_, output = self.run_test(
             num_steps=num_steps,
             tag='fixed_pt'
         )
 
-        error = np.abs(np.cumsum(input, axis=1) - output).max()
+        error = np.abs(np.cumsum(input_, axis=1) - output).max()
 
         if verbose:
             print(f'Max abs error = {error}')
         self.assertTrue(error == 0)
 
     def test_sigma_decoding_float(self) -> None:
         """Test sigma decoding with cumulative sum."""
         num_steps = 100
 
-        input, output = self.run_test(
+        input_, output = self.run_test(
             num_steps=num_steps,
             tag='floating_pt'
         )
 
-        error = np.abs(np.cumsum(input, axis=1) - output).max()
+        error = np.abs(np.cumsum(input_, axis=1) - output).max()
 
         if verbose:
             print(f'Max abs error = {error}')
         self.assertTrue(error < 1e-6)
 
 
 class TestSigmaDeltaModels(unittest.TestCase):
@@ -86,19 +86,19 @@
         vth: int,
         act_mode: ActivationMode,
         spike_exp: int,
         state_exp: int,
         cum_error: bool,
         tag: str = 'fixed_pt',
     ) -> Tuple[np.ndarray, np.ndarray]:
-        input = np.sin(0.1 * np.arange(num_steps).reshape(1, -1))
-        input *= (1 << spike_exp + state_exp)
-        input[:, 1:] -= input[:, :-1]
+        input_ = np.sin(0.1 * np.arange(num_steps).reshape(1, -1))
+        input_ *= (1 << spike_exp + state_exp)
+        input_[:, 1:] -= input_[:, :-1]
 
-        source = io.source.RingBuffer(data=input.astype(int) * (1 << 6))
+        source = io.source.RingBuffer(data=input_.astype(int) * (1 << 6))
         sdn = SigmaDelta(
             shape=(1,),
             vth=vth,
             act_mode=act_mode,
             spike_exp=spike_exp,
             state_exp=state_exp,
             cum_error=cum_error
@@ -111,152 +111,152 @@
         run_condition = RunSteps(num_steps=num_steps)
         run_config = Loihi1SimCfg(select_tag=tag)
 
         sdn.run(condition=run_condition, run_cfg=run_config)
         output = sink.data.get()
         sdn.stop()
 
-        input = np.cumsum(input, axis=1)
+        input_ = np.cumsum(input_, axis=1)
         output = np.cumsum(output, axis=1)
 
-        return input, output
+        return input_, output
 
     def test_reconstruction_fixed(self) -> None:
         """Tests fixed point sigma delta reconstruction. The max absolute
         error must be smaller than threshold.
         """
         num_steps = 100
         spike_exp = 6
         state_exp = 6
         vth = 10 << (spike_exp + state_exp)
-        input, output = self.run_test(
+        input_, output = self.run_test(
             num_steps=num_steps,
             vth=vth,
             act_mode=ActivationMode.UNIT,
             spike_exp=spike_exp,
             state_exp=state_exp,
             cum_error=False,
         )
 
-        error = np.abs(input - output).max()
+        error = np.abs(input_ - output).max()
 
         if verbose:
             print(f'Max abs error = {error}')
         self.assertTrue(error < vth * (1 << spike_exp))
 
     def test_reconstruction_float(self) -> None:
         """Tests floating point sigma delta reconstruction. The max absolute
         error must be smaller than threshold.
         """
         num_steps = 100
         spike_exp = 0
         state_exp = 0
         vth = 10
-        input, output = self.run_test(
+        input_, output = self.run_test(
             num_steps=num_steps,
             vth=vth,
             act_mode=ActivationMode.UNIT,
             spike_exp=spike_exp,
             state_exp=state_exp,
             cum_error=False,
             tag='floating_pt'
         )
 
-        error = np.abs(input - output).max()
+        error = np.abs(input_ - output).max()
 
         if verbose:
             print(f'Max abs error = {error}')
         self.assertTrue(error < vth * (1 << spike_exp))
 
     def test_reconstruction_cum_error_fixed(self) -> None:
         """Tests fixed point sigma delta reconstruction with cumulative error.
         The max absolute error must be smaller than threshold.
         """
         num_steps = 100
         spike_exp = 6
         state_exp = 6
         vth = 10 << (spike_exp + state_exp)
-        input, output = self.run_test(
+        input_, output = self.run_test(
             num_steps=num_steps,
             vth=vth,
             act_mode=ActivationMode.UNIT,
             spike_exp=spike_exp,
             state_exp=state_exp,
             cum_error=True,
         )
 
-        error = np.abs(input - output).max()
+        error = np.abs(input_ - output).max()
 
         if verbose:
             print(f'Max abs error = {error}')
         self.assertTrue(error < vth * (1 << spike_exp))
 
     def test_reconstruction_cum_error_float(self) -> None:
         """Tests floating point sigma delta reconstruction with cumulative
         error. The max absolute error must be smaller than threshold.
         """
         num_steps = 100
         spike_exp = 0
         state_exp = 0
         vth = 10
-        input, output = self.run_test(
+        input_, output = self.run_test(
             num_steps=num_steps,
             vth=vth,
             act_mode=ActivationMode.UNIT,
             spike_exp=spike_exp,
             state_exp=state_exp,
             cum_error=True,
             tag='floating_pt'
         )
 
-        error = np.abs(input - output).max()
+        error = np.abs(input_ - output).max()
 
         if verbose:
             print(f'Max abs error = {error}')
         self.assertTrue(error < vth * (1 << spike_exp))
 
     def test_reconstruction_relu_fixed(self) -> None:
         """Tests fixed point sigma delta reconstruction with RELU.
         The max absolute error must be smaller than threshold.
         """
         num_steps = 100
         spike_exp = 0
         state_exp = 0
         vth = 10 << (spike_exp + state_exp)
-        input, output = self.run_test(
+        input_, output = self.run_test(
             num_steps=num_steps,
             vth=vth,
             act_mode=ActivationMode.RELU,
             spike_exp=spike_exp,
             state_exp=state_exp,
             cum_error=False,
         )
 
-        error = np.abs(np.maximum(input, 0) - output).max()
+        error = np.abs(np.maximum(input_, 0) - output).max()
 
         if verbose:
             print(f'Max abs error = {error}')
         self.assertTrue(error < vth * (1 << spike_exp))
 
     def test_reconstruction_relu_float(self) -> None:
         """Tests floating point sigma delta reconstruction with RELU.
         The max absolute error must be smaller than threshold.
         """
         num_steps = 100
         vth = 10
         spike_exp = 0
         state_exp = 0
-        input, output = self.run_test(
+        input_, output = self.run_test(
             num_steps=num_steps,
             vth=vth,
             act_mode=ActivationMode.RELU,
             spike_exp=spike_exp,
             state_exp=state_exp,
             cum_error=False,
             tag='floating_pt',
         )
 
-        error = np.abs(np.maximum(input, 0) - output).max()
+        error = np.abs(np.maximum(input_, 0) - output).max()
 
         if verbose:
             print(f'Max abs error = {error}')
         self.assertTrue(error < vth * (1 << spike_exp))
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/sdn/test_process.py` & `lava_nc-0.8.0/tests/lava/proc/sdn/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tests/lava/proc/spiker/test_models.py` & `lava_nc-0.8.0/tests/lava/proc/spiker/test_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 class TestSpikerModels(unittest.TestCase):
     """Tests spiker PyProcModel."""
 
     def test_single_spiker_counter(self):
         "Tests a single spiker for multiple time steps."
         spiker = Spiker(shape=(1,), period=5)
         counter = []
-        for timestep in range(20):
+        for _ in range(20):
             spiker.run(condition=RunSteps(num_steps=1),
                        run_cfg=Loihi2SimCfg())
             counter.append(spiker.counter.get()[0])
         spiker.stop()
         expected = np.asarray([1.0, 2.0, 3.0, 4.0, 5.0, 1.0, 2.0, 3.0, 4.0,
                                5.0, 1.0, 2.0, 3.0, 4.0, 5.0, 1.0, 2.0, 3.0,
                                4.0, 5.0])
         self.assertTrue(np.all(counter == expected))
 
     def test_multiple_spikers_counter(self):
         spiker = Spiker(shape=(2,), period=5)
         counter1 = []
         counter2 = []
-        for timestep in range(20):
+        for _ in range(20):
             spiker.run(condition=RunSteps(num_steps=1),
                        run_cfg=Loihi2SimCfg())
             counter1.append(spiker.counter.get()[0])
             counter2.append(spiker.counter.get()[1])
         spiker.stop()
         expected = np.asarray([1.0, 2.0, 3.0, 4.0, 5.0, 1.0, 2.0, 3.0, 4.0,
                                5.0, 1.0, 2.0, 3.0, 4.0, 5.0, 1.0, 2.0, 3.0,
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/test_utils/utils.py` & `lava_nc-0.8.0/tests/lava/test_utils/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import os
-import subprocess
+import subprocess  # noqa S404
 import importlib
 
 
 class Utils:
-    """Utility Class containing testing helper
-    code that can be reused between tests
+    """Utility Class containing testing helper code that can be reused
+    between tests.
     """
 
     @staticmethod
     def get_bool_env_setting(env_var: str):
         """Get an environment varible and return
         True if the variable is set to 1 else return
         false
@@ -22,26 +22,26 @@
         test_setting = False
         if env_test_setting == "1":
             test_setting = True
         return test_setting
 
     @staticmethod
     def is_loihi2_available() -> bool:
-        """"Checks if Loihi2 is available and can be accessed."""
+        """Checks if Loihi 2 is available and can be accessed."""
 
         is_loihi2 = False
         is_slurm = False
         is_nxcore = False
 
         # Check if SLURM is running
         if os.getenv("SLURM") == "1":
             is_slurm = True
 
             # Check if Loihi2 is available
-            sinfo = subprocess.run("sinfo",  # noqa: S603, S607
+            sinfo = subprocess.run("sinfo",  # nosec # noqa: S603, S607
                                    stdout=subprocess.PIPE).stdout.decode(
                 'utf-8')
             for line in sinfo.split("\n"):
                 if line.startswith(("oheogulch", "kp")):
                     is_loihi2 = True
 
         # Check if NxSDK is working
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/tutorials/test_tutorials.py` & `lava_nc-0.8.0/tests/lava/tutorials/test_tutorials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import glob
 import os
 import platform
-import subprocess  # noqa: S404
+import subprocess  # noqa S404
 import sys
 import tempfile
 import typing as ty
 import unittest
 from test import support
 
 import lava
@@ -114,15 +114,15 @@
                 "notebook",
                 "--execute",
                 "--ExecutePreprocessor.timeout=-1",
                 "--output",
                 fout.name,
                 notebook,
             ]
-            subprocess.check_call(args, env=env)  # noqa: S603
+            subprocess.check_call(args, env=env)  # nosec # noqa: S603
 
             fout.seek(0)
             return nbformat.read(fout, nbformat.current_nbformat)
 
     def _collect_errors_from_all_cells(
         self, nb: nbformat.NotebookNode
     ) -> ty.List[str]:
@@ -276,10 +276,21 @@
             "three_factor_learning/tutorial01_Reward_Modulated_STDP.ipynb")
 
     @unittest.skipIf(system_name != "linux", "Tests work on linux")
     def test_in_depth_10_custom_learning_rules(self):
         """Test tutorial sigma_delta_neurons."""
         self._run_notebook("tutorial10_sigma_delta_neurons.ipynb")
 
+    @unittest.skipIf(system_name != "linux", "Tests work on linux")
+    def test_in_depth_11_serialization(self):
+        """Test tutorial serialization."""
+        self._run_notebook("tutorial11_serialization.ipynb")
+
+    @unittest.skipIf(system_name != "linux", "Tests work on linux")
+    def test_in_depth_clp_01(self):
+        """Test tutorial CLP 01."""
+        self._run_notebook(
+            "clp/tutorial01_one-shot_learning_with_novelty_detection.ipynb")
+
 
 if __name__ == "__main__":
     support.run_unittest(TestTutorials)
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/utils/test_plots.py` & `lava_nc-0.8.0/tests/lava/utils/test_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,45 +26,45 @@
 
     def test_bad_spikes_shape(self) -> None:
         spikes = np.array([0, 1, 2])
 
         with self.assertRaises(ValueError) as cm:
             raster_plot(spikes)
 
-        self.assertEquals(
+        self.assertEqual(
             str(cm.exception),
             "Parameter <spikes> must have exactly two dimensions and "
             "they must be non-empty.",
         )
 
     def test_non_binary_values(self) -> None:
         error_msg = "All values in spikes must be either 0 or 1."
 
         spikes = np.array([[0, 2], [0, 0]])
         with self.assertRaises(ValueError) as cm:
             raster_plot(spikes)
 
-        self.assertEquals(str(cm.exception), error_msg)
+        self.assertEqual(str(cm.exception), error_msg)
 
         spikes = np.array([[0, -1], [0, 0]])
         with self.assertRaises(ValueError) as cm:
             raster_plot(spikes)
 
-        self.assertEquals(str(cm.exception), error_msg)
+        self.assertEqual(str(cm.exception), error_msg)
 
     def test_bad_stride(self) -> None:
         with self.assertRaises(ValueError) as cm:
             raster_plot(self.spikes, stride=11)
 
-        self.assertEquals(
+        self.assertEqual(
             str(cm.exception),
             "Stride must not be greater than the number of neurons.",
         )
 
     def test_both_fig_and_figsize_provided(self) -> None:
         with self.assertRaises(ValueError) as cm:
             raster_plot(self.spikes, fig=plt.figure(), figsize=(10, 10))
 
-        self.assertEquals(
+        self.assertEqual(
             str(cm.exception),
             "Must use at most one of the following: fig, figsize.",
         )
```

### Comparing `lava_nc-0.7.0.post2/tests/lava/utils/test_weightutils.py` & `lava_nc-0.8.0/tests/lava/utils/test_weightutils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/LICENSE` & `lava_nc-0.8.0/tutorials/LICENSE`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/end_to_end/convert_params.py` & `lava_nc-0.8.0/tutorials/end_to_end/convert_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     mean_inp : float
         Mean input received by each neuron
     '''
     mean_inp = num_neurons_exc * (1 - gamma * g_factor) * weight * rate + bias
 
     return mean_inp
 
+
 def _std_input(num_neurons_exc, gamma, g_factor, weight, rate):
     '''
     Calculate mean input to single neuron given mean excitatory weight.
 
     Parameters
     ----------
     num_neurons_exc : int
@@ -58,14 +59,15 @@
     Returns
     -------
     mean_inp : float
         Mean input received by each neuron
     '''
     return num_neurons_exc * (1 + gamma * g_factor**2) * weight ** 2 * rate
 
+
 def _y_th(vth, mean, std, dv_exc, du_exc):
     '''
     Effective threshold, see Grytskyy et al. 2013.
 
     Parameters
     ----------
     vth : float
@@ -85,14 +87,15 @@
         Effective threshold of neuron in network
     '''
     y_th = (vth - mean) / std
     y_th += np.sqrt(2) * np.abs(zetac(0.5)) * np.sqrt(dv_exc / du_exc) / 2
 
     return y_th
 
+
 def _y_r(mean, std, dv_exc, du_exc):
     '''
     Effective reset, see Grytskyy et al. 2013.
 
     Parameters
     ----------
     vth : float
@@ -112,20 +115,22 @@
         Effective reset of neuron in network
     '''
     y_r = (- 1 * mean) / std
     y_r += np.sqrt(2) * np.abs(zetac(0.5)) * np.sqrt(dv_exc / du_exc) / 2
 
     return y_r
 
+
 def f(y):
     '''
     Derivative of transfer function of LIF neuron at given argument.
     '''
     return np.exp(y ** 2) * (1 + erf(y))
 
+
 def _alpha(vth, mean, std, dv_exc, du_exc):
     '''
     Auxiliary variable describing contribution of weights for weight
     mapping given network state, see Grytskyy et al. 2013.
 
     Parameters
     ----------
@@ -148,14 +153,15 @@
     val = np.sqrt(np.pi) * (mean * dv_exc * 0.01) ** 2
     val *= 1 / std
     val *= (f(_y_th(vth, mean, std, dv_exc, du_exc))
             - f(_y_r(mean, std, dv_exc, du_exc)))
 
     return val
 
+
 def _beta(vth, mean, std, dv_exc, du_exc):
     '''
     Auxiliary variable describing contribution of square of weights for
     weight mapping given network state, see Grytskyy et al. 2013.
 
     Parameters
     ----------
@@ -172,22 +178,24 @@
 
     Returns
     -------
     val : float
         Contribution of square of weights
     '''
     val = np.sqrt(np.pi) * (mean * dv_exc * 0.01) ** 2
-    val *= 1/(2 * std ** 2)
+    val *= 1 / (2 * std ** 2)
     val *= (f(_y_th(vth, mean, std, dv_exc, du_exc)) * (vth - mean) / std
             - f(_y_r(mean, std, dv_exc, du_exc)) * (-1 * mean) / std)
 
     return val
 
-def convert_rate_to_lif_params(shape_exc, dr_exc, bias_exc, shape_inh, dr_inh,
-                              bias_inh, g_factor, q_factor, weights, **kwargs):
+
+def convert_rate_to_lif_params(
+        shape_exc, dr_exc, bias_exc, shape_inh, dr_inh, bias_inh, g_factor,
+        q_factor, weights, **kwargs):
     '''Convert rate parameters to LIF parameters.
     The mapping is based on A unified view on weakly correlated recurrent
     network, Grytskyy et al. 2013.
 
     Parameters
     ----------
     shape_exc : int
@@ -220,15 +228,16 @@
     num_neurons_exc = shape_exc
     num_neurons_inh = shape_inh
 
     # Ratio of excitatory to inhibitory neurons.
     gamma = float(num_neurons_exc) / float(num_neurons_inh)
 
     # Assert that network is balanced.
-    assert gamma * g_factor > 1, "Network not balanced, increase g_factor"
+    if gamma * g_factor <= 1:
+        raise AssertionError("Network not balanced, increase g_factor")
 
     # Set timescales of neurons.
     dv_exc = 1 * dr_exc  # Dynamics of membrane potential as fast as rate.
     du_exc = 7 * dr_exc  # Dynamics of current 7 times as fast as rate.
 
     dv_inh = 1 * dr_inh  # Dynamics of membrane potential as fast as rate.
     du_inh = 7 * dr_inh  # Dynamics of current 7 times as fast as rate.
@@ -271,15 +280,15 @@
     def func(weight):
         '''
         Adapted from Grytskyy et al..
         '''
         mean_inp = _mean_input(num_neurons_exc, gamma,
                                g_factor, weight, rate, bias)
         std_inp = _std_input(num_neurons_exc, gamma,
-                            g_factor, weight, rate)
+                             g_factor, weight, rate)
         alpha = _alpha(vth_exc, mean_inp, std_inp, dv_exc, du_inh)
         beta = _beta(vth_exc, mean_inp, std_inp, dv_exc, du_inh)
 
         return mean_exc_weight - alpha * weight - beta * weight**2
 
     # Solve for weights of LIF network retaining correlation structure of
     # rate network.
```

### Comparing `lava_nc-0.7.0.post2/tutorials/end_to_end/mnist_pretrained.npy` & `lava_nc-0.8.0/tutorials/end_to_end/mnist_pretrained.npy`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/end_to_end/tutorial00_tour_through_lava.ipynb` & `lava_nc-0.8.0/tutorials/end_to_end/tutorial00_tour_through_lava.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.956758931530755%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '*Copyright (C) 2022 Intel Corporation*<br>\\n'), (1, "*

 * *            "'*SPDX-License-Identifier: BSD-3-Clause*<br>\\n'), (2, '*See: "*

 * *            "https://spdx.org/licenses/*\\n'), (3, '\\n'), (4, '---\\n'), (5, '\\n'), (20, '- "*

 * *            "[lava-dnf](https://github.com/lava-nc/lava-dnf) for Dynamic Neural Fields\\n'), (21, "*

 * *            "'\\n'), (22, '## 1. Usage of the Process Library\\n'), (23, '\\n'), (24, 'In this "*

 * *            'section, we will use a simple 2 […]*

```diff
@@ -1,56 +1,39 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "f1bfa603",
+            "id": "3ebce42a",
             "metadata": {},
             "source": [
                 "*Copyright (C) 2022 Intel Corporation*<br>\n",
                 "*SPDX-License-Identifier: BSD-3-Clause*<br>\n",
                 "*See: https://spdx.org/licenses/*\n",
                 "\n",
-                "---"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "3ebce42a",
-            "metadata": {},
-            "source": [
+                "---\n",
+                "\n",
                 "# Walk through Lava\n",
                 "\n",
                 "Lava is an open-source software library dedicated to the development of algorithms for neuromorphic computation. To that end, Lava provides an easy-to-use Python interface for creating the bits and pieces required for such a neuromorphic algorithm. For easy development, Lava allows to run and test all neuromorphic algorithms on standard von-Neumann hardware like CPU, before they can be deployed on neuromorphic processors such as the Intel Loihi 1/2 processor to leverage their speed and power advantages. Furthermore, Lava is designed to be extensible to custom implementations of neuromorphic behavior and to support new hardware backends.\n",
                 "\n",
                 "Lava can fundamentally be used at two different levels: Either by using existing resources which can be used to create complex algorithms while requiring almost no deep neuromorphic knowledge. Or, for custom behavior, Lava can be easily extended with new behavior defined in Python and C.\n",
                 "\n",
                 "![lava_overview.png](https://raw.githubusercontent.com/lava-nc/lava-docs/dev/walk-through-tutorial/_static/images/tutorial00/lava_overview.png)\n",
                 "\n",
                 "This tutorial gives an high-level overview over the key components of Lava. For illustration, we will use a simple working example: a feed-forward multi-layer LIF network executed locally on CPU.\n",
                 "In the first section of the tutorial, we use the internal resources of Lava to construct such a network and in the second section, we demonstrate how to extend Lava with a custom process using the example of an input generator.\n",
                 "\n",
                 "In addition to the core Lava library described in the present tutorial, the following tutorials guide you to use high level functionalities:\n",
                 "- [lava-dl](https://github.com/lava-nc/lava-dl) for deep learning applications\n",
                 "- [lava-optimization](https://github.com/lava-nc/lava-optimization) for constraint optimization\n",
-                "- [lava-dnf](https://github.com/lava-nc/lava-dnf) for Dynamic Neural Fields"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "47e4bb81",
-            "metadata": {},
-            "source": [
-                "## 1. Usage of the Process Library"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "910bc90a",
-            "metadata": {},
-            "source": [
+                "- [lava-dnf](https://github.com/lava-nc/lava-dnf) for Dynamic Neural Fields\n",
+                "\n",
+                "## 1. Usage of the Process Library\n",
+                "\n",
                 "In this section, we will use a simple 2-layered feed-forward network of LIF neurons executed on CPU as canonical example. \n",
                 "\n",
                 "The fundamental building block in the Lava architecture is the `Process`. A `Process` describes a functional group, such as a population of `LIF` neurons, which runs asynchronously and parallel and communicates via `Channels`. A `Process` can take different forms and does not necessarily be a population of neurons, for example it could be a complete network, program code or the interface to a sensor (see figure below).\n",
                 "\n",
                 "![process_overview.png](https://raw.githubusercontent.com/lava-nc/lava-docs/dev/walk-through-tutorial/_static/images/tutorial00/proc_overview.png)\n",
                 "\n",
                 "For convenience, Lava provides a growing Process Library in which many commonly used `Processes` are publicly available.\n",
@@ -62,63 +45,61 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "f5f304d1",
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "\u001b[0;31mInit signature:\u001b[0m \u001b[0mLIF\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;34m*\u001b[0m\u001b[0margs\u001b[0m\u001b[0;34m,\u001b[0m \u001b[0;34m**\u001b[0m\u001b[0mkwargs\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n",
-                            "\u001b[0;31mDocstring:\u001b[0m     \n",
-                            "Leaky-Integrate-and-Fire (LIF) neural Process.\n",
-                            "\n",
-                            "LIF dynamics abstracts to:\n",
-                            "u[t] = u[t-1] * (1-du) + a_in         # neuron current\n",
-                            "v[t] = v[t-1] * (1-dv) + u[t] + bias  # neuron voltage\n",
-                            "s_out = v[t] > vth                    # spike if threshold is exceeded\n",
-                            "v[t] = 0                              # reset at spike\n",
-                            "\n",
-                            "Parameters\n",
-                            "----------\n",
-                            "shape : tuple(int)\n",
-                            "    Number and topology of LIF neurons.\n",
-                            "u : float, list, numpy.ndarray, optional\n",
-                            "    Initial value of the neurons' current.\n",
-                            "v : float, list, numpy.ndarray, optional\n",
-                            "    Initial value of the neurons' voltage (membrane potential).\n",
-                            "du : float, optional\n",
-                            "    Inverse of decay time-constant for current decay. Currently, only a\n",
-                            "    single decay can be set for the entire population of neurons.\n",
-                            "dv : float, optional\n",
-                            "    Inverse of decay time-constant for voltage decay. Currently, only a\n",
-                            "    single decay can be set for the entire population of neurons.\n",
-                            "bias_mant : float, list, numpy.ndarray, optional\n",
-                            "    Mantissa part of neuron bias.\n",
-                            "bias_exp : float, list, numpy.ndarray, optional\n",
-                            "    Exponent part of neuron bias, if needed. Mostly for fixed point\n",
-                            "    implementations. Ignored for floating point implementations.\n",
-                            "vth : float, optional\n",
-                            "    Neuron threshold voltage, exceeding which, the neuron will spike.\n",
-                            "    Currently, only a single threshold can be set for the entire\n",
-                            "    population of neurons.\n",
-                            "\n",
-                            "Example\n",
-                            "-------\n",
-                            ">>> lif = LIF(shape=(200, 15), du=10, dv=5)\n",
-                            "This will create 200x15 LIF neurons that all have the same current decay\n",
-                            "of 10 and voltage decay of 5.\n",
-                            "\u001b[0;31mInit docstring:\u001b[0m Initializes a new Process.\n",
-                            "\u001b[0;31mFile:\u001b[0m           ~/lava-nc/lava/src/lava/proc/lif/process.py\n",
-                            "\u001b[0;31mType:\u001b[0m           ProcessPostInitCaller\n",
-                            "\u001b[0;31mSubclasses:\u001b[0m     LIFReset\n"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\u001b[0;31mInit signature:\u001b[0m \u001b[0mLIF\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;34m*\u001b[0m\u001b[0margs\u001b[0m\u001b[0;34m,\u001b[0m \u001b[0;34m**\u001b[0m\u001b[0mkwargs\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n",
+                        "\u001b[0;31mDocstring:\u001b[0m     \n",
+                        "Leaky-Integrate-and-Fire (LIF) neural Process.\n",
+                        "\n",
+                        "LIF dynamics abstracts to:\n",
+                        "u[t] = u[t-1] * (1-du) + a_in         # neuron current\n",
+                        "v[t] = v[t-1] * (1-dv) + u[t] + bias  # neuron voltage\n",
+                        "s_out = v[t] > vth                    # spike if threshold is exceeded\n",
+                        "v[t] = 0                              # reset at spike\n",
+                        "\n",
+                        "Parameters\n",
+                        "----------\n",
+                        "shape : tuple(int)\n",
+                        "    Number and topology of LIF neurons.\n",
+                        "u : float, list, numpy.ndarray, optional\n",
+                        "    Initial value of the neurons' current.\n",
+                        "v : float, list, numpy.ndarray, optional\n",
+                        "    Initial value of the neurons' voltage (membrane potential).\n",
+                        "du : float, optional\n",
+                        "    Inverse of decay time-constant for current decay. Currently, only a\n",
+                        "    single decay can be set for the entire population of neurons.\n",
+                        "dv : float, optional\n",
+                        "    Inverse of decay time-constant for voltage decay. Currently, only a\n",
+                        "    single decay can be set for the entire population of neurons.\n",
+                        "bias_mant : float, list, numpy.ndarray, optional\n",
+                        "    Mantissa part of neuron bias.\n",
+                        "bias_exp : float, list, numpy.ndarray, optional\n",
+                        "    Exponent part of neuron bias, if needed. Mostly for fixed point\n",
+                        "    implementations. Ignored for floating point implementations.\n",
+                        "vth : float, optional\n",
+                        "    Neuron threshold voltage, exceeding which, the neuron will spike.\n",
+                        "    Currently, only a single threshold can be set for the entire\n",
+                        "    population of neurons.\n",
+                        "\n",
+                        "Example\n",
+                        "-------\n",
+                        ">>> lif = LIF(shape=(200, 15), du=10, dv=5)\n",
+                        "This will create 200x15 LIF neurons that all have the same current decay\n",
+                        "of 10 and voltage decay of 5.\n",
+                        "\u001b[0;31mInit docstring:\u001b[0m Initializes a new Process.\n",
+                        "\u001b[0;31mFile:\u001b[0m           ~/Documents/lava/src/lava/proc/lif/process.py\n",
+                        "\u001b[0;31mType:\u001b[0m           ProcessPostInitCaller\n",
+                        "\u001b[0;31mSubclasses:\u001b[0m     LIFReset"
+                    ]
                 }
             ],
             "source": [
                 "from lava.proc.lif.process import LIF\n",
                 "from lava.proc.dense.process import Dense\n",
                 "\n",
                 "LIF?"
@@ -159,14 +140,15 @@
                 "           dv=0.1,                              # Inverse membrane time-constant\n",
                 "           du=0.1,                              # Inverse synaptic time-constant\n",
                 "           bias_mant=0.,                        # Bias added to the membrane voltage in every timestep\n",
                 "           name='lif2')"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "1fbfed43",
             "metadata": {},
             "source": [
                 "As you can see, we can either specify parameters with scalars, then all units share the same initial value for this parameter, or with a tuple (or list, or numpy array) to set the parameter individually per unit.\n",
                 "\n",
                 "\n",
@@ -182,93 +164,44 @@
                 "\n",
                 "![process.png](https://raw.githubusercontent.com/lava-nc/lava-docs/dev/walk-through-tutorial/_static/images/tutorial00/proc.png)\n",
                 "\n",
                 "The `Vars` are used to store internal states of the `Process` while the `Ports` are used to define the connectivity between the `Processes`. Note that a `Process` only defines the `Vars` and `Ports` but not the behavior. This is done separately in a `ProcessModel`. To separate the interface from the behavioral implementation has the advantage that we can define the behavior of a `Process` for multiple hardware backends using multiple `ProcessModels` without changing the interface. We will get into more detail about `ProcessModels` in the second part of this tutorial.\n",
                 "\n",
                 "### Ports and connections\n",
                 "\n",
-                "Let's take a look at the `Ports` of the `LIF` and `Dense` processes we just created.  The output `Port` of the `LIF` neuron is called `s_out`, which stands for 'spiking' output. The input `Port` is called `a_in` which stands for 'activation' input."
+                "Let's take a look at the `Ports` of the `LIF` and `Dense` processes we just created.  The output `Port` of the `LIF` neuron is called `s_out`, which stands for 'spiking' output. The input `Port` is called `a_in` which stands for 'activation' input.\n",
+                "\n",
+                "For example, we can see the size of the `Port` which is in particular important because `Ports` can only connect if their shape matches."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "3f8f656a",
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "['s_out']"
-                        ]
-                    },
-                    "execution_count": 3,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "lif1.out_ports.member_names"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "f8ed37d8",
-            "metadata": {},
-            "source": [
-                "For example, we can see the size of the `Port` which is in particular important because `Ports` can only connect if their shape matches."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 4,
-            "id": "f77b750d",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "assert(lif1.s_out.size == dense.s_in.size)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "7378d13d",
-            "metadata": {},
-            "source": [
-                "Similarly we can investigate the input port of the second `LIF` population."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 5,
-            "id": "706dc863",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "['a_in']"
-                        ]
-                    },
-                    "execution_count": 5,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Proc: lif1   Name: a_in   Size: 3\n",
+                        "Proc: lif1   Name: s_out  Size: 3\n",
+                        "Proc: lif2   Name: a_in   Size: 2\n",
+                        "Proc: lif2   Name: s_out  Size: 2\n",
+                        "Proc: dense  Name: s_in   Size: 3\n",
+                        "Proc: dense  Name: a_out  Size: 2\n"
+                    ]
                 }
             ],
             "source": [
-                "lif2.in_ports.member_names"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
-            "id": "521bf370",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "assert(dense.a_out.size == lif2.a_in.size)"
+                "for proc in [lif1, lif2, dense]:\n",
+                "    for port in proc.in_ports:\n",
+                "        print(f'Proc: {proc.name:<5}  Name: {port.name:<5}  Size: {port.size}')\n",
+                "    for port in proc.out_ports:\n",
+                "        print(f'Proc: {proc.name:<5}  Name: {port.name:<5}  Size: {port.size}')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1c5da64b",
             "metadata": {},
             "source": [
@@ -277,187 +210,137 @@
                 "![process_comm.png](https://raw.githubusercontent.com/lava-nc/lava-docs/dev/walk-through-tutorial/_static/images/tutorial00/procs.png)\n",
                 "\n",
                 "As can be seen in the figure above, by `connecting` two processes, a `Channel` between them is created which means that messages between those two `Processes` can be exchanged."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 4,
             "id": "657063e9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Connect the OutPort of lif1 to the InPort of dense\n",
                 "lif1.s_out.connect(dense.s_in)\n",
-                "\n",
-                "# Connect the OutPort of dense to the InPort of lif2\n",
                 "dense.a_out.connect(lif2.a_in)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "7f0add01",
             "metadata": {},
             "source": [
                 "### Variables\n",
                 "\n",
-                "Similar to the `Ports`, we can investigate the `Vars` of a `Process`."
+                "Similar to the `Ports`, we can investigate the `Vars` of a `Process`.\n",
+                "\n",
+                "`Vars` are also accessible as member variables. We can print details of a specific `Var` to see the shape, initial value and current value. The `shareable` attribute controls whether a `Var` can be manipulated via remote memory access. Learn more about about this topic in the [remote memory access tutorial](https://github.com/lava-nc/lava/blob/main/tutorials/in_depth/tutorial07_remote_memory_access.ipynb)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 5,
             "id": "d6be4fa0",
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "['bias_exp', 'bias_mant', 'du', 'dv', 'u', 'v', 'vth']"
-                        ]
-                    },
-                    "execution_count": 8,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Var: bias_exp   Shape: (3,)  Init: 0\n",
+                        "Var: bias_mant  Shape: (3,)  Init: (1.1, 1.2, 1.3)\n",
+                        "Var: du         Shape: (1,)  Init: 0.1\n",
+                        "Var: dv         Shape: (1,)  Init: 0.1\n",
+                        "Var: u          Shape: (3,)  Init: 0\n",
+                        "Var: v          Shape: (3,)  Init: 0\n",
+                        "Var: vth        Shape: (1,)  Init: 10.0\n"
+                    ]
                 }
             ],
             "source": [
-                "lif1.vars.member_names"
+                "for var in lif1.vars:\n",
+                "    print(f'Var: {var.name:<9}  Shape: {var.shape}  Init: {var.init}')"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "971d5ed7",
             "metadata": {},
-            "source": [
-                "`Vars` are also accessible as member variables. We can print details of a specific `Var` to see the shape, initial value and current value. The `shareable` attribute controls whether a `Var` can be manipulated via remote memory access. Learn more about about this topic in the [remote memory access tutorial](https://github.com/lava-nc/lava/blob/main/tutorials/in_depth/tutorial07_remote_memory_access.ipynb)."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 9,
-            "id": "46c18b1f",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "Variable: v\n",
-                            "    shape: (3,)\n",
-                            "    init: 0\n",
-                            "    shareable: True\n",
-                            "    value: 0"
-                        ]
-                    },
-                    "execution_count": 9,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "lif1.v"
-            ]
+            "source": []
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "7574279a",
             "metadata": {},
             "source": [
-                "We can take a look at the random weights of `Dense` by calling the `get` function."
+                "We can take a look at the random weights of `Dense` by calling the `get` function.\n",
+                "\n",
+                "<div class=\"alert alert-block alert-info\">\n",
+                "<b>Note: </b> There is also a `set` function available to change the value of a `Var` after the network was executed.\n",
+                "</div>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 6,
             "id": "e60c16db",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([[0.48667088, 0.24619592, 0.89903799],\n",
-                            "       [0.96371252, 0.58821522, 0.37490556]])"
+                            "array([[0.39348157, 0.11634913, 0.17421253],\n",
+                            "       [0.51148951, 0.9046173 , 0.04863679]])"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dense.weights.get()"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "6afa9b38",
-            "metadata": {},
-            "source": [
-                "<div class=\"alert alert-block alert-info\">\n",
-                "<b>Note: </b> There is also a `set` function available to change the value of a `Var` after the network was executed.\n",
-                "</div>"
-            ]
-        },
-        {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "49a7f22e",
             "metadata": {},
             "source": [
                 "### Record internal Vars over time\n",
                 "\n",
                 "In order to record the evolution of the internal `Vars` over time, we need a `Monitor`.\n",
-                "For this example, we want to record the membrane potential of both `LIF` Processes, hence we need two `Monitors`."
+                "For this example, we want to record the membrane potential of both `LIF` Processes, hence we need two `Monitors`.\n",
+                "\n",
+                "We can define the `Var` that a `Monitor` should record, as well as the recording duration, using the `probe` function."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 7,
             "id": "635bf66b",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lava.proc.monitor.process import Monitor\n",
                 "\n",
                 "monitor_lif1 = Monitor()\n",
-                "monitor_lif2 = Monitor()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "05dc0a83",
-            "metadata": {},
-            "source": [
-                "We can define the `Var` that a `Monitor` should record, as well as the recording duration, using the `probe` function."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 12,
-            "id": "ef93825c",
-            "metadata": {},
-            "outputs": [],
-            "source": [
+                "monitor_lif2 = Monitor()\n",
+                "\n",
                 "num_steps = 100\n",
                 "\n",
                 "monitor_lif1.probe(lif1.v, num_steps)\n",
                 "monitor_lif2.probe(lif2.v, num_steps)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "84a02b97",
-            "metadata": {},
-            "source": [
-                "<div class=\"alert alert-block alert-info\">\n",
-                "<b>Note: </b> Currently, the `Monitor` can only record a single `Var` per `Process` and supports only CPU. This functionality will be extended in future releases.\n",
-                "</div>"
-            ]
-        },
-        {
-            "cell_type": "markdown",
             "id": "ce0c6495",
             "metadata": {},
             "source": [
                 "### Execution\n",
                 "\n",
                 "Now, that we finished to set up the network and recording `Processes`, we can execute the network by simply calling the `run` function of one of the `Processes`.\n",
                 "\n",
@@ -472,39 +355,40 @@
                 "#### Run Conditions\n",
                 "\n",
                 "Let's investigate the different possibilities for `RunConditions`. One option is `RunContinuous` which executes the network continuously and non-blocking until `pause` or `stop` is called."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 8,
             "id": "0cf86c34",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lava.magma.core.run_conditions import RunContinuous\n",
+                "\n",
                 "run_condition = RunContinuous()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "865e2ca9",
             "metadata": {},
             "source": [
                 "The second option is `RunSteps`, which allows you to define an exact amount of time steps the network should run."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 9,
             "id": "91fbce5e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from lava.magma.core.run_conditions import RunSteps, RunContinuous\n",
+                "from lava.magma.core.run_conditions import RunSteps\n",
                 "\n",
                 "run_condition = RunSteps(num_steps=num_steps)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2366d304",
@@ -519,15 +403,15 @@
                 "For example, we could run the network on the Loihi1 processor using the `Loihi1HwCfg`, on Loihi2 using the `Loihi2HwCfg`, or on CPU using the `Loihi1SimCfg`. The compiler and runtime then automatically select the correct `ProcessModels` such that the `RunConfig` can be fulfilled.\n",
                 "\n",
                 "For this section of the tutorial, we will run our network on CPU, later we will show how to run the same network on the Loihi2 processor."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 10,
             "id": "14c301f7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lava.magma.core.run_configs import Loihi1SimCfg\n",
                 "\n",
                 "run_cfg = Loihi1SimCfg(select_tag=\"floating_pt\")"
@@ -541,15 +425,15 @@
                 "#### Execute\n",
                 "\n",
                 "Finally, we can simply call the `run` function of the second `LIF` process and provide the `RunConfig` and `RunCondition`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 11,
             "id": "331f71b7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "lif2.run(condition=run_condition, run_cfg=run_cfg)"
             ]
         },
@@ -561,15 +445,15 @@
                 "### Retrieve recorded data\n",
                 "\n",
                 "After the simulation has stopped, we can call `get_data` on the two monitors to retrieve the recorded membrane potentials."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 12,
             "id": "582215cd",
             "metadata": {},
             "outputs": [],
             "source": [
                 "data_lif1 = monitor_lif1.get_data()\n",
                 "data_lif2 = monitor_lif2.get_data()"
             ]
@@ -580,23 +464,23 @@
             "metadata": {},
             "source": [
                 "Alternatively, we can also use the provided `plot` functionality of the `Monitor`, to plot the recorded data. As we can see, the bias of the first `LIF` population drives the membrane potential to the threshold which generates output spikes. Those output spikes are passed through the `Dense` layer as input to the second `LIF` population."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 13,
             "id": "32f48b10",
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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fvDjjn4mERERUbbc6/NcFgqFcOGFF2Lz5s3a12RZxubNmzOeJhMRERER2YXXpERERESF8XRGIwDcdtttWLt2LZYvX44VK1bge9/7HsbGxrSOf0REREREduM1KREREVF+ng80fu5zn8OJEydw5513ore3F+eddx6eeuqpGcW4iYiIiIjswmtSIiIiovw83QzGCiyeTkREROWO1zPljfNHRERE5a7Q6xlP12gkIiIiIiIiIiKi8sBAIxEREREREREREZWMgUYiIiIiIiIiIiIqGQONREREREREREREVDIGGomIiIiIiIiIiKhkDDQSERERERERERFRyRhoJCIiIiIiIiIiopIx0EhEREREREREREQlY6CRiIiIiIiIiIiISsZAIxEREREREREREZUs4PYG2E0IAQAYHh52eUuIiIiIZke9jlGva6i88HqUiIiIyl2h16NzPtA4MjICAJg/f77LW0JERERUmpGREdTX17u9GVQkXo8SERHRXJHvelQSc/zRuCzLOHr0KGprayFJkm2fMzw8jPnz5+Pw4cOoq6uz7XOoeJwbb+P8eBfnxts4P95lx9wIITAyMoKOjg74fKx8U254PUqcG2/j/HgX58bbOD/e5eb16JzPaPT5fOjq6nLs8+rq6niAeRTnxts4P97FufE2zo93WT03zGQsX7weJRXnxts4P97FufE2zo93uXE9ykfiREREREREREREVDIGGomIiIiIiIiIiKhkDDRaJBwO46677kI4HHZ7UygL58bbOD/exbnxNs6Pd3FuyC3c97yLc+NtnB/v4tx4G+fHu9ycmznfDIaIiIiIiIiIiIjsx4xGIiIiIiIiIiIiKhkDjURERERERERERFQyBhqJiIiIiIiIiIioZAw0EhERERERERERUckYaLTAgw8+iIULF6KqqgoXXXQRXnrpJbc3qeJs2LAB73vf+1BbW4u2tjZ84hOfwN69ezNeMzk5iXXr1qG5uRnRaBSf/vSncezYMZe2uHLde++9kCQJ69ev177GuXHXkSNH8PnPfx7Nzc2orq7G0qVL8fLLL2vfF0LgzjvvxLx581BdXY1Vq1bhnXfecXGLK0cymcQdd9yBRYsWobq6Gqeccgruuece6Pu4cX6c8fzzz+Oqq65CR0cHJEnCb3/724zvFzIP/f39WLNmDerq6tDQ0IAvfvGLGB0ddfB/QXMZ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izvuuEPEYjERDofFhz/8YbF3716XtrayDA8Pi1tuuUV0d3eLqqoqsXjxYvF3f/d3YmpqSnsN58cZzz77rOHPmbVr1wohCpuHkydPitWrV4toNCrq6urEddddJ0ZGRlz439BcxOtRb+A1aXnhNam38JrUm3g96i3lcE0qCSGENbmRREREREREREREVKlYo5GIiIiIiIiIiIhKxkAjERERERERERERlYyBRiIiIiIiIiIiIioZA41ERERERERERERUMgYaiYiIiIiIiIiIqGQMNBIREREREREREVHJGGgkIiIiIiIiIiKikjHQSERERERERERERCVjoJGI5rxrr70Wn/jEJ9zeDCIiIiKqULweJaJKEXB7A4iISiFJUs7v33XXXfj+978PIYRDW1SY5557DpdddhkGBgbQ0NDg9uYQERER0SzxepSIKI2BRiIqaz09PdqfH3vsMdx5553Yu3ev9rVoNIpoNOrGphERERFRBeD1KBFRGpdOE1FZa29v137V19dDkqSMr0Wj0RlLVf7iL/4CN998M9avX4/GxkbEYjE89NBDGBsbw3XXXYfa2lqceuqpePLJJzM+a9euXfjoRz+KaDSKWCyGa665Bn19fabbdvDgQVx11VVobGxETU0Nzj77bPzHf/wH3n33XVx22WUAgMbGRkiShGuvvRYAIMsyNmzYgEWLFqG6uhrLli3DL3/5S+09n3vuOUiShE2bNuHcc89FVVUV3v/+92PXrl3WDSoRERERFYzXo7weJaI0BhqJqCI9/PDDaGlpwUsvvYSbb74ZN954Iz7zmc/gAx/4AHbu3InLL78c11xzDcbHxwEAg4OD+NCHPoTzzz8fL7/8Mp566ikcO3YMn/3sZ00/Y926dZiamsLzzz+PN954A/fddx+i0Sjmz5+PX/3qVwCAvXv3oqenB9///vcBABs2bMCPf/xjbNy4Ebt378att96Kz3/+89iyZUvGe3/lK1/B/fffj+3bt6O1tRVXXXUVpqenbRotIiIiIrIar0eJaE4SRERzxI9+9CNRX18/4+tr164VH//4x7W/X3rppeKSSy7R/p5IJERNTY245pprtK/19PQIAGLr1q1CCCHuuececfnll2e87+HDhwUAsXfvXsPtWbp0qfjGN75h+L1nn31WABADAwPa1yYnJ0UkEhF/+tOfMl77xS9+UaxevTrj3z366KPa90+ePCmqq6vFY489ZvhZREREROQMXo/yepSo0rFGIxFVpHPPPVf7s9/vR3NzM5YuXap9LRaLAQCOHz8OAHjttdfw7LPPGtbX2bdvH04//fQZX//Sl76EG2+8EX/84x+xatUqfPrTn8743Gx//vOfMT4+jo985CMZX4/H4zj//PMzvrZy5Urtz01NTTjjjDPw5ptv5vovExEREZGH8HqUiOYiBhqJqCIFg8GMv0uSlPE1tXugLMsAgNHRUVx11VW47777ZrzXvHnzDD/jr/7qr3DFFVdg06ZN+OMf/4gNGzbg/vvvx80332z4+tHRUQDApk2b0NnZmfG9cDhc4P+MiIiIiMoBr0eJaC5ioJGIqAAXXHABfvWrX2HhwoUIBAo/dc6fPx833HADbrjhBnzta1/DQw89hJtvvhmhUAgAkEwmtdeeddZZCIfDOHToEC699NKc7/viiy+iu7sbADAwMIC3334bZ5555iz+Z0RERERUDng9SkTlgM1giIgKsG7dOvT392P16tXYvn079u3bhz/84Q+47rrrMi7O9NavX48//OEPOHDgAHbu3Ilnn31Wu/hasGABJEnCE088gRMnTmB0dBS1tbX48pe/jFtvvRUPP/ww9u3bh507d+KBBx7Aww8/nPHe3/zmN7F582bs2rUL1157LVpaWjI6GRIRERHR3MLrUSIqBww0EhEVoKOjA//1X/+FZDKJyy+/HEuXLsX69evR0NAAn8/4VJpMJrFu3TqceeaZuPLKK3H66afjn/7pnwAAnZ2duPvuu3H77bcjFovhpptuAgDcc889uOOOO7Bhwwbt323atAmLFi3KeO97770Xt9xyCy688EL09vbi8ccf155KExEREdHcw+tRIioHkhBCuL0RRERUmOeeew6XXXYZBgYG0NDQ4PbmEBEREVGF4fUoEeXCjEYiIiIiIiIiIiIqGQONREREREREREREVDIunSYiIiIiIiIiIqKSMaORiIiIiIiIiIiISsZAIxEREREREREREZWMgUYiIiIiIiIiIiIqGQONREREREREREREVDIGGomIiIiIiIiIiKhkDDQSERERERERERFRyRhoJCIiIiIiIiIiopIx0EhEREREREREREQl+/8B4AJoLz0rWzsAAAAASUVORK5CYII=",
                         "text/plain": [
                             "<Figure size 1600x500 with 2 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -613,24 +497,25 @@
                 "\n",
                 "# Plot the recorded data\n",
                 "monitor_lif1.plot(ax0, lif1.v)\n",
                 "monitor_lif2.plot(ax1, lif2.v)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "cf5fcea8",
             "metadata": {},
             "source": [
-                "As a last step we can stop the runtime by calling the `stop` function. `Stop` will terminate the `Runtime` and all states will be lost."
+                "As a last step we must stop the runtime by calling the `stop` function. `Stop` will terminate the `Runtime` and all states will be lost."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 14,
             "id": "0ddcd735",
             "metadata": {},
             "outputs": [],
             "source": [
                 "lif2.stop()"
             ]
         },
@@ -674,15 +559,15 @@
                 "The example of the previous section implemented a bias driven LIF-Dense-LIF network. One crucial aspect which is missing this example, is the input/output interaction with sensors and actuators. Commonly used sensors would be Dynamic Vision Sensors or artificial cochleas, but for demonstration purposes we will implement a simple `SpikeGenerator`. The purpose of the `SpikeGenerator` is to output random spikes to drive the LIF-Dense-LIF network. \n",
                 "\n",
                 "Let's start by importing the necessary classes from Lava."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 15,
             "id": "656ac8dc",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lava.magma.core.process.process import AbstractProcess\n",
                 "from lava.magma.core.process.variable import Var\n",
                 "from lava.magma.core.process.ports.ports import OutPort"
@@ -694,15 +579,15 @@
             "metadata": {},
             "source": [
                 "All `Processes` in Lava inherit from a common base class called `AbstractProcess`. Additionally, we need `Var` for storing the spike probability and `OutPort` to define the output connections for our `SpikeGenerator`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 16,
             "id": "00bde8ce",
             "metadata": {},
             "outputs": [],
             "source": [
                 "class SpikeGenerator(AbstractProcess):\n",
                 "    \"\"\"Spike generator process provides spikes to subsequent Processes.\n",
                 "\n",
@@ -740,59 +625,47 @@
                 "So, let's go ahead and define the behavior of the `SpikeGenerator` on a CPU in Python. Later in this tutorial we will show how to implement the same behavior on an embedded CPU in C and how to implement the behavior of a `LIF` process on a Loihi2 neuro-core.\n",
                 "\n",
                 "We first import all necessary classes from Lava."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 17,
             "id": "c68411dc",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lava.magma.core.model.py.model import PyLoihiProcessModel\n",
                 "from lava.magma.core.resources import CPU\n",
                 "from lava.magma.core.decorator import implements, requires\n",
                 "from lava.magma.core.sync.protocols.loihi_protocol import LoihiProtocol\n",
                 "from lava.magma.core.model.py.type import LavaPyType\n",
                 "from lava.magma.core.model.py.ports import PyOutPort"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "524df362",
             "metadata": {},
             "source": [
                 "All `ProcessModels` defined to run on CPU are written in Python and inherit from the common class called `PyLoihiProcessModel`. Further, we use the decorators `requires` and `implements` to define which computational resources (i.e. CPU, GPU, Loihi1NeuroCore, Loihi2NeuroCore) are required to execute this `ProcessModel` and which `Process` it implements. Finally, we need to specify the types of `Vars` and `Ports` in our `SpikeGenerator` using `LavaPyType` and `PyOutPort`.\n",
-                "\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "6cad5b03",
-            "metadata": {},
-            "source": [
+                "\n",
                 "<div class=\"alert alert-block alert-info\">\n",
                 "<b>Note: </b> It is important to mention that the `ProcessModel` needs to implement the exact same Vars and Ports of the parent process using the same class attribute names.\n",
-                "</div>"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "8d45cc48",
-            "metadata": {},
-            "source": [
+                "</div>\n",
+                "\n",
                 "Additionally, we define that our `PySpikeGeneratorModel` follows the `LoihiProtocol`. The `LoihiProtocol` defines that the execution of a model follows a specific sequence of phases. For example, there is the *spiking phase* (`run_spk`) in which input spikes are received, internal `Vars` are updated and output spikes are sent. There are other phases such as the *learning phase* (`run_lrn`) in which online learning takes place, or the *post management phase* (`run_post_mgmt`) in which memory content is updated. As the `SpikeGenerator` basically just sends out spikes, the correct place to implement its behavior is the `run_spk` phase. \n",
                 "\n",
                 "To implement the behavior, we need to have access to the global simulation time. We can easily access the simulation time with `self.time_step` and use that to index the `spike_data` and send out the corresponding spikes through the `OutPort`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 18,
             "id": "068cb965",
             "metadata": {},
             "outputs": [],
             "source": [
                 "@implements(proc=SpikeGenerator, protocol=LoihiProtocol)\n",
                 "@requires(CPU)\n",
                 "class PySpikeGeneratorModel(PyLoihiProcessModel):\n",
@@ -805,34 +678,29 @@
                 "        spike_data = np.random.choice([0, 1], p=[1 - self.spike_prob/100, self.spike_prob/100], size=self.s_out.shape[0])\n",
                 "        \n",
                 "        # Send spikes\n",
                 "        self.s_out.send(spike_data)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "642ad797",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-block alert-info\">\n",
                 "<b>Note: </b> For the `SpikeGenerator` we only needed an `OutPort` which provides the `send` function to send data. For the `InPort` the corresponding function to receive data is called `recv`.\n",
-                "</div>"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "5b61fee8",
-            "metadata": {},
-            "source": [
+                "</div>\n",
+                "\n",
                 "Next, we want to redefine our network as in the example before with the exception that we turn off all biases."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 19,
             "id": "069e687d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Create processes\n",
                 "lif1 = LIF(shape=(3, ),                         # Number of units in this process\n",
                 "           vth=10.,                             # Membrane threshold\n",
@@ -877,15 +745,15 @@
                 "\n",
                 "To define the connectivity between the `SpikeGenerator` and the first `LIF` population, we us another `Dense` Layer.\n",
                 "Now, we can connect its `OutPort` to the `InPort` of the `Dense` layer and the `OutPort` of the `Dense` layer to the `InPort` of the first `LIF` population.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 20,
             "id": "4e1a6b58",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Instantiate SpikeGenerator\n",
                 "spike_gen = SpikeGenerator(shape=(lif1.a_in.shape[0], ), spike_prob=7)\n",
                 "\n",
@@ -907,15 +775,15 @@
                 "### Execute and plot\n",
                 "\n",
                 "Now that our network is complete, we can execute it the same way as before using the `RunCondition` and `RunConfig` we created in the previous example."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 21,
             "id": "af9da307",
             "metadata": {},
             "outputs": [],
             "source": [
                 "lif2.run(condition=run_condition, run_cfg=run_cfg)"
             ]
         },
@@ -925,21 +793,21 @@
             "metadata": {},
             "source": [
                 "And now, we can retrieve the recorded data and plot the membrane potentials of the two `LIF` populations."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 22,
             "id": "7cbc2b21",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAABRoAAAHWCAYAAAAYQDX3AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/NK7nSAAAACXBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOzdd3hUBdbH8e+UdFIoqST03juKoiAgoGJv2OuuvaDriq+6dnTXrtgLlrWwFuxYEER6772HkISEkN4z8/5xMwmRljIzdyb5fZ4nz1wmd+6cKCSTM6dYnE6nExEREREREREREZEGsJodgIiIiIiIiIiIiPg/JRpFRERERERERESkwZRoFBERERERERERkQZTolFEREREREREREQaTIlGERERERERERERaTAlGkVERERERERERKTBlGgUERERERERERGRBlOiUURERERERERERBpMiUYRERERERERERFpMCUaRUSOYNq0aVgsFnbt2gXAiBEjGDFiRI1z0tPTufDCC2nZsiUWi4UXX3zR63GKiIiISOOl16Qi4m+UaBQRqae7776bn3/+mcmTJ/PRRx8xbtw4AJ588knOPvtsYmNjsVgsPPLII+YGKiIiIiKN1pFek27atIn77ruPfv36ER4eTnx8PGeeeSbLli0zO1wRaeTsZgcgIuIPfvnll8Pu+/333znnnHO49957a9z/4IMPEhcXR//+/fn555+9FaKIiIiINHK1fU1677338u6773LBBRdwyy23kJOTw5tvvskJJ5zAzJkzGT16tDfDFpEmRIlGEZFaCAwMPOy+/fv3ExUVddj9O3fupF27dmRmZhIdHe2F6ERERESkKajta9KJEyfyyCOP0KxZs6r7rrvuOrp3784jjzyiRKOIeIxap0VEauHQeTiuWTlOp5OpU6disViwWCxV57Zr186cIEVERESkUavta9KBAwfWSDICtGzZkuHDh7Nx40Zvhy0iTYgSjSIidXTKKafw0UcfATBmzBg++uijqj+LiIiIiHhDfV6TpqWl0apVK2+EJyJNlFqnRUTqqEOHDnTo0IErr7ySLl26cMUVV5gdkoiIiIg0MXV9Tfrnn3+ycOFCHnzwQS9FKCJNkSoaRURERERERBqx/fv3c9lll9G+fXvuu+8+s8MRkUZMFY0iIiIiIiIijVRBQQFnnXUWeXl5zJs377DZjSIi7qREo4iIiIiIiEgjVFpayvnnn8+aNWv4+eef6dWrl9khiUgjp0SjiIiIiIiISCPjcDi46qqrmDVrFtOnT+fUU081OyQRaQKUaBQRERERERFpZG6//XY+//xz3nzzTc4//3yzwxGRJkKJRhERN/voo4/YvXs3hYWFAMydO5cnnngCgCuvvJK2bduaGZ6IiIiINHIvvvgir732GieeeCKhoaF8/PHHNT5/3nnnERYWZlJ0ItKYKdEoIuJm7777Ln/88UfVn2fPns3s2bMBOPnkk5VoFBERERGPWrVqFQALFy5k4cKFh31+586dSjSKiEdYnE6n0+wgRERERERERERExL9ZzQ5ARERERERERERE/J8SjSIiIiIiIiIiItJgSjSKiIiIiIiIiIhIgynRKCIiIiIiIiIiIg2mRKOIiIiIiIiIiIg0mBKNIiIiIiIiIiIi0mB2swPwNIfDwb59+wgPD8disZgdjoiIiEidOZ1O8vLySEhIwGrV+8T+Rq9HRURExN/V9vVoo0807tu3j6SkJLPDEBEREWmw5ORkEhMTzQ5D6kivR0VERKSxON7r0UafaAwPDweM/xAREREmRyMiIiJSd7m5uSQlJVW9rhH/otejIiIi4u9q+3q00ScaXe0pERERemEnIiIifk1tt/5Jr0dFRESksTje61EN+REREREREREREZEGU6JRREREREREREREGkyJRhEREREREREREWkwJRpFRERERERERESkwZRoFBERERERERERkQZTolFEREREREREREQazNRE49y5c5kwYQIJCQlYLBZmzJhR4/NOp5OHH36Y+Ph4QkJCGD16NFu3bjUnWBERERERERERETkqUxONBQUF9O3bl6lTpx7x8//+9795+eWXeeONN1i8eDFhYWGMHTuW4uJiL0cqIiIiIiIiIiIix2I388nHjx/P+PHjj/g5p9PJiy++yIMPPsg555wDwIcffkhsbCwzZszg0ksv9WaoIiIiIiIiIiIicgw+O6Nx586dpKWlMXr06Kr7IiMjGTp0KAsXLjzq40pKSsjNza3xISIiIiIiIiIiIp7ls4nGtLQ0AGJjY2vcHxsbW/W5I5kyZQqRkZFVH0lJSR6NU0RERERERERERHw40VhfkydPJicnp+ojOTnZ7JBEREREREREREQaPZ9NNMbFxQGQnp5e4/709PSqzx1JUFAQERERNT5ERERERERERETEs3w20di+fXvi4uKYNWtW1X25ubksXryYE0880cTIREREGp8ZK1O4btpSDhaUmh2KiIiIiIhv2rcSvrwRPr4QFk6FzG1mR+RzTN06nZ+fz7Zt1f9Tdu7cyapVq2jRogVt2rThrrvu4oknnqBz5860b9+ehx56iISEBM4991zzghYREWlkHA4nT/+0ibTcYhbtOMD43vFmhyQiIiIi4hucTtj1J/z5POyYXX3/tl/h5wegRQfoPBZ6nA1th5kXp48wNdG4bNkyRo4cWfXnSZMmAXD11Vczbdo07rvvPgoKCvjb3/5GdnY2J598MjNnziQ4ONiskEVERBqdtSk5pOUWA1DmcJocjYiIiIiIj9j2G8yeAinLjD9bbND7IojrbSQad82HrB2w+HXj45R/wMj/A4vF3LhNZGqiccSIETidR/+FxmKx8Nhjj/HYY495MSoRERH3+nFtKvGRwfRv09zsUI7o1w3V85AdSjSKiIiIiMDWX+G/FxrHtiAYcCUMuwOatzXuG3YblOTB9tmw8TtYOx3m/gfy98OZz4PN1JSbaZrmVy0iIuIluw8UcMt/V9CmRShz7xt5/AeY4JcNaVXH5Uo0ioiIiEhTl58BM24xjntdAOOehmYxh58XFG60TPc4G9qeCD/cAys+gMIDcMG7END0OnJ9dhmMiIhIY7A9Ix+AnKIykyM5sl2ZBWxJz6/6c4XDYWI0IiIiIiImczrh29uhYD9Ed4dzph45yfhXg66Diz4AWyBs+h4+vgCKczwfr49RolFERMSD9h4sAqDCRysFD22bBlU0ioiIiEgTt/x92PKTkTC84B0ICKn9Y3ucDVd8BUERsHsevH+mUR3ZhCjRKCIi4kEplYnGch+tFHQlGl3zqjWjUURERESarMytMPMB43jUvyCuV92v0X44XPMDhMVA+lr4+u/go78LeIISjSIiIh7kyxWNB/JLWLY7C4ABlYtqVNEoIiIiIk1SeSl8eQOUF0GHEXDCLfW/VnwfuPpbsAfD9lmw5E23henrlGgUERHxoL3ZropG30vgzdq0H4cTeiZE0KZFKOCbCVEREREREY+bMwVSV0FIczj3dbA2MGUW0x1Of8I4/vVhSFvX4BD9gRKNIiIiHpRysBAwZkr7WlvyL+uNtunTe8Rhsxq9076YEBURERER8ah9K2HeC8bxhJchIsE91x18A3QZBxWV1ZJlRe65rg9TolFERMRDissqyMwvrfpzhdN3knhFpRXM22YMph7TIxZb5ZBGVTSKiIiISJOz5G3ACT3PNxa6uIvFAme/asxrzNhoVDY2cko0ioiIeIhrPqOLLyXx5m7NoLjMQWLzELrHh2OzKdEoIiIiIk1QcQ6s/9o4HnqT+6/fLNpoxQZY8hZs+cX9z+FDlGgUERHxkJTsmolGX2pLdm2bHtMjFovFgl2t0yIiIiLSFK37EsoKoVVXSBrimefoPBqG3mwcf3ML5O/3zPP4ACUaRUREPGRv5XxGl4oK30jilVc4mLWxej4jUDWjscLhMC0uERERERGvW/GhcTvgKqPV2VNGPwIxPaEgA366z3PPYzIlGkVERDzkr63T5T6SxFu2+yAHC8uICg1gcLvmAKpoFBEREZGmJ3WNsQjGGgB9L/XscwUEw3lvABajVTt5iWefzyRKNIqIiHhIyl9nNPrIMhhX2/Rp3WKw24yXAlZXRaOPVF2KiIiIiHicq5qx+1kQ1srzzxffB/pfbhz//AD4yO8H7qREo4iIiIcc1jrtI9WCv1W1TcdW3eeqaPSVZKiIiIiIiEeVFcGa6cbxgKu897wjH4SAMNi7FNZ/5b3n9RIlGkVERDzksGUwPlAtmJFXwu4DhVgscFKn6ndtbVbjJYGvJENFRERERDxqw7dQkgORbaD9CO89b0Q8nHSncfzbI1BW7L3n9gIlGkVERDygpLyC9NySGvf5QhJvzd5sADpFNyM8OKDqfs1oFBEREZEmpWoJzJVg9XJ6bNhtEB4P2XtgyZvefW4PU6JRRETEA1KzjXcmgwOsRIYYCT1fSOKt3psDQJ/EqBr32zSjUURERESaisxtsHseWKzQ7zLvP39gGIx62Die+ywUZHo/Bg9RolFERMQDXBunE5uHVlULOnxg/uHq5GwA+iVF1rjfphmNIiIiItJUrPzIuO00GiITzYmhz6UQ1wdKcmHO0+bE4AFKNIqIiHhASraxCCaxeUhVEs/sGY1Op5PVla3TfZOianyuahmMD1RdioiIiIh4TEUZrPrEOPbmEpi/slph7JPG8bL3IGOLebG4kRKNIiIiHuCqaGwdFeIzSbzkrCKyC8sItFnpFhdR43M2zWiURmDu3LlMmDCBhIQELBYLM2bMOOb511xzDRaL5bCPnj17Vp3zyCOPHPb5bt26efgrEREREY/Z8jMU7IewGOgyztxY2p8CXc8AZ4WxGKYRUKJRRETEAw5tnbbZXEk8h5khsaqymrF7QgSB9povAaqToebGKNIQBQUF9O3bl6lTp9bq/JdeeonU1NSqj+TkZFq0aMFFF11U47yePXvWOG/evHmeCF9ERES8YdMPxm2fi8EWcOxzvWH0o8asyM0/QNpas6NpMLvZAYiIiDRGKa6KxuYh2Cu32Jld0Vg1nzEx8rDPWX2kvVukIcaPH8/48eNrfX5kZCSRkdX/HmbMmMHBgwe59tpra5xnt9uJi4tzW5wiIiJiEqcTdv1pHHc8zdxYXKK7QI9zYf1X8OdzcNE0syNqEFU0ioiIeMDeg0eY0WhyonFNZUXjXzdOAz61sEbELO+++y6jR4+mbdu2Ne7funUrCQkJdOjQgcsvv5w9e/Yc8zolJSXk5ubW+BAREREfcHAX5CSDNQDanGB2NNWG32Pcrp8BmVtNDaWhlGgUERFxs7IKB2m5xQAkRoVgs1Qm8UxMNJZXOFibkgMcvggGwFZZdWl2MlTELPv27eOnn37ihhtuqHH/0KFDmTZtGjNnzuT1119n586dDB8+nLy8vKNea8qUKVXVkpGRkSQlJXk6fBEREakNVzVj64EQGGZuLIeK6wVdxgNOmPeC2dE0iBKNIiIibpaWU4zDCYF2K62aBflEReOW9HyKyxyEB9np0OrwF1W+srBGxCwffPABUVFRnHvuuTXuHz9+PBdddBF9+vRh7Nix/Pjjj2RnZzN9+vSjXmvy5Mnk5ORUfSQnJ3s4ehEREamVnZWJxvbDzY3jSE6517hd8zlkH7t7wpcp0SgiIuJmVYtgokKwWi3YbeYn8Vxt070TI6vmMR7KphmN0oQ5nU7ee+89rrzySgIDA495blRUFF26dGHbtm1HPScoKIiIiIgaHyIiImKyQ+cztvPBRGPiIGh/KjjKYf5LZkdTb0o0ioiIuJlrPmPr5iEAPlHRuLoy0XiktmmojlEVjdIU/fHHH2zbto3rr7/+uOfm5+ezfft24uPjvRCZiIiIuM2B7ZCXCrZASBpidjRHdso/jNsVH0Femrmx1JMSjSIiIm6Wkl1Z0ViZaKxuS3aYFtOq5Mr5jEdYBAOHJBq1DEb8WH5+PqtWrWLVqlUA7Ny5k1WrVlUtb5k8eTJXXXXVYY979913GTp0KL169Trsc/feey9//PEHu3btYsGCBZx33nnYbDYmTpzo0a9FRERE3GzXXOM2cQgEhJgby9G0OxmShkJFCSx81exo6kWJRhERETdztU63jjJewFgtrkSjOfEUlVawJd1YXNE3KfKI59h9oOpSpKGWLVtG//796d+/PwCTJk2if//+PPzwwwCkpqYetjE6JyeHL7/88qjVjHv37mXixIl07dqViy++mJYtW7Jo0SKio6M9+8WIiIiIe/nyfEYXiwWGV85qXPoeFGaZG0892M0OQEREpLFxtU4nNg8FqJrRWG5SReP6fTlUOJzEhAcRFxF8xHNsPlB1KdJQI0aMwHmMqtxp06Yddl9kZCSFhYVHfcxnn33mjtBERETETE4n7JpnHPvifMZDdR4DcX0gbQ0seh1O+z+zI6oTVTSKiIi4mat1unpGo/Hj1qz5h6uSswFjPqPFcvgiGAB7ZYxaBiMiIiIijU7GZijYD/ZgY+mKL7NYYPg9xvGSN6Ek39x46kiJRhERETeqcDhJzS4GDp/RaFZb8uq9rvmMR26bBqjMM+LQjEYRERERaWxc26aThoI9yNxYaqP72dCiAxTnwOpPzY6mTpRoFBERcaP03GLKHU4CbBZiwo02ZbM3Oq85zsZpOKSiUTMaRURERKSx2Vm5CMaX5zMeymqFoTcZx4vfBD8ab6REo4iIiBu5FsHER4ZUJRjNrGg8WFDK7gPG/Lk+raOOep7ZyVAREREREY9wOA6Zz3iKubHURb/LICgCDmyF7bPMjqbWlGgUERFxo5Rs1yKYkKr7rJVJPIcJSbzVldWM7VuFERkacNTzqpKhmtEoIiIiIo3J/g1QlAUBYdB6gNnR1F5QOPS/0jhe9Lq5sdSBEo0iIiJutDerchFMVHWi0cyKxjW1mM8IqmgUERERkUbKNZ+x7YlgO/ob7z5p6N/AYjUqGjM2mx1NrSjRKCIi4kaujdOJzUOr7qtO4nl/tsrqQzZOH0tVjFoGIyIiIiKNyc7KRGM7P5nPeKjm7aDrGcbx4jdMDaW2lGgUERFxI9eMxtbNza9odDqdVa3TfRKjjnmuXRWNIiIiItLYOCpgd+V8Rn9ZBPNXJ9xs3K76FAqzzI2lFpRoFBERcaO9Bw+f0Wir3Ohc4eX5h2m5xWTml2KzWuiZEHHMc21VMxr9Z6OdiIiIiMgxpa2F4hxjqUpcX7OjqZ+2J0FsbygvghUfmh3NcSnRKCIi4iYOh5N92cXAXxONxq23Kxq37y8AoG3LUIIDbMc81+5KhqqiUUREREQai6r5jMPAZjc3lvqyWKqrGpe8DRXl5sZzHEo0ioiIuElGfgmlFQ5sVgtxEcFV97uSeA4vzz/cmZkPQIdWYcc912pSMlRERERExGN2LzRu251sbhwN1esCCG0FuXth03dmR3NMSjSKiIi4iWs+Y1xEMHZb9Y9Ym0kzGrdnGBWNHaKbHfdcs5KhIiIiIiIek77WuE0YYG4cDRUQDIOvN44XvW5uLMehRKOIiIibuDZOt44KqXG/WYtWdmYaicb2tahoNCsZKiIiIiLiEcU5kL3HOI7tYW4s7jDoerAGQPJi2LfS7GiOSolGERERN8nIKwEgJiKoxv3Vi1a8m8TbUYfWaVcy1Ok0Zk2KiIiIiPi1/RuN24hECGlubizuEB4LPc4xjpe9Z24sx6BEo4iIiJu4Eo3R4TUTjdUVjd7b6FxcVlHVyl2b1mmbzVJ1rKpGEREREfF76euM28ZQzejiap9e+4VRsemDlGgUERFxk8z8Iycara5EoxfnH+7JKsTphPAgO62aBR73fJulOtGoOY0iIiIi4vfS1xu3sT3NjcOd2pwI0d2hrBBWf252NEekRKOIiIibVFU0NjtaRaP3Eng7MirbpqPDsBySRDwaV3s3qKJRRERERBqB9A3GbWwvc+NwJ4sFBl1nHC9715h75GOUaBQREXGTo7VO2yo3OntzRmNdNk5DdTIUoMLLsyRFRERERNzK6WycFY0AfS+BgFDI2AR7FpodzWGUaBQREXGTjMrW6VY+UNFYl43T8NeKRu/NkhQRERERcbvsPVCaZ2xpbtnJ7GjcKzgSel9oHC9919xYjkCJRhERETeocDg5UJlojDmsorFy67RJrdO1YbFYcOUavZkQFRERERFxO1c1Y3Q3sAWYG4snuNqnN3wD+RnmxvIXSjSKiIi4QVZBKQ6nMTalRVjN5Ss2M2Y0VlY0dmhVu9ZpAHtli7c3l9aIiIiIiLjd/kbaNu2S0B8SBoCjDFZ9bHY0NSjRKCIi4gau+YwtwwKx22r+ePV2ovFgQSnZhWUAtGsVWuvHVVVeakajiIiIiPizxjqf8VCDrzdul70PPjT6SIlGERERN8g8ynxGqJ7R6K3W6R2ZRtt0QmQwoYH2Wj/OjFmSIiIiIiJu1xQSjT3PN+Y1Zu+G7b+bHU0VJRpFRETc4Ggbp+HQikbvvNO4o3LjdPtazmd0sdm8P0tSRERERMStyorgwDbjuDEnGgNDoe9lxvEy31kKo0SjiIiIG7g2TkcfqaLRywm8+sxnBLBZVNEoIiIiIn4uYxM4HRDaEprFmh2NZw261rjdMhNy9pobSyUlGkVERNzg2BWNlUtWvJVorOPGaRczltaIiIiIiLhV+gbjNransamxMYvuCu2GG4nVtf8zOxoAaj+4SURERI7qmIlGL1cK7qysaGzfqm6JRs1oFBERERG/VzWfsZe5cXjLyAegJB86jTI7EkCJRhEREbeo3YxGzyfwKhxOdh0oBKBjdB1bp6tavH1na52IiIiISJ2krzNuY3qYG4e3tB1mdgQ1qHVaRETEDY45o9GLW6dTDhZRWu4g0G4lISqkTo+1e7nFW0RERETErZzO6kRjY14E48OUaBQREXGDzPxjVDTavFfRuCPTmM/YrmVoVSVlbblO19ZpEREREfFL+fuh8ABYrBDdzexomiSfTjRWVFTw0EMP0b59e0JCQujYsSOPP/44Tqd+ARIREd9RUl5BdmEZcOREozcrGndk1G/jNFRXNDqUaBQRERERf7S/cj5ji44QGGpuLE2UT89ofOaZZ3j99df54IMP6NmzJ8uWLePaa68lMjKSO+64w+zwREREADiQXwpAgM1CZEjAYZ+vntHo+dmHrorG9nXcOA3VcaqiUURERET8UtUiGLVNm8WnE40LFizgnHPO4cwzzwSgXbt2fPrppyxZssTkyERERKq5FsG0ahaExXJ4u7I3t067Nk53qOPGaQC7F1u8RURERETcTolG0/l06/SwYcOYNWsWW7ZsAWD16tXMmzeP8ePHH/UxJSUl5Obm1vgQERHxpGNtnAbvJvCqWqfruHEawGpRRaOIiIiI+DEtgjGdT1c03n///eTm5tKtWzdsNhsVFRU8+eSTXH755Ud9zJQpU3j00Ue9GKWIiDR1x9o4DWCrnH3o6QReYWk5qTnFQD0rGq2qaBQRERERP1VRBhmbjWMlGk3j0xWN06dP57///S+ffPIJK1as4IMPPuDZZ5/lgw8+OOpjJk+eTE5OTtVHcnKyFyMWEZGmKPN4FY1eSuC52qabhwbQPCywzo+3KdEoIiIiIv7qwHaoKIXAcIhsY3Y0TZZPJxr/8Y9/cP/993PppZfSu3dvrrzySu6++26mTJly1McEBQURERFR40NERMSTqioaj5Jo9NaSlYa0TUN1i3e5F5bWiHjC3LlzmTBhAgkJCVgsFmbMmHHM8+fMmYPFYjnsIy0trcZ5U6dOpV27dgQHBzN06FDNCxcREfFFrrbpmO5g9el0V6Pm0//lCwsLsf7lL4fNZsOhX4BERMSHHLoM5ki8VSnoqmhsX4+2aahu8VZFo/irgoIC+vbty9SpU+v0uM2bN5Oamlr1ERMTU/W5zz//nEmTJvGvf/2LFStW0LdvX8aOHcv+/fvdHb6IiIg0hBbB+ASfntE4YcIEnnzySdq0aUPPnj1ZuXIlzz//PNddd53ZoYmIiFQ53jIYbyUad2TkA9Ahup6JxsqF2VoGI/5q/Pjxx1waeDQxMTFERUUd8XPPP/88N954I9deey0Ab7zxBj/88APvvfce999//xEfU1JSQklJSdWftZxQRETEC5Ro9Ak+XdH4yiuvcOGFF3LLLbfQvXt37r33Xv7+97/z+OOPmx2aiIhIleO1TntrRuOOyorGDq3q1zrtqmh0KNEoTUy/fv2Ij49nzJgxzJ8/v+r+0tJSli9fzujRo6vus1qtjB49moULFx71elOmTCEyMrLqIykpyaPxi4iICLB/o3GrRKOpfLqiMTw8nBdffJEXX3zR7FBERESOqqqi8Tit056cfeh0OtlZNaOxfhWNdi/NkmwMKhxOlu8+yI9rU8kvKefZi/qaHZLUQ3x8PG+88QaDBg2ipKSEd955hxEjRrB48WIGDBhAZmYmFRUVxMbG1nhcbGwsmzZtOup1J0+ezKRJk6r+nJubq2SjiIiIJ5WXQu5e47hFR3NjaeJ8OtEoIiLi6wpKyiksrQCOVdHo+dmHGfkl5JWUY7FA25ah9bqGzaat08dSXuFgya4sflqbxsz1aVUJZrvVwoNndicqtO6bvsVcXbt2pWvXrlV/HjZsGNu3b+eFF17go48+qvd1g4KCCAo68vcDERER8YCcZHA6wB4CzWKOf754jBKNIiIiDZBZ2TYdGmgjLOjIP1a9sXXaVc2Y2DyEILutXtdQRePRrUvJ4cYPl5GaU1x1X3iwnTE9YjmjVzyhgXpJ1VgMGTKEefPmAdCqVStsNhvp6ek1zklPTycuLs6M8ERERORIDu4ybpu3A4vFzEiaPL0qFhERaYDjLYKB6kSj02nMP7Ra3f/iZ+/BIgDatKhfNSOAzeKqaPRci7c/2rY/j6veW0JWQSlRoQGc3iOW8b3jOaljKwLtPj3uWuph1apVxMfHAxAYGMjAgQOZNWsW5557LgAOh4NZs2Zx2223mRiliIiI1JC927ht3tbcOESJRhERkYZwJRpbHWU+I1QnGgEqnE6suD/RmJpjJBrjI0PqfY3q7dhuCalRSM4q5PJ3FpNVUEqfxEj+e8NQwoMDzA5LjiI/P59t27ZV/Xnnzp2sWrWKFi1a0KZNGyZPnkxKSgoffvghAC+++CLt27enZ8+eFBcX88477/D777/zyy+/VF1j0qRJXH311QwaNIghQ4bw4osvUlBQULWFWkRERHzAoRWNYiolGkVERBqgauP0MRKN9kMTjQ4nAfXrbD6mfZUtvQmRwfW+ht2misZDpeUUc9k7i0jPLaFLbDM+uHaIkow+btmyZYwcObLqz66FLFdffTXTpk0jNTWVPXv2VH2+tLSUe+65h5SUFEJDQ+nTpw+//fZbjWtccsklZGRk8PDDD5OWlka/fv2YOXPmYQtiRERExERKNPoMJRpFREQaoC6t0+C5+Yep2ZUVjVENr2jUjEbIKijlincXk5xVRNuWoXx8/VCah2nZi68bMWIETufR//5Omzatxp/vu+8+7rvvvuNe97bbblOrtIiIiC9TotFnKNEoIuImZRUOdmUWEGS3ERZkLAYJsluxaBhxo1abRGONisYKDyUaKysa4xtQ0Vg9o7FpJxrzisu46r3FbNufT1xEMB9fP5SYiPr/dxURERERD1Oi0Wco0Sgi0kBOp5NfN6Tz5I8b2X2gsMbn7FYLUaGBXDo4iZtGdKTZUbYSi/+qe0WjZ9qS91VWNCY0qKLRWGzS1BONz/2yhXUpubQMC+TjG4aS1IAFOyIiIiLiYUUHoTjHOI5qY24sokSjiEhDbE7L47Hv1zN/2wEAQgJsWCxQWFoBGC2omfklvDp7G58tTWbSmC5cPCgRu02bahuLzFrMaLRYLFgt4HAay2DcraCknNzicqBhFY3VMxqbbqIxJbuITxYbM/xevLQfnWKamRyRiIiIiBzTwcqN02ExEBhmbiyiRKOISH1kF5by/K9b+HjRbhxOCLRb+dvwDtw8oiNhQXYqHE4KS8spKKlg5Z6DPDNzE7sOFPLA12v5YMEuHjizO6d2iTb7yxA3qNo6fYyKRgC71UpphcMjSTzXxunwIHuDlpVoRiO8+vs2SiscnNChBSd3amV2OCIiIiJyPGqb9ilKNIqI1FFecRnnvbaAnZkFAIzvFccDZ3Sv0V5ps1oIDw4gPDiA8b3jGdU9lo8X7ealWVvZnJ7H1e8t4eJBiUw5v0+NtlrxL06ns3rr9HESjTarBSqg3AMzGvdlV85njGrYHEHXLMmmWtG450Ah/1uWDMA9p3fVfFURERERf6BEo09RolFEpA6cTif3f7WWnZkFxEcG89xFfRlWi6qnQLuV605uzwUDEnnl9628v2AX05ftpbC0ghcu6UeAWqn9Uk5RGWWVicNWzY69kdiTSTxXRWN8ZP3nMwJYLa6KRs/MkfR1L83aSrnDySldohncroXZ4YiIiIhIbSjR6FP0m62ISB18uiSZH9akYrdamHr5gFolGQ8VGRrAg2f1YOpl/QmwWfh+TSq3/ncFJeUVHopYPMnVNh0ZEkCQ3XbMc202z7UluyoaE9xW0djgkPzO9ox8vl65F4BJY7qYHI2IiIiI1JoSjT5FiUYRkVramJrLo9+tB+C+cV0Z0KZ5va81rlc8b145kEC7lV82pPP3j5ZTXKZko7+pzcZpF1tltaDDA8tg3FXRaKtaBtP0Mo0v/rYVhxNGd4+lX1KU2eGIiIiISG1VJRrbmhqGGJRoFBGphYKScm79ZAUl5Q5Gdo3mhpM7NPiap3WL5b2rBxMcYGXO5gyum7aUwtJyN0Qr3pJRi43TLlWLVjwwozE1p3JGYwM2TkN1RWNTWwazKS2X79fsA1TNKCIiIuJXHBWQY8zYVkWjb1CiUUSkFh76Zh07MgqIiwjmuYv7YXXTApeTO7fig2uHEBZoY8H2A9zwwTLKm2Lfqp+qS0WjJ2c07ss2KhoTotwzo7GpLYN54dctOJ1wRu84eiREmB2OiIiIiNRWbgo4ysEWCOHxZkcjKNEoInJcXyzfy1crUrBa4OWJ/WkRduylH3U1tENLPrphaFWy8T8/b3br9cVzXBWNrWpT0WjzzKIVp9OpisYGWJeSw8/r07FY4O7RqmYUERER8SuutumoNmA99sx08Q4lGsV3OJ2wewHMewHWTIe9y6HooNlRSRN3IL+Eh79ZBxgtlUPae2YT7YA2zfnPRX0BeHPuDn5am+qR5xH3qltFo/Ej193VgrlF5RSWGvM9Gz6j0YjR0YQSjW/O3QHAOX0T6BwbbnI0IiIiIlInWgTjc+xmByBCeSms/woWvQapqw//fEhzaNUFhvwNel0AFve0rIrUxieL91BYWkHv1pHcPKKTR5/rjN7x3Di8PW//uZN/fLGGLnHhdIxu5tHnlIap0zIYD1UL7qtcBNM8NICQwIa9i9vUKhqLSiuYtTEdgGtPam9yNCIiIiJSZ0o0+hxVNIp5CrPgj//Ai73g678bSUZ7MHQ7C9qeVD1foeggJC+GL6+HD8+BzK3mxi1NRkl5BR8u2g3ADcPbVyWKPOmf47oxtH0L8kvKuemj5RSUaDmML6vX1mk3J/HctXEaqpOhTWVG4x9b9lNYWkHrqBD6JEaaHY6IiIiI1FVV67Q2TvsKVTSKOfL3wzujIdtI4tAsDobcCAOvhbCW1eeVFkDWTtj0Pfz5POz8A14fBifdCcPvgYCG/2ItcjQ/rEklI6+E2IggzujtncHCdpuVVy7rz1kvz2Pr/nz++eUaXpnYH4sqeX1SZn22Tru7ojHbmM+YENWw+YxQnQxtKhWNP6xNA4wlMPo3JiIiIuKHDlbmFFTR6DNU0SjeV1oAn1xiJBkj28D5b8Nda+GUe2smGQECwyCuF4y4H25dBJ1GQ0UpzP0PTB1qzHQU8QCn08m783YCcNWJ7Qiwee/bZUx4MK9dPgC71cL3a1J5f/4urz231F6Fw0lWQSlQyxmNNs9UC7qzotEVY1OY0VhcVt027a03EkRERETEzdQ67XOUaBTvclTAlzfCvhXG7MUrv4Y+F4O9Flt8W3SAy7+Aiz+E8AQjUfnRebBtlufjliZnyc4s1u/LJTjAymVD2nj9+Qe1a8H/ndkdgKd+3MjG1FyvxyDHdqCgBIcTrBZqtYncUxWNqZUVjfHuqGi0emYzti/6Y0tGVdt0v6Qos8MRERERkboqyYPCTOO4uVqnfYUSjeJdP/8fbP4BbEEw8TNoVcflGhYL9DgHblsCXcZBeTF8OhG2/uaZeKXJem++Uc14/oBEmtciieQJ1wxrx+k9Yil3OLnvizWUVzT+5I8/cc1nbBEWVKv5nfaq+Yfu/f/oWgaT4I6KxiY0o/HHys3u43upbVpERETEL7napkNaQLDmbfsKJRrFexa9DotfN47Pex3anFD/awWFG5WNXc+EihL4bCJs+dk9cUqTt+dAIb9sMFoqrzupnWlxWCwWnji3FxHBdtam5PBOZSu3+Ia6LIIBsHpo/mFqTmVFY6Q7KhqNlwWNfUaj0Ta9H4DxapsWERER8U9qm/ZJSjSKd2z8HmZONo5HPwq9Lmj4Ne1BcNE06D7BmNv42eWw6ceGX1eavGkLduF0wqldoukUE25qLDERwTx0Vg8Anv91C9sz8k2NR6rVNdHoiRmNTqezKtGYEOWOrdPGbWOvaJy7JYP8knLiI4Ppr7ZpEREREf9UlWhU27QvUaJRPC9/P3z1N8AJg64zNka7iz0QLnwfepwLjjKYfqWR1BSpp7ziMqYvSwbgupPbmxyN4cKBiZzSJZrScgf3f7mmSSzq8AcZddg4DdXVgu5M4h0oKKW03IHFArER7qtobOyJxp/WGdumx/eKx1qLtncRERER8UHZ2jjti5RoFM+b/xKUFUDCABj/H2POojvZAuCCd40qSUc5fHk9pK5273NIkzF92V7yS8rpFNOMUzq3MjscwGihfuq8XoQF2li66yAfLdptdkgC7MosACChlktY7B5YBuNaBNOqWRCB9ob/SG8KMxpLyiv4rXI0wpl94kyORkRERETqTa3TPkmJRvGs/AxY+q5xPPIBsNk98zw2O5z3FnQ+3VgQ8/mVUJjlmeeSRqvC4WTaAmMO4nUntfepBRGJzUO5f3w3AJ6ZuYnkrEKTI5KNqXkAdI+PqNX5Ng8k8aoXwTS8mhE8txnbl/y5JZO8knLiIoLpn9Tc7HBEREREpL6UaPRJSjSKZy14GcqLjGrGTqM9+1w2O5z/lvFNJnu30a7t5u2u0rjN35ZJclYRUaEBnNe/tdnhHObyoW0Z0r4FhaUVTP5qLU5n400G+bryCgeb041EY49aJho9UdGYVrUIpuHzGcEzyVBf49o2Pa5XnNqmRURERPyVw1G9dVqJRp+iRKN4TkEmLH3HOB5xv/tbpo8kpDlc/BHYg2HbrzD3355/Tmk0Zm002inH94ojJNBmcjSHs1otPHNBH4LsVuZty+Tb1fvMDqnJ2pFZQGm5g7BAG21ahNbqMa6kljtnbLoqGuNr2b59PNUVjY3zTZqS8gp+3ehqm9a2aRERERG/lZ8GFSVgsUFEotnRyCGUaBTPWfAKlBVCQn+jpdlb4vvAWS8ax3Oehi2/eO+5xW85nU5+37wfgJFdY0yO5ujatwrj9tM6ATDlx00UlpabHFHTtDE1F4Bu8RG1rorz5IzGeDe1TturkqFuuZzPmb8tk7zicmLCgxjYRm3TIiIiIn7L1TYdmei5EW1SL0o0imcUHIAlbxvHp/7TO9WMh+o3EQZdDzjhqxsga6d3n1/8zvaMfJKzigi0Wzmpk28sgTmaG4Z3IKlFCGm5xbw2e7vZ4TRJGyoTjd3jw2v9mOq2ZPdl8VJdFY1ubp1urBWNP6xxbZtW27SIiIiIX1PbtM9SolE8Y+Grxqbp+L7QZZw5MYybAq0HQXEOTL8SykvMiUP8wqyNRjXjCR1aEhbk2++IBQfYePDMHgC89ecO9hzQYhhv27DPlWis3XxG8ExF477Kisbabr4+HrvVeFnQGGc0Op1O5m7NAGBsL22bFhEREfFrWgTjs5RoFPcrzIIlbxnHZlQzutiD4OIPIbQlpK2Fuf8xJw7xC79vMhKNp3WNNjmS2jm9Rywnd2pFabmDJ3/cYHY4TY5r43RtF8EA2FxJvAr3JPEqHE7Sc929DMa4bYxbp/dkFZKRV0KgzcoAtU2LiIiI+DclGn2WEo3ifgunQmk+xPWGrmeYG0tkazjrBeP4z+dh3ypTwxHflFNUxrLdBwE4rVusydHUjsVi4V8TemCzWvh5fTrztmaaHVKTsT+vmMz8EiwW6BpXl9Zp49ZdSbzM/BLKHU6sFogJD3LLNd2dDPUly3YZ/8Z7J0YSHOB7y55EREREpA6UaPRZSjSKexUdhMVvGsdmVjMeqsc50PM8cFbAjFugvNTsiMTHzN2SQYXDSaeYZrRpWbsNwr6gc2w4V53YFoBHv1tPWUXjnKvna1zVjO1bhhEaWPs2e1dbssPpniTevmxjPmNsRDB2m3t+nLvauyvcFKMvWbY7C4BBbVXNKCIiIuL3qhKNbU0NQw6nRKO414ZvoTQPortB1zPNjqbaGc8aLdT716uFWg4z29U23c13t00fzV2ju9AiLJCt+/P5eNFus8PxCXnFZSzZmUVaTrFHru/aON09ofZt03DoohX3JPFSc9y7cRrcH6MvcVU0DmrXwuRIRERERKRByooh31jyR1Q7U0ORw/n2xgPxPxu/NW57XwRWH8pjh7WCM5+D/10Dfz4H3c6EhH5mRyU+oMLhZM4WY0HEyK7+l2iMDAngH2O7MvmrtTz/6xbO7ptAy2buaaP1FzmFZSzZlcXiHQdYvDOL9ftycOXJOkSHMaxjS4Z1bMWJHVrSPCywwc/nSjTWZT4jHFIt6KYknquiMT7KPfMZwf0x+orswlK27s8HYKAqGkVERET8W16qcWsPhlC9iexrlGgU9yk6CDvmGMc9zjE1lCPqeR6snwEbZsA3t8KNs8He8KSD+LfVe7PJKiglPNjOoHb+mYC4eFAS/128m3Upubw8ayuPntPL7JC8wul08sJvW5k6e9thibHYiCAy8krYkVHAjowCPl60B4AxPWJ5/JxexDWgCrB643Tt5zPCIdWCbpp/6KpoTHBjRaP1kESj0+nE4gvjL9xgeeUM1g7RYbRwQ7JZREREREyUV1nNGB7nG+PapAYlGsV9Nv8EjnKI6QGtOpsdzZGd8Szs+hPS18Gfz8LIB8yOSEz2+0ajbfqULtEEuGnOnbfZrBYeOKM7l729mP8u3sO1J7WnXasws8PyqJLyCv75xRpmrNoHQIdWYQzt0IKh7VsytEML4iNDyCksY/HOAyzYfoAF2zPZkp7PrxvSWbTjAA+f1YMLBybWOZFWXFbBjswCAHrER9bpsdXVgu6ZpZmaU1nR6KaN01AdI4DDCbZG8rrNtexpcFu94y0iIiLi91wVjeHx5sYhR+Sfv1WLb9pQ2Tbti9WMLs2ijWQjGC3U6evNjUdM97trPqMftk0faljHVozoGk25w8mzv2w2OxyPyi4s5cp3lzBj1T7sVgv/vqAPv987ginn9+Hc/q2rEm+RoQGc3jOOR87uyS93n8ovd59C38RI8orL+ccXa7hu2tI6z3Hcmp5PhcNJ89AAYiPq1qJudfP8w33ZlRWNUe6f0QhQ7qaEqC9YtstYBDPQT6uWpfbmzp3LhAkTSEhIwGKxMGPGjGOe/9VXXzFmzBiio6OJiIjgxBNP5Oeff65xziOPPILFYqnx0a1bNw9+FSIiInJM+enGbXicuXHIESnRKO5RnAvbZxnH3c82N5bj6XkedDvLqL784V5ohNtVpXbScorZkJqLxQIjukabHU6D/XNcNywW+H5NKquTs80OxyP2HCjk/NcXsGRnFuFBdt6/djAXD06q1WO7xIbz5c3D+Oe4bgTarMzenMGYF/7g65V7a/38G1JzAOgeH1HnakhXtaC7tk57pqKx+mVBY5nTWFJeweq9xv+3wVoE0+gVFBTQt29fpk6dWqvz586dy5gxY/jxxx9Zvnw5I0eOZMKECaxcubLGeT179iQ1NbXqY968eZ4IX0RERGpDFY0+Ta3T4h5bfoaKUmjZGWK6mx3NsVksMO5p2P477FkAa6ZD30vMjkpMMHuzUc3YNzGqUSxQ6R4fwXn9W/PVihSe/mkTn9w4tNHM2ANYszeba99fyoGCUhIig3nv2sF0i6vjQhablZtHdGR09xju/d9qVu/N4e7PV5NVUMb1J7c/7uM3puYBdV8EA2CrTOK5Y0ZjWYWD/XklAMS7saLx0B1ejWXz9LqUHErLHbQMC6Rdy1CzwxEPGz9+POPHj6/1+S+++GKNPz/11FN88803fPfdd/Tv37/qfrvdTlycqiZERER8wqEzGsXnqKJR3GPjN8Ztj3P8YxhrVBKccq9x/OtDRkWmNDmzKuczjurm323Th7rn9K4E2q0s3HGgapt2Y1BYWs7NH6/gQEEpPRMi+PrWk+qcZDxU58rqxr+f0gGAx7/fwNtzdxz3cRtSXYtg6v7c7tzonJ5bjNMJATYLrcLclySvUdHopqU1Zlu2y5jPOLBt80aVeBfPcDgc5OXl0aJFzerXrVu3kpCQQIcOHbj88svZs2fPMa9TUlJCbm5ujQ8RERFxE1U0+jQlGqXhSvJh66/GcQ8fb5s+1Im3QYuOxnyHOU+bHY14WXFZBfO3ZQIwshElGltHhXD1iW0BeOanTY2m/fWlWVtJyS6idVQIn//9RGIjGl7FZ7dZuX98N+44rRMAT/64kTf/2H7U851OJxsbkGi0uXFGo2vjdFxkcNXsR3c49FIVjWSsRNUiGLVNSy08++yz5Ofnc/HFF1fdN3ToUKZNm8bMmTN5/fXX2blzJ8OHDycvL++o15kyZQqRkZFVH0lJtRvxICIiIrXgqmhsFmtuHHJESjRKw237FcqLoXk7iOtjdjS1Zw+CM/5tHC9+A9I3mBuPeNXinVkUlVUQGxFEz4T6V8b5oltHdiIi2M6mtDxmrEwxO5wG25yWx7t/7gTgsXN60izIfVM/LBYLk07vyl2jOwMw5adNvDZn2xHP3XuwiLzicgJsFjrFNKvzc9lt7qto3Jft/vmMYPz3cGflpdmcTifLKxONWgQjx/PJJ5/w6KOPMn36dGJiqt+AGj9+PBdddBF9+vRh7Nix/Pjjj2RnZzN9+vSjXmvy5Mnk5ORUfSQnJ3vjSxAREWkaqlqnVdHoi5RolIY7dNu0v7WldRoN3SeAs4KiHyeRkrcXZyOp4pFjW7zjAACndI5udO2UUaGB3DLSqNJ7/tctFJdVmBxR/TkcTh6csZZyh5OxPWMZ1d0z71reNboLk8Z0AeDfMzfz6u9bDzvHVc3YKSacQHvdf3xaLe5L4Lm2ZSdEum8+o4s7Ky/NtiOzgKyCUoLsVnolRJodjviwzz77jBtuuIHp06czevToY54bFRVFly5d2LbtyG9KAAQFBREREVHjQ0RERNygtABKKkeSaEajT9IyGGmYsiJjEQxA93PMjaUOisqLWJa2jM0HN7O5ZSSbExPYbdmL46vxxITGMLz1cIYnDueE+BMICwgzO1zxgNV7swEY0LZxVjldM6wdHyzYRUp2ER8t3M2NlbMI/c0Xy/eydNdBQgNt/GtCT48+1x2jOmOzWvjPz5t59pctxEQEc/Gg6nbH6vmM4fW6vt2NCbzMfGMRTHS4+5cYuRKNjWFG47JdWQD0TYqqV3JYmoZPP/2U6667js8++4wzzzzzuOfn5+ezfft2rrzySi9EJyIiIjW4qhkDwiCofq/LxbOUaJSG2f47lBVARCK0HmB2NLWyPnM99/xxDyn5h7SUBhj/FKxOJ/sL9/Pl1i/5cuuX2K12BsYO5IbeN3BC/AkmRSzu5nA4WZOcAxgbpxuj4AAbd4/uwn1fruG1OduYOLSNW1uOvSGroJSnftoIwN2ju5AQ5d424SO5dWQnSsodvDxrKw9+vY7OMc3o38ZIRrsqGuuzcRoOSeA5HA2O80B+KYBHtqVXVzQ2PE6zuRbBDGqkbyjI4fLz82tUGu7cuZNVq1bRokUL2rRpw+TJk0lJSeHDDz8EjHbpq6++mpdeeomhQ4eSlmb88hISEkJkpFEFe++99zJhwgTatm3Lvn37+Ne//oXNZmPixIne/wJFRESaukM3TjeyzrTGQm/vS8Ns8J9t006nk+mbp3PlT1eSkp9CdEg049uP564Bd/H6yJeZnWtjye5k3mhxEpd3v5yk8CTKHeUsTl3Mjb/cyBOLnqCwrNDsL0PcYEdmAXkl5QQHWOkSW/dZe/7i/AGt6dAqjIOFZbw/b6fZ4dTZ0z9tJLuwjG5x4VxzUjuvPe9dozoztmcspRUObvp4OftzjTbljanG4of6JhpdMxrdUdGYUVnR2MoDiUZX5aWjEYyRWK5FME3OsmXL6N+/P/379wdg0qRJ9O/fn4cffhiA1NTUGhuj33rrLcrLy7n11luJj4+v+rjzzjurztm7dy8TJ06ka9euXHzxxbRs2ZJFixYRHR3t3S9OREREtHHaD/hXeYv4lvIS2PyTcezj26YLywp5fNHjfL/jewBGJo3kiZOfICLwkITB6U/Dp5dw0qqvOOm2pdw/5H525+7mow0f8fnmz/l88+fMS5nHY8MeY0j8EJO+EnGH1cnZAPRuHYnd1njfb7HbrNw1pgt3fLqSt/7cwVUntiMyNMDssGpl6a4spi/bC8CT5/UmwIv/n6xWC89d3I8dU+ezdX8+N328nLevGsSeLOONhvpsnAawWY2vwR0zGqsrGgMbfK2/csXp7zMaM/NL2JFZAMCANqpobCpGjBhxzFnL06ZNq/HnOXPmHPean332WQOjEhEREbc5tKJRfFLj/Q1bPG/HH8YQ1mZxkOi7ibedOTu5/MfL+X7H99gsNu4eeDcvjXypZpIRoMtYaH8KVJTArMcAaBvRlgdPeJB3Tn+HhLAEUvJTuP6X63lq8VOqbvRjrvmMjbVt+lBn9Y6na2w4ecXlvPXndrPDqRWn08m/vlkPwMQhbRhoQttrsyA7b181iIhgOyv2ZHP9B8sAiI8MpnlY/ZJ7Nov7KhoPFFTOaPRgRWO5n89odFUzdolt5jcJdhERERE5jqqKRiUafZUSjVJ/O/8wbruMBatv/lXKLMrk6p+uZlv2NlqFtOLt09/mul7XHXnLsMUCpz8JWGDdF7B3edWnhsYP5atzvuKiLhcB8OmmT7l65tUcLD7opa9E3MlV0dg3KcrUOLzBarUw6XRjm/L783dVLRHxZct3H2RDai4hATb+Oa6raXG0axXGyxP7Y7HAqsq/M/WtZoTq2YeOBiYaHQ6nhysa3bcd20yuRTCD1DYtIiIi0njkpxu3SjT6LN/MDol/2LPIuG17krlxHIXT6eTRhY9ysOQgnZt35n8T/sfguMHHflB8H+h3mXH88wNwSPtVWEAYD5/4MG+NeYsWwS3YlLWJ636+jsyiTA9+FeJuJeUVVduD+zWBRCPA6T1i6ZMYSWFpBW/M8f2qxk+XJANwVp94okLdn0irixFdY7hvbLeqP9d34zS4b+t0bnFZ1TVa1LO68liqEo1+PqNx2W4tghERERFpdKpapzWj0Vcp0Sj1U1YEqauN4zZDzY3lKL7b8R1zkudgt9p5evjTtAppVbsHnvYgBIRC8iLY+O1hnz4x4UTeH/c+0SHRbMvexnU/X8f+wv3uDV48ZmNqHmUVTlqEBZLY3PNbjH2BxWLhntONysAPF+0mLafY5IiOLqeojB/W7gPg0iFtTI7GcNOpHbhgQCJWC5zWLbbe17HZ3FMp6KpKjQi2E2S3NehaR2JvBBWNpeUO1qUYm+UHtVVFo4iIiEijodZpn6dEo9RPygpwlBnzGaPamh3NYdIK0nh68dMA3NrvVro071L7B0ckwLDbjeNfHzaW3vxFh8gOTBs3jbiwOHbm7OTamdeSVpDmjtDFw6raphMjj9xC30id0rkVg9s1p7Tcwauzt5odzlF9uyqF4jIHXWKbMaBNlNnhAEai9rmL+7Lu0bENmhfprorGzMq2aU9snIbqikZ/ntG4M7OAsgon4UF2klo0jTcURERERJoEVTT6PCUapX72LDRu25xgzDb0IU6nk0cWPEJeWR69W/Xmmp7X1P0iw+4wkqgHd8GSt494SpuINkwbN43WzVqzJ28P18y8hpT8lAbFLp7XlOYzHspisXBvZVXj50uTSc7yvWVGTqezqm360sFtfC4RHBpob9Djq2cfOhp0HU/OZ4TGMaNxc3oeAF3iwn3u75GIiIiI1FNJHpTmG8fN6t9pJJ6lRKPUT/Ji47bNCebGcQRfbv2S+fvmE2QL4omTn8BurUdyIKiZ0UINMPffUJh1xNNaN2vNtHHTSApPMjZS/3w9WcVHPld8wyrXxukmlmgEGNqhJcM7t6KswslLs3yvqnFtSg4bUnMJtFs5f0Brs8NxO9fWaXe1Tnu8orGBCVEzbUmrTDTG1n+mpoiIiIj4GFc1Y2C48Tu7+CQlGqXuHA6fTTSm5Kfwn6X/AeD2/rfTIbJD/S/W7zKI7QXFOTD3P0c9LS4srkay8e7Zd1NWUVb/5xWPySkqY0dGAQB9E6PMDcYkk8YYYwS+XpnCrswCk6Op6bOlRjXj+F5xpi+B8QS7m2Y0HqhMNHqqotHV4u3w42UwrorGrrF6ASoiIiLSaGg+o1/w+URjSkoKV1xxBS1btiQkJITevXuzbNkys8Nq2jI2Gcm3gDCI7W12NFUcTgcPz3+YwvJCBsQM4IruVzTsglYbnP64cbz0Hcjec9RTY0JjePW0V2kW0IwV+1fw+KLHcfrxL+mN1dq9xnKINi1CPbKt1x/0b9OckV2jqXA4efl336lqLCgp59tVlUtgBvvGEhh3s1mNH7kNntFYUNk6HaYZjUezNV0VjSIiIiKNTl66catEo0/z6UTjwYMHOemkkwgICOCnn35iw4YNPPfcczRvXv9h/OIGrvmMiYPA1rCZZe40L2UeS9KWEGIP4fGTHsdmdcM21o6nQftToaIUZj91zFM7RHXg36f8G6vFytfbvubjjR83/PnFrVY34bbpQ9012qhqnLEyhR0Z+SZHY/hhTSr5JeW0bxXGCR0a55Zgd21zzsyrbJ0O90yi0V6ZEPXXGY1FpRXsrpxB2iVOiUYRERGRRqOqolGLYHyZTycan3nmGZKSknj//fcZMmQI7du35/TTT6djx45mh9a0+Wjb9CcbPwHgoi4X0SbCjRVRox8xbld/Bunrj3nq8MTh3DPwHgCeXfYs81Pmuy8OabBDN043ZX2TohjVLQaHE179fZvZ4QDw6VKjYviSwUmNdnmHzU1bpw9UVjS28lBVbmWescFxmmXb/nycTmgZFuixOZYiIiIiYoKqjdOqaPRlPp1o/Pbbbxk0aBAXXXQRMTEx9O/fn7ffPvIGYJeSkhJyc3NrfIib7Vlk3CYNNTeOQ+zM2cn8ffOxYOHSbpe69+KtB0CPcwEnzHrsuKdf2eNKzut0Hg6ng3/88Q925OxwbzxSb66Kxn5NvKIR4M7RnQGYsSqF7SZXNW5Oy2PlnmzsVgsXDEg0NRZPctc25+oZjapoPJLNapsWERERaZxU0egXfDrRuGPHDl5//XU6d+7Mzz//zM0338wdd9zBBx98cNTHTJkyhcjIyKqPpKQkL0bcBOSmQvZusFghcbDZ0VT5dNOnAJyaeCpJ4R74f37aQ2CxwZaZsHvhMU+1WCw8eMKDDIgZQF5ZHrfPup38Ut9oT23K0nKKSc8twWa10DOhaVc0AvRJjGJ0d6Oq8RWTN1B/usSoZhzdPZZoD7UD+wJ3JRoz8ysrGj20DMZdcZpli2sRjNqmRURERBoXVTT6BZ9ONDocDgYMGMBTTz1F//79+dvf/saNN97IG2+8cdTHTJ48mZycnKqP5ORkL0bcBCRXVjPG9oTgCHNjqZRfms83274BYGL3iZ55kladYMBVxvFv/4LjLHoJtAXy/IjniQ+LZ0/eHp5Y/IRn4pJaW1XZNt01NpyQQDfM72wEXLMav129j237zUmGl5RX8PXKFAAuHdK43xhyx4zG4rIK8kvKAU9WNDaORGNnbZwWERERaVy0ddov+HSiMT4+nh49etS4r3v37uzZc/Ttv0FBQURERNT4EDdytU23OdHcOA7xzfZvKCwvpENkB06M92Bcp/4T7CHGjMrNPx339JYhLfn3Kf/GZrHxw44f+G77d56LTY5Li2AO16t1JGN6xOJwwssmVTUu23WQnKIyosODGN452pQYvKV6RqOj3tdwzWcMtFmJCPbMMi53zZI0y5a0yopGtU6LiIiINB5OJ+Rr67Q/8OlE40knncTmzZtr3Ldlyxbatm1rUkTia/MZHU5HVdv0xG4TPbtEIiIeTrjZOJ71KDgqjvuQfjH9uKnvTQA8segJknNVYWsW1yKYfklqmz7UXZWzGr9bs4+tlZVg3jR3awYAp3SOrkpwNVbumH3o2jjdslmgx77fVbdO1z8hapbc4jL25RQD0FmJRhEREZHGoyQXygqN42ZKNPoyn0403n333SxatIinnnqKbdu28cknn/DWW29x6623mh1a01SSD2lrjWMf2Tg9P2U+u3N30yygGWd3PNvzT3jSnRAcBRmbYPWntXrIjb1vZGDsQArLC/nnn/+kzFHm2RjlMA6HkzV7cwBjNqFU65kQydiesTid8JIJVY1zt2QCcEqXVl5/bm9zR6XggYLqRKOn+POMRleyPD4ymMiQAJOjERERERG3cc1nDI6EwFBzY5Fj8ulE4+DBg/n666/59NNP6dWrF48//jgvvvgil19+udmhNU0py8BZAZFJEOkbm2E/2fQJAOd2OpfQAC98swmJglPuNY5nT4HykuM+xGa18fTwpwkPDGdt5lqmrpzq2RjlMDsy88kvKSckwEbnGM1t+6s7RxmzGn9Ym+rVqsb9ecVsTM3FYoGTOzWdRKPTaSS/68O1CKZlmOeW5tj9uHV6c5oxa1TVjCIiIiKNjDZO+w2fTjQCnHXWWaxdu5bi4mI2btzIjTfeaHZITdeexcatj7RN78rZxbyUeViwMLGbh5bAHMngGyE8AXL3wrL3a/WQuLA4Hh32KADvrXuPxamLPRmh/MWqZKOasXfrSOw2n/+253U9EiKqqhpf/n2b15533lajmrFXQqTHFpv4kkNbwyuOs1DqaDLzjTc3Wnnwv5fNDS3eZqnaOK1FMCIiIiKNizZO+w39xi21t2ehcesjbdOfbf4MgOGJw2kT0cZ7TxwQDKfeZxz/+azRUl4LY9qO4YLOF+DEyQN/PkB2cbbnYpQa1lQugumTqPmMR3PHKGNW4/dr9rFtv3eqGv+sTDQO79z4qxmhulIQ6p/EO1BZ0djKo63Txq0/VjS6Eo1dVNEoIiIi0ri4Kho1n9HnKdEotVNRDnuXGsc+kGgsKCtgxrYZAFzezYRW+v5XQPP2UJABi9+o9cPuG3wf7SPbs79oP08vfdqDAcqhtqYbyeAeCdpCfzQ9EyI5vUdlVeMsz1c1OhxO/nQtgunSuLdNuxxa0VjfJN6BfG/MaGwEFY1xSjSKiIiINCp52jjtL5RolNrZvx5K8yEoAmJ6mB0Nv+z6hYKyAtpFtOOEBBMSn7YAGPl/xvGCl6HoYK0eFhoQypMnPYnVYuWHHT8wJ3mOx0KUatsyjERjx2i1Ux6Lq6rxuzX72La/dpW69bUxLZfM/FLCAm0MaNPco8/lK2pUNFY0bEajJ1un7X66DOZAfgmZ+aVYLNBJs1hFREREGhfNaPQbSjRK7bjmMyYOBqvN3FiAP/b+AcAZ7c/AajHpr3GvCyCmJxTnwIJXav2w3tG9ubrH1QA8tvAxckpyPBWhADlFZWTkGVVgHaLDTI7Gt/VqHcmYyqrGV3737AZq17bpEzu2JNDeNH4U1axodNTrGplVFY2enNHon4nGLZWVy0nNQwkNtJscjYiIiIi4lWY0+o2m8dudNFzKcuPWBxbBlFaUsmDfAgBOSTrFvECsVjjtQeN40euQv7/WD72l3y20i2hHRlEG/1n6Hw8F6CeKc2DPIlj2Hvz4D5h2FjzXDd4eBb8+DFt/heLcel9+R2U1Y1xEMOHBAe6KutG6s7Kq8dvVnq1qdLVND+/cNNqmASwWC65cY32XwRwocG2d9lzrtL9undZ8RhEREZFGTBWNfkOJRqmd/RuM27he5sYBLEtbRlF5EdEh0XRv0d3cYLqOh9aDoKwQ/nyu1g8Ltgfz+EmPY8HCN9u/4c+9f3owSB9VVgQzH4Bn2sN7Y+H7u2HJW7DrT+OHSMoymP8S/PdCeKYtvDXS+HNZcZ2expUs6xijasba6NU6ktHdjarGVz1U1VhYWs6yXca4gaayCMbF3oD5hw6Hk6zKRGN0uDcqGutXdWmWzVXzGdU2LSIiItKoOJ2qaPQjSjTK8TkqIGOzcRxjcmKP6rbpUxJPMa9t2sVigVEPGcfL3oPsPbV+aL+Yflze3Vhk8+jCR8kv9exMPJ+ybyW8eSosmgrOCohoDZ1Gw7Db4dzX4fpf4dw3oN8V0LwdOB2wb4VR4fjaUNj0o/HDpha2ZxQAms9YF3eNrq5q3J7h/r+Xi3dkUVrhILF5CO1bNa0EsCuJV16PGY3ZRWVVCcoWHqxotPlrRWOaKhpFREREGqWig1BhjBBSotH3KdEox5e10/hHbQ+BqHamhuJ0OmskGn1ChxHQ/hSoKIU5z9TpoXcMuIOk8CTSC9N5bnntKyL9VkWZ8d/ondGQuRnCYuCy6TBpA1zxJZz+BPS7DJKGQL+JcO5UuHM13L0eznrRKJM/uAs+mwgfn1+dAD8GV6JMyyFqz6hqjMHhhFd/d/8G6j+2VLdNWyyW45zduDRk0YprPmNUaAABNs/9+HbF6PCjRKPT6TykolGJRhEREZFGJb9y43RIc7B7rrNH3EOJRjk+V9t0TDdjLqGJduTsICU/hUBrICfEm7Bt+mhOe9i4Xf0JZNa+3TTEHsKjwx4F4IstX7AodZEnovMNWTvh3dNhzlPgKIce58Ati6DL2OM/NjIRBl0Lty2DkyeBLRC2/w6vD4NfHjISmEexfb82TtfHnaO6APDNqpSqOZfu4prPeGqXptU2DWCz1b9asGoRjAerGQFsld/n/amiMT23hLzicmxWS5OrkhURERFp9DSf0a8o0SjHt3+jcRvTw9w4qG6bHhw/mNCAUJOjOUTSYOgy3mjxnTOlTg8dHDeYS7peAsATi56gxFUS3pgU5xqzFvetgOBIOP8duOgDCGtZt+sENYPR/6pMUI43EpYLXjauXZR92Oml5Q52ZxUCSjTWVe/ESEZ1c39VY0p2EdszCrBZLZzYsQkmGi31r2g8kF+5CMaDG6cB7Db/2zrtqmZs3yqMILvN5GhERERExK00n9GvKNEox7d/vXHrC/MZk41E46mJp5ocyRGc9n/G7bovIW1dnR5654A7iQmJYXfubt5Z+44HgjOR0wnf3QEHthmzGG9eAH0uMuZb1lfLjnDZZ3DxRxAQBjvmGNWSB3fVOG1PVgEVDifNguzERqjEvq7urJzVOMONVY1/VrZN90uKIjKk6W0Bt7mhdTraw4lGq8X/ZjS65jN21XxGERERkcZHFY1+RYlGOb6qikZzE405JTmsylgF+NB8xkPF9Yae5xvHs5+s00PDA8P555B/AvDO2nfYkbPD3dGZZ8nbsP5rsNrhomlGG7S79DgbrvsJwhOMmY9vj4I9i6s+XbVxOjqsyc0CdIc+iVGc5qpqnO2eqsa5W13zGZteNSM0bEZjdUWjZ1unGxKjWVwVjVoEIyIiItIIqaLRryjRKMdWVgwHthvHMT1NDWVeyjwcTgedojrRullrU2M5qhGTwWKFzT/C3uV1euiYtmMY3no45Y5yHl/4OM5ablX2aSnL4ecHjOMxjxlLXtwtvi/cOAvi+kBhJnwwAdZ+AWjjtDvcOaqyqnFlCjszCxp0rQqHk3lbMwE4pUt0g2PzR9UzGh11fuyBAteMRs9WNDak6tIsW6sWwejfuoiIiEijo4pGv6JEoxzbga3grIDgKNPfPXDNZ/TJtmmX6C7Qd6Jx/PvjdXqoxWLh/074P4JtwSxLX8a327/1QIBeVJgF068BRxl0nwAn3OK554pIgGt/gq5nGBvSv7weln9QvQhGG6frrW9SFCO7RrtlVuPalBxyi8uJCLbTp3WkmyL0L/bKRSv1SeJl5BkVja3CPVzR6GczGh0OJ1vSjX/rnVXRKCIiItL4uCoam8WaG4fUihKNcmyHLoIxsfW03FHO/JT5AJya5MOJRoBT/wnWANgxG3bNq9NDWzdrzc39bgbg2WXPcrD4oCci9DyHA2bcDDl7oHl7OGeq5//+BDWDSz6GIX83/vzdncTt/RFQRWND3Tna2EA9Y1UKuxpQ1bhyj/H3eVC7FthtTfPHj6tasD7zD71V0Vg9o7HuVZdm2HuwiKKyCgLtVtq28KElYSIiIiLiHnnpxq0qGv1C0/xNT2pv/wbj1uT5jKszVpNbmktkUCR9WvUxNZbjat4WBl5tHP/+hLEMpQ6u7HElnZt3Jrskm+eXP++BAL1g4SuwZSbYguDiD4xN095gtcH4Z2DgNYCTu3OfZaR1JZ1iwrzz/I1Uv6QoRnSNpsLhbNCsxrUpOQD0SWya1YxQvXXa0YAZja00o7GGXQeM5HfbFqFNNoEtIiIi0mg5nYe0TmtGoz/QK3I5Nh9ZBONqmx7eejg2q83UWGpl+L1gD4Y9C2HbrDo9NMAawMMnPAzAjG0zWJq21BMRek7BAZjztHE8/hljhqI3WSxw5vMUdTufAEsFrwe8SNvcld6NoRFyzWr8emUKuw/Ur6px7V4lGhtS0ejaOt3Kw1un/W1GY/LBQgDaqJpRgLlz5zJhwgQSEhKwWCzMmDHjuI+ZM2cOAwYMICgoiE6dOjFt2rTDzpk6dSrt2rUjODiYoUOHsmTJEvcHLyIiIocrzDLGcYFap/2EEo1ybOmuisYepoYxN3ku4OPzGQ8VEQ+DbzCOf3+8zlWN/WL6cWGXCwF4ctGTlLm+sfqDxa9DWaGRYBx4jTkxWG2s6P8Uv1YMJNhSRsD0iXVeziM19W/TnFO7VFY11mNWY0FJOdsyjDl6vZrofEao//zDwtJyCksrAC9snbbVPxlqhuSsIgCSlGgUoKCggL59+zJ16tRanb9z507OPPNMRo4cyapVq7jrrru44YYb+Pnnn6vO+fzzz5k0aRL/+te/WLFiBX379mXs2LHs37/fU1+GiIiIuOytLLwJbQV2z74OFvdQolGOrjjXmLEHplY0Juclsz1nOzaLjWGth5kWR52dPAkCm0HqKtj4XZ0ffteAu2ge1JztOdv5ZOMn7o/PE4pzYPFbxvHwe02d67ntQAm3ld3OxuD+UJoPH58P+zeZFk9jcOdoo6rxq3pUNa7fl4vTCXERwcSEB3siPL9Q34pGV9t0oN1KsyC72+M6lK0BC2vMkJxlVDQq0SgA48eP54knnuC8886r1flvvPEG7du357nnnqN79+7cdtttXHjhhbzwwgtV5zz//PPceOONXHvttfTo0YM33niD0NBQ3nvvPU99GSIiIgKwewF8cZ1x3HmMubFIrSnRKEeXsdm4DY+H0BamhTF3r1HNOCB2ABGBEabFUWdhLas3Lc9+EhwVdXp4ZFAkdw+8G4DXVr3G/kI/qJxY8jaU5EB0N+h2lqmhbM/Ip4RAfuz1PCQOhuJs+PQSo/Re6mVAA6oa1+zNBqB3E26bhkPnH9Zt0YqrbTq6WRAWDyfwbRY/q2isbJ1Oah5iciTijxYuXMjo0aNr3Dd27FgWLlwIQGlpKcuXL69xjtVqZfTo0VXnHElJSQm5ubk1PkRERKQOdi+Ejy+EsgLoMBLOeuH4jxGfoESjHJ2PLIJZkb4CgGEJflTN6DLsNgiOgoxNsPaLOj/8nE7n0Ce6D4XlhTy77Fn3x+dOpQWw6DXjePg9YDX328u2/Uabbtv4GJj4OUS1hYO7YPpVUOFHreg+5q5DqhrrsoF6nWsRTBNum4ZDNzrXr6LR023T4H8zGveoolEaIC0tjdjYmvOeYmNjyc3NpaioiMzMTCoqKo54Tlpa2lGvO2XKFCIjI6s+kpKSPBK/iIhIo7RnEfzXlWQcARM/hQC9qewvlGiUo6taBGPufMY1mWsA6Bvt5aUi7hAcCSfdaRzPearOCS6rxcr/Df0/LFj4aedPvr0YZvk0KDwAzdtBz/PNjobtlfMAO0aHGdWlEz8zWtl3/QkzJ5scnf/q36Z51QbqV+pQ1bimMtHY5Csa6zmj8UCBUdHYMszziUZ/2jqdV1xGdqHxfVWJRvElkydPJicnp+ojOTnZ7JBERET8w57F8PEFxvir9qfCpUoy+hslGuXofKCicX/hftIK0rBarPRs2dO0OBpk6N8hLMaoplv5UZ0f3qNlDy7uejHgw4thyophwSvG8cmTwObZGXLHk1tcRnqukZjpGNPMuDO2B5z/NmCBpW/DMs3Wqq+7RncB4OuVe9lZi6rGvOIydmQY5/Vu4hWN9Z1/mFlZ0ejpjdMAtnomQ83gWgTTIizQ47MrpXGKi4sjPT29xn3p6elEREQQEhJCq1atsNlsRzwnLi7uqNcNCgoiIiKixoeIiIgcR/qGQ5KMp1QWi+jNZH+jRKMcXVVFo3mJxrUZawHoFNWJ0AA//QYTGGa0EgP88R8jKVdHt/e/3bcXw6z6L+SlQkRr6DvR7Giqklox4UFEBAdUf6LbGXDag8bxj/+AXfNMiM7/9UuK4rRuMTic8Mqsrcc9f12KMZusdVQILb2QKPNl9noug3HNaPTGf7/6xmgGtU1LQ5144onMmjWrxn2//vorJ554IgCBgYEMHDiwxjkOh4NZs2ZVnSMiIiJu4HTC93dDaR60PdkYf6Uko19SolGOrCATCvYDFmOxh0lWZ64GoHer3qbF4BaDroWIRMjbB8verfPDfXoxTEUZzH/ROB52B9g939p5PNv3u9qmmx3+yeH3GK3djnL4/Eqj0lTqzDWrccaqlKo29aNZm5INqJoR6j//8EBVRaMXZjRa6rewxgx7tQhG/iI/P59Vq1axatUqAHbu3MmqVavYs2cPYLQ0X3XVVVXn33TTTezYsYP77ruPTZs28dprrzF9+nTuvvvuqnMmTZrE22+/zQcffMDGjRu5+eabKSgo4Nprr/Xq1yYiItKorf4MkhdBQBic/5aSjH5MiUY5MlfbdPN2RkWeSVwVjX45n/FQ9iA49T7j+M/noeTYiZkj8dnFMGu/gOw9EBYNA646/vlesM01nzHmCH93LRY4ZyrE94WiLGM5THmJlyP0f30Soxjd3ahqfPk4VY1rKysam/p8Rmh4RaNXWqf9qKIxWRWN8hfLli2jf//+9O/fHzCShP379+fhhx8GIDU1tSrpCNC+fXt++OEHfv31V/r27ctzzz3HO++8w9ixY6vOueSSS3j22Wd5+OGH6devH6tWrWLmzJmHLYgRERGReirOgV+Nn9Wc+g+IbG1uPNIgSjTKkfnAIphyRznrD6wHoE90H9PicJt+l0GLDlCYCYtfr/PDrRYrDw59EKvF6juLYZxOmPe8cXzirT7zrpOrorHTkSoawYjz0k8gpAWkroZfHvRidI2Ha1bjt6v3sW1/3lHPW7s3G4A+SjRidVU0VtStWtCbW6ddC2scfpBodLVOt1GiUSqNGDECp9N52Me0adMAmDZtGnPmzDnsMStXrqSkpITt27dzzTXXHHbd2267jd27d1NSUsLixYsZOnSo578YERGRpmL2FKOjsmVnOOFWs6ORBlKiUY7MBxbBbM/eTlF5Ec0CmtE+sr1pcbiNLQBGPGAcz38FCrPqfInuLbtzYecLAZiyZArljnJ3Rlh3Kcshc4tR3j7oenNjOUTVxumYoyQaASIT4bw3jeMlb8H6GZ4PrJHp1TqSMT1icTrhpVlH3kCdU1jGrgNGMkit04dsdK5jDq9667Q3KhqNlwZ+UdF40FgGk9RciUYRERERv5S+3vh9DOCMf/vEKK5jcTicbE3PY1VyNtmFpWaH45PqnGi84YYbDnsnWBohH1gEszrDmM/Yq1UvrJZGkhPvdYFRJVqSAwtertclbu9/O5FBkWw9uJXpm6e7OcA6Wv+1cdt1PAT7xkbNsgoHuysTW0ec0XioLqfDSXcZx9/eDlk7PBtcI+Sa1fj9mn1sST+8qnHdvhwAklqEEBXq2y8avKF6RmPtKxorHE6yCipnNIZ7c0ajbycanU7nIa3TmtHo7/T6UkREpAlyOo0lnc4K6H42dDzN7IgOU1bhYOWeg7w1dzs3fLCMAU/8ypgX5nLu1Pn0e+xX+j/2C+e/Np97pq/mnT93cLBAycc6Z28yMjIYN24cSUlJ/OMf/2D16tWeiEvM5HT6ROv0mow1QCNYBHMoq7V66/GiNyAvvc6XiAqO4vZ+twPw6qpXySque2WkWzgc1VWAPc8zJ4Yj2H2gkHKHk9BAG/GRwcd/wGkPQtIJUJIL/7tG8xrrqGdCJGN7VlY1/nb4rMY1e41EY5/WUV6OzDfVZ0bjwcJSXKe38EKy1l9mNGbklVBS7sBqgYQoJRr9nV5fioiINEFrv4Dd88EeAmOfMjuaw8zamM6wp3/nvNcW8NSPm/htYzrZhWWEBNiIjTA6jQ4WlrFiTzZfrtjLEz9sZNjTv/PIt+ur3hBviuqcaPzmm29ITU3loYceYunSpQwYMICePXvy1FNPsWvXLg+EKF6Xm2IkXax2aNnJtDDWZjaSRTB/1fUMSBwM5UUw9z/1usSFXS6kW4tu5JXm8fKK+lVGNljKcsjdC4HNoNMoc2I4gqq26ehmWCors47JFgAXvqt5jQ1w95guWCzww9pUNuzLrfG5dSlGolGLYAyutuSKOvROu+YzNg8NwG7zfHW3v8xoTK7cOB0fGUKAF/67iGfp9aWIiEgTU5xb/bvXKfdAVJK58RyiuKyCh79Zx/UfLCMjr4So0ABGd4/l/87ozoxbT2LNI6ez+IHRrH90LD/ccTJTLxvAPWO60CM+gqKyCqYt2MWIZ+dw+6crq34fakrq9cq8efPm/O1vf2POnDns3r2ba665ho8++ohOncxLSokbuaoZW3Y2bT5CbmkuO3KMNtbe0Y2oohGMrcejKjdqLZ8GB3fV+RI2q40HhhrzHr/a+hXrM9e7L77aOrRtOsC71URZBaUs3nGAjxft5qOFu1ix5yDFZRUAbNvvSjTWYVu65jU2SLe4CM7qkwDA879uqfG5NSnZAPTRfEagfhWN3tw4Df5T0bhHbdONjl5fioiINCELXoH8NGNh6rA7zI6myoZ9uZz1yjw+XLgbgOtPbs/iB0bxztWDuPGUDvRLiqp6kzssyE7PhEjO7BPP7aM688MdJ/PR9UMY3rkVFQ4n363ex1mvzOP/vl5LUWmFmV+WV9kb8uCysjKWLVvG4sWL2bVrF7Gxse6KS8yUXpm0ijWvbXpd5joAEpsl0iK4hWlxeEz7U6DDSNgxG+Y8Dee9UedL9I/pz1kdzuL7Hd/z1JKn+Gj8R96bZelwwIYZxrEX2qZzi8t4648dLNmVxfb9+Rw4wtwLm9VC55hmFFZ+Az/ufMa/cs1rnP8ifHsHtB7oU++q+bq7RnfmhzX7+G1jOquTs+mbFMXBglKSs4xlHT2VaASqk3gOZ90Tjd7YOA2HLKzx8USj6++WNk43Pnp9KSIi0shVlBlFNwCnPQR277yhfixOp5N35+3k3zM3U1rhIDo8iOcu6sspXaJrfQ2LxcLwztEM7xzNupQc3pq7g29X7+O/i/ewcMcBXrqkf5Po9KpXVmL27NnceOONxMbGcs011xAREcH333/P3r173R2fmMEHFsG45jP2ie5jWgweN+oh43b1Z9X/zeto0sBJhNpDWZOxhm+3f+vG4I5j71KjxT4wHDp6rm3a6XTyzaoUTnv2D16dvY0lO7OqkoyJzUMY2TWakV2jadUsiAqHk01peVVVTl3iwuv+hKc9CK0HGct6vr4JHE3nXaeG6hjdjHP7twaqqxrXVrYJtGsZSmRIgGmx+ZL6VAtmVrZOe6ui0WpxxVj7hTVmqFoEo43TjYZeX4qIiDQRm36Agv3QLBa6TzA7GgBe/2M7T/ywkdIKB6O7xzLzzuF1SjL+Va/Wkbw8sT8fXz+U2IggdmQUcN5r83ltzjaff0O/oepc0di6dWuysrIYN24cb731FhMmTCAoyPzss7hR5mbjNrqbaSE0iURj64HGN9WN38HvT8Cl/63zJaJDo7mp7008v/x5Xlj+AqPajCI8sB4JtrpyVTN2HQ8BtVi4Ug/b9ufz8DfrWLD9AAAdWoVx04iO9IiPoEN0GKGB1d++nE4nabnFrN2bw7qUHJzAqG4xdX9SWwCc/xa8MRx2zzM2g598t5u+osbvzlGd+XbVPv7YksGyXVlVicbeiVHmBuZD6lMteMDLrdOuGY2+/gLI9aZCm5ZKNDYGen0pIiLShCx/37jtf4XxO5jJFmzL5NmfjTzI/eO78fdTOtRu3n8tnNy5FTPvPIUHvl7LT+vS+PfMzczZnMFLl/YjPrJxjgCqc6LxkUce4aKLLiIqKsoD4YhPcM0MbNHBlKd3Op1Vi2D6tGrEiUYwysQ3/QCbvoe9yyBxUJ0vcUX3K/hq61fsyt3FG6vf4B+D/+GBQA/h4W3T5RUOXvxtK2/O3U5ZhZMgu5XbRnbib6d2IMhuO+JjLBYL8ZEhxEeGcHrPuIYF0LIjjH8Gvr0Nfn/SaHFP6NewazYRbVuGcdGgRD5dksxzv2whIsT4EaP5jNWqKhrrsQymZZh3WqdtftI6vfeg0TqdqIrGRkGvL0VERJqIA9thxxzAAgOuNjsaUnOKuP3TlTiccOHARLcmGV2ahwXy2uUD+N/yvTz67XqW7MzivKkL+OC6IXStTyeej6tz6/SNN96oF4GNWXEOFB00jqPamhJCcl4y2SXZBFoD6dbCvKpKr4juCn0nGsezHqvXJQJsAfxzyD8B+GTjJ+zI3uGu6I5s7xLI2wdBEdDxNLde2ul08tA363l19jbKKpyM7BrNr3efyu2jOh81yegR/a8wqk0dZfDlDVBa6L3n9nO3ndaZQJuVhTsOMHtzBuBHG6fLio2E/5K34Y9/w7ovIW0dlBW57SmqKxpr35Z8sLBy67SXEo32ys3YDqfvbp4uLXeQmmP8f9EymMZBry9FRESaCNdsxk6jobk5OQeX0nIHt/x3BQcKSukRH8ET5/Zye5LRxWKxcPGgJH68czidYpqRllvMRW8sYMnOLI88n5m8tDlC/MZBY7MSoa0gqI7LNNxkTabRNt2tZTcCfKCM2uNG3A/WANj5B2yfXa9LnNz6ZEYkjaDcWc7TS57GWYdFE3Xmqmbseobb26bfnLuDT5fswWKB5y7qy3vXDDanLdJigQkvQ3g8HNgKvzzo/Rj8VOuoECYOMZbolJY7sFigZ0KEyVEdhdMJm36E7+402uWntIZ3RsGP98LsJ+GL6+CNk+DJeHixD3x6GWz+yajqrSdrPWY0ZheVARAV6p3vh66KRoAKT34vaYB92UU4nBAcYCXaSy3lIiIiItJA5SWwqnJk2KBrzY0FeOrHjazck01EsJ03rhhIcIDni1vatgzji5tOZFDb5uQWl3PFu4v5eX2ax5/Xm5RolJpcbdPN25kWQtV8xsbeNu0S1QYGX28c//ZIvZMY9w26j0BrIAtTF/J78u/ui+9QNbZNn+vWS/+wJpWnf9oEwINn9uCCgYkeezepVkJbwLmvGcfL3oXNM82Lxc/cOrITQXbjx0v7VmGEB/vgGwY5KfDppfDZRONd1bQ14Cg33mTpfDr0uxyShkJwFOCE7N2w+QfjMVOHwLL36lXpaK/H1uncykSjtxbq1Eg0+mhFY/LB6kUwpn6fEBEREZHa2/gdFB6A8AToPNbUUL5ZlcK0BbsAeOGSfl4tcIkKDeTjG4YyunsspeUObv54OR8v2u215/c0JRqlJl9KNDbmRTB/NfxeCGwGqauqE3l1lBSRxNU9jRkX/1n6H4rLi90Xn0vyYshLdXvb9PLdB7l7+ioArhnWjutOaue2azdIx9PghFuN429uhYJMc+PxEzERwVw9rB0Ag9u2MDeYv3I4YNn78NoJsGUm2AJh6E1w8Ydw11r4xza4/H9Gkvn6X+Cfu+DebXDNj3DSnRAUaVS5fn83vNATZk8xRk7Ukq2yLbkuMxqzCysrGkO81TpdnbirS+WlN7kWwSS10HxGEREREb/hapsecCXY6rwyxG22pudx/5fGXojbRnZiVPdYr8cQHGDjjSsGMHFIGxxOeHDGOl6ZtdXrcXiCEo1Sk8mJxuLyYjZnGduemlSisVk0DLvdOP79cagoq9dlbuh9A7GhsaTkpzBt/TT3xeey/mvjttuZYHdPu+LuAwXc+OEySssdjO4ew0Nn9fCtCqVRD0NMTyjMhO/vMtpt5bjuPb0rz13Ul/vGdTU7lGpZO+DDs43/jyW50HoQ/P1PY/lPj3OM6uK//t2zWIx/n+1OgjGPwaT1MHYKRLYx3o3942l4bVjlQOvjq8/W6ewiY0ajKhqrJWcZ1aRtlGgUERER8Q8ZW2DXn2CxwoCrTA3liR82UlRWwcmdWnH3mC6mxWG3WXnqvF7cNbozAM/9uoW35m43LR53UaJRajI50bgpaxPlznJaBrckISzBlBhMc+KtEBZtJENWfFCvS4QGhHLvoHsBeHftu6Tmp7ovPocDNnxjHPc41y2XzC4s5dppS8kqKKVX6wheurR/jSSHTwgIhvPeAKvdKPVfM93siPxCoN3KBQMTaekr8/P2LofXTzZe3ASEGsnC63+BmDounAoKhxNvgTtWwoXvQ/P2kLsXPjwHfrgXSguO+XBbHWc0FpdVUFxmjFOI9NaMRosfJBorW6cTm2sRjIiIiIhfcFUzdj4dIhPNC2P3Qf7YkoHNauHJ83qZ/vunxWLhrtFd+MdYo0DjqR838dHCXabG1FBKNEpN2ZVzAUxKNLrapntH9/atqjZvCAqHU+4zjuc8AyX59brM2HZjGRQ7iOKKYp5d9qz74tu3AvLTKtumR7rlkk//tIkdGQUkRAbz3tWDCQsyr3z+mOL7wKn3G8c//sOY7yf+I2evMYuxrACSToCbFxjJQmsDhj3b7NDrfLhpHgy+wbhv6dvwxsmQvOSoD7Pb6lbR6JrPaLVAuJf+fVitlqrCzvIGLL7xpGS1TouIiIj4j7JiWP2JcTzoOlNDefG3LQCc3781bVuGmRrLoW4d2YlbR3YE4KFv1vPF8r0mR1R/SjRKNUcFZO8xjk1aM78205iT0De6rynPb7qB1xhJ3oL9sOj1el3CYrFw/5D7sVqs/LL7F5akHj3pUSe75hm37Ya7pW16S3oe05clA/DyxP7ERLh3g7XbnXw3tB4IJTnw7W1qofYXpQXGApf8dIjpYcxfbNHefdcPagZnPgdXfGUMtc7aAe+NhT/+fcS/I1ZL3RKNro3TESEBVRurvaE+Ld7e5Eo0qnVaRERExA9s+AaKDkJkEnQabVoYy3dn8efWTOxWC7ef1tm0OI7m3tO7ck3lrPv7vljND2vc2KHoRUo0SrW8VKgoNVpEI1qbEsLWg8bw067NfWiumzfZA+G0h4zj+S9BwYF6XaZri65c3OViAKYsmUKZo34zH2vYPd+4bXdSw68FTPlxIw4njO8Vx6B2PrYw5Ehsdjj3DbAHw/bfjU3U4tscDvjqb5C21tgmPfEzCI7wzHN1GgW3LIS+E8HpgNlPwtc3QXlpjdPsdWydzilyLYLx7uZumw8nGvOKyzhYuSBHFY0iIiIifmDVf43bAVc1rKuogV741cg3XDAg0atbpmvLYrHwrwk9uHRwEg4n3PnZSmZtTDc7rDpTolGqueYzRrUx5R9/maOM3blG63anqE5ef36f0fN8iOsDpXnwZ/1bn2/rfxtRQVFsy97G55s+b1hMjgrYs8g4btvwROOCbZnM3pyB3WrhvnF1nJFnpuguMPoR4/iXh4zqNfFdvz8Om743Nktf+onnK7VDoox5nhNeBosN1nwGH59vvHtbqTqBV7uWZNfGaW8tgnGxV27H9sVEo2sRTIuwQJr56rgFERERETEU51YXrfS6wLQwlu7KYt42o5rxttN8N99gsVh48rzenN03gXKHk1v+u4KVew4e/4E+RIlGqWbyIpjk3GTKneWE2kOJC4szJQafYLVWJ7OWvgMHd9frMpFBkdw54E4Apq6aSmZRZv1jSltjbOkNioS43vW/DuBwOHnyx40AXHFCW9q38p25GLUy5O9G+3hZIXx9s5GEFd+z6lOY97xxfPar0Gao95574NVw+XQIDDeWz7wzBrJ2AtUzGuta0RgZGuiZWI+irktrvMm1CCZJi2BEREREfN+OOeAoh5adoGVH08J44VdjNuNFgxJ9vivGZrXw3MV9Gdk1mpJyBzd8sKxqdJA/UKJRqpmcaNyWvQ2AjlEdm94imL/qeBq0P9VoZZ/9ZL0vc16n8+jRsgf5Zfm8tOKl+sezq/IdqDYnNLja9ZvVKazfl0t4kJ07RvneXIzjslrhnKlGEil5ESx6zeyI5K/2rYLv7jCOh98DfS/xfgydRsN1M40xFAe2wjujIXkptjpWCmYXGq3Xap2u5nqRlejjLxBFREREBNj6i3Hb+XTTQli84wALth8gwGbh1pG+W814qACblVcvG0CP+AgOFJRyzftLyCl0w0g0L1CiUaqZnGjcnrMdgA6RHUx5fp9iscCYR43jNZ8biZN6sFltPDD0AQBmbJvB6ozV9YvHTfMZi8sqePZn452km0d2pEWYd6u03KZ5Wxj7hHH8+xOQscXceKSa0wk/P2Ak6bueASMfNC+WuF5wwyxjFEJhJnx4Dq0OLAfqUdFoUqKxvMJ3E41aBCMiIiLi45xO2Pqrcdx5jGlhvPCbq5oxicTm/vMaMizIznvXDCY+MpjtGQX8/eNllJbXbgSTmZRolGquFt0oczZO78g25t11jDKvnNqnJPSH3hcZx788WO8tx32j+3JOx3MAmLJ4Cg5nHb8xORywe4Fx3MD5jNMW7CIlu4j4yGCuO8mNm3/NMOBqo/K0vBhmqIXaZ2z9xUiM24LgjP8YFahmioiHa3+CDiOgrIAh8//GYMsmHHVdBhPq7RmNRqLR4YPb1ZMPGjMak/zoRaKIiIhIk5S2BvLTICDMLbP+62Ph9gMs2pHlV9WMh4qLDOa9awbTLMjOoh1Z3P/lGpw++Br9UEo0SjUfqWhUovEQpz1kLLLY9Wd1yXk93DXwLpoFNGP9gfV8vfXruj14/wYozjZ+OMT3rXcMBwtKmTrbaI+/5/SuBAeYt23MLSwWOPsVCIqAlGWw4BWzIxJHBfz2iHE89O8QmWhqOFWCmhkbrzuMwF5RyLTAZ+hcsq5WDzVrGYwvz2jcU1nRmNRCMxpFREREfJrrd9gOI8AeZEoIb8018gyXDE6idZR/vn7sHh/B1MsHYLNa+GplCi/+ttXskI5JiUYxlBZAwX7j2IREY7mjnF05uwAlGmto3haG3mQc//owVJTX6zKtQlpxS79bAHhpxUvklOTU/sGutuk2Q8FW/2TH639sJ6+4nO7xEZzXv3W9r+NTIhNh7FPG8eynYP8mc+Np6lZ/ZiTGgyNh+CSzo6kpIAQu/ZSs2GGEWUp4KPvh6k3ux2B263Rtt2N7i9PpZO9BtU6LiIiI+AWT26Yz80uYu9VYiurvHXWndonm8XN6AfDSrK18t3qfyREdnRKNYnC1TQdHQUiU158+OS+ZMkcZIfYQ4sPivf78Pm34PRDSHDI2waqP632ZS7tdSqeoThwsOcirK1+t/QN3zTNuG1DqXlJewfRlyQDcM6ZLVRKjUeh/BXQaAxUlRgt1PZPB0kBlRdWLk1z/ZnxNYCgbR7zJvIqehFIEH19w3GRjdlXrtElbp31sRmNGfgnFZQ6sFkjw03ekRURERJqEwizYu9Q4NinR+MOaVCocTvokRtIhupkpMbjTZUPbcONwI2H6jy9Ws35fHQqIvEiJRjGY3Dbtms/YPrI9Vov+WtYQEgWn3Gccz34KSvLrdZkAawCTh0wGYPqW6Ww4sOH4D3I6q+cztju5Xs8L8NuG/WQXlhEXEczIbjH1vo5Psljg7JchKBL2rYAFDdjuLfW35C3ITYGIRBjyd7OjOSpLYCg3lN3LSlsfKM03ko3HWPaUU7l12tsVjXYf3TrtWgQTHxlCgE0/K0RERER81rZZ4HRAbC/TRhp9syoFgHP6NZKOOuD+8d0Z3rkVxWUO/vbhcg7kl5gd0mH0Kl0MVYlGcxbBVM1njFTb9BENvgGat4f8dFhYh2rEvxgSP4Tx7cfjcDp4cvGTx18Mk7HZ2JZrD4GEAfV+Xlc14wUDWzeuakaXiAQY/7RxPHsKpNciiSvuU3QQ/nzOOB75AAQEmxvPMdgsFooJ4oGQB6HdcCPZ+N8LIWvHEc83axmMrXKJToWPDZr+fk0qAG1bqm1aRERExKe55jOaVM2450AhK/ZkY7XAhD6Np2vSZrXw6sQBtGsZSkp2Ebf8dwVlFb417kiJRjFkV7ZOm7UIJttINHaI6mDK8/s8eyCM/pdxPP8lyEur96XuHXQvofZQ1mSs4Ztt3xz7ZNd8xqTBRgz1sC+7iLlbMwC4aGBSva7hF/pOhC7jwFFW2UJdZnZETcefz0NxDsT0gL6Xmh3NMdltRqK9yBkIl/4X4npDQQZ8dB7k769xrsPhNG1Go90Hl8HM2byf9+fvAuCG4f49Y0dERESkUXNUwLbfjOPOp5sSgquacVjHVsRE+G4hQn1Ehgbw1lWDCAu0sXhnFk9871uFLko0isHsjdOVicZOUf63bt5repwLiYOhrLB6Fl09xITGVC2GeWH5C8deDONKNDZgPuNXK/bidMLQ9i1o1yqs3tfxeRYLnPWisYgkdRXMf9HkgJqI7GRY/KZxPPoRsPr2NnNXpWC5w2n8Xbn8S4hqa3wP/vgCKM6tOje/tBxXns/biUarq3XaR2Y0ZuSVcO//VgNw9YltOa1brMkRiYiIiMhRpSyHoizj9W7iEK8/vdPpZEZV23SC15/fG7rEhvPCJf0A+GDhbj5fusfcgA6hRKMYTEw0Vjgq2JmzE1Dr9DFZLHD6E8bxyo8hbW29L3VZ98voGNmRgyUHeWXlK0c+yemEXQ1LNDocTqYv2wvAxYMacTWjS0Q8jHvGOJ7zDKSvNzeepmDBy8YinrYnm/ZuaV0cNvswPBau/BpCW0HaGvj8cig35qzkFBrVjMEBVoIDvJtA9aWKRofDyb3/W01mfind4sKZfEZ3s0MSERERkWNxtU13HAU2u9effv2+XLZnFBBktzKuV5zXn99bTu8Zx92juwDw4Ix1LN990OSIDEo0ipFQMjHRmJKfQqmjlCBbEAnNGue7DW7T5gToeZ4xVHfmZOP/XT0EWAP4vxP+D4Dpm6ez/sAREmJZOyA/DWyBkDioXs+zeGcWe7IKaRZkZ3zvxvsNvoa+l6qF2lvKimHNdON4+N1GMt7H2Y6UwGvZEa74AgKbwc658NXfwOEgu9CctulD4/SFZTDvzd/JH1syCLJbeXlif68nXUVERESkjqrmM5rbNj26eyzhwd5/Le1Nt5/WiXE947BgYe/BQrPDAZRoFDAWjJQXg8UKkd6vOnO1TbePbI/Nx9sefcLoR8EWBLv+hM0/1vsyg+MGc0b7M3Di5KlFTx2+GGbXPOO29SAICKnXc/yvcgnMhL7xhAZ6/50sU9RooV6tFmpP2vwjFGdDRGvoMNLsaGrlqNucE/rDJR+DNQA2zIDf/lW9CCakfvNRG6IqTpOXwaxLyeGZmZsAePCsHnSJDTc1HhERERE5jrw04/cgLNBptNefvsLh5NvV+4DG2zZ9KKvVwnMX9+V/N53oM9u1/SrR+PTTT2OxWLjrrrvMDqVxcVUzRiSCzfvZftfG6Q6RWgRTK83bwrDbjOOf/6+qzbI+7hl0D2EBYazJXMPXW7+u+UnXfMZ29Wubzi0u48d1xobYi5pC2/ShIuJh/L+NY7VQe87Kj43bfpf5/GxGF+uxKgU7joRzXzeOF7xM+Ib/AsawZ2+rrmg0b4NdYWk5d3y2krIKJ6f3iOWKoW1Mi0VEREREamnrr8Zt6wHQLNrrT794xwHSc0uICLZzalfvP78ZwoLs9E2KMjuMKn6TaFy6dClvvvkmffr0MTuUxuega+N0W1OeXotg6uHku6FZLBzcCUveqvdlYkJjuKVv5WKYFS9wsPiQmQ67Fxi39ZzP+P3qVIrLHHSKaUZ/H/qm5zV9LoEu49VC7Sk5KbD9d+O432XmxlIHR61odOlzEYyYDEDvVY8xzLrO1NbpchOXwbzy+zZ2ZBQQFxHMMxf0weIHrfEiIiIiTZ7JbdOuJTBn9oknyO4fxQiNjV8kGvPz87n88st5++23ad68udnhND4+snG6Q5QqGmstKBxGPWwc//FvKMis96Uu634ZXZp3Iackh+eXP2/ceXA35CSD1Q5J9dsSNr2ybfqSQUlNM0FgscCEFyE4ymgdmPeC2RE1Lqs/BZxGIryF/3zvqJ7ReIxKwVP/Cb0vwuos5/WAF+ls3eel6KodNyHqYQcLSvlwwS4AHjunJ83DvN8+Lv5t6tSptGvXjuDgYIYOHcqSJUuOeu6IESOwWCyHfZx55plV51xzzTWHfX7cuHHe+FJERET8h8MBO/4wjjuN8frTF5dV8NO6NACfaSNuivwi0Xjrrbdy5plnMnr08fv7S0pKyM3NrfEhx2FiotHhdGjjdH31vQzi+kBJLsx+st6XsVvtPHTCQwDM2DaD5enLYc8i45MJ/SEwrM7X3JKex6rkbOxWC+f2b8Lf4MPjqluo//h3gzaFyyGcTlhltBXT73JzY6kju9X4sXvMBJ7FgnPCKyyK7MHPEVZS8idz7tcTmPj9RP7+69+59497eWzhY7y84mXmp8ynzOH+almbyTMa35+/k4LSCnrERzCmR6wpMdTW3L1zySrOMjsMOcTnn3/OpEmT+Ne//sWKFSvo27cvY8eOZf/+/Uc8/6uvviI1NbXqY926ddhsNi666KIa540bN67GeZ9++qk3vhwRERH/kbkFSnIgIBTi+3r96eds3k9ecTnxkcEMadfC688vBp/fzvDZZ5+xYsUKli5dWqvzp0yZwqOPPurhqBoZExON+/L3UVxRTIA1gMTwRK8/v1+zWmHc0zDtDFg+DQbfALE963WpfjH9uKDzBXy59UueWPQE04O6EQDQemC9rjd9qVHNeFq3GKLDg+p1jUajz8Ww4RvY/IPRQn3D72BXdVaD7FlkbEUPbAY9zjE7mjo54tbpQyxNW8rXW79mSdoS0lvkA5UvkHJ3HfH8t9e+TXhgOCOTRjK6zWiGtR5GkK3h/+ZqlRD1kNziMt6vrGa8/bROPl0RfbD4ILfNug2LxcLsi2fTIlgvaH3B888/z4033si1114LwBtvvMEPP/zAe++9x/3333/Y+S1a1Pz/9tlnnxEaGnpYojEoKIi4uDjPBS4iIuLv9lbmbRIGgM376aYZK41OoLP7JlTNRhfv8+lEY3JyMnfeeSe//vorwcHBtXrM5MmTmTRpUtWfc3NzSUpqYoso6qoq0dje60/taptuF9kOu9Wn/zr6pnYnGYmWDd/AzMlw1TdGy2493D3wbn7f8zvbsrfxIQe4HiC2V52v43Q6+X5NE10CcyQWC5z1AuxZYFQ0/vkcjJxsdlT+zbUEpue5ENTM1FDqypVodDrB4XBWvQDKLc3luWXP8dXWr6rOtWDHXhjLdWXb6FeUR3mHEeT2v4zc0jzySvNILUjlj71/kFWcxbfbv+Xb7d8Sag9lQscJ/L3P34kOrf/wa6uJMxo/XLCLvOJyusQ2Y2xP307qLNi3ACdOOkd1VpLRR5SWlrJ8+XImT67+Pmu1Whk9ejQLFy6s1TXeffddLr30UsLCalb0z5kzh5iYGJo3b85pp53GE088QcuWLY94jZKSEkpKqpe1qcNGRESahJRlxm1i/QpWGqK03MEfWzIAmNC38W+b9mU+ndlZvnw5+/fvZ8CAAVX3VVRUMHfuXF599VVKSkqw2WoO9wwKCiIoqIlXUNVFWTHkVc7/MmEZjGvjdKdILYKptzGPweaZsPMP2PQ9dJ9Qr8tEBkVyz6B7eHD+g7zpyGK83UZCXO86X2dzeh5pucUEB1gZ3rlVvWJpdMJj4Yxn4cvr4c9noet4SOhndlT+qSQf1lduSO93hbmx1IPtkHdWK5xOrFj4fc/vPLHoCTKKjBdGF3S+gHHtx/HctyUs3Z3PgFFFDFvwN1g/ExJPgRNvrb6Go4KV+1fy257f+G33b6QXpvP55s/5Zts3XNHjCq7tdS0RgRF1jtOsGY0FJeW8O88Yp3HryE4+/070/JT5AJzc+mSTIxGXzMxMKioqiI2t2XIfGxvLpk2bjvv4JUuWsG7dOt59990a948bN47zzz+f9u3bs337dh544AHGjx/PwoULD3stCuqwERGRJmqvK9E42OtPvSo5m6KyClqGBdIjvu6vf8V9fDrROGrUKNaurTnT7Nprr6Vbt27885//POILO6mj7D3GbWAzCD38Xfms4ix+3/M7v+7+lRXpKyh3ltf4vBUrXVt05YT4Ezgh/gT6xfQj0Fb7ttC6LoIpKq3gjy37+XFtGn9syaCwtPywc5JahHJSx1ac1KkVJ3ZsacrGVq9q3g6G3W4ksGY+AB1HQWBovS51dsez+XrT5yw/sJYpLVvwSnS3Ol/jj81GsuTEDi0JDtC/0Sq9LjAqTzd+CzNugb/NBrveFKmzDd9AWQG06AhtTjA7mjqzH5I421+QyQsr/83Pu34GoF1EOx4Z9ggDY413gPOK5gJQ3vZUCH8SZt4PvzwI0d2g0ygAbFYbg+IGMShuEPcNvo+laUt5eeXLrMlYwztr32H65ulc3/t6Lut2GcH22nUGGNc9dou3p3y8aDcHC8to3yqMs/r49jvRDqeD+fuUaGxs3n33XXr37s2QITUXoV166aVVx71796ZPnz507NiROXPmMGrUqMOuow4bERFpckryYf8G47j1IK8//fxtxoLUEzu29Pk3qxs7n040hoeH06tXzdbNsLAwWrZsedj9Uk/Zu43b5u2qWm5zS3P5cceP/Lr7V5alL8PhPMZ2VGBt5lrWZq7l7bVvE2wLpn9Mf8a1H8eEDhMIsB07ybcjewcAHaOOvgimrMLBz+vT+HFtKrM3ZVBUVnHsa2YUsCOjgI8W7cZqgd6JUYzpHsMVJ7QlKrSRzsYbPglWfwY5e2D+S/VuzbVYLDzY+nQuylzDnNAQfk9dwGltTqvTNVzl6qd2qX/bZqNkscCZz8Pu+bB/vbEcZtRDZkflf1xLYPpfXu8xAWZyJfAs9myunDmRjKL92Cw2rul5DTf1valGMjCnyFjyEhkSAENvgrR1sOpj+OJauHE2tKz5fdNqsTI0figfx33M7OTZvLziZbbnbOeF5S8wffN0njz5yaok5vG4EqIOLy6DKS6r4O0/jZ8Jt4zoWKP60xdtzNpIVnEWofZQ+kX3MzscqdSqVStsNhvp6ek17k9PTz/ufMWCggI+++wzHnvsseM+T4cOHWjVqhXbtm07YqJRHTYiItLk7FsJTgdEJEJEvNeffsF2I9F4Uid11ZnNpxON4gV/WQSzJHUJk/+czP6i6s2MPVr2YEzbMYxIHEF4YHiNh5dUlLBy/0oWpS5iUeoiMosyWZi6kIWpC3lt1Wtc0/Mazu98PqEBh1fYOZyOqtbpo22c3nOgkNs/W8nq5Oyq+xKbhzC+VxzjesXROqrmdSucTtan5DB/WybztmWyPaOA1cnZrE7O5rU527nihLbccHJ7YiJqX9njFwLDYOwT8L9rYN4L0G9ivZf7dMrN4OqcXN6NiuSpxU8xNH4oYQG12zxdUFLO0l3G9tVTu8bU6/kbtWbRRrLxf1cb/5+6nVHvhTtN0oHtRqLWYoW+E82Opl7sVgtYCwlp8x4ZRftpF9GOp095mp4tD1/k5Eo0RoUGVM76fN7Y5Ld3CXx6KdzwGwRHHvY4i8XCaW1O49TEU/l+x/e8uupVUvJTuHbmtVzT6xpu63fbcSvPbSbMaPx0yR4y80tJbB7iF9vqXW3TQ+OHHvdNNfGewMBABg4cyKxZszj33HMBcDgczJo1i9tuu+2Yj/3f//5HSUkJV1xx/LEMe/fu5cCBA8THe/8XKREREZ/kWgST6P1qxoKSclbuyQbgpI5KNJrN7xKNc+bMMTuExqUy0Vge1YbXV77C22vexomTNuFtuLjrxYxqM+q426DbRLThnE7n4HQ62Z69nT/2/sEnGz8hvTCdZ5Y+w1tr3uKKHldwabdLa8wKSytIo6i8CLvVTlLE4e1E367ex/99tZa8knIigu1cfkJbzugVT6/WEcfcQto6KoTTKxcIpOYU8eeWTKYt2MWG1FzemruDafN3cdGgRG46tSNJLerXYuyTepwL7U+BnXPh5/+DS/9bv+ukr+Xv2bnMbJVISmE6r6x8hfuHHL6l80gWbj9AWYWTNi1CadeyEf23daee58LGC2Ddl/D1zfD3uRDQyBLfnrLqE+O242kQ4dtttUdT7iwlJPEjbEH7aRUczdunv01c2OFVViXlFRSWGtXbUSGVSUF7EFzyMbw90kg4fnkDTPwMrEceUWCz2jin0zmMajOKfy/9N19v+5r3173P/JT5TBk+hS7Nuxw1TlvVjMZjV7S7S0l5BW/+YVQz3jyiIwE2q1eetyE0n9F3TZo0iauvvppBgwYxZMgQXnzxRQoKCqq2UF911VW0bt2aKVOm1Hjcu+++y7nnnnvYgpf8/HweffRRLrjgAuLi4ti+fTv33XcfnTp1YuzYsV77ukRERHyaifMZl+zMotzhJKlFCG30e6jpfP+VvHjWwV3ss9u4Nnc5b615CydOLuh8Af+b8D+u7nn1cZOMh7JYLHRq3onre1/PTxf8xMMnPkxis0QOlhzklZWvcOZXZ/Ld9u9wVrbiVW2cjmhHgLW6GqSwtJx//G81d3y6kryScga3a85Pd53CP8d1o3di5DGTjH8VHxnCxYOT+OGOk3n/msEMbNuc0goH/128h5HPzuG5XzZTUn7sVmy/YbHA+H+DxWYshdn6W/2uk7aWEKeTh7tdCcAnGz9hbcba4zzIcGjbdF3+PzU5ZzwLYTGQuRl+f9zsaPzHhm+MWz+tZnQ4HTw4/0HsYTtxVgTx1EkvHTHJCNXVjBYLhAcf8p5geKzxJoI9GLb+ArOO3+LZLLAZj530GC+NfIkWwS3YcnALl35/KR+s/6Dq+/FfeXtG4xfL95KWW0x8ZDAXDqz9zx2z5JbmsjpjNQAntT7J5Gjkry655BKeffZZHn74Yfr168eqVauYOXNm1YKYPXv2kJqaWuMxmzdvZt68eVx//fWHXc9ms7FmzRrOPvtsunTpwvXXX8/AgQP5888/1R4tIiIC4HQesnHavPmMqmb0DUo0NnGzcrdyYUI8q4pSaRbQjP+c8h8eGfbIEVud6yLQFshFXS7iu/O+4+nhT9MhsgPZJdk8MO8Bbp51M/vy97Ejx6he6RBZvQhmc1oeZ70yj/8t34vVAneM6synN55A66iQBsVjsVgY2S2GL246kc//dgInd2pFucPJK79v48yX57F8d1aDru8zYrobs9wA/r+9+46Pqs7+P/6amfTeIAUChN47IqBiQcCKvbEqrGID63fV1Z+9LOpiW9e1YMGObW2oWGiu0puC9F5DgJDeZ+7vj5sZCCSQkHLvJO/n45EHw8ydO2f2uuEzZ87nnOn3QllJzZ5fnAuZ5nUZ3Pkyzm17LgYGj857lFJP6VGfahgGs9eZW+7Vn/EYwuLg/JfM2/Nehq1zrY3HHxzYCvvXm4n0DmdaHc1xmbR4Ej9s+QHDcFG442raRLav8tic8kRjVEjgkc2sU/rAqJfN27+9ACv/W63XP73V6Xx+/uec2vJUSj2lTFo8ibt/uZuC0oIjjm3oqdPvzTP7BY87uS3BAfYfIjV/13zchpu06DRaRNh/m3dTNGHCBLZu3UpxcTELFixg4MCBvsdmz57NlClTKhzfqVMnDMPgzDOP/P0SGhrKDz/8QEZGBiUlJWzZsoXXX3/9iMnWIiIiTVb2dsjbA84ASO7V4C//28b9AAxWf0ZbUKKxCVu4dDL/F1RArstJz5hOfHrep4xMG1mnrxHgDOCctufw2fmfcVuf2wh0BvLbzt+44KsL+O9688OxdxBMenYRV7+5gE1780mKCuHDcSdy15kdCajDLXQOh4OBbeN577oTePmqviREBLEhI49LXp3Hw1+tJK/4yCnWfufUe81quf0bYP5/avbcPeVTwiJTIDyeuwfcTXRwNGsPrOW9Ve8d9alb9hewPbOQQJeDQe2OnGAuh+k0Evr8BTDgy5vNKW1StY0zzD9TT6i0L6Hdvfvnu77/D3n2XI67oP1R+x9mFRwyCKYyPS4xp80DfDXeHBRTDQmhCfzr9H/x4IkPEuAM4IctP3Dt9GvZnVexusvlNH/vNkSicW16LmvScwl0Obi4r/2rGQFNmxYRERE5lLc/Y1IPCKxdkVBN7c8rZvXuHAAG63OoLSjR2ERt3/4bd/3+Im6Hg7MC4ply3kc12iZdU4HOQMb1HMdn539G3+Z9KSwrPFjRGNOWolI3N7y3mIzcYjomRvD97SdzYtv6+yXhcDg4p2cyP981lEv6tcQw4J15Wxn+3BwWbvbz6saQaDjzUfP2nGcge2f1n5v+h/lnUg8A4kLiuLv/3QC8svwVtudsr/Kpc9aa1YwD2sQRHux37V+tMWIiRKeavVJ/0gTqo9pQnmhsf+R0V7v7Y+8fTFo8CYC7+t2Fq6AvcPQknjfRGBN2lCEjZzwCbU+D0gKYehUUVO93l8Ph4LJOl/Hm8DeJC4ljTeYarvj2CpbuWeo7JqABt05//bv5O2pox+ZEH+392oRhGPy681cATkpRolFERESEHUvMP1s0/LbpeZvMasbOSZEkRKiliR0o0dgE5eXu5tafbibb6aC7J4DHLvqiQo/E+tQ2ui1vj3ybBwY+QHhgOC6Hi+7x3bn7sz/4Y0c2sWGBvHHNAGLDjz4Rta7EhAUx6dJevH/dQFLjQtmVXcSVk+cz+ZdNVfYu8ws9r4DUgVCaD9OrN8gFgPTyXozliUaA89udz8CkgRS5i3h8/uNV/u9yaH9GqaaQKLigvOp08Vuw4Tj7ajZ27lLYNMe83X6YtbHUkMfwMHHBRAwMzml7DmO6jcHlOnYSz9ujscqKRgBXAFzyFsS0hqyt8NlfwV39quy+iX2Zes5UOsd1JrMok+t+vI7P1n0G4NuuXd8VjYZh8PXvuwAY1ds/Bvysz1pPRkEGIa4Q+iVparyIiIjIwYnTDT8I5rcN5dum1Z/RNpRobGLcZSXc+8VFbHQZNHcbvHj2e4SExjZoDE6Hk8s7X873F33Pl6O+5MtFhXzz+y4CnA5e+Us/S6ZEndQhgem3n8Ko3im4PQZPfream99fSm7R0fsS2pbTCec8Z/azW/01rPuhes/bU779Mqm77y6Hw8FDgx4i2BXMvN3zmLZp2hFPKyp1+75JGtpJicYaSTvlYF/NryZA4QFr47Gj7QuhJBfCEiCp4Xu+1MZXG75i5f6VhAeG87f+f8PhcOByHDuJl1WdRCOY/T6v+BACw2DTLJjxaI3iS45I5p2R7zC89XDKPGU8Ou9RXljyAuW50HqvaFy2PYvtmYWEBbkY1sU/+t15p033T+pPsEvfmouIiEgTV1YMu80heZYOgmmvbdN2oURjE/PiV1fwi5FHsMfgxRMfpnli92M/qZ7EhsSydkcIk35cB8Cjo7rV63bpYwkPDuCFy3vz+KhuBLocTP8znfP//Rtr0nMsi6lWkrrDoFvM29/9DUqOHPhQgbsM9vxZ/tyeFR5qFdWKm3qZybBnFj3D/sL9FR5ftCWTolIPiVHBdEqMrJPwm5QzHob49pC7G767x+po7Mdb6dnudDOJ7idyS3J5YekLANzc62YSQs1vWV3VqBb0VjQedeu0V1L3g8Nh5v4LVnxWozjDAsOYNHQSt/Q2f1+8ufJNfs36D+DGU8+Jxq+Xm9WMw7smEhpk/yEwcDDRqP6MIiIiIpi9wt3FEBoHcW2PfXwd2p5ZwLbMAlxOByekxTXoa0vV/OcTm9TaN7P+H2/nrQfg0bYX073rpZbGs3p3Dnd+vByAawa1ZvTA1pbGA2b13tWD2vDJjYNIiQ5h8758Lnj5N6b9scvq0I7P0L9DVEvI2ga//PPox2ZuhLIiCAyH2LQjHr6227V0iu1EVnEWTy18qsJjs9ce3DbtcDiOeK4cQ1AYXPgaOJyw4pNqTxFuMryJRj/bNv3K76+QWZRJWnQaV3W+ynd/dSY6ZxeYE+OPWdHo1f0iGHKHefurCQfbIFSTw+Hg5l4388igR3A6nKzJn0FIy/cpdhfX6Dw1Ueb2+H63jurtH5ObC0oLWJJh9iBSolFEREQE2LnY/LNlf2jgz4JzN5rVjL1TY4gMsX+v76ZCicYmYvv2eTyy9SsAxkV25pyhNdteV9dKyjyM/2ApBSVuhrSP58Fzu1oaz+H6tIpl2m0nc3KHBIpKPUz4cBmvzN7of30bgyPg7GfM23P/BRmrqz7Wm5hI7FZp1VigM5DHhjyGy+Fi+pbpzNg6w/eYtz/jqZ2a11noTU7L/nDy38zb0+6EHD9Nbte1vIyDQ4ranW5tLDWwMWsjH63+CIC/D/g7ga6DC5+DPRo9VT7fu3U6JrQG/WrPeAjanQFlhTB1dLWHwxzq4o4X89ypz+FyBBIYuZolxU+TU1I/Vd3zNu1nX14JsWGBnNTBP3rqLNi9gDJPGS0jWtIqspXV4YiIiIhYzwb9GYdo2rStKNHYRLw4515KHA5OMIKZMOojq8PhgwVb2bQvn4SIIF6+qi+BLvv9pxgXHsSUsScwdkgbAJ6evoYHvlxJmbvq5IAtdT4HOp0NnjKYdhdUlSytZBDM4brGd2Vs97EAPLHgCbKLs9lxoIANGXm4nA6GtPePZIFtDb0HUvpAURZ8eQscJRHVZGycaf6Z3Asi/KP/p2EYPLXwKcqMMk5LPY3BLQZXeDygPJFfna3TNZrC7HTBxW8cHA7z+XXgcdc4/jNancHFKY9iuEPIMtYyZvoY9hbsrfF5juWr8m3T5/RMtuW/AZX5bZe5bXpIiyGq3hYRERGBg4nGFg07JM8wDOZuLB8Eo8+htuIfK3upleUrP+QH9wEchsE9Qx7F6QqwNJ7sglJenGFu4b7rzE7EhDXMhOnj4XI6ePi8bjx0blccDvhgwTauf3cxecXVn+xqC2c9bQ6L2DYXln9Y+THVSDQC3NTrJtKi09hXuI9/Lvonv6wzy9X7pMZUf5unVM4VCBdNhoBQc7DHwtetjsh6frhteua2mczfPZ8gZxB3D7j7iMe9PRqPNmglq6Caw2AOd+hwmI0zYebjNXt+uTbhPSjYeiOBRLP+wHrG/jCW9Pz04zpXZYpK3UxfaZ7v/F7+sW3aMAx+3fkrACe3ONniaERERERsIH8fHNhi3m7gROO6PXnsyysmJNBJn1YxDfracnRKNDZyhsfDpEWTALggOIlOHc6xOCJ4efYGsgpK6dA8gsv6t7Q6nGr560lpvPqXfoQEOpm9di+XvzaPPTlFVodVfTGt4NS/m7d/fADy9x95jC/R2PPIxw4R7ArmscGP4cDBVxu/4su15hbqoR39o9rM9hI6wPDy5NDPD0PGGmvjsZLHc7Ci0U8SjUVlRfxzsdkPdUz3MaRGph5xTHWmTuf4tk4fR/I+qTuc/5J5+9fn4c8vanwKl9OJpziZ7txPi4gWbM3ZytjpY9mVVzdb+metySCvuIyU6BD6t46tk3PWt605W9mZt5NAZyADkhp+a5CIiIiI7ewo78+Y0AlCYxr0pb3Tpge0iSM4wD+GCjYVSjQ2cj/+9iS/O0sJ9RhMOP0Fq8Nhe2YBU37bAsD953QhwE+2ywGM6JbE1BsGkRARxJ+7crj4lbls2ZdvdVjVd+It0LwbFGbCD/dXfCx3D+RnmMNImnc55ql6N+/N6C6jAVhV+hY4ixjaSYnGOjPgejOxVlYE/70eykqsjsgau5dDwX4IirSk58vx+HLDl+zM20liWCLXdb+u0mOqM3Xa16PxeCu+e1wCg28tD2o87FlVo6d7B9YEGs14e8TbtIxoyY68HYydPpbtuduPL6ZDeLdNn9c7BafTP7YgL95jLqR7N+9NWGCYxdGIiIiI2ICl/RnNRKPad9mP/2R5pMZKinN5fv0nAIyJ6UHzxO4WRwRPTV9DidvDSe0TONUPK+B6p8bwxS1DSEsIZ8eBQi59bR5r0utnUEKdcwXCeS8CDvhjKqz/+eBje8qrGePbmxOQq+HWPreSGJqCIyCLiOTpdEuJrvuYmyqHA0a9DKGxZqXp7H9YHZE1NpQPHGo71Pzv1+YMw+CjNWYP3LHdx1aZjApwHT3RaBjGwR6NtWlHcMYjkDYUSvPh49FQeKDaT3Uesr07OSKZKSOn0CaqDbvydzF2+li25mw97rByikqZuTYDgFF+sm0aYMU+8/dkr2a9LI5ERERExCZ8E6cbdtt0mdvDgs3m4MMh7ZRotBslGhuxj37+P3a6oJnbYMyIl6wOhyVbD/DtH7txOOD+s7v4bSP91LgwPrlxEJ2TItmbW8zlr81n2bbqf4C3VOoAOPFm8/a0O6A417xdzf6MhwoLDOOMhAkAOKLmszB9fh0GKkQmlSeGgV9fgC2/WhqOJfysP+Oi9EVsyt5EaEAo57c7v8rjjtWjMa+4zJeEjKnJMJgjXigALnkboltB5ib4fFy1h8MEHFZ1mRieyFsj3qJtdFv2FOxh7PSxbMredFxh/bAynZIyD+2bR9AlOfK4zmGFP/aa08+7J1j/pZ2IiIiI5Txu2LHEvN3AFY0b9uaRV1xGeJCLrilRDfracmxKNDZSWQc281rGXABubXUWYWHWZvkNw+DJb82te5f2a+n3vwyaRQbz8Q2D6NsqhuzCUka/sYC5G/dZHVb1nP6A2bMxezvMKO8F6E001rDqNSuzNSWZJwLw0NyHyC3JrctIpeso6P0XwID/3lCjijS/V5h1cCtG+zMsDaW6pq6dCsB5bc8jMqjqBNrBJF7lU8W9g2CCApyEBNay30x4PFzxvjlgaMNPMOvJaj3tYDL0YIzNwprx1oi36BDbgb2Fe7nuh+vYkr2lxiF9/bu5bXpUrxS/+cIpvzSfjVkbAeiZcPQ+tiIiIiJNQuZmKMk115nNjt1+qy6t2JENQLcW0b51q9iHEo2N1Gs/3Uau00FHj5PzT63eB8v69N2KdJZuyyI00MX/De9kdTh1IjoskPeuG8hJ7RMoKHEz5u1F/LRqj9VhHVtQ+MFKuYWvw7YFkL7S/PsxBsEcbvn2LIozziY+OIX0/HSeXvh0HQcrnPU0xLWDnJ3wze1gVN3Xr1HZPAcMNyR0NBPjNpeen87Mbebgmis6X3HUY49V0Zhdm0EwlUnudXA4zP+ehVVfHfMp3mTo4bnQ+NB43hz+Jh1iO7CvcB/X/Xgd23Oq37OxoKSM+ZvMYVRn90yu9vOs9ue+PzEwSApPolmY/7X9EBEREalze1ebfzbraO6kaUArd5qJxh4t1L7LjpRobIS2b5/H1ILNAPxfjxtxBRznMIE6Uub28PR0c3LuDae0JTEqxNJ46lJ4cABvXNuf4V0TKSnzcPP7S/h+xW6rwzq2dqdD79GAAV+Nh/3rzftrsHU6r7iMdRm5YATx0MCDU6hnbZtVPzE3VcERcPEb4AwwE0TL3rM6oobhZ9umP1v3GW7DTb/EfnSI7XDUY481DMaXaKzNtunD9bwUBpmtDvji5mMOh6msotErNiSWyWdOpl10OzIKMvjrj39lR+6OaoWxcHMmpW6DFjGhtE0Ir9l7sNAf+8xt0z0Sqv87UkRERKRRyzA/4zd0NSPAivJEY8+WSjTakRKNjdCnC56hzOHgREIZ3P8Wq8Nh5poMtmUWEBcexA2ntLU6nDoXEujiP6P7ckHvFMo8BhM+Wsa0P3ZZHdaxDX8CwpubSUbDY96OTKz20//YkYVhQEp0CKenDWRMtzEAPDrvUQ4UNaEtvg2hRV84/UHz9vf3wr711sbTEDbONv/0g23Tpe5SPl//OXDsakYAl9P8p7eqRKN363StBsFUZtijB4fDTL3qqFvxj5UMjQ+N540Rb9Amqg3p+elc/+P17M479pcsczea1YxD2sf7zbZpgBV7zfYS2jYtIiIiUs5b0di8c4O+bJnbw6rd5kDW7qpotCUlGhuZkuJcvsw1kxBXdbzM4mhMHy7cBsCl/VsSHtywJdUNJcDl5NnLenNR3xa4PQa3fbSMr5bvtDqsowuLg7P/efDvSTXrz/j7dvNbpN6tYgAY32c87WPas79oP4/PfxyjqWzxbSiDb4O0U6C0AD77K5QVWx1R/cnZDdnbwOGE1BOtjuaYZmybwb7CfTQLbcYZrY6dGA2o5tbp6NA6rkY/dDjMgc3w+fVVDoc51vZugITQBN4c8SatIluxM28n1/14HXvyj94+4rcNZi/bIe39azrgyn1me4kezVTRKCIiIgJYVtG4YW8eRaUeIoIDSIv3nx0yTYkSjY3MjPnPcsDpoLnb4OT+E6wOh+2ZBcxZtxeAKwfYv89abbicDv55SS8u7dcSjwF3frycL5ZVbzuhZbqOgs7nmrdbnlCjpy7fblZD9U6NASDYFcwTJz1BgCOAn7b+xPebv6/LSMXphAtfg9A4SP8DZj5udUT1Z2f59LrmXc2t4zb30ZqPALik4yUEOo9dhXisasGswhKgHioa4bDhMD9X+d9RwDGqLr2ahzXnzRFv0iKiBdtzt3P9j9ezr7DywViZ+SX8ucv89nlQu/havImGlZ6fTkZhBi6Hi67xXa0OR0RERMR67rKD7bcauKLROwima0oUTg2CsSUlGhuZTzdPA+Ci2B4EBFrfC/HjRdsxDHObXBs/6sd1vFxOB09f3JMrBqTiMeCuT37nsyU2TjY6HHDRZLj4TRh8a42eunx7FgC9U2N993WL78YNPW8A4MkFTx6zuklqKCoFRv3bvD33pYN9DBubnYvNP1v0tTaOalh3YB1LM5bicri4uMPF1XrOMSsaC+qhR+Ohknsd/O/o1+dhxWdHHHKsZOihksKTeGvEWySHJ7MlZwvjfhxHVlHWEcfNK9823SkxkuaR1v/7VF0r9pnbpjvEdiA0INTiaERERERsIHMTuEsgMMzcLdOAvINgemrbtG0p0diIbNkyh0WOYpyGwUUD/2Z1OJS6PXyy2JxGetUJrS2OpuE4nQ7+cWEPRg9shWHA3Z/ZPNkYFAY9LqlR5dju7EL25BTjcjro3iKqwmPX97yervFdySnJ4f/99v/wGEcOk5Ba6HwODLjevP3fG81txo3NDm+isb+1cVTD1DVTATi91ekkhlevx6n3m1e3u/L/b9T51OnK9LgEhtxh3v5qAuxaXuHhmiQaAVIiUnhj+Bs0C23GhqwN3PjzjeSW5FY45reNZqXj4Pb+U80IB/szahCMiIiISDnfxOlO5s6rBuQdBNNDg2BsS4nGRuSzRc8DcJIzkuSUfhZHAzNWZ5CRW0xCRBBndq3+kJHGwOl08MQF3bn6xNa+ZKPtt1HXwO/l1YwdEyMJC6rYdzPQGchTJz9FaEAoC3Yv4L1VTWRKckMa/qQ5IbxgH/x3XJV99vySxw27lpm3W9o70Zhbksu0TWYV+ZWdr6z287wVje4qcni+YTD1VdHodcZD0P5MKCuEqaMhb6/voer0aDxcq6hWTB4+mdjgWFbtX8X4GeMpKC3wPe7rz9jOv/ozauK0iIiIyGEs6s+oQTD+QYnGRqK4KJuv8jYAcGnHSyyOxuQdAnNJv1SCApref2oOh4NHz+/GVeWVjf/3ye/2HxBTTct826ZjKn08LTqNewbcA8ALS19gTeaaBoqsiQgMgUumQFAEbPkfzHnG6ojqzr51UJIHgeHQrGH7vdTUNxu/obCskPYx7emfWP2k6MFqwaNXNNZLj8ZDOV1w8RsQ1w5ydsAn10CZ2R8yoIYVjV7tYtrx2pmvERkUybKMZdw+63aK3cXsOFDA1v0FuJwOBraNq/O3Ul/KPGWs2r8KUKJRRERExMeiidMaBOMfml72p5GaseA5spwOEt0GJ/Ubb3U4bM8s4H/ry4fAnJBqcTTWcTodPDGqu69n450fL2faH7usDqvWlm/LAqBPFYlGgIs7XMzpqadT5inj3l/upbCssGGCayoS2sO5L5i35zwNm+ZYGk6d8W6bTuljJsJs7KetPwFwYfsLcTiq34j6WD0asxoq0QgQGgNXToXgKNg2F6bfC9R86/ShusR34ZVhrxAaEMr83fP5v9n/x//Wm/1ae7WMJjKkAd5XHdmYtZHCskLCA8NJi06zOhwRERERe7CootE7CKabBsHYmhKNjcSnm78F7DMEZuqibRgGnNQ+gdZN/JsGb89G7zTq26cu5/sV/ttXz+0xfH0xeh0l0ehwOHhk8CM0C23GpuxNPLv42QaKsAnpeSn0vQYwzC3UeRlWR1R73kEwLa1v/3A0B4oOsDRjKWD2Z6wJl3eicxV7p7MLzKrCmLCgWkRYA806mkOhcMDit2DhZAJcNd86fahezXrx8hkvE+wKZs6OObyx9knAw5D2/rltunt8d1w2T3yLiIiINAh3Kew3d1M2dEWjdxBMD22btjUlGhuBTZtnstg7BObEe6wOp3wIjNmP8KqBDTuByq6cTgdPXdyTi/q2wO0xuPWjZfz4Z7rVYR2X9Rm5FJS4CQ9y0b750QfIxIbE8sRJTwDw8dqPmb19dv0H2NSMfBqad4W8PfDfG6CK7bh+Y+cS888W9k40/rLjFzyGh06xnWgZ2bJGzz3m1OmGGAZzuE4j4YwHzdvf30vEzrlA1du7q2NA0gCeP/V5ApwBZHgWEJz8Xwa1859t03DIIJhm2jYtIiIiAsD+jeApNds4RTfs7sU/NAjGLyjR2Ah8vvhFAE52RpKU3MfiaGDG6j3sLR8CM6xL0xoCczQup4N/XtKLC3qnUOYxGP/hUmat9b8KNO+26Z4tY3zbK49mcMpgrul6DQAP/fYQewv2HuMZUiNBYXDJ2xAYBptmwf8mWR3R8SspgD1mPzy7T5yeuW0mAKe1Oq3Gz/X+/8ZjHJloLHV7yC8xh/s0yNbpQ510F/S4FAw3yT/eSGtH+nFXNHqd3PJkbu/xCIbhIChmMbP3voFRyfu2qxX7NHFaREREpIJDJ07XoH1QbZW5PawuHwSjikZ7U6LRz5lDYDYCcGnHSy2OxvTBAnMIzKX9m+YQmKNxOR1MurQX5/RIptRtcON7S/h1/T6rw6qR5d5BMK1iqv2c2/veTqfYThwoPsB9/7sPd2OakmwHzTvDOc+Zt2f9AzbOtDae47V7ORhuiEyG6BZWR1OlwrJC5u4yK/5OT63Ztmk4+kRnbzUjQFRDJxodDjj/JWjRD1dxFm8GTiLMk1fr03ryelK02xxS9tHaD3l5+cu1PmdDyC/NZ2OW+e9rz2Y9LY5GRERExCYs6s946CCYNk28PZvdKQvk52YseI5s7xCY/hOsDqd8CIyZOLtygLZNVybA5eSFK3ozvGsiJWUern93EfM37bc6rGrzJhp7tYyp9nOCXEE8M/QZQgNCWZC+gNdXvF4/wTVlva+EfmMAAz67DrK2Wx1RzfnJtun5u+ZT5C4iOTyZznE170tztInOWQVmojEyJKBaFcN1LjAUrvgQd0Qy7Z27mMSL4C6r1Sl/27CPsux+nBJ3AwCv/fEab698uy6irVd/7vsTA4Pk8GQSQv2rt6SIiIhIvbFo4rQGwfgPJRr93M/bZgBwfkwXXAENNDjgKH4o7zs4MC2OVvFhFkdjX4EuJy9d1YfTOjWjqNTDX6csYvGWTKvDOqb84jLW7ckFoE8NKhoB2ka35cETzR5wr/7+KovSF9V1eDLyaUjuDYWZ8Om1UFZsdUQ14504bfNE48zt5dumU0+r0bRpL19FYyXDYLILvYNgLJzMHJlE1qh3KTSCONn5O/z04HGfqsztYcFm83fbzX2v4fa+twPw3JLn+GTtJ3USbn3xDoLRtmkRERGRQ1g1cVqDYPyGEo1+rKQ4l9/KsgA4rdNl1gZTbsZqs+fgmV3Vm/FYggNcvPKXfpzcIYGCEjdj3l7kqxa0qxU7s/EYkBwdQmJUzaebn9fuPEa1G4XH8HDvL/eyv9B/Kjn9QmAIXPYuhMSY1YE//D+rI6oZb0VjS/v2Z3R73MzZPgeo+bRpr4MVjUcOWjk4CMbaL448Sb34v9KbzL/M/w8smXJc5/l9RzZ5xWXEhAXSNTmK63tcz/U9rgfgiflP8M3Gb+oo4rrnHQSjbdMiIiIi5cpKINNsLdPgFY0aBOM3lGj0Y4tXvEeB00GC26Bb5wutDofswlIWlVflaQhM9YQEunj96v6c2DaOvOIyrn5zASvLf4Haka8/Y2rMcZ/j/oH30y66HXsL93L/r/fjMfx8SrLdxLaGi98AHLBoMvxh76oxn9w9kL0dcJhVmTa1fO9yDhQfICooir6JfY/rHM6j9Gj0bp1u8EEwhwlwOvjOcyLPlZq9Ffn2/2DjrBqf57cNZiuNwe3ife/7tj63cVXnqzAwePC3B5mxdUadxV1XDMPQIBgRERGRw+3fAJ4yCI6CqIbrqa5BMP5FiUY/NmfTdwCcEpqM0xVgcTTwy7q9lHkM2jULp02CmrNWV2iQizevHUD/1rHkFpXxlzcX+H6J2s3v3v6MtUg0hgWGMWnoJEJcIczdNZe3Vr5VN8HJQR3OhKH3mLe/uf3gJGc781YzNusMIVHWxnIU3mnTp7Q8hUDn8SUDA44yddqXaLRy6zTgcpkx/st9Ie5ul5gLyk+uhb1ra3Seg4nGgz0OHQ4H955wL6PajcJtuPnbL3/jt52/1V3wdWBPwR72Fu7F5XDRJb5htwWJiIiI2JZFE6c1CMa/KNHopwyPhzl5WwEY2vpMi6MxzVi9B1A14/EIDw7g7bED6J0aQ1ZBKaPfWMD68l6IdlIXFY0A7WPbc//A+wH497J/s2TPklpGJkcYei+0Ox1KC2DqVVBg8x6gO8v7M7a0b39GwzCYtd2s6jvebdMALqf5T2/lPRrtU9FoclByzr8g9UQozoYPLoW8vdU6R1Gpm2XbsgA4qX3FYSpOh5NHBz/KiDYjKPOUccesO1icvrgO30Ht/LHX7M/YIbYDoQGhFkcjIiIiYhO+/owNu236Dw2C8StKNPqpDZt+ZKcLggyDE3v/1epwKHN7mLXW/PB5hhKNxyUyJJB3/noC3VtEkZlfwpWTF7Bxb57VYfnsySlid3YRTkfdlKtf0P4Czml7jlnRNOdv7C2oXvJCqsnpgovfhJhWcGAzfH5dracH1ys/mDi9IWsD23O3E+QMYkjKkOM+z9GmTh/s0WhtotF5yDfUZc4guOJDiG0DWVvNxHVp0THPsWp3DiVuDwkRQbSuZDiYy+li4kkTOaXlKRS5i5gwcwIr962sy7dx3FZnmt/Wd4vvZnEkIiIiIjbimzjdsDs+vO3Feqo/o19QotFPzVn1EQADnRGEhSUc4+j6t2TrAbILS4kJC6RvDacRy0HRoYG8f91AOidFsi+vmKsmz2fLvnyrwwLMpAFAu2YRhAfXfqu+w+HgoRMfon1Me/YV7uNvc/5Gqae01ueVQ4TFwRUfQWAYbJwJMx6xOqLKeTywc6l5u4V9B8F4t02fmHIiYYFHJs6qy3WUHo2+RKPFW6cDDvmm2O0xIDwervoUQqJhx0L46hbzuh3Fih3eBWFMldO5A12BPDv0WU5IOoH80nxu/OlG1mbWbHt2fdiQtQEwKxpFREREpJxFFY3eQTDd1Z/RLyjR6Kdm7zeb1J+aONDiSEwz1pjTpk/r1JwAl/6zqo2YsCA+uH4gHZpHsCfHTDZuzyywOizfVu6OiZF1ds6wwDCeP/V5IgIjWJqxlOcWP1dn55ZySd3hgv+Yt+e+ZM/hMPvXQ3EOBIRC865WR1Ml37bp1OPfNg0Q4Kq6ojGroASwfuu065BEoy8h2qwjXP4+OANg5ecw68mjnsO7xeVYFdAhASG8dPpL9GrWi5ySHG746QY2ZW2q3RuoJe/rt49pb2kccvxefvll2rRpQ0hICAMHDmThwoVVHjtlyhQcDkeFn5CQkArHGIbBQw89RHJyMqGhoQwbNoz169fX99sQERGxj7JiyCxfozVgRWOZ28OqXRoE40+UEfJD+/et4w+H+WH0lF5jLY7G9HN5f8YzujS3OJLGIT4imA/GDaRts3B2ZRdxxevz2XHA2mTj+j3mNu4OiRF1et420W148iQzYfH+6vf5rnzIkdShbhfCyf9n3v76Vti13NJwjuDdNp3SG2ww2Koy6fnp/Ln/Txw4GJo6tFbn8m5LLqukIjDL16MxqFavUVsOh8OXbPQcmhBNOwXOe9G8/b9JsPjtKs+xYmcWUL0tLmGBYbwy7BW6xnclsyiT63+8nm052447/tooKitie+52ANrFtLMkBqmdjz/+mLvuuouHH36YpUuX0qtXL0aMGEFGRkaVz4mKimL37t2+n61bt1Z4/JlnnuFf//oXr776KgsWLCA8PJwRI0ZQVHTsNgIiIiKNwr71YLghOBoikxvkJf/clc1N7y+huEyDYPyJEo1+6H+/v4nhcNDF4yIpqbfV4bB5Xz6b9uYT6HJwSsdmVofTaDSPDOGjcSeSlhDOzqxCrpq8gF1ZhZbFsy7DTDTWZUWj1+mtTmdcj3EAPDLvEdYdWFfnr9Hknfb/oMNwKCuCqaOrPdCjQewoHwJi4/6Ms7fPBqBXs14khNauXcXBHo1HPpZTnmiMCrU+4VrlFu8+fzGHDQF8exesnX7Ec/OLy9hQ/jujut88RwZF8tqw12gf0569hXu5/sfr2ZW36/jfwHHanL0ZA4Po4GjiQ+Ib/PWl9p577jnGjRvH2LFj6dq1K6+++iphYWG89dZbVT7H4XCQlJTk+0lMPNhv2jAMXnjhBR544AFGjRpFz549effdd9m1axdffvllA7wjERERG9hbvm26eed6nzi9Jj2Hm99fwjn/+pWfV2fgcMBtZ7TXIBg/oUSjH5qz6zcAhsY0bAPWqninTQ9MiycqxNrtfo1NYlQIH44bSKu4MLZlFnDV5PmkZzd89YRhGGwo3zrdoXndVjR6je89nkHJgygsK+SOWXeQU5JTL6/TZDldcPEbEN8ecnbAJ1eb2x/swDdx2r79GX/Z8QsAp7U6rdbncvkSjUdmGvOKzYE9dvhd6nJUvcWbU++D3qPB8MBnYw9WpZZbtTsHjwFJUSE0jwo58vlViAmJYfLwybSJasPu/N1c/+P1ZBRUXYVWHzZmbwSgXXS7KntLin2VlJSwZMkShg0b5rvP6XQybNgw5s2bV+Xz8vLyaN26NampqYwaNYo///zT99jmzZtJT0+vcM7o6GgGDhxY5TmLi4vJycmp8CMiIuLXMsoHwdRjf8Z9ecVM+HApI1/4H9+vTMfhgPN6pfDTnadwwynaaeIvlGj0MyXFucwtywLg1M6XWBtMOW2brl/J0aF8dMOJtIwNZct+M9mYkdOwycZd2UXkl7gJcDpok1A/5eoup4unT3ma5PBktudu577/3Yfb466X12qyQqLN4TDB0bBtHnx9GxiVJJEaUmkh7Cn/QG/Tika3x82yjGUAnJh8Yq3P5+3RWNkwmLwiM9EYUQcDl2or4ChDa8xV34vQ7nQoLYAPLjvYs4eDg2B6HMdkwITQBCYPn0yLiBZsz93OdT9cx77Cfcf3Jo7Dxiwz0aj+jP5p3759uN3uChWJAImJiaSnp1f6nE6dOvHWW2/x1Vdf8f777+PxeBg8eDA7duwA8D2vJuecOHEi0dHRvp/U1NTavjURERFr+Soa66fgaW16LqP+/RvT/tgNwDk9kvnhjlN46co+tG9e97vqpP4o0ehnFv3xDgVOB83cBl06jrI6HLILSlm05QAAw7okHuNoOV4tYkL5aNyJtIgJZdO+fK5s4GTjuvJqxrSEcALrcdhPbEgsz5/2PMGuYH7Z8QsvLnux3l6ryWrWES6bAg4X/DEV/vestfHsXQueMgiNg2h7fhBfn7WevNI8wgPD6RTbqdbncznN/w8dXino9hjkl5jJ9YgQ6xONLlfVlZfmAYFw2buQ1AMK9sH7l0D+fuDgZMCex9mwOyk8iTeGv0FSeBJbcrZw/Q/Xk1mUeVznqinvxGn1Z2w6Bg0axDXXXEPv3r0ZOnQo//3vf2nWrBmvvfbacZ/zvvvuIzs72/ezffv2OoxYRETEAvVY0ThrTQYXvzKXnVmFtIkPY9qtJ/Hy6L710rZL6p8SjX5mdvmgjFNCU3DaYGjC7HUZuD0GHRMjSI0LszqcRi01LoyPxp1ISnQIG/fmc0UDJhs37Km//oyH6xbfjccGPwbA2yvf5uuNX9f7azY57U6Hs/9p3p75OPz5hXWx7F1r/tm8S733ejleS/aY24J7N+uNy+mq9flcjsorBfNLyny37VTRWFkvSZ/gSBj9mZkkztwIH14GJfn8sSMLOL6KRq+WkS15c/ibNA9tzsbsjYz7cRxZRVnHfb7q8lY0KtHonxISEnC5XOzZs6fC/Xv27CEpKala5wgMDKRPnz5s2GAmnb3Pq8k5g4ODiYqKqvAjIiLit0qL4MBm83YdVjQahsHbv23muncWkVdcxsC0OL64ZQjdNV3arynR6EcMj4c5+eYUzlPTRlgcjWnGarN31hmqZmwQreLD+OgGM9m4qQGTjd6KxrqeOF2Vs9uefXA4zNxH+H3v7w3yuk3KgOvgxFvM21/cBDuWHP34+rK3/nu91JY30dg3sW+dnK/Sac4c3DYd6HIQHGD9P88Hh8EcLdMIRCbBXz6HkBjYuZiyqVezfV/51ulaLhJbRbXizRFvkhCawLoD67jhpxvILs6u1TmPpqisiB255nZZJRr9U1BQEP369WPGjBm++zweDzNmzGDQoEHVOofb7WbFihUkJ5sTNdPS0khKSqpwzpycHBYsWFDtc4qIiPi1/evN3twhMRBRN5/9y9weHvrqTx79ZhUeAy7r35L3rhtIbHhQnZxfrGP9JxmptnUbv2e3y0Gwx2Bgz7FWh0Op28PstWaicZj6MzaY1vHhTL1hUIMmG9eXT4/t0IC9MSb0mcDpqadT6inl9pm3k55feR8sqYXhT0DHkeYk6o+ugCwLtvZl1G+vl9oyDIOle5YC0Ld53SQaq+p96B0EExEcYIshJEcdBnO4Zp1g9KcQGEbAphn8M+BVWkYHEx8RXOs42kS34c3hbxIXEsfqzNXc+NON9TYsyjtxOiY4RhOn/dhdd93F5MmTeeedd1i9ejU333wz+fn5jB1rrp2uueYa7rvvPt/xjz32GD/++CObNm1i6dKl/OUvf2Hr1q1cf/31gDmR+o477uCJJ57g66+/ZsWKFVxzzTWkpKRwwQUXWPEWRUREGtZ+s8qfZp3qZBeSYRj8/b8reG/+VhwOuO+szjx9cU+CbPBlu9SerqIfmbN6KgAnuiIJDYuzOBpYvOUAOUVlxIUH0Ts11upwmpRW8WEVk42v11+y0TAMNmR4t043TEUjgNPhZOLJE+kY25H9Rfu5beZtFJQWNNjrNwneSdSJ3SE/Az68HIrqr1qsUt6m0s1q3/uwPmzL3cb+ov0EOgPp0axHnZzzYO/Digm8XO8gGBv0Z4SDcVY6DKYyqSfAZe/icQQwyjWXx0Ler7NhQ21j2vLG8DeIDY7lz/1/ctNPN9VLsvHQ/ox2SPbK8bn88suZNGkSDz30EL1792b58uVMnz7dN8xl27Zt7N6923f8gQMHGDduHF26dOHss88mJyeHuXPn0rVrV98x99xzD7feeis33HADAwYMIC8vj+nTpxMSUv2p6iIiIn7rwBbzz9g2dXK6d+dt5bMlO3A64D9X9eXGoVp7NSZKNPqRBZnmFsOTEwdYHIlp7kZzCujQjs18W+yk4XiTjd4BMVe8Pp/07LpPNu7KLiKvuKxeJ05XJSwwjJdOf8lXyfTAbw/gMY6xjVNqJjgSrvrY3AKR8SdMHQ1lxQ3z2iUFBxctzexZ0eitZuye0J1gV+2r86A6FY2BdfI6tRVQxdCao+pwJu8l3QvA6dlfwC+T6iyeDrEdmDx8MtHB0azYt4Ibf6z7ysZN2ebk7HbR2jbt7yZMmMDWrVspLi5mwYIFDBw40PfY7NmzmTJliu/vzz//vO/Y9PR0vv32W/r06VPhfA6Hg8cee4z09HSKior4+eef6dixY0O9HREREWvVYaJxwab9PD5tFQB/P6szZ/VIrvU5xV6UaPQTpaUFrDDMJFK/9udaHI1pcfm06RPSrK+ubKrMZOPBadSXvTaPHQfqtupvfQNNnK5KSkQKz5/6PAHOAH7a+hMvLHmhwWNo9KJbmgM9giJhy//gy1vgWH356sK+dYABYfEQ0az+X+84+Poz1tG2aTjY+/Dwac7eHo2RNhgEA4fGWbOqxLdzBvBI6TXmX2Y9AYverLOYOsV14s3hbxITHMPK/Su54ce67dmoidMiIiIilaijROOurELGf7iUMo/Beb1SGHdy21qHJvajRKOfWLv+WwqdDiI9Bm3bnG51OJS6PSzbbiYa+7fWtmkrpcaF8fGNJ5IaF8q2zAIuf20+2/bXXbJxfQNOnK5K38S+PD7kcQDe/vNtPlrzkWWxNFrJPeHy98AZACs/g58fqv/X9E6ctvEgmKUZ5f0Z62gQDFQ9dTqvuBSw0dbpmvRoLJddUMqW/QVMcY+kaNBd5p3f/h/88UmdxdUprlOFbdR1OSDGO3G6fUz7OjmfiIiISKNQB4nGolI3N7+/hH15JXROiuTpi3tou3QjpUSjn1i25WcA+rgicbqs/xC6alcORaUeYsICades4fr2SeVaxobxyY2DSEsIZ2dWIZe9No9Ne/Pq5NzrM8yKxvbNrb3O57Y9l9v63AbAUwufYta2WZbG0yi1Ow1G/ce8PfclmPef+n09m0+c3luwl+2523HgoE/zPsd+QjUFuCqfOu3t0Rhpl0RjFVu8j2blLjPh1youjJDhD8GA6wHDnGy++ps6i61TXCfeHGEOiFm1fxXjfhxX62TjoROn28bo23URERERANxlkG2ukY430WgYBg9+uZLfd2QTExbI5Gv6ExZkjzWv1D0lGv3Esv1mD4M+MfboB7RoSyYA/VrF4lR/RltIjg7l4xtOpEPzCNJzirj89fm+bc+1sc4GFY1e1/e4nos7XIzH8HDPL/ewct9Kq0NqfHpdDsMeMW//cD+s/G/9vZbNJ04vyTC3TXeK60RkUN399+8q7314eALPNwzGJlunA1yVb/E+mj92mMm+Hi2jzYmEZ/0Teo8Gww2fjoX1P9VZfB1iO/DG8Dd8PVyv//F6Mosyj/t8mjgtIiIiUomcneApA1cwRCQd1yk+XLiNT8uHv7x0ZR9S48LqOEixEyUa/YDh8bCs1Nym3Ke19dumAZZsNePp10bbpu2keVQIH91wIp2TItmbW8wVr8/nz13HX+Vj1cTpqjgcDh448QGGtBhCkbuI8TPG+yqQpA4NuQNOuAGzEu1G2Dizfl7H5hOnvYNg6rI/IxwcBnP4lmTfMBibVTS6a9Cuc8XOLAB6tog273A64fyXoNuF4CmFj/8Cm/9XZzF2iO3Am8PNysY1mWv46/S/srdg73GdSxOnRURERCrh3TYd08pc29XQ3txiJn5nrvvvGdmZkzvYsze71B0lGv3Ajp0L2OdyEGAYdOt4vtXhYBgGi8oHwQxoo0EwdpMQEcxH406ke4so9ueXcMXr832J4ZrafcjE6dbxDTtxuioBzgCeHfosXeK6kFmUyc0/38yBouN7f1IFhwNGPgVdR4G7xJxEvX1h3b6GH02crsv+jFD1lmS7DYMJqGJozdFUqGj0crrgosnQ8SwoK4IPL6/T/57ax7ZnysgpNA9rzsbsjYyZPobdebtrfB71ZxQRERGpRC37Mz7741ryisvo2TKaGzT8pUlQotEPLFtv9rXqZgQREmp9BeG2zAL25RUT5HLSo0X0sZ8gDS42PIgPx51I/9ax5BaVcfWbC/h1/b4an2fdIROngwLs8+siPDCcl894meTwZLbkbOHmn28mvzTf6rAaF29yqN3pUFoAH1wC6Svq7vw2nzidU5LDugPrAOiX2K9Oz33MikabJBqdVQytqUpmfgk7DhQC0P3wfxtcgXDpFGh7GpTmw/uXwM4ldRZrWnQaU0ZOoUVEC7blbmPM9DFsz91eo3NszDYTjW2jtQAWERER8alFonHlzmw+XmyuyR4+r6varjUR9skcSJWWlfcJ6xPZ2uJITIvLqxl7tIwmJNBlcTRSlaiQQN697gRO7pBAQYmbv05ZxI9/ptfoHHaYOF2VZmHNeO3M13yTZ2+beRvF7mKrw2pcAoLh8vch9UQoyob3LoT9G+vm3DafOL08YzkGBq0iW5EQmlCn53ZWkWjM9W2dDqzT1zteB3s0Vi/RuGKnWc2YlhBOVGXvITAErvgAWg2G4mx490LYUXfJxtTIVKaMnELrqNbsyt/FmO/HsCl7U7Wfr4pGERERkUocZ6LRMAwe+2YVhgGjeqfQr7V2QzYVSjT6geUF5haw3iknWhyJafFWs9l+/9bWV1fK0YUFBfDGtf0Z2S2JEreHmz9YyhfLqt/T0C4Tp6uSFp3GK2e+QnhgOAvTF3LPnHso85RZHVbjEhQOV30MST0gfy+8O+rg1LnasPnE6fraNg1HqWgsKgXsU9HoG1rjrmaicUcWwNEr3YPCYfSn0GqQmWx8r26TjUnhSUwZOYX2Me3JKMxg7PSxrN6/+pjPKywr9PV7bRfTrs7iEREREfF7x5lo/G5FOgu3ZBIS6OTekfZc80v9UKLR5rKztrDBZX7I69P5YoujMXkrGvsp0egXggNc/PuqPlzUtwVuj8Fdn/zOO3O3VOu5dpo4XZVu8d146fSXCHIGMXP7TB6Z+wgeowbTK+TYQmPgL19AfHvI3m4mG/MyandOm0+cXppRP4Ng4NAejRX/O/VunY60yTAYX0LUqF6i0dufsWfLY7TUCI6A0Z8drGx874I6TTYmhCbw1oi3fH1c//rDX1mcvvioz9mSvQUDg9jgWOJDNXFaRERExCdrq/lnbPV3WBaVuvnHd+aXvTcNbUdKTGh9RCY2pUSjzf2+9gsA2rghLs767VxZBSWsL59CrESj/whwOZl0SS/GDG6DYcDDX//Jsz+uxThKAsFuE6ePZkDSAP459J+4HC6+2vgVkxZPOup7k+MQ0Qyu+QqiU2H/BnjnPMg7vum+gK0nTheVFbFin9mPsq77MwIElFcKHlnRaK8eja4qKi+r4t06Xa3evcERZmVj6yFQnFPnycbYkFjeHPEm/RL7kVeax00/38Sc7XOqPN47cbptjPozioiIiPgU5UDBfvN2TPUTjZN/2cTOrEJSokO48RTtFmlqbJ1onDhxIgMGDCAyMpLmzZtzwQUXsHbtWqvDalBLd/wGQJ/QRIsjMXmnF7dtFk58RLDF0UhNOJ0OHj6vK3ed2RGAl2Zu4P4vVlDmrrz6z44Tp4/m9Fan89iQxwB4b9V7/Of3/1gcUSMU3RKu/RoiU8xE4TvnQX7NhwzZfeL0in0rKPOUkRCaQGpkap2fv6qp0wd7NNok0ViDYTB7c4vZnV2EwwHdqjskLDgCrvqkYrKxDqdRRwZF8uqwVxnacijF7mJun3U732z8ptJj1Z9RREREpBLeasaweAiJqtZT0rOL+M9sc23197O7EBqkuQ5Nja0TjXPmzGH8+PHMnz+fn376idLSUoYPH05+ftOZLrssdzMAfZr1sTgS06LybdPqz+ifHA4Ht53RgScv7I7TAR8t3M4tHyylqNR9xLF2nTh9NOe3O5+/n/B3AF79/VVe+f0ViyNqhOLawphpEJls9ll85/yaJxttPnHa15+xeV8cjrqfjOdNNBoGeMqTeIZhHNw6bZeKRu8wmCq+jDjUqt05gPn7okYVmb7KxpPMZOO7F8CmqisPayokIITnT3uec9uei9twc/+v9/PB6g+OOM6baFR/RhEREZFDHEd/xmemr6Gw1E3/1rGc1zO5XsISe7N19mD69OmMGTOGbt260atXL6ZMmcK2bdtYsqTq7VXFxcXk5ORU+PFXJcW5/GmYU3T7tD/X4mhMS7yDYNpoYpQ/Gz2wNf8Z3Zcgl5MfV+3hmrcWkl1YWuEY77bpDjbfNn240V1G87f+fwPgP8v/w+Q/JlscUSMU3w6unQYRSZDxp9mzMX9/9Z9v84nTvv6M9TAIBg4mGuFg/8OCEjfe3f52qWgMqKLysjK+NgvNj6Ofq3dATLvToTQfPrgU1k6v+XmqEOgM5MmTnmR0l9EAPLXwKV5c+mKF9gobs8sTjdFKNIqIiIj41DDRuD2zgC+X7wTgofO61suX9mJ/tk40Hi472+z/FBdXdZJr4sSJREdH+35SU+t+21tDWbX+G4qdDuI8Bq1bnWx1OBSXufm9vNm/Khr938juybzz1xOIDA5g4eZMLn11LjuzCn2PeysaOxxP4sBi13a7ljv63gHAv5b9i7dWvmVtQI1RQnuzsjEiEfasrFmy0cYTpw3D8PVn7NO8firJAw5NNJYn8bzVjC6ng9BAe2wv8SZEPdXod+pNNB73hPqgMLhyKnQ+F9zF8PFoWPn58Z2rEk6Hk3sH3Mv43uMBeGPFGzzw2wOUuks1cVpERESkKjVMNL47bwseA07ukEDPljH1FZXYnN8kGj0eD3fccQdDhgyhe/fuVR533333kZ2d7fvZvn17A0ZZt5ZvmQlAL1c0Dqf1l2rlzmxKyjzEhweRlmD/nn1ybIPaxTP1xhNpHhnMuj15XPjyb6wsH+iwPsP+E6eP5roe13Frn1sBeH7J87zz5zsWR9QIJXQwKxvDm8OeFTDlHMhNP/bzbDxxenf+bnJLcglwBtAhpkO9vMahFY3easHcIrOiOCI4wDbf/NakR+PGvebvi3bNa/FvQ0AwXPoO9LwcPGXw2XWw9L3jP99hHA4HN/W6iccGP4bL4eLrjV8zfsZ4Vu5bqYnTIiIiIpU5UN6jsRqDYPKLy5i6yMy/jB3Sph6DEruzPntVTePHj2flypVMnTr1qMcFBwcTFRVV4cdfLc00q376xtnjw/ji8v6M/VrH2uaDsNRet5Rovhg/hI6JEWTkFnPZa/OYtTaDDXv8c+v0oW7oeQO39LoFgEmLJzFl5RRrA2qMmnWEMd8e7Nn49lmQte3oz7HxxOk1mWZs7aLbEegKrJfXqFDR6PYmGu01cRogwNejsRqJRm9FY7NafjHhCoALXoV+YwEDvp4Ac/9du3Me5sIOF/LS6S8RGhDKvN3zuHWm+YWEqhlFREREDlODisb/LttJblEZbeLDOLVj83oNS+zNLxKNEyZMYNq0acyaNYuWLVtaHU6DMDwefneblWW925xucTQm3yCYNto23di0iAnls5sHM6R9PAUlbv46ZRG55ROn2/jBxOmjuanXTdzY80YAnl3yLK8sf6VCbzapA806wtjvzW86MzfBW2fBvg2VH2vzidNrM83+kZ3i6i8JWrGi0Ry04hsEY5P+jFD1dOzDHcgvYX9+CVDLikYvpxPOfR4GmwlAfvx/8OMD4Dn2UJrqOrnlybw94m3iQuLILzUHzCnRKCIiInIIj+fg1OljJBoNw2DKb+Yg22sHt8HpVGFSU2brRKNhGEyYMIEvvviCmTNnkpaWZnVIDWbrtv+R6XQQ7DHo2uE8q8PBMAwNgmnkokICeXvMCVzct6VvKIU/TZyuisPhYEKfCdzW5zYA/vP7f3h+yfNKNta1uDQz2RjfAXJ2mJWNe/488jibT5z2VjR2jqu//pEOhwPv2svXo9GOFY3lLTuO1aNxQ/m26RYxoYQF1VH8Dgec+Tic+Zj597kvwRc3QllJ3Zwf6JbQjffPep9Wka0A6NmsZ52dW0RERMTv5e4Gdwk4AyCqxVEP/d/6fWzcm09EcACX9GsaxWFSNVtnEMaPH8/777/Phx9+SGRkJOnp6aSnp1NYWHjsJ/u5ZRumAdDNEUxQsPU98jbuzedAQSnBAU66p0RbHY7Uk6AAJ5Mu7cntZ5i96Ya0T7A4orozruc47hlwDwBv//k2Ty54Eo9RdxVSAkS3MJONiT0gPwPePht2LKl4jM0nTq89YMZXn4lGOJjE806dzi2vaLTLxGmofkWjdxBMu+MdBFMVhwOG3A4XvmYucFd8Ah9dDsW5dfYSqVGpTD13Kq8Oe5Wz086us/OKiIiI+D3vLqToVLO9zVFMmWsee0m/lkSG1E/7IfEftk40vvLKK2RnZ3PqqaeSnJzs+/n444+tDq3eLdu7DIA+kfao4vRWM/ZKjfH7Cjc5OofDwZ1ndmTxA8N46NyuVodTp67uejUPD3oYBw4+XvsxD/72IGWeMqvDalwimsGYb6DlACjKgnfOhfU/HXzcxhOnc0py2Jm3E4COsR3r9bV8STy3fSsavTG6q5lobN+snvq59roCrvwYAsNh40yYci7k7a2z00cGRTKkxRACnPb5315ERETEcr7+jEcfBLN5Xz4z12TgcJjbpkVsnTEyDKPSnzFjxlgdWr37ozADgD4tBlsciWnZtizAHAQjTUNCRHCj7K1xScdL+MfJ//BNnb17zt0Uu4utDqtxCY2Fq7+EdqdDaQF8eDks+8B8zMYTp739GVPCU4gOrt/K7YDDkni27tF4jGEwvkRjXVc0HqrDMDOBHRYPu5fDG2ccrI4VERERkbpXzf6M75RXM57WqTlpCf7d31/qhq0TjU1VUeEBNjvNLZ1d0oZbHI1p1e4cAG2blkbh3LbnMmnoJAKdgfy87Wdu+PEGsouzrQ6rcQmOMKvQel4Ohhu+ugV+mXRIRaP9Jk43xCAYL5er4rZkb6LRThWNB5OhR28x0CCJRoAW/eC6nyA2zVz4vnEmbJxVv68pIiIi0lRVY+J0blEpny7eDsAYVTNKOSUabWjjlpl4HA5iPQbNmlm/dbXM7WFtutkTq0uy9f0iRerCsNbDeO3M14gIjGBpxlLGTB9Den661WE1LgFBcMGrZp89gJmP23vidAP1ZwRwOSpWNOb6tk7bp6eNb+v0UYbBFJa42Zll9k1u16wBvsGObwfXz4DUE6E4G96/GJZMqf/XFREREWlqqpFo/HTxDvJL3LRvHsHJHRpPf3+pHSUabWjdzvkAdHSG4nBaf4m27C+guMxDaKCL1vEqhZbGY0DSAKaMnELz0OZsyNrA6O9Gs/7AeqvDalycTnNy8MingfKt+DadON2gFY1VbJ221TAYx7F7NG4snzgdGxZIfERwg8RFeDxc+zX0uMyslv3mdvjxQThG5aWIiIiI1MAxEo0ej8E788xjrh3cBoej8bXdkuNjfRZLjrA20+xh1iksxeJITKvLt013Sor0fTgWaSw6xXXi/bPfp210WzIKMrh2+rUsTl9sdViNz4k3wSVvmQM9Op1ldTRHKHWXsiFrAwCdYus/0XhEj8aiUgAibbR12re9+yg9Gr2JxnrfNn24gGC46HU49X7z73P/BR//pU4nUouIiIg0WSUFkLfHvF1FonHJtgNs3V9AZHAAF/dt0XCxie0p0WhDawt2A9Ax3h5bC72JRm2blsYqOSKZd896l97NepNbksu4n8bx1YavrA6r8el+EdyzCc7/t9WRHGFT9iZKPaVEBEbQIqL+F0oHezSaVXh2HAZzeDK0Mg3Wn7EyDgecei9c9Aa4gmDtt/DGMNi/seFjEREREWlMvINggqPNQY+V+PYPM29xZtdEwoLss4YV6ynRaDOGx8NaowiATjaZOH0w0RhlcSQi9Sc6OJrJwydzZuszKfOU8cBvD/D8kufxGNqOWacCQ8wEkc14+zN2iuvUINs+AsrbYhzRo9FGiUZXeYxl1Ug0tmtmQaLRq+elMPZ7iEyGvWvg9dNg/U/WxSMiIiLi73zbpltX+rDHY/D9SjPReE7P5AYKSvyFEo02s2fP7+Q6HQQYBm3bnGZ1OACs8Q2CUaJRGreQgBAmDZ3EuB7jAHhr5VvcOetOCkoLLI5M6tua8pYVDTEIBg72aCw7YhiMfRKNAdUYBmNpReOhWvaHG+ZA6kBzSMwHl8L/noOjxC4iIiIiVThQXtF4lG3Te3KKiQwO4CQNgZHDKNFoM2u3zgIgzXARFGz9VuWsghJ2Z5dXWCZZH49IfXM6nNzW9zb+cdI/CHQGMnP7TK6dfq0mUjdyvkEwDdCfEY4ctGLHrdNOb6Kxih6NZW4PW/bnAzZINAJEJsK106DfGMCAGY/Cp9dCUY7VkYmIiIj4l2MMgjl023RwgKthYhK/oUSjzazNWAZAx6A4iyMxrSrfNt0yNpSokECLoxFpOOe1O4+3RrxFXEgcazLXcMW0KzQkppEyDMOyika3x8AwjINTp4Pt83s24LCqy8NtzSyg1G0QGugiJTq0IUOrWkAQnPcinPs8OANh1Vfw+qmQvsLqyERERET8x1ESjYdumz67h7ZNy5GUaLSZtTlbAOgU3dbaQMqt3q1t09J09W7em4/O+YgOsR3YX7Sf63+8nvdWvYeh7ZiNSnp+OjklOQQ4AmgX065BXjPAdTDRWFTq8VU22qtHozfGyvuUbizfNt22Wbiv+tE2+v/V7NsY1RIyN5pDYpa+q63UIiIiItVxlB6Nh26bPrmjtk3LkZRotJl1JVkAdErsa20g5TQIRpq6lIgU3j/rfc5OOxu34eaZRc9w7y/3qm9jI+KtZmwb05YgV1CDvOahPRpzi0sBc0ZOWKB9tp4cq6Jxw16b9GesSuoAuOl/0P5MKCuCr2+FL2+BknyrIxMRERGxL8M4JNGYdsTD2jYtx6JEo40UFmSy1Wl+oOuYdobF0ZjWpJuJxq7J6s8oTVdYYBhPnfwUfz/h7wQ4Avh+y/eM/m40W3O2Wh2a1IE1Bxp22zQcMmjF4yHPOwgmKMBWlYHeZKiniipA3yAYKydOH0tYHFz1CZzxEDic8PuHMPl02POn1ZGJiIiI2FNeBpQVAg6ITq3wkLZNS3Uo0WgjGzbPwHA4iHcbJCQ03AfeqpS5PazbY36QVEWjNHUOh4PRXUbz5og3SQhNYEPWBq6YdgXTt0y3OjSppXWZ64CGGwQDFSsaff0ZbbRtGg6JsYphMBvtMnH6WJxOOPn/4NpvICIR9q6B10+D+a9qK7WIiIjI4bLKiymiW5r9rw+xVNumpRqUaLSRtbvmAdDRFWZxJKZN+/IpKfMQHuQiNdYeMYlYrW9iXz459xP6Nu9LXmked8+5m0fmPkJhWaHVoclxauhBMFBxGIyvojHYXonGAGfFydiHMgyDjXttNHG6OtqcBDf9Bh1GgLsYpt8LH1wCuXusjkzqwcsvv0ybNm0ICQlh4MCBLFy4sMpjJ0+ezMknn0xsbCyxsbEMGzbsiOPHjBmDw+Go8DNy5Mj6fhsiIiIN7yiDYKZp27RUgxKNNrK2/MNup/AWFkdi8vZn7JQUaavtfCJWaxbWjDdHvMm4HuNw4ODz9Z9z5bQrWXdgndWhSQ3lluSyI28HAJ3iGrKi0fzn1+0xyLVtRaMZY2U9GtNzisgrLsPldNA6PryhQzt+Ec3gqo/h7EkQEAIbfoZXBsFaVSY3Jh9//DF33XUXDz/8MEuXLqVXr16MGDGCjIyMSo+fPXs2V155JbNmzWLevHmkpqYyfPhwdu7cWeG4kSNHsnv3bt/PRx991BBvR0REpGF5KxpjWlW4W9umpbqUaLSRdYVmVUXH+G4WR2JapUEwIlUKcAZwW9/bmDx8MgmhCWzM3shV317Fx2s+1lRqP+JNDieFJxEdHN1gr3vooBVvRWNkSGCDvX51BBylR6O3P2Pr+DCCAvxsKeFwwAnj4IbZkNgdCvbDR5ebw2KKcqyOTurAc889x7hx4xg7dixdu3bl1VdfJSwsjLfeeqvS4z/44ANuueUWevfuTefOnXnjjTfweDzMmDGjwnHBwcEkJSX5fmJjYxvi7YiIiDSsHDOZSFRKhbu1bVqqy88+HTRehsfDOqMYgE6pQyyOxrRmdy6gRKPI0QxMHshn533GSS1OothdzBMLnmDCzAnsLdhrdWhSDb5t07EN2xe3wtbp8orGSJttnXYepUejXwyCOZbmXWDcTBg0wfz70nfhP4Ngw4yjP09sraSkhCVLljBs2DDffU6nk2HDhjFv3rxqnaOgoIDS0lLi4uIq3D979myaN29Op06duPnmm9m/f3+V5yguLiYnJ6fCj4iIiF/ILU80RlasWvx2hbZNS/Uo0WgTu3YvJs/pIMAwSEs9xepwgINbp7to4rTIUcWHxvPyGS/zt/5/I9AZyC87fuHCry9k+mZtx7S7tZlrgYbdNg2HVTQW+1+PRm+isZ2/9GesSkAwjHgSxnxn9iHK2QHvXwRf36bqRj+1b98+3G43iYmJFe5PTEwkPT29Wue49957SUlJqZCsHDlyJO+++y4zZszg6aefZs6cOZx11lm43e5KzzFx4kSio6N9P6mpqZUeJyIiYjs5u8w/D6lo9HgMvl9h/juqbdNyLEo02sTarbMBaGe4CAy2vt/V/rxiMnLLKyyTVNEocixOh5Nru13Lx+d+TJe4LmQXZ3P3L3dz95y7ySrKsjo8qYIVg2DgYLWg2+0hp6gUsGOPRm8y1HPEYxv3NoKKxkO1GQI3z4UTbjT/vvQdeGUwrP/Z2rikwT311FNMnTqVL774gpCQEN/9V1xxBeeffz49evTgggsuYNq0aSxatIjZs2dXep777ruP7Oxs38/27dsb6B2IiIjUUiUVjct3ZJGeU6Rt01ItSjTaxNqM3wHoFBxvcSSm1eXbplvHh9muykbEzjrEduCDsz/gxp434nK4mL5lOhd+fSEztmk7pt2UecrYkLUBsK6i0W3gl1OnN2T42cTp6ggKh7OfgTHfmtWN2dvhg4vhs79qMrUfSUhIwOVysWdPxWu2Z88ekpKSjvrcSZMm8dRTT/Hjjz/Ss2fPox7btm1bEhIS2LBhQ6WPBwcHExUVVeFHRETE9tylkFc+PO2Qisb/rdsHwCkdm2nbtByTEo02sT7XnOzUMbq9xZGY1qSXb5tWNaNIjQW6ApnQZwLvn/0+adFp7Cvcxx2z7uDOWXeSUVD51FNpeDvzdlLqKSXEFUKLiBYN+toHezR6DvZotGlFo/uwYTDZBaXsyzMr3v1+63Rl2pxkVjeeOB4cTlj5Ofx7ACx+Cyqp7hR7CQoKol+/fhUGuXgHuwwaNKjK5z3zzDM8/vjjTJ8+nf79+x/zdXbs2MH+/ftJTtb2MRERaURy0wEDnIEQdrBy8beNZqJxcHt7FEaJvSnRaBNrS7MB6JTUz+JITJo4LVJ73RO688m5n3Bd9+twOVz8vO1nLvjyAj5Z+wkeQwkLq23J3gJA66jWOB0N+89hZVOn7VbR6Es0HjYMZsNes+I9OTrEdjHXmaBwGPkPGDcLkntDcTZMuxPeGgHpK62OTo7hrrvuYvLkybzzzjusXr2am2++mfz8fMaOHQvANddcw3333ec7/umnn+bBBx/krbfeok2bNqSnp5Oenk5entkiIC8vj7vvvpv58+ezZcsWZsyYwahRo2jfvj0jRoyw5D2KiIjUC9+26SRwmuvjgpIylm07AMBJ7bVtWo5NiUYbKMjLYLvT/CDXMe0Mi6MxebdOd9YgGJFaCQkI4Y5+dzD13Kl0i+9Gbmkuj89/nLHTx7Ixa6PV4TVpW3K2AGaisaG5yhdubrdBrncYjE0rGssO2zq9sTFum65KSm9zMvXIpyEoAnYshNdOhu/uhoJMq6OTKlx++eVMmjSJhx56iN69e7N8+XKmT5/uGxCzbds2du/e7Tv+lVdeoaSkhEsuuYTk5GTfz6RJkwBwuVz88ccfnH/++XTs2JHrrruOfv368b///Y/g4GBL3qOIiEi98A6COaQ/46ItByh1G7SICaVVXJhFgYk/sdenmiZq3ZafMRwOmrkN4uKs3zpdUuZhQ4aZaOyqikaROtE5rjMfnP0BH675kJeWvcTSjKVc8vUljO4ympt63UREUBNI2tjM1hyzZYUViUZ/qGgM8CZDD0s0bsssAMwevk2C0wUn3gRdzoPpf4fVX8PC12HFZ3DGg9D3WvMYsZUJEyYwYcKESh87fIDLli1bjnqu0NBQfvjhhzqKTERExMa8FY1RBxONv20wt00PaR+Pw+GwIirxM6potIF1OxcA0NFl/bRpMKeJlroNIoMDaBkbanU4Io2Gy+ni6q5X8+WoLzm15amUGWW8s+odzvvyPL7Z+A2GceTQDak/3kRjWnRag7+265BBK3bv0Xh4ReP2A2aisWVsE0k0ekW3gMvfg2u+hmZdoDDT3E79+lDYOs/q6ERERERqz1fReHAQzMFEo7ZNS/Uo0WgD6w6sA6BTREuLIzF5B8F0To7UNxYi9SAlIoWXzniJ/5zxH1pHtWZf4T7u//V+rvn+GlbtX2V1eE2GtVunDw5a8SYaI4IDGzyOo/FWXXoOTzSWVzSmNrVEo1fboXDTr3DWMxASDekr4O2zIHOT1ZGJiIiI1M5hFY0H8kt88xsGtdMgGKkeJRptYG3RHgA6xnezOBKTrz+jJk6L1KuTW57Mf8//L7f3vZ3QgFCW713O5dMu577/3ceuvF1Wh9eoFZQW+CaAW7l12n3o1mk/qWjccaAQgNS4Jlzx7gqAgTfCrUuh3xjoMxri2lodlYiIiEjt5HgTjS0AmLdpP4YBHRMjaB4ZYmFg4k+UaLSY4fGw3igBoFPqSRZHY1qtidMiDSbIFcT1Pa7n6wu+5py25wAwbdM0zvviPJ5b/Bw5JTkWR9g4ebdNxwbHEh0c3eCv703iFZSUUeI2J5Dbdev0oT0ai0rdZOQWA024ovFQ4Qlw3otw3ktWRyIiIiJSe7kVh8F4t00Pbqdt01J9SjRaLGPvSvKdDlyGQetW9kg0btprThTtkKjhFCINJSk8iadOfoqp50xlQNIASjwlvP3n25z937N59893KXYXWx1io2LlIBg4WNGYVVDquy88yF6JxoMDazy++7zVjOFBLmLC7LXV21JOLadERETEzxnGIRWNZqJx7sb9gPozSs1oZWyxbbsWAdDC4yAw0PrqkKJSN7uyzQ+SaQn2GE4j0pR0S+jGm8Pf5N+n/5u20W3JLs7mn4v/ydmfn83UNVMpcZdYHWKj4O3P2Ca6jSWv7yxP4mUXmonG8CCXr4LQLrzxeAx8g4p2lA+CSY0LUw9fERERkcakKAvKzFwAkcnszCpk8758XE4HA9vGWRqa+BclGi22Ze9KAFrZZOL0tswCDAMigwOIDw+yOhyRJsnhcDA0dSifn/85Dw96mKTwJDIKM3hywZOc+8W5fL7uc0o9pcc+kVTJbhWNduvPCFRIfHq3T28vr2hschOnRURERBo7bzVjaCwEhvq2TfdsGU1UiHaySPUp0Wixbd6qmtBm1gZSzrttOq1ZuKpVRCwW4Azgko6X8O2F33L/wPtpFtqM3fm7eWTeI5z/xfl8uu5TVTgepy3ZWwBoE9XGktd3lW+1zSo0r19EsL0Tjd6BMDu8E6eb8iAYERERkcbI158xBYC55YnGIerPKDWkRKPFtpZPPW1lUVXN4bbsNxONbeLtUWEpIubAmCs7X8l3F33H3f3vJi4kjh15O3hs3mOM/HwkU1ZOIb803+ow/YZhGDasaLTft8QBh/QdPFjRaCYaVdEoIiIi0sgc0p/RMAx+K+/POLh9vIVBiT9SotFiW8tyAWgd38XiSEybyysa26g/o4jthASEcE23a/j+ou+5d8C9JIYlsrdwL88ueZbhnw3n38v+zb7CfVaHaXuZRZnklubiwEGrqFaWxOCtFswtKgPMdhV2U2lFY/nW6dRYVTSKiIiINCo5BydOb8jIY29uMcEBTvq2irU2LvE7SjRayF1WwnanOc2zdcoAi6MxbS6vaGyrRKOIbYUFhvGXrn/h+4u+57HBj9Emqg05JTm89sdrDP9sOA/+9iBrM9daHaZteasZUyJSCHYFWxJDgKtiawo7bp0OOCTR6PFWNGYeHAYjIiIiIo2Id+t0VIqvP+OANnGEBLosDEr8kRKNFtqdvpRSh4NAwyApsbfV4QCweZ8qGkX8RaArkAs7XMiXo77k2aHP0jOhJ6WeUr7c8CWXfHMJ1/9wPbO3z8btcVsdqq1YvW0awHlYD1w7DoNxHlbRmFdcxoHyrd4tVdEoIiIi0rh4t05HJmvbtNSK/T7ZNCHbdi8BoJXHiSvA+gnPecVl7M0tBiBNPRpF/IbL6WJ4m+EMbzOc3/f+znur3uPnrT+zIH0BC9IX0CKiBZd0vIQL2l9AQqiaOW/O2QxYm2g8tFoQ7FnRCGacZR4Dt8fwVTPGhAUSacOekiIiIiJSC+UVje6IJOZvMhONGgQjx8Oen2yaiC37VwHQKiDS4khMW8qrGePCg4gO04dIEX/Uq1kveg3txe683Xy05iM+W/8ZO/N28uLSF3l5+csMazWMyzpdRv/E/k12svzWbOsrGl2HJRojbVjRCGacZR6DMo/nkP6M2jYtIiIi0uiUVzSuL4wktyibqJAAureItjgo8UfaOm2hbTnbAGgT1tziSEzebdNp2jYt4veSI5K5q/9dzLx0Jk8MeYKezXpS5ilj+pbp/PWHv3LuF+fy+h+vsztvt9WhNjjv1um0qDTLYvCHHo1wsPLy0IrG1DhtmxYRERFpVMqKocDsyzhvbwgAJ7aNP+LLcZHqUKLRQlsKMwBoFW3dh91DeSsa22jbtEijERIQwqj2o/jg7A/49LxPubTjpYQFhLEtdxsvLXuJEZ+PYNyP4/h207cUlhVaHW69c3vcbMs1v+RpHW1lRWPFf37tuhXZdWii8YCZaGypikYRERGRxiU33fzTFcyC8pv9WmvatBwfe5ZQNBHb3AXggtYJ3awOBTi0olEfIkUao85xnXlo0EP8rf/f+GnrT3y18SsWpS9i/u75zN89n7CAME5vdTpnpZ3FoJRBBDrtmfyqjV35uyj1lBLkDCIpLMmyOI7o0WjjrdNgJhoPbp1WRaOIiIhIo5LrHQSTxB87swHolRpjXTzi1+z5yaYJKC3OZ5fTABy0ThlodTgAbN7vTTRGWByJiNSnsMAwRrUfxaj2o9ieu51vNn7D1xu/ZmfeTqZtmsa0TdOICY7hzNZnclbaWfRt3heX02V12HXCu226VVQrS9/T4VOnI226ddpbeVl2yNbplnH6MkpERESkUckxB8GUhCexK70IpwN6qD+jHCd7frJpAnbsXoTb4SDUY9CsWVerwwEO2TqtikaRJiM1MpVbet/Czb1u5ve9v/Pd5u/4YcsPZBZl8um6T/l03afEhcRxWuppDGs9jIFJAwl0+W+lozfRaOUgGPCfisaASisa9W+EiIiISKNSXtGY6YwHoEPzSMJt+kW42J/+y7HItvSlALTGhcNpfavMrIISDhSUAurRKNIUORwOejfvTe/mvblnwD0sTF/I95u/Z+a2mWQWZfL5+s/5fP3nRAZGcnLLkzkt9TQGtxhMVFCU1aHXyJbsLQC0iWpjaRwuPxkG4906vS+vmLziMgBaauu0iIiISONSXtG4oywGgJ4tVc0ox8+en2yagC371wDQKtAeH9K9/RkTo4L1zYVIExfgDGBwymAGpwzmoUEPsTh9MT9v/ZkZ22awv2g/323+ju82f4fL4aJvYl+GthzKyS1PJi0qDYfD3pPpbFvRaNPfu95E49b95rbpZpHBhAQ2jm30IiIiIlKuvKJxbaHZRk39GaU27PnJpgnwTT21cBjBoTZr4rSIVCLQGciglEEMShnE/QPv5/e9vzN7+2zm7JjDpuxNLEpfxKL0RUxaPImU8BQGpQxicMpgBiYPJDrYft+EbsnZAkCb6DaWxuE6LNEYafOt095/IzQIRkRERKQRyjETjcuzzBY5vZVolFqw5yebJmBr8X4AWse0szgSk7c/Y9tmSjSKSOVcTrOCsW9iX+7qfxfbc7bzy85f+GXHLyxKX8Su/F2+LdZOh5Pu8d0ZmDyQ/kn96dO8D6EB1iapisqK2J1vLqKsrmh0HVb5addKcm9CdEv5sLCW6s8oIiIi0vjkmlunNxdHERTgpFNSpMUBiT+z5yebJmCruxBcDlo362F1KABsUkWjiNRQalQqo6NGM7rLaApKC1iyZwlzd81l7q65bMrexB/7/uCPfX8wecVkApwB9EjowYCkAfRL7EevZr0ID2zY3zfeSvLIoEhig2Mb9LUPF3BIj8aQQCeBLut79Vbm8K3TqXGqaBQRERFpVAzDV9GYThzdUqJsuzYV/6BEowUKCzJJL/+Q2brFiRZHY/JWq6QlKNEoIjUXFhjGyS1P5uSWJwOQnp/OvF3zWJS+iIXpC9lTsIdlGctYlrEMAKfDSafYTvRN7GsOoWnWm6Tw+m0l4e3PaIdekq5DhoBFBNt3irc3Ibo9szzRqIpGERERkcalIBPcxQBkGLEMaxljbTzi95RotMD2XQsAiPQYxMSkWRwNGIbBln3mh0glGkWkLiSFJ3Fhhwu5sMOFGIbBjtwdLExfyKI9i1i2Zxm78nexOnM1qzNX88HqDwBoHtqcHs160CPB/OmW0K1Oqx7tMggGKg6DsWt/Rji4xbvMYwCQGqdEo4iIiEijUr5tOtsRRQmB9Eq1X5918S/2/XTTiG1LXw5AGwJxOK0vSd6bV0xecRkOB7SK14dIEalbDoeD1KhUUqNSubjjxYBZ8bg8Y7mvynHdgXVkFGYwY9sMZmybYT4PB62jWtM1vitd47vSJa4LneM7ExUUdVxxbM7eDNgj0XjoMBi7TpyGI4fWtNQwGBEREZHGpXzb9E5PHAC9VNEotWTfTzeN2JYDawFoFRRjbSDlvNWMLWJCCQ5wWRyNiDQFSeFJjEwbyci0kQAUlBawOnM1K/au4I99f7Bi3wrS89PZkrOFLTlb+G7zd77npoSn0DGuIx1jO9IpthMdYzuSGpmKy3n031++isZo6xON/lLRGHDIl2FOB6TEKNEoIiIi0qiUVzTu9sQSFRKguQ1Sa/b9dNOIbcvbAUDr8GSLIzFt3pcHaNu0iFgnLDCMfon96JfYz3ff/sL95vbq/atZtX8VqzNXszNvJ7vyd7Erfxezt8/2HRvkDCItOo12Me1oH9OedjHtSItOo2VkSwKdZg9Eb6KxTVSbBnxnlXP6YUVjcnSoGoOLiIiINDblFY17jFh6toypsE4VOR72/XTTiG0tPgAOaB3bwepQANis/owiYkPxofGc1OIkTmpxku++7OJs1h1Y5/tZm7mWDVkbKHYXs/bAWtaWV4x7BTgCaBnZklZRrcgqzgKgVWSrhnwblTq0ojHCzhWNh0zH1rZpERERkUaovKIx3YhTf0apE/b9dNOIbfUUg8tB6+Y9rQ4FgC37zInTKpEWEbuLDo5mQNIABiQN8N3n9rjZmbeTjVkb2Zi9kQ1ZG9iYtZGtOVspLCv0bb8GaBHRgrBA63vRHlopGGnjikan49BEo/X/u4mIiIhIHSuvaExHE6elbtj3000jlZe7m/3lFSKtWpxocTSmzeWJxrRmSjSKiP9xOV20impFq6hWnMZpvvs9hoeMggw2Z29mS84WduTuYGjLoRZGetChvQ9tXdF4SEI0NU4VjSIiIiKNjTtnFy5gjxFHr9QYq8ORRsC+n24aqa075wEQ5zGIjGphcTTg8Rhs2V+eaFRFo4g0Ik6Hk6TwJJLCkxiUMsjqcCqoOHU60MJIju7QOFNV0SgiIiLS6HiyzURjWVgSiVEhVocjjYC6ujewrXt+B6CNI9jiSEy7c4ooLvMQ4HSo/5aISANxqUejiIiIiFittIjA4gMANG/ZxtpYpNFQorGBbT2wAYBWQbEWR2Ly9mdsFRdGgKaJiog0CH/s0Zgap4pGERERkUYl1+zPWGQE0r5VqsXBSGPhF5mll19+mTZt2hASEsLAgQNZuHCh1SEdt2355kSn1hHWb5sG2OQdBKOJ0yIiDabC1GkbJxq9cQa6HNpKI36lpmvHTz/9lM6dOxMSEkKPHj347rvvKjxuGAYPPfQQycnJhIaGMmzYMNavX1+fb0FERKT+lSca0404ereyRzGU+D/bJxo//vhj7rrrLh5++GGWLl1Kr169GDFiBBkZGVaHdly2lmQB0Dquk7WBlPNWNKYp0Sgi0mD8Zeu0q3xoTYuY0Aoxi9hZTdeOc+fO5corr+S6665j2bJlXHDBBVxwwQWsXLnSd8wzzzzDv/71L1599VUWLFhAeHg4I0aMoKioqKHeloiISJ3L3bsNgD3E0qNltMXRSGNh+0Tjc889x7hx4xg7dixdu3bl1VdfJSwsjLfeesvq0GrM8HjYQikArRJ7WRyNaYsqGkVEGpy/VTS21CAY8SM1XTu++OKLjBw5krvvvpsuXbrw+OOP07dvX/79738DZjXjCy+8wAMPPMCoUaPo2bMn7777Lrt27eLLL79swHcmIiJSt/bs2ARAXlBzokLsO6BQ/It9P90AJSUlLFmyhPvuu893n9PpZNiwYcybN6/S5xQXF1NcXOz7e05OTr3H+eT71zKvcGm1js0NMj+0/W2aQanjl/oMq1o2lyca2yrRKCLSYCr0aLRzRWP5MJjUOA2CEf9wPGvHefPmcdddd1W4b8SIEb4k4ubNm0lPT2fYsGG+x6Ojoxk4cCDz5s3jiiuuOOKcVqxHd21eQ/F7l9f764iISOMR58kEwBGVYnEk0pjY99MNsG/fPtxuN4mJiRXuT0xMZM2aNZU+Z+LEiTz66KMNEZ5Pdsl+tgZV//g2xbBijwPIrbeYaiIk0EmX5CirwxARaTIcDgepcaFkFZTSPNK+vQ9TyysZe6fGWBuISDUdz9oxPT290uPT09N9j3vvq+qYw1mxHi0tKSLNs6VBX1NERBqHyLS+VocgjYitE43H47777qvwrXROTg6pqfU7PemSAXfQe9fv1T6+eeIwQk6zxzAYgNbxYcSF1yBTKiIitfb1+JMocXsIDXJZHUqVbjylLWd0aU77ZhFWhyLiV6xYjzZrkcaK09+t19cQEZHGJzgilv69T7I6DGlEbJ1oTEhIwOVysWfPngr379mzh6SkpEqfExwcTHBwcEOE53NCj2Gc0GPYsQ8UEREpF+sHX/A4nQ46JkZaHYZItR3P2jEpKemox3v/3LNnD8nJyRWO6d27d6XntGI9GhYRTY9TRjXoa4qIiIgcztbDYIKCgujXrx8zZszw3efxeJgxYwaDBg2yMDIRERERsZvjWTsOGjSowvEAP/30k+/4tLQ0kpKSKhyTk5PDggULtB4VEREROYytKxoB7rrrLq699lr69+/PCSecwAsvvEB+fj5jx461OjQRERERsZljrR2vueYaWrRowcSJEwG4/fbbGTp0KM8++yznnHMOU6dOZfHixbz++uuA2VP1jjvu4IknnqBDhw6kpaXx4IMPkpKSwgUXXGDV2xQRERGxJdsnGi+//HL27t3LQw89RHp6Or1792b69OlHNOQWERERETnW2nHbtm04nQc39QwePJgPP/yQBx54gPvvv58OHTrw5Zdf0r17d98x99xzD/n5+dxwww1kZWVx0kknMX36dEJC7DvMSURERMQKDsMwDKuDqE85OTlER0eTnZ1NVJQmK4uIiIj/0XrGv+n6iYiIiL+r7nrG1j0aRURERERERERExD8o0SgiIiIiIiIiIiK1pkSjiIiIiIiIiIiI1JoSjSIiIiIiIiIiIlJrSjSKiIiIiIiIiIhIrSnRKCIiIiIiIiIiIrWmRKOIiIiIiIiIiIjUmhKNIiIiIiIiIiIiUmtKNIqIiIiIiIiIiEitKdEoIiIiIiIiIiIitRZgdQD1zTAMAHJyciyOREREROT4eNcx3nWN+BetR0VERMTfVXc92ugTjbm5uQCkpqZaHImIiIhI7eTm5hIdHW11GFJDWo+KiIhIY3Gs9ajDaORfjXs8Hnbt2kVkZCQOh6PeXicnJ4fU1FS2b99OVFRUvb2O1Jyujb3p+tiXro296frYV31cG8MwyM3NJSUlBadTnW/8jdajomtjb7o+9qVrY2+6PvZl5Xq00Vc0Op1OWrZs2WCvFxUVpf+D2ZSujb3p+tiXro296frYV11fG1Uy+i+tR8VL18bedH3sS9fG3nR97MuK9ai+EhcREREREREREZFaU6JRREREREREREREak2JxjoSHBzMww8/THBwsNWhyGF0bexN18e+dG3sTdfHvnRtxCr6b8++dG3sTdfHvnRt7E3Xx76svDaNfhiMiIiIiIiIiIiI1D9VNIqIiIiIiIiIiEitKdEoIiIiIiIiIiIitaZEo4iIiIiIiIiIiNSaEo0iIiIiIiIiIiJSa0o01oGXX36ZNm3aEBISwsCBA1m4cKHVITU5EydOZMCAAURGRtK8eXMuuOAC1q5dW+GYoqIixo8fT3x8PBEREVx88cXs2bPHooibrqeeegqHw8Edd9zhu0/Xxlo7d+7kL3/5C/Hx8YSGhtKjRw8WL17se9wwDB566CGSk5MJDQ1l2LBhrF+/3sKImw63282DDz5IWloaoaGhtGvXjscff5xD57jp+jSMX375hfPOO4+UlBQcDgdffvllhcercx0yMzMZPXo0UVFRxMTEcN1115GXl9eA70IaM61H7UFrUv+hNan9aE1qT1qP2os/rEmVaKyljz/+mLvuuouHH36YpUuX0qtXL0aMGEFGRobVoTUpc+bMYfz48cyfP5+ffvqJ0tJShg8fTn5+vu+YO++8k2+++YZPP/2UOXPmsGvXLi666CILo256Fi1axGuvvUbPnj0r3K9rY50DBw4wZMgQAgMD+f7771m1ahXPPvsssbGxvmOeeeYZ/vWvf/Hqq6+yYMECwsPDGTFiBEVFRRZG3jQ8/fTTvPLKK/z73/9m9erVPP300zzzzDO89NJLvmN0fRpGfn4+vXr14uWXX6708epch9GjR/Pnn3/y008/MW3aNH755RduuOGGhnoL0ohpPWofWpP6B61J7UdrUvvSetRe/GJNakitnHDCCcb48eN9f3e73UZKSooxceJEC6OSjIwMAzDmzJljGIZhZGVlGYGBgcann37qO2b16tUGYMybN8+qMJuU3Nxco0OHDsZPP/1kDB061Lj99tsNw9C1sdq9995rnHTSSVU+7vF4jKSkJOOf//yn776srCwjODjY+OijjxoixCbtnHPOMf76179WuO+iiy4yRo8ebRiGro9VAOOLL77w/b0612HVqlUGYCxatMh3zPfff284HA5j586dDRa7NE5aj9qX1qT2ozWpPWlNal9aj9qXXdekqmishZKSEpYsWcKwYcN89zmdToYNG8a8efMsjEyys7MBiIuLA2DJkiWUlpZWuFadO3emVatWulYNZPz48ZxzzjkVrgHo2ljt66+/pn///lx66aU0b96cPn36MHnyZN/jmzdvJj09vcL1iY6OZuDAgbo+DWDw4MHMmDGDdevWAfD777/z66+/ctZZZwG6PnZRneswb948YmJi6N+/v++YYcOG4XQ6WbBgQYPHLI2H1qP2pjWp/WhNak9ak9qX1qP+wy5r0oA6OUsTtW/fPtxuN4mJiRXuT0xMZM2aNRZFJR6PhzvuuIMhQ4bQvXt3ANLT0wkKCiImJqbCsYmJiaSnp1sQZdMydepUli5dyqJFi454TNfGWps2beKVV17hrrvu4v7772fRokXcdtttBAUFce211/quQWW/53R96t/f//53cnJy6Ny5My6XC7fbzZNPPsno0aMBdH1sojrXIT09nebNm1d4PCAggLi4OF0rqRWtR+1La1L70ZrUvrQmtS+tR/2HXdakSjRKozN+/HhWrlzJr7/+anUoAmzfvp3bb7+dn376iZCQEKvDkcN4PB769+/PP/7xDwD69OnDypUrefXVV7n22mstjk4++eQTPvjgAz788EO6devG8uXLueOOO0hJSdH1ERGxOa1J7UVrUnvTmtS+tB6VmtLW6VpISEjA5XIdMYlsz549JCUlWRRV0zZhwgSmTZvGrFmzaNmype/+pKQkSkpKyMrKqnC8rlX9W7JkCRkZGfTt25eAgAACAgKYM2cO//rXvwgICCAxMVHXxkLJycl07dq1wn1dunRh27ZtAL5roN9z1rj77rv5+9//zhVXXEGPHj24+uqrufPOO5k4cSKg62MX1bkOSUlJRwzmKCsrIzMzU9dKakXrUXvSmtR+tCa1N61J7UvrUf9hlzWpEo21EBQURL9+/ZgxY4bvPo/H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AXDgwAHWrVtHly5djuOdiYiIiIg/0HpURPyBhsGIiFTD+PHjyczM5Morr2TRokVs3LiRH374gbFjx1ZYnB3qjjvu4IcffmDz5s0sXbqUWbNm+RZfrVu3xuFwMG3aNPbu3UteXh6RkZH87W9/48477+Sdd95h48aNLF26lJdeeol33nmnwrkfe+wxZsyYwcqVKxkzZgwJCQkVJhmKiIiISOOi9aiI+AMlGkVEqiElJYXffvsNt9vN8OHD6dGjB3fccQcxMTE4nZX/KnW73YwfP54uXbowcuRIOnbsyH/+8x8AWrRowaOPPsrf//53EhMTmTBhAgCPP/44Dz74IBMnTvQ979tvvyUtLa3CuZ966iluv/12+vXrR3p6Ot98843vW2kRERERaXy0HhURf+AwDMOwOggREame2bNnc9ppp3HgwAFiYmKsDkdEREREmhitR0XkaFTRKCIiIiIiIiIiIrWmRKOIiIiIiIiIiIjUmrZOi4iIiIiIiIiISK2polFERERERERERERqTYlGERERERERERERqTUlGkVERERERERERKTWlGgUERERERERERGRWlOiUURERERERERERGpNiUYRERERERERERGpNSUaRUREREREREREpNaUaBQREREREREREZFa+/8RnBH3vuZ4GAAAAABJRU5ErkJggg==\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAABRoAAAHWCAYAAAAYQDX3AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOzddXhU19bH8e9M3EOAkADB3YNLhRZKlZa6U3fX+3Irl1uj7i31UtdbFyiFAm1xd7cgwZMQl5n3j51JQkkgMjNnZvL7PE+ec0hmZi9aBs6ss/ZaNqfT6URERERERERERESkDuxWByAiIiIiIiIiIiL+T4lGERERERERERERqTMlGkVERERERERERKTOlGgUERERERERERGROlOiUUREREREREREROpMiUYRERERERERERGpMyUaRUREREREREREpM6UaBQREREREREREZE6U6JRRERERERERERE6kyJRhGRSkyYMAGbzcbmzZsBGDp0KEOHDj3kMbt27eK8886jYcOG2Gw2XnzxRa/HKSIiIiKBS9ekIuJvlGgUEamlu+66i0mTJjFmzBg++ugjTjnlFAAef/xxzjzzTJo0aYLNZmPs2LHWBioiIiIiAauya9LVq1dz//3306tXL2JiYkhOTub0009n/vz5VocrIgEu2OoARET8wW+//XbY96ZOncpZZ53Fvffee8j3H3zwQZKSkkhNTWXSpEneClFEREREAlx1r0nvvfde3n33Xc4991xuvvlmMjMzefPNNxk4cCATJ05k+PDh3gxbROoRJRpFRKohNDT0sO/t3r2b+Pj4w76/adMmWrVqxd69e2ncuLEXohMRERGR+qC616QXX3wxY8eOJTo6uux7V199NZ07d2bs2LFKNIqIx2jrtIhINVTsh+PqleN0Onnttdew2WzYbLayx7Zq1cqaIEVEREQkoFX3mrRPnz6HJBkBGjZsyLHHHsuqVau8HbaI1CNKNIqI1NBxxx3HRx99BMBJJ53ERx99VPZrERERERFvqM01aXp6Oo0aNfJGeCJST2nrtIhIDbVp04Y2bdpw+eWX06FDBy677DKrQxIRERGReqam16R//vkns2bN4sEHH/RShCJSH6miUURERERERCSA7d69m0suuYTWrVtz//33Wx2OiAQwVTSKiIiIiIiIBKicnBzOOOMMDh48yF9//XVY70YREXdSolFEREREREQkABUWFnLOOeewdOlSJk2aRLdu3awOSUQCnBKNIiIiIiIiIgHG4XAwevRopkyZwpdffsnxxx9vdUgiUg8o0SgiIiIiIiISYG677Ta++OIL3nzzTc455xyrwxGRekKJRhERN/voo4/YsmULubm5AMyYMYPHHnsMgMsvv5yWLVtaGZ6IiIiIBLgXX3yR119/nUGDBhEZGcnHH398yM/PPvtsoqKiLIpORAKZEo0iIm727rvvMn369LJf//HHH/zxxx8AHHPMMUo0ioiIiIhHLV68GIBZs2Yxa9asw36+adMmJRpFxCNsTqfTaXUQIiIiIiIiIiIi4t/sVgcgIiIiIiIiIiIi/k+JRhEREREREREREakzJRpFRERERERERESkzpRoFBERERERERERkTpTolFERERERERERETqTIlGERERERERERERqbNgqwPwNIfDwY4dO4iJicFms1kdjoiIiEiNOZ1ODh48SNOmTbHbdZ/Y3+h6VERERPxdda9HAz7RuGPHDlJSUqwOQ0RERKTO0tLSaN68udVhSA3pelREREQCxdGuRwM+0RgTEwOY/xCxsbEWRyMiIiJSc1lZWaSkpJRd14h/0fWoiIiI+LvqXo8GfKLRtT0lNjZWF3YiIiLi17Tt1j/pelREREQCxdGuR9XkR0REREREREREROpMiUYRERERERERERGpMyUaRUREREREREREpM6UaBQREREREREREZE6U6JRRERERERERERE6kyJRhERERGpN8aPH0+PHj3KJkAPGjSIX3/9tcrHT5gwAZvNdshXeHi4FyMWERER8R/BVgcgIiIiIuItzZs358knn6R9+/Y4nU4++OADzjrrLBYtWkTXrl0rfU5sbCxr1qwp+7XNZvNWuCIiIiJ+RYlGEREREak3Ro4cecivH3/8ccaPH8/s2bOrTDTabDaSkpK8EZ6IiIiIX7N06/SMGTMYOXIkTZs2xWaz8d133x3yc6fTycMPP0xycjIREREMHz6cdevWWROsiIiIiASUkpISPv/8c3Jychg0aFCVj8vOzqZly5akpKRw1llnsWLFiiO+bkFBAVlZWYd8iYiIiNQHliYac3Jy6NmzJ6+99lqlP3/66ad5+eWXeeONN5gzZw5RUVGcfPLJ5OfnezlSEREREQkUy5YtIzo6mrCwMG688Ua+/fZbunTpUulj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hATvbf75z3/y4osv8uqrr7J48WKioqIYP3485eXlJkYeHJ566ileeeUVXnrpJdavX89TTz3FP//5T/71r395byOPT8soKSmhf//+vPzyy/V+vSGPw2WXXcbatWuZPXs23377LQsWLOCGG25oqX+CCGByPmodck7qH+Sc1HrknNS65HzUWvzinFQXzTJs2DB94sSJ3v92Op1669at9WnTppkYlcjJydEBff78+bqu63p+fr4eEhKif/rpp97brF+/Xgf0hQsXmhVmUCkqKtK7du2qz549Wx89erR+22236bouj43Z7r77bv3YY4894tddLpeelpamP/30097P5efn62FhYfp///vflggxqJ1++un6NddcU+dz5557rn7ZZZfpui6Pj1kA/csvv/T+d0Meh3Xr1umAvmTJEu9tfvjhB13TNH3Pnj0tFrsITHI+al1yTmo9ck5qTXJOal1yPmpdVj0nlYrGZqisrGTZsmWMHTvW+zmbzcbYsWNZuHChiZGJgoICABITEwFYtmwZVVVVdR6rHj160K5dO3msWsjEiRM5/fTT6zwGII+N2b7++muGDBnCBRdcQEpKCgMHDuT111/3fn379u1kZWXVeXzi4uIYPny4PD4tYOTIkcyZM4dNmzYB8Oeff/Lrr79y6qmnAvL4WEVDHoeFCxcSHx/PkCFDvLcZO3YsNpuNxYsXt3jMInDI+ai1yTmp9cg5qTXJOal1yfmo/7DKOanDkKMEqQMHDuB0OklNTa3z+dTUVDZs2GBSVMLlcjFp0iRGjRpFnz59AMjKyiI0NJT4+Pg6t01NTSUrK8uEKIPLRx99xPLly1myZMlhX5PHxlzbtm3jlVdeYfLkydx7770sWbKEW2+9ldDQUK688krvY1Df7zl5fHzvnnvuobCwkB49emC323E6nTz++ONcdtllAPL4WERDHoesrCxSUlLqfN3hcJCYmCiPlWgWOR+1LjkntR45J7UuOSe1Ljkf9R9WOSeVRKMIOBMnTmTNmjX8+uuvZocigMzMTG677TZmz55NeHi42eGIQ7hcLoYMGcITTzwBwMCBA1mzZg2vvvoqV155pcnRiU8++YQPPviADz/8kN69e7Ny5UomTZpE69at5fERQgiLk3NSa5FzUmuTc1LrkvNR0VjSOt0MycnJ2O32wzaRZWdnk5aWZlJUwe2WW27h22+/Ze7c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",
                         "text/plain": [
                             "<Figure size 1600x500 with 2 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -961,52 +829,41 @@
             "metadata": {},
             "source": [
                 "As we can see, the spikes provided by the `SpikeGenerator` are sucessfully sent to the first `LIF` population. which in turn sends its output spikes to the second `LIF` population."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 23,
             "id": "a922b4aa",
             "metadata": {},
             "outputs": [],
             "source": [
                 "lif2.stop()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "a9fadbe3",
             "metadata": {},
             "source": [
                 "### Summary\n",
                 "\n",
                 "- Define custom a `Process` by inheritance from `AbstractProcess`\n",
                 "- `Vars` are used to store internal data in the `Process`\n",
                 "- `Ports` are used to connect to other `Processes`\n",
                 "- The behavior of a `Process` is defined in a `ProcessModel`\n",
                 "- `ProcessModels` are aware of their hardware backend, they get selected automatically by the compiler/runtime\n",
                 "- `PyProcessModels` run on CPU\n",
-                "- Number and names of `Vars` and `Ports` of a `ProcessModel` must match those of the `Process` it implements"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "f90d252c",
-            "metadata": {},
-            "source": [
+                "- Number and names of `Vars` and `Ports` of a `ProcessModel` must match those of the `Process` it implements\n",
+                "\n",
                 "### Learn more about\n",
-                "- [ProcessModels](https://github.com/lava-nc/lava/blob/main/tutorials/in_depth/tutorial03_process_models.ipynb)\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "2e335eee",
-            "metadata": {},
-            "source": [
+                "- [ProcessModels](https://github.com/lava-nc/lava/blob/main/tutorials/in_depth/tutorial03_process_models.ipynb)\n",
+                "\n",
                 "### How to learn more?\n",
                 "\n",
                 "If you want to find out more about Lava, have a look at the [Lava documentation](https://lava-nc.org/) or dive deeper with the [in-depth tutorials](https://github.com/lava-nc/lava/tree/main/tutorials/in_depth).\n",
                 "\n",
                 "To receive regular updates on the latest developments and releases of the Lava Software Framework please subscribe to [our newsletter](http://eepurl.com/hJCyhb)."
             ]
         }
@@ -1023,13 +880,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.4"
+            "version": "3.10.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lava_nc-0.7.0.post2/tutorials/end_to_end/tutorial01_mnist_digit_classification.ipynb` & `lava_nc-0.8.0/tutorials/end_to_end/tutorial01_mnist_digit_classification.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9512370959857372%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '*Copyright (C) 2021 Intel Corporation*<br>\\n'), (1, "*

 * *            "'*SPDX-License-Identifier: BSD-3-Clause*<br>\\n'), (2, '*See: "*

 * *            "https://spdx.org/licenses/*\\n'), (3, '\\n'), (4, '---\\n'), (5, '\\n'), (6, '# MNIST "*

 * *            "Digit Classification with Lava\\n'), (7, '\\n'), (8, '_**Motivation**: In this "*

 * *            "tutorial, we will build a Lava Process for an MNIST\\n'), (9, 'classifier, using the "*

 * *            "Lava Processes for LIF neuron […]*

```diff
@@ -1,91 +1,62 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "*Copyright (C) 2021 Intel Corporation*<br>\n",
                 "*SPDX-License-Identifier: BSD-3-Clause*<br>\n",
                 "*See: https://spdx.org/licenses/*\n",
                 "\n",
                 "---\n",
                 "\n",
-                "# MNIST Digit Classification with Lava"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "# MNIST Digit Classification with Lava\n",
+                "\n",
                 "_**Motivation**: In this tutorial, we will build a Lava Process for an MNIST\n",
                 "classifier, using the Lava Processes for LIF neurons and Dense connectivity.\n",
-                "The tutorial is useful to get started with Lava in a few minutes._"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "The tutorial is useful to get started with Lava in a few minutes._\n",
+                "\n",
                 "#### This tutorial assumes that you:\n",
                 "- have the [Lava framework installed](../in_depth/tutorial01_installing_lava.ipynb \"Tutorial on Installing Lava\")\n",
                 "- are familiar with the [Process concept in Lava](../in_depth/tutorial02_processes.ipynb \"Tutorial on Processes\")\n",
                 "\n",
                 "#### This tutorial gives a bird's-eye view of\n",
                 "- how Lava Process(es) can perform the MNIST digit classification task using\n",
                 "[Leaky Integrate-and-Fire (LIF)](https://github.com/lava-nc/lava/tree/main/src/lava/proc/lif \"Lava's LIF neuron\") neurons and [Dense\n",
                 "(fully connected)](https://github.com/lava-nc/lava/tree/main/src/lava/proc/dense \"Lava's Dense Connectivity\") connectivity.\n",
                 "- how to create a Process \n",
                 "- how to create Python ProcessModels \n",
                 "- how to connect Processes\n",
-                "- how to execute them"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "- how to execute them\n",
+                "\n",
                 "#### Our MNIST Classifier\n",
                 "In this tutorial, we will build a multi-layer feed-forward classifier without\n",
                 " any convolutional layers. The architecture is shown below.\n",
                 "\n",
                 "> **Important Note**:\n",
                 ">\n",
                 "> The classifier is a simple feed-forward model using pre-trained network \n",
                 "> parameters (weights and biases). It illustrates how to build, compile and \n",
                 "> run a functional model in Lava. Please refer to \n",
                 "> [Lava-DL](https://github.com/lava-nc/lava-dl) to understand how to train \n",
-                "> deep networks with Lava."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "> deep networks with Lava.\n",
+                "\n",
                 "<center><img src=\"https://raw.githubusercontent.com/lava-nc/lava-nc.github.io/main/_static/images/tutorial01/mnist_process_arch.png\" alt=\"MNIST Process AA\"\n",
-                "style=\"width: 800px;\"/></center>"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "style=\"width: 800px;\"/></center>\n",
+                "\n",
                 "The 3 Processes shown above are:\n",
                 " - *SpikeInput* Process - generates spikes via integrate and fire dynamics,\n",
                 " using the image input\n",
                 " - *ImageClassifier* Process - encapsulates feed-forward architecture of\n",
                 " Dense connectivity and LIF neurons\n",
                 " - *Output* Process - accumulates output spikes from the feed-forward process\n",
-                "and infers the class label"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "and infers the class label\n",
+                "\n",
                 "#### General Imports"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
@@ -234,14 +205,15 @@
                 "\n",
                 "# Import MNIST dataset\n",
                 "from lava.utils.dataloader.mnist import MnistDataset\n",
                 "np.set_printoptions(linewidth=np.inf)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
@@ -253,21 +225,16 @@
                 "according to the `LoihiProtocol`. Which means, similar to the Loihi \n",
                 "chip, each time-step is divided into _spiking_, _pre-management_, \n",
                 "_post-management_, and _learning_ phases. It is necessary to specify \n",
                 "behaviour of a ProcessModel during the spiking phase using `run_spk` \n",
                 "function. Other phases are optional.\n",
                 "- `@requires`: specifies the hardware resource on which a ProcessModel \n",
                 "will be executed. In this tutorial, we will execute all ProcessModels \n",
-                "on a CPU."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "on a CPU.\n",
+                "\n",
                 "**SpikingInput ProcessModel**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
@@ -486,28 +453,24 @@
                 "spike_input.spikes_out.connect(mnist_clf.spikes_in)\n",
                 "mnist_clf.spikes_out.connect(output_proc.spikes_in)\n",
                 "# Connect Input directly to Output for ground truth labels\n",
                 "spike_input.label_out.connect(output_proc.label_in)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If you receive an ``UnpicklingError`` when instantiating the ``ImageClassifier``, make sure to download the pretrained weights from GitHub LFS in the current directory using:\n",
                 "```bash\n",
                 "   git lfs fetch\n",
                 "   git lfs pull\n",
-                "```"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "```\n",
+                "\n",
                 "#### Execution and results\n",
                 "Below, we will run the classifier process in a loop of `num_images`\n",
                 "number of iterations. Each iteration will run the Process for \n",
                 "`num_steps_per_image` number of time-steps. \n",
                 "\n",
                 "We take this approach to clear the neural states of all three LIF \n",
                 "layers inside the classifier after every image. We need to clear \n",
@@ -572,30 +535,26 @@
                 "\n",
                 "print(f\"\\nGround truth: {ground_truth}\\n\"\n",
                 "      f\"Predictions : {predictions}\\n\"\n",
                 "      f\"Accuracy    : {accuracy}\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> **Important Note**:\n",
                 ">\n",
                 "> The classifier is a simple feed-forward model using pre-trained network \n",
                 "> parameters (weights and biases). It illustrates how to build, compile and \n",
                 "> run a functional model in Lava. Please refer to \n",
                 "> [Lava-DL](https://github.com/lava-nc/lava-dl) to understand how to train \n",
-                "> deep networks with Lava."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "> deep networks with Lava.\n",
+                "\n",
                 "## How to learn more?\n",
                 "\n",
                 "#### Follow the links below for deep-dive tutorials on the concepts in this tutorial:\n",
                 "- [Processes](../in_depth/tutorial02_processes.ipynb \"Tutorial on Processes\")\n",
                 "- [ProcessModel](../in_depth/tutorial03_process_models.ipynb \"Tutorial on ProcessModels\")\n",
                 "- [Execution](../in_depth/tutorial04_execution.ipynb \"Tutorial on Executing Processes\")\n",
                 "- [SubProcessModels](../in_depth/tutorial06_hierarchical_processes.ipynb) or [Hierarchical Processes](../in_depth/tutorial06_hierarchical_processes.ipynb)\n",
@@ -619,15 +578,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.10"
+            "version": "3.10.6"
         },
         "vscode": {
             "interpreter": {
                 "hash": "7ebb4c32c029abbab1fd16ef4d8ac43152261b56d4033e55d2744ce843ecba08"
             }
         }
     },
```

### Comparing `lava_nc-0.7.0.post2/tutorials/end_to_end/tutorial02_excitatory_inhibitory_network.ipynb` & `lava_nc-0.8.0/tutorials/end_to_end/tutorial02_excitatory_inhibitory_network.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/in_depth/three_factor_learning/tutorial01_Reward_Modulated_STDP.ipynb` & `lava_nc-0.8.0/tutorials/in_depth/three_factor_learning/tutorial01_Reward_Modulated_STDP.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/in_depth/three_factor_learning/utils.py` & `lava_nc-0.8.0/tutorials/in_depth/three_factor_learning/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 # Copyright (C) 2021-22 Intel Corporation
 # SPDX-License-Identifier: BSD-3-Clause
 # See: https://spdx.org/licenses/
 
 import matplotlib.pyplot as plt
-import typing as ty
 import numpy as np
 
-from lava.proc.lif.process import LIF, AbstractLIF, LogConfig, LearningLIF
-from lava.proc.io.source import RingBuffer
-from lava.proc.dense.process import LearningDense, Dense
-from lava.magma.core.process.neuron import LearningNeuronProcess
-from lava.proc.learning_rules.r_stdp_learning_rule import RewardModulatedSTDP
-from lava.magma.core.process.variable import Var
-from lava.magma.core.process.ports.ports import InPort, OutPort
+from lava.proc.lif.process import LearningLIF
 from lava.magma.core.model.py.neuron import (
     LearningNeuronModelFloat, LearningNeuronModelFixed
 )
 from lava.magma.core.sync.protocols.loihi_protocol import LoihiProtocol
-from lava.magma.core.model.py.ports import PyInPort, PyOutPort
+from lava.magma.core.model.py.ports import PyOutPort
 from lava.magma.core.model.py.type import LavaPyType
 from lava.magma.core.resources import CPU
 from lava.magma.core.decorator import implements, requires, tag
 from lava.proc.lif.models import (
     AbstractPyLifModelFloat, AbstractPyLifModelFixed
 )
 
@@ -184,125 +177,130 @@
 
         self.s_out_bap.send(self.s_out_buff)
         self.s_out_y1.send(self.y1)
         self.s_out_y2.send(self.y2)
         self.s_out_y3.send(self.y3)
 
 
-def generate_post_spikes(pre_spike_times, 
-        num_steps, spike_prob_post):
+def generate_post_spikes(pre_spike_times, num_steps, spike_prob_post):
     """generates specific post synaptic spikes to
     demonstrate potentiation and depression.
     """
-    pre_synaptic_spikes = np.where(pre_spike_times==1)[1]
+    pre_synaptic_spikes = np.where(pre_spike_times == 1)[1]
 
     spike_raster_post = np.zeros((len(spike_prob_post), num_steps))
 
     for ts in range(num_steps):
         for pre_ts in pre_synaptic_spikes:
-            if ts in range(pre_ts, pre_ts+20):
+            if ts in range(pre_ts, pre_ts + 20):
                 if np.random.rand(1) < spike_prob_post[0]:
                     spike_raster_post[0][ts] = 1
 
     for ts in range(num_steps):
         for pre_ts in pre_synaptic_spikes:
-            if ts in range(pre_ts-12, pre_ts-2):
+            if ts in range(pre_ts - 12, pre_ts - 2):
                 if np.random.rand(1) < spike_prob_post[1]:
                     spike_raster_post[1][ts] = 1
-    
+
     return spike_raster_post
 
+
 def plot_spikes(spikes, figsize, legend, colors, title, num_steps):
     offsets = list(range(1, len(spikes) + 1))
-    num_x_ticks = np.arange(0, num_steps+1, 25)
-    
+    num_x_ticks = np.arange(0, num_steps + 1, 25)
+
     plt.figure(figsize=figsize)
 
-    spikes_plot = plt.eventplot(positions=spikes, 
-                                lineoffsets=offsets,
-                                linelength=0.9,
-                                colors=colors)
+    plt.eventplot(positions=spikes,
+                  lineoffsets=offsets,
+                  linelength=0.9,
+                  colors=colors)
 
     plt.title(title)
     plt.xlabel("Time steps")
     plt.ylabel("Neurons")
 
     plt.xticks(num_x_ticks)
     plt.grid(which='minor', color='lightgrey', linestyle=':', linewidth=0.5)
     plt.grid(which='major', color='lightgray', linewidth=0.8)
     plt.minorticks_on()
-    
+
     plt.yticks(ticks=offsets, labels=legend)
 
-    
     plt.show()
 
+
 def plot_time_series(time, time_series, ylabel, title, figsize, color):
     plt.figure(figsize=figsize)
     plt.step(time, time_series, color=color)
-   
+
     plt.title(title)
     plt.xlabel("Time steps")
     plt.grid(which='minor', color='lightgrey', linestyle=':', linewidth=0.5)
     plt.grid(which='major', color='lightgray', linewidth=0.8)
     plt.minorticks_on()
 
     plt.ylabel(ylabel)
-    
+
     plt.show()
 
-def plot_time_series_subplots(time, time_series_y1, time_series_y2, ylabel, title, figsize, color, legend, leg_loc="upper left"):    
+
+def plot_time_series_subplots(time, time_series_y1, time_series_y2, ylabel,
+                              title, figsize, color, legend,
+                              leg_loc="upper left"):
     plt.figure(figsize=figsize)
-    
+
     plt.step(time, time_series_y1, label=legend[0], color=color[0])
     plt.step(time, time_series_y2, label=legend[1], color=color[1])
-        
+
     plt.title(title)
     plt.xlabel("Time steps")
     plt.ylabel(ylabel)
     plt.grid(which='minor', color='lightgrey', linestyle=':', linewidth=0.5)
     plt.grid(which='major', color='lightgray', linewidth=0.8)
     plt.minorticks_on()
     plt.xlim(0, len(time_series_y1))
 
     plt.legend(loc=leg_loc)
-    
+
     plt.show()
 
-def plot_spikes_time_series(time, time_series, spikes, figsize, legend, colors, title, num_steps):
+
+def plot_spikes_time_series(time, time_series, spikes, figsize, legend,
+                            colors, title, num_steps):
 
     offsets = list(range(1, len(spikes) + 1))
-    num_x_ticks = np.arange(0, num_steps+1, 25)
-    
+    num_x_ticks = np.arange(0, num_steps + 1, 25)
+
     plt.figure(figsize=figsize)
-    
+
     plt.subplot(211)
-    plt.eventplot(positions=spikes, 
+    plt.eventplot(positions=spikes,
                   lineoffsets=offsets,
                   linelength=0.9,
                   colors=colors)
 
     plt.title("Spike Arrival")
     plt.xlabel("Time steps")
 
     plt.xticks(num_x_ticks)
     plt.xlim(0, num_steps)
     plt.grid(which='minor', color='lightgrey', linestyle=':', linewidth=0.5)
     plt.grid(which='major', color='lightgray', linewidth=0.8)
     plt.minorticks_on()
-    
+
     plt.yticks(ticks=offsets, labels=legend)
     plt.tight_layout(pad=3.0)
 
     plt.subplot(212)
     plt.step(time, time_series, color=colors)
-   
+
     plt.title(title[0])
     plt.xlabel("Time steps")
     plt.grid(which='minor', color='lightgrey', linestyle=':', linewidth=0.5)
     plt.grid(which='major', color='lightgray', linewidth=0.8)
     plt.minorticks_on()
     plt.margins(x=0)
 
     plt.ylabel("Trace Value")
-    
+
     plt.show()
```

### Comparing `lava_nc-0.7.0.post2/tutorials/in_depth/tutorial01_installing_lava.ipynb` & `lava_nc-0.8.0/tutorials/in_depth/tutorial01_installing_lava.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/in_depth/tutorial02_processes.ipynb` & `lava_nc-0.8.0/tutorials/in_depth/tutorial02_processes.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/in_depth/tutorial03_process_models.ipynb` & `lava_nc-0.8.0/tutorials/in_depth/tutorial03_process_models.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/in_depth/tutorial04_execution.ipynb` & `lava_nc-0.8.0/tutorials/in_depth/tutorial04_execution.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/in_depth/tutorial05_connect_processes.ipynb` & `lava_nc-0.8.0/tutorials/in_depth/tutorial05_connect_processes.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/in_depth/tutorial06_hierarchical_processes.ipynb` & `lava_nc-0.8.0/tutorials/in_depth/tutorial06_hierarchical_processes.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/in_depth/tutorial07_remote_memory_access.ipynb` & `lava_nc-0.8.0/tutorials/in_depth/tutorial07_remote_memory_access.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/in_depth/tutorial08_stdp.ipynb` & `lava_nc-0.8.0/tutorials/in_depth/tutorial08_stdp.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/in_depth/tutorial09_custom_learning_rules.ipynb` & `lava_nc-0.8.0/tutorials/in_depth/tutorial09_custom_learning_rules.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0.post2/tutorials/in_depth/tutorial10_sigma_delta_neurons.ipynb` & `lava_nc-0.8.0/tutorials/in_depth/tutorial10_sigma_delta_neurons.ipynb`

 * *Files identical despite different names*

