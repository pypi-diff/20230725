# Comparing `tmp/triton_model_navigator-0.6.2-py3-none-any.whl.zip` & `tmp/triton_model_navigator-0.6.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,147 +1,147 @@
-Zip file size: 254449 bytes, number of entries: 145
--rw-r--r--  2.0 unx      881 b- defN 23-Jul-18 03:12 model_navigator/__init__.py
--rw-r--r--  2.0 unx      649 b- defN 23-Jul-19 07:20 model_navigator/__version__.py
--rw-r--r--  2.0 unx     3915 b- defN 23-Jul-18 03:12 model_navigator/exceptions.py
--rw-r--r--  2.0 unx     1716 b- defN 23-Jul-18 03:12 model_navigator/api/__init__.py
--rw-rw-rw-  2.0 unx    24220 b- defN 23-Jul-19 07:20 model_navigator/api/config.py
--rw-rw-rw-  2.0 unx     6263 b- defN 23-Jul-19 07:20 model_navigator/api/jax.py
--rw-rw-rw-  2.0 unx     5268 b- defN 23-Jul-19 07:20 model_navigator/api/onnx.py
--rw-rw-rw-  2.0 unx    16279 b- defN 23-Jul-19 07:20 model_navigator/api/package.py
--rw-r--r--  2.0 unx     4795 b- defN 23-Jul-18 03:12 model_navigator/api/python.py
--rw-rw-rw-  2.0 unx     7751 b- defN 23-Jul-19 07:20 model_navigator/api/pytriton.py
--rw-rw-rw-  2.0 unx     6350 b- defN 23-Jul-19 07:20 model_navigator/api/tensorflow.py
--rw-rw-rw-  2.0 unx     6158 b- defN 23-Jul-19 07:20 model_navigator/api/torch.py
--rw-rw-rw-  2.0 unx     1585 b- defN 23-Jul-19 07:20 model_navigator/api/triton.py
--rw-r--r--  2.0 unx     1811 b- defN 23-Jul-18 03:12 model_navigator/api/utilities.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/__init__.py
--rw-rw-rw-  2.0 unx     5542 b- defN 23-Jul-19 07:20 model_navigator/commands/base.py
--rw-r--r--  2.0 unx     9486 b- defN 23-Jul-18 03:12 model_navigator/commands/execution_context.py
--rw-r--r--  2.0 unx    12793 b- defN 23-Jul-18 03:12 model_navigator/commands/infer_metadata.py
--rw-r--r--  2.0 unx     3325 b- defN 23-Jul-18 03:12 model_navigator/commands/load.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/__init__.py
--rw-rw-rw-  2.0 unx     9876 b- defN 23-Jul-19 07:20 model_navigator/commands/convert/base.py
--rw-rw-rw-  2.0 unx     7642 b- defN 23-Jul-19 07:20 model_navigator/commands/convert/tf.py
--rw-rw-rw-  2.0 unx    10251 b- defN 23-Jul-19 07:20 model_navigator/commands/convert/torch.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/converters/__init__.py
--rw-r--r--  2.0 unx     3418 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/converters/sm2tftrt.py
--rw-r--r--  2.0 unx     3105 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/converters/ts2onnx.py
--rw-rw-rw-  2.0 unx     4992 b- defN 23-Jul-18 14:03 model_navigator/commands/convert/converters/ts2torchtrt.py
--rw-r--r--  2.0 unx      680 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/onnx/__init__.py
--rw-r--r--  2.0 unx     1727 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
--rw-rw-rw-  2.0 unx    11390 b- defN 23-Jul-19 07:20 model_navigator/commands/convert/onnx/onnx2trt.py
--rw-r--r--  2.0 unx     2235 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/onnx/trt_load_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/copy/__init__.py
--rw-r--r--  2.0 unx     1798 b- defN 23-Jul-18 03:12 model_navigator/commands/copy/onnx.py
--rw-r--r--  2.0 unx      678 b- defN 23-Jul-18 03:12 model_navigator/commands/correctness/__init__.py
--rw-rw-rw-  2.0 unx     5674 b- defN 23-Jul-19 07:20 model_navigator/commands/correctness/correctness.py
--rw-r--r--  2.0 unx     4733 b- defN 23-Jul-18 03:12 model_navigator/commands/correctness/correctness_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/data_dump/__init__.py
--rw-r--r--  2.0 unx    10740 b- defN 23-Jul-18 03:12 model_navigator/commands/data_dump/samples.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/export/__init__.py
--rw-r--r--  2.0 unx     3611 b- defN 23-Jul-18 03:12 model_navigator/commands/export/jax.py
--rw-r--r--  2.0 unx     5598 b- defN 23-Jul-18 03:12 model_navigator/commands/export/tf.py
--rw-r--r--  2.0 unx     9156 b- defN 23-Jul-18 03:12 model_navigator/commands/export/torch.py
--rw-r--r--  2.0 unx     1056 b- defN 23-Jul-18 03:12 model_navigator/commands/export/exporters/__init__.py
--rw-r--r--  2.0 unx     3945 b- defN 23-Jul-18 03:12 model_navigator/commands/export/exporters/jax2savedmodel.py
--rw-r--r--  2.0 unx     3171 b- defN 23-Jul-18 03:12 model_navigator/commands/export/exporters/keras2savedmodel.py
--rw-r--r--  2.0 unx     3122 b- defN 23-Jul-18 03:12 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
--rw-r--r--  2.0 unx     3077 b- defN 23-Jul-18 03:12 model_navigator/commands/export/exporters/torch2onnx.py
--rw-r--r--  2.0 unx     2728 b- defN 23-Jul-18 03:12 model_navigator/commands/export/exporters/torch2torchscript.py
--rw-r--r--  2.0 unx      715 b- defN 23-Jul-18 03:12 model_navigator/commands/find_max_batch_size/__init__.py
--rw-r--r--  2.0 unx     7156 b- defN 23-Jul-18 03:12 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
--rw-r--r--  2.0 unx     3075 b- defN 23-Jul-18 03:12 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
--rw-r--r--  2.0 unx      784 b- defN 23-Jul-18 03:12 model_navigator/commands/performance/__init__.py
--rw-r--r--  2.0 unx     5260 b- defN 23-Jul-18 03:12 model_navigator/commands/performance/performance.py
--rw-r--r--  2.0 unx     6964 b- defN 23-Jul-18 03:12 model_navigator/commands/performance/profile.py
--rw-r--r--  2.0 unx     3104 b- defN 23-Jul-18 03:12 model_navigator/commands/performance/profile_script.py
--rw-rw-rw-  2.0 unx     7269 b- defN 23-Jul-18 15:55 model_navigator/commands/performance/profiler.py
--rw-rw-rw-  2.0 unx     5476 b- defN 23-Jul-19 07:20 model_navigator/commands/performance/results.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/verification/__init__.py
--rw-r--r--  2.0 unx     4657 b- defN 23-Jul-18 03:12 model_navigator/commands/verification/verify.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/configuration/__init__.py
--rw-rw-rw-  2.0 unx     2002 b- defN 23-Jul-19 07:20 model_navigator/configuration/common_config.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/configuration/model/__init__.py
--rw-rw-rw-  2.0 unx    15653 b- defN 23-Jul-19 07:20 model_navigator/configuration/model/model_config.py
--rw-rw-rw-  2.0 unx    13677 b- defN 23-Jul-19 07:20 model_navigator/configuration/model/model_config_builder.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/core/__init__.py
--rw-rw-rw-  2.0 unx     1389 b- defN 23-Jul-19 07:20 model_navigator/core/constants.py
--rw-r--r--  2.0 unx     5299 b- defN 23-Jul-18 03:12 model_navigator/core/logger.py
--rw-r--r--  2.0 unx     9941 b- defN 23-Jul-18 03:12 model_navigator/core/tensor.py
--rw-r--r--  2.0 unx     2147 b- defN 23-Jul-18 03:12 model_navigator/core/workspace.py
--rw-r--r--  2.0 unx     2817 b- defN 23-Jul-18 03:12 model_navigator/frameworks/__init__.py
--rw-r--r--  2.0 unx      669 b- defN 23-Jul-18 03:12 model_navigator/frameworks/jax/__init__.py
--rw-r--r--  2.0 unx     1554 b- defN 23-Jul-18 03:12 model_navigator/frameworks/jax/model.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/frameworks/onnx/__init__.py
--rw-r--r--  2.0 unx     1085 b- defN 23-Jul-18 03:12 model_navigator/frameworks/onnx/utils.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/frameworks/tensorrt/__init__.py
--rw-r--r--  2.0 unx    27191 b- defN 23-Jul-18 03:12 model_navigator/frameworks/tensorrt/cuda.py
--rw-rw-rw-  2.0 unx    10627 b- defN 23-Jul-19 07:20 model_navigator/frameworks/tensorrt/utils.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/frameworks/torch/__init__.py
--rw-r--r--  2.0 unx     1513 b- defN 23-Jul-18 03:12 model_navigator/frameworks/torch/utils.py
--rw-r--r--  2.0 unx      622 b- defN 23-Jul-18 03:12 model_navigator/package/__init__.py
--rw-r--r--  2.0 unx    12176 b- defN 23-Jul-18 03:12 model_navigator/package/builder.py
--rw-r--r--  2.0 unx     4651 b- defN 23-Jul-18 03:12 model_navigator/package/loader.py
--rw-r--r--  2.0 unx    11860 b- defN 23-Jul-18 03:12 model_navigator/package/package.py
--rw-rw-rw-  2.0 unx     2819 b- defN 23-Jul-19 07:20 model_navigator/package/profiling_results.py
--rw-rw-rw-  2.0 unx    21135 b- defN 23-Jul-19 07:20 model_navigator/package/status.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/pipelines/__init__.py
--rw-r--r--  2.0 unx     5232 b- defN 23-Jul-18 03:12 model_navigator/pipelines/pipeline.py
--rw-rw-rw-  2.0 unx    14762 b- defN 23-Jul-19 07:20 model_navigator/pipelines/pipeline_context.py
--rw-r--r--  2.0 unx     3832 b- defN 23-Jul-18 03:12 model_navigator/pipelines/pipeline_manager.py
--rw-rw-rw-  2.0 unx     9693 b- defN 23-Jul-19 07:20 model_navigator/pipelines/validation.py
--rw-rw-rw-  2.0 unx     1883 b- defN 23-Jul-19 07:20 model_navigator/pipelines/builders/__init__.py
--rw-r--r--  2.0 unx     2106 b- defN 23-Jul-18 03:12 model_navigator/pipelines/builders/correctness.py
--rw-rw-rw-  2.0 unx     5682 b- defN 23-Jul-19 07:20 model_navigator/pipelines/builders/find_device_max_batch_size.py
--rw-r--r--  2.0 unx     1660 b- defN 23-Jul-18 03:12 model_navigator/pipelines/builders/jax.py
--rw-rw-rw-  2.0 unx     2509 b- defN 23-Jul-19 07:20 model_navigator/pipelines/builders/onnx.py
--rw-r--r--  2.0 unx     2516 b- defN 23-Jul-18 03:12 model_navigator/pipelines/builders/performance.py
--rw-r--r--  2.0 unx     2239 b- defN 23-Jul-18 03:12 model_navigator/pipelines/builders/preprocessing.py
--rw-r--r--  2.0 unx     2504 b- defN 23-Jul-18 03:12 model_navigator/pipelines/builders/profiling.py
--rw-rw-rw-  2.0 unx     2921 b- defN 23-Jul-19 07:20 model_navigator/pipelines/builders/tensorflow.py
--rw-rw-rw-  2.0 unx     3326 b- defN 23-Jul-19 07:20 model_navigator/pipelines/builders/torch.py
--rw-r--r--  2.0 unx     2112 b- defN 23-Jul-18 03:12 model_navigator/pipelines/builders/verify.py
--rw-r--r--  2.0 unx      622 b- defN 23-Jul-18 03:12 model_navigator/pipelines/wrappers/__init__.py
--rw-r--r--  2.0 unx     2747 b- defN 23-Jul-18 03:12 model_navigator/pipelines/wrappers/optimize.py
--rw-rw-rw-  2.0 unx     4881 b- defN 23-Jul-18 15:55 model_navigator/pipelines/wrappers/profile.py
--rw-r--r--  2.0 unx     1584 b- defN 23-Jul-18 03:12 model_navigator/runners/__init__.py
--rw-rw-rw-  2.0 unx    13796 b- defN 23-Jul-18 15:55 model_navigator/runners/base.py
--rw-r--r--  2.0 unx     2620 b- defN 23-Jul-18 03:12 model_navigator/runners/jax.py
--rw-r--r--  2.0 unx     9999 b- defN 23-Jul-18 03:12 model_navigator/runners/onnx.py
--rw-r--r--  2.0 unx     2267 b- defN 23-Jul-18 03:12 model_navigator/runners/python.py
--rw-r--r--  2.0 unx     2290 b- defN 23-Jul-18 03:12 model_navigator/runners/registry.py
--rw-r--r--  2.0 unx     7976 b- defN 23-Jul-18 03:12 model_navigator/runners/tensorflow.py
--rw-r--r--  2.0 unx    26748 b- defN 23-Jul-18 03:12 model_navigator/runners/tensorrt.py
--rw-r--r--  2.0 unx    10041 b- defN 23-Jul-18 03:12 model_navigator/runners/torch.py
--rw-r--r--  2.0 unx     3559 b- defN 23-Jul-18 03:12 model_navigator/runners/utils.py
--rw-r--r--  2.0 unx      937 b- defN 23-Jul-18 03:12 model_navigator/runtime_analyzer/__init__.py
--rw-r--r--  2.0 unx    11714 b- defN 23-Jul-18 03:12 model_navigator/runtime_analyzer/analyzer.py
--rw-r--r--  2.0 unx     2304 b- defN 23-Jul-18 03:12 model_navigator/runtime_analyzer/strategy.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/triton/__init__.py
--rw-rw-rw-  2.0 unx     3180 b- defN 23-Jul-19 07:20 model_navigator/triton/model_config.py
--rw-r--r--  2.0 unx     5218 b- defN 23-Jul-18 03:12 model_navigator/triton/model_config_builder.py
--rw-rw-rw-  2.0 unx    23090 b- defN 23-Jul-19 07:20 model_navigator/triton/model_config_generator.py
--rw-rw-rw-  2.0 unx    15243 b- defN 23-Jul-19 07:20 model_navigator/triton/model_repository.py
--rw-rw-rw-  2.0 unx     2081 b- defN 23-Jul-19 07:20 model_navigator/triton/utils.py
--rw-rw-rw-  2.0 unx      997 b- defN 23-Jul-18 15:55 model_navigator/triton/specialized_configs/__init__.py
--rw-rw-rw-  2.0 unx     2872 b- defN 23-Jul-19 07:20 model_navigator/triton/specialized_configs/base_model_config.py
--rw-rw-rw-  2.0 unx    22326 b- defN 23-Jul-19 07:20 model_navigator/triton/specialized_configs/common.py
--rw-r--r--  2.0 unx     2229 b- defN 23-Jul-18 03:12 model_navigator/triton/specialized_configs/internal.py
--rw-rw-rw-  2.0 unx     2685 b- defN 23-Jul-19 07:20 model_navigator/triton/specialized_configs/onnx_model_config.py
--rw-r--r--  2.0 unx     1785 b- defN 23-Jul-18 03:12 model_navigator/triton/specialized_configs/python_model_config.py
--rw-r--r--  2.0 unx     2239 b- defN 23-Jul-18 03:12 model_navigator/triton/specialized_configs/pytorch_model_config.py
--rw-rw-rw-  2.0 unx     3162 b- defN 23-Jul-19 07:20 model_navigator/triton/specialized_configs/tensorflow_model_config.py
--rw-r--r--  2.0 unx     3040 b- defN 23-Jul-18 03:12 model_navigator/triton/specialized_configs/tensorrt_model_config.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/utils/__init__.py
--rw-r--r--  2.0 unx    14509 b- defN 23-Jul-18 03:12 model_navigator/utils/common.py
--rw-r--r--  2.0 unx     8132 b- defN 23-Jul-18 03:12 model_navigator/utils/dataloader.py
--rw-r--r--  2.0 unx     3902 b- defN 23-Jul-18 03:12 model_navigator/utils/devices.py
--rw-r--r--  2.0 unx     1308 b- defN 23-Jul-18 03:12 model_navigator/utils/enums.py
--rw-r--r--  2.0 unx     6163 b- defN 23-Jul-18 03:12 model_navigator/utils/environment.py
--rw-r--r--  2.0 unx     4096 b- defN 23-Jul-18 03:12 model_navigator/utils/format_helpers.py
--rw-r--r--  2.0 unx     2330 b- defN 23-Jul-18 03:12 model_navigator/utils/module.py
--rw-r--r--  2.0 unx    10140 b- defN 23-Jul-19 07:24 triton_model_navigator-0.6.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    10798 b- defN 23-Jul-19 07:24 triton_model_navigator-0.6.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 07:24 triton_model_navigator-0.6.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-19 07:24 triton_model_navigator-0.6.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    14493 b- defN 23-Jul-19 07:24 triton_model_navigator-0.6.2.dist-info/RECORD
-145 files, 769697 bytes uncompressed, 230829 bytes compressed:  70.0%
+Zip file size: 254452 bytes, number of entries: 145
+-rw-r--r--  2.0 unx      881 b- defN 23-Jul-25 01:05 model_navigator/__init__.py
+-rw-r--r--  2.0 unx      649 b- defN 23-Jul-25 11:44 model_navigator/__version__.py
+-rw-r--r--  2.0 unx     3915 b- defN 23-Jul-24 01:05 model_navigator/exceptions.py
+-rw-rw-rw-  2.0 unx     1716 b- defN 23-Jul-25 01:05 model_navigator/api/__init__.py
+-rw-rw-rw-  2.0 unx    24220 b- defN 23-Jul-25 11:44 model_navigator/api/config.py
+-rw-rw-rw-  2.0 unx     6263 b- defN 23-Jul-25 11:44 model_navigator/api/jax.py
+-rw-rw-rw-  2.0 unx     5268 b- defN 23-Jul-25 11:44 model_navigator/api/onnx.py
+-rw-rw-rw-  2.0 unx    16279 b- defN 23-Jul-25 11:44 model_navigator/api/package.py
+-rw-rw-rw-  2.0 unx     4795 b- defN 23-Jul-24 01:05 model_navigator/api/python.py
+-rw-rw-rw-  2.0 unx     7751 b- defN 23-Jul-25 11:44 model_navigator/api/pytriton.py
+-rw-rw-rw-  2.0 unx     6350 b- defN 23-Jul-25 11:44 model_navigator/api/tensorflow.py
+-rw-rw-rw-  2.0 unx     6158 b- defN 23-Jul-25 11:44 model_navigator/api/torch.py
+-rw-rw-rw-  2.0 unx     1585 b- defN 23-Jul-25 11:44 model_navigator/api/triton.py
+-rw-rw-rw-  2.0 unx     1811 b- defN 23-Jul-24 01:05 model_navigator/api/utilities.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/commands/__init__.py
+-rw-rw-rw-  2.0 unx     5542 b- defN 23-Jul-25 11:44 model_navigator/commands/base.py
+-rw-rw-rw-  2.0 unx     9486 b- defN 23-Jul-24 01:05 model_navigator/commands/execution_context.py
+-rw-rw-rw-  2.0 unx    12793 b- defN 23-Jul-24 01:05 model_navigator/commands/infer_metadata.py
+-rw-rw-rw-  2.0 unx     3325 b- defN 23-Jul-24 01:05 model_navigator/commands/load.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/commands/convert/__init__.py
+-rw-rw-rw-  2.0 unx     9876 b- defN 23-Jul-25 11:44 model_navigator/commands/convert/base.py
+-rw-rw-rw-  2.0 unx     7642 b- defN 23-Jul-25 11:44 model_navigator/commands/convert/tf.py
+-rw-rw-rw-  2.0 unx    10251 b- defN 23-Jul-25 11:44 model_navigator/commands/convert/torch.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/commands/convert/converters/__init__.py
+-rw-rw-rw-  2.0 unx     3418 b- defN 23-Jul-25 11:44 model_navigator/commands/convert/converters/sm2tftrt.py
+-rw-rw-rw-  2.0 unx     3105 b- defN 23-Jul-25 11:44 model_navigator/commands/convert/converters/ts2onnx.py
+-rw-rw-rw-  2.0 unx     4992 b- defN 23-Jul-25 11:44 model_navigator/commands/convert/converters/ts2torchtrt.py
+-rw-rw-rw-  2.0 unx      680 b- defN 23-Jul-24 01:05 model_navigator/commands/convert/onnx/__init__.py
+-rw-rw-rw-  2.0 unx     1727 b- defN 23-Jul-24 01:05 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
+-rw-rw-rw-  2.0 unx    11390 b- defN 23-Jul-25 11:44 model_navigator/commands/convert/onnx/onnx2trt.py
+-rw-rw-rw-  2.0 unx     2235 b- defN 23-Jul-24 01:05 model_navigator/commands/convert/onnx/trt_load_script.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/commands/copy/__init__.py
+-rw-rw-rw-  2.0 unx     1798 b- defN 23-Jul-24 01:05 model_navigator/commands/copy/onnx.py
+-rw-rw-rw-  2.0 unx      678 b- defN 23-Jul-24 01:05 model_navigator/commands/correctness/__init__.py
+-rw-rw-rw-  2.0 unx     5674 b- defN 23-Jul-25 11:44 model_navigator/commands/correctness/correctness.py
+-rw-rw-rw-  2.0 unx     4733 b- defN 23-Jul-24 01:05 model_navigator/commands/correctness/correctness_script.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/commands/data_dump/__init__.py
+-rw-rw-rw-  2.0 unx    10740 b- defN 23-Jul-24 01:05 model_navigator/commands/data_dump/samples.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/commands/export/__init__.py
+-rw-rw-rw-  2.0 unx     3611 b- defN 23-Jul-24 01:05 model_navigator/commands/export/jax.py
+-rw-rw-rw-  2.0 unx     5598 b- defN 23-Jul-24 01:05 model_navigator/commands/export/tf.py
+-rw-rw-rw-  2.0 unx     9156 b- defN 23-Jul-25 11:44 model_navigator/commands/export/torch.py
+-rw-rw-rw-  2.0 unx     1058 b- defN 23-Jul-25 11:44 model_navigator/commands/export/exporters/__init__.py
+-rw-rw-rw-  2.0 unx     3945 b- defN 23-Jul-24 01:05 model_navigator/commands/export/exporters/jax2savedmodel.py
+-rw-rw-rw-  2.0 unx     3171 b- defN 23-Jul-24 01:05 model_navigator/commands/export/exporters/keras2savedmodel.py
+-rw-rw-rw-  2.0 unx     3122 b- defN 23-Jul-24 01:05 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
+-rw-rw-rw-  2.0 unx     3077 b- defN 23-Jul-25 11:44 model_navigator/commands/export/exporters/torch2onnx.py
+-rw-rw-rw-  2.0 unx     2728 b- defN 23-Jul-25 11:44 model_navigator/commands/export/exporters/torch2torchscript.py
+-rw-rw-rw-  2.0 unx      715 b- defN 23-Jul-24 01:05 model_navigator/commands/find_max_batch_size/__init__.py
+-rw-rw-rw-  2.0 unx     7156 b- defN 23-Jul-25 10:21 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
+-rw-rw-rw-  2.0 unx     3075 b- defN 23-Jul-24 01:05 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
+-rw-rw-rw-  2.0 unx      784 b- defN 23-Jul-24 01:05 model_navigator/commands/performance/__init__.py
+-rw-rw-rw-  2.0 unx     5260 b- defN 23-Jul-24 01:05 model_navigator/commands/performance/performance.py
+-rw-rw-rw-  2.0 unx     6964 b- defN 23-Jul-24 01:05 model_navigator/commands/performance/profile.py
+-rw-rw-rw-  2.0 unx     3104 b- defN 23-Jul-24 01:05 model_navigator/commands/performance/profile_script.py
+-rw-rw-rw-  2.0 unx     7269 b- defN 23-Jul-25 11:44 model_navigator/commands/performance/profiler.py
+-rw-rw-rw-  2.0 unx     5476 b- defN 23-Jul-25 11:44 model_navigator/commands/performance/results.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/commands/verification/__init__.py
+-rw-rw-rw-  2.0 unx     4657 b- defN 23-Jul-24 01:05 model_navigator/commands/verification/verify.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/configuration/__init__.py
+-rw-rw-rw-  2.0 unx     2002 b- defN 23-Jul-25 11:44 model_navigator/configuration/common_config.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/configuration/model/__init__.py
+-rw-rw-rw-  2.0 unx    15653 b- defN 23-Jul-25 11:44 model_navigator/configuration/model/model_config.py
+-rw-rw-rw-  2.0 unx    13677 b- defN 23-Jul-25 11:44 model_navigator/configuration/model/model_config_builder.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/core/__init__.py
+-rw-rw-rw-  2.0 unx     1389 b- defN 23-Jul-25 11:44 model_navigator/core/constants.py
+-rw-rw-rw-  2.0 unx     5299 b- defN 23-Jul-24 01:05 model_navigator/core/logger.py
+-rw-rw-rw-  2.0 unx     9941 b- defN 23-Jul-24 01:05 model_navigator/core/tensor.py
+-rw-rw-rw-  2.0 unx     2147 b- defN 23-Jul-24 01:05 model_navigator/core/workspace.py
+-rw-rw-rw-  2.0 unx     2817 b- defN 23-Jul-25 11:16 model_navigator/frameworks/__init__.py
+-rw-rw-rw-  2.0 unx      669 b- defN 23-Jul-24 01:05 model_navigator/frameworks/jax/__init__.py
+-rw-rw-rw-  2.0 unx     1554 b- defN 23-Jul-24 01:05 model_navigator/frameworks/jax/model.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/frameworks/onnx/__init__.py
+-rw-rw-rw-  2.0 unx     1085 b- defN 23-Jul-24 01:05 model_navigator/frameworks/onnx/utils.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/frameworks/tensorrt/__init__.py
+-rw-rw-rw-  2.0 unx    27191 b- defN 23-Jul-24 01:05 model_navigator/frameworks/tensorrt/cuda.py
+-rw-rw-rw-  2.0 unx    10627 b- defN 23-Jul-25 11:44 model_navigator/frameworks/tensorrt/utils.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/frameworks/torch/__init__.py
+-rw-rw-rw-  2.0 unx     1513 b- defN 23-Jul-24 01:05 model_navigator/frameworks/torch/utils.py
+-rw-rw-rw-  2.0 unx      622 b- defN 23-Jul-24 01:05 model_navigator/package/__init__.py
+-rw-rw-rw-  2.0 unx    12176 b- defN 23-Jul-24 01:05 model_navigator/package/builder.py
+-rw-rw-rw-  2.0 unx     4651 b- defN 23-Jul-25 01:05 model_navigator/package/loader.py
+-rw-rw-rw-  2.0 unx    11860 b- defN 23-Jul-24 01:05 model_navigator/package/package.py
+-rw-rw-rw-  2.0 unx     2819 b- defN 23-Jul-25 11:44 model_navigator/package/profiling_results.py
+-rw-rw-rw-  2.0 unx    21135 b- defN 23-Jul-25 11:44 model_navigator/package/status.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/pipelines/__init__.py
+-rw-rw-rw-  2.0 unx     5232 b- defN 23-Jul-24 01:05 model_navigator/pipelines/pipeline.py
+-rw-rw-rw-  2.0 unx    14762 b- defN 23-Jul-25 11:44 model_navigator/pipelines/pipeline_context.py
+-rw-rw-rw-  2.0 unx     3832 b- defN 23-Jul-24 01:05 model_navigator/pipelines/pipeline_manager.py
+-rw-rw-rw-  2.0 unx     9693 b- defN 23-Jul-25 11:44 model_navigator/pipelines/validation.py
+-rw-rw-rw-  2.0 unx     1883 b- defN 23-Jul-25 11:44 model_navigator/pipelines/builders/__init__.py
+-rw-rw-rw-  2.0 unx     2106 b- defN 23-Jul-24 01:05 model_navigator/pipelines/builders/correctness.py
+-rw-rw-rw-  2.0 unx     5682 b- defN 23-Jul-25 11:44 model_navigator/pipelines/builders/find_device_max_batch_size.py
+-rw-rw-rw-  2.0 unx     1660 b- defN 23-Jul-24 01:05 model_navigator/pipelines/builders/jax.py
+-rw-rw-rw-  2.0 unx     2509 b- defN 23-Jul-25 11:44 model_navigator/pipelines/builders/onnx.py
+-rw-rw-rw-  2.0 unx     2516 b- defN 23-Jul-24 01:05 model_navigator/pipelines/builders/performance.py
+-rw-rw-rw-  2.0 unx     2239 b- defN 23-Jul-24 01:05 model_navigator/pipelines/builders/preprocessing.py
+-rw-rw-rw-  2.0 unx     2504 b- defN 23-Jul-24 01:05 model_navigator/pipelines/builders/profiling.py
+-rw-rw-rw-  2.0 unx     2921 b- defN 23-Jul-25 11:44 model_navigator/pipelines/builders/tensorflow.py
+-rw-rw-rw-  2.0 unx     3326 b- defN 23-Jul-25 11:44 model_navigator/pipelines/builders/torch.py
+-rw-rw-rw-  2.0 unx     2112 b- defN 23-Jul-24 01:05 model_navigator/pipelines/builders/verify.py
+-rw-rw-rw-  2.0 unx      622 b- defN 23-Jul-24 01:05 model_navigator/pipelines/wrappers/__init__.py
+-rw-rw-rw-  2.0 unx     2747 b- defN 23-Jul-24 01:05 model_navigator/pipelines/wrappers/optimize.py
+-rw-rw-rw-  2.0 unx     4881 b- defN 23-Jul-25 11:44 model_navigator/pipelines/wrappers/profile.py
+-rw-rw-rw-  2.0 unx     1584 b- defN 23-Jul-24 01:05 model_navigator/runners/__init__.py
+-rw-rw-rw-  2.0 unx    13796 b- defN 23-Jul-25 11:44 model_navigator/runners/base.py
+-rw-rw-rw-  2.0 unx     2620 b- defN 23-Jul-24 01:05 model_navigator/runners/jax.py
+-rw-rw-rw-  2.0 unx     9999 b- defN 23-Jul-24 01:05 model_navigator/runners/onnx.py
+-rw-rw-rw-  2.0 unx     2267 b- defN 23-Jul-24 01:05 model_navigator/runners/python.py
+-rw-rw-rw-  2.0 unx     2290 b- defN 23-Jul-24 01:05 model_navigator/runners/registry.py
+-rw-rw-rw-  2.0 unx     7976 b- defN 23-Jul-24 01:05 model_navigator/runners/tensorflow.py
+-rw-rw-rw-  2.0 unx    26748 b- defN 23-Jul-24 01:05 model_navigator/runners/tensorrt.py
+-rw-rw-rw-  2.0 unx    10041 b- defN 23-Jul-24 01:05 model_navigator/runners/torch.py
+-rw-rw-rw-  2.0 unx     3559 b- defN 23-Jul-24 01:05 model_navigator/runners/utils.py
+-rw-rw-rw-  2.0 unx      937 b- defN 23-Jul-24 01:05 model_navigator/runtime_analyzer/__init__.py
+-rw-rw-rw-  2.0 unx    11714 b- defN 23-Jul-24 01:05 model_navigator/runtime_analyzer/analyzer.py
+-rw-rw-rw-  2.0 unx     2304 b- defN 23-Jul-24 01:05 model_navigator/runtime_analyzer/strategy.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/triton/__init__.py
+-rw-rw-rw-  2.0 unx     3180 b- defN 23-Jul-25 11:44 model_navigator/triton/model_config.py
+-rw-rw-rw-  2.0 unx     5218 b- defN 23-Jul-24 01:05 model_navigator/triton/model_config_builder.py
+-rw-rw-rw-  2.0 unx    23090 b- defN 23-Jul-25 11:44 model_navigator/triton/model_config_generator.py
+-rw-rw-rw-  2.0 unx    15243 b- defN 23-Jul-25 11:44 model_navigator/triton/model_repository.py
+-rw-rw-rw-  2.0 unx     2081 b- defN 23-Jul-25 11:44 model_navigator/triton/utils.py
+-rw-rw-rw-  2.0 unx      997 b- defN 23-Jul-24 01:05 model_navigator/triton/specialized_configs/__init__.py
+-rw-rw-rw-  2.0 unx     2872 b- defN 23-Jul-25 11:44 model_navigator/triton/specialized_configs/base_model_config.py
+-rw-rw-rw-  2.0 unx    22326 b- defN 23-Jul-25 11:44 model_navigator/triton/specialized_configs/common.py
+-rw-rw-rw-  2.0 unx     2229 b- defN 23-Jul-24 01:05 model_navigator/triton/specialized_configs/internal.py
+-rw-rw-rw-  2.0 unx     2685 b- defN 23-Jul-25 11:44 model_navigator/triton/specialized_configs/onnx_model_config.py
+-rw-rw-rw-  2.0 unx     1785 b- defN 23-Jul-24 01:05 model_navigator/triton/specialized_configs/python_model_config.py
+-rw-rw-rw-  2.0 unx     2239 b- defN 23-Jul-24 01:05 model_navigator/triton/specialized_configs/pytorch_model_config.py
+-rw-rw-rw-  2.0 unx     3162 b- defN 23-Jul-25 11:44 model_navigator/triton/specialized_configs/tensorflow_model_config.py
+-rw-rw-rw-  2.0 unx     3040 b- defN 23-Jul-24 01:05 model_navigator/triton/specialized_configs/tensorrt_model_config.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jul-24 01:05 model_navigator/utils/__init__.py
+-rw-rw-rw-  2.0 unx    14509 b- defN 23-Jul-24 01:05 model_navigator/utils/common.py
+-rw-rw-rw-  2.0 unx     8132 b- defN 23-Jul-24 01:05 model_navigator/utils/dataloader.py
+-rw-rw-rw-  2.0 unx     3902 b- defN 23-Jul-24 01:05 model_navigator/utils/devices.py
+-rw-rw-rw-  2.0 unx     1308 b- defN 23-Jul-24 01:05 model_navigator/utils/enums.py
+-rw-rw-rw-  2.0 unx     6163 b- defN 23-Jul-24 01:05 model_navigator/utils/environment.py
+-rw-rw-rw-  2.0 unx     4096 b- defN 23-Jul-24 01:05 model_navigator/utils/format_helpers.py
+-rw-rw-rw-  2.0 unx     2330 b- defN 23-Jul-24 01:05 model_navigator/utils/module.py
+-rw-rw-rw-  2.0 unx    10140 b- defN 23-Jul-25 11:49 triton_model_navigator-0.6.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10798 b- defN 23-Jul-25 11:49 triton_model_navigator-0.6.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 11:49 triton_model_navigator-0.6.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-25 11:49 triton_model_navigator-0.6.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    14493 b- defN 23-Jul-25 11:49 triton_model_navigator-0.6.3.dist-info/RECORD
+145 files, 769699 bytes uncompressed, 230832 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -414,23 +414,23 @@
 
 Filename: model_navigator/utils/format_helpers.py
 Comment: 
 
 Filename: model_navigator/utils/module.py
 Comment: 
 
-Filename: triton_model_navigator-0.6.2.dist-info/LICENSE
+Filename: triton_model_navigator-0.6.3.dist-info/LICENSE
 Comment: 
 
-Filename: triton_model_navigator-0.6.2.dist-info/METADATA
+Filename: triton_model_navigator-0.6.3.dist-info/METADATA
 Comment: 
 
-Filename: triton_model_navigator-0.6.2.dist-info/WHEEL
+Filename: triton_model_navigator-0.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: triton_model_navigator-0.6.2.dist-info/top_level.txt
+Filename: triton_model_navigator-0.6.3.dist-info/top_level.txt
 Comment: 
 
-Filename: triton_model_navigator-0.6.2.dist-info/RECORD
+Filename: triton_model_navigator-0.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## model_navigator/__version__.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # noqa: D100
-__version__ = "0.6.2"
+__version__ = "0.6.3"
```

## model_navigator/commands/export/exporters/__init__.py

```diff
@@ -18,9 +18,9 @@
     from . import torch2onnx  # noqa: F401
     from . import torch2torchscript  # noqa: F401
 
 if is_tf_available():
     from . import keras2savedmodel  # noqa: F401
     from . import savedmodel2savedmodel  # noqa: F401
 
-if is_tf_available and is_jax_available():
+if is_tf_available() and is_jax_available():
     from . import jax2savedmodel  # noqa: F401
```

## Comparing `triton_model_navigator-0.6.2.dist-info/LICENSE` & `triton_model_navigator-0.6.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `triton_model_navigator-0.6.2.dist-info/METADATA` & `triton_model_navigator-0.6.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-model-navigator
-Version: 0.6.2
+Version: 0.6.3
 Summary: Triton Model Navigator provides tools supporting to create Deep Learning production ready inference models
 License: Apache 2.0
 Project-URL: Documentation, https://triton-inference-server.github.io/model_navigator
 Project-URL: Source, https://github.com/triton-inference-server/model_navigator
 Project-URL: Tracker, https://github.com/triton-inference-server/model_navigator/issues
 Keywords: triton,inference,server,service,nvidia,tensorrt,onnx,tensorflow,pytorch,jax
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `triton_model_navigator-0.6.2.dist-info/RECORD` & `triton_model_navigator-0.6.3.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 model_navigator/__init__.py,sha256=YQ8MA8xQgnLgxeQ_oK_E7W8Tpxavwj0SKvbiq4r-JJE,881
-model_navigator/__version__.py,sha256=7vvkQh0eqmNgtq6_vPlJXbvzyGqtMkGz68y6ijnvTtw,649
+model_navigator/__version__.py,sha256=IIjyLFpMSG42fEdenfyjzQkLk5S5yaZdgY9rRKpj-e4,649
 model_navigator/exceptions.py,sha256=AnYKlbe6WHk4_3lEhksgONKjtcNK7_g0-qs8mIHARuA,3915
 model_navigator/api/__init__.py,sha256=Jt9Du5gr7UP0ljMEur81SAqLg99DokO0vyw1qaonOqY,1716
 model_navigator/api/config.py,sha256=buMLeLqvirV4efpIAxgDBFo0gSoHGNttOns4dHkU_V4,24220
 model_navigator/api/jax.py,sha256=QwOjMl89TPZpj4lOOMLrGOnNrWMoVMCFhgTgk1mmCLA,6263
 model_navigator/api/onnx.py,sha256=CwX50QTt6seCbCDAOvgPLbOQjw29sL-bVWvMViFlU18,5268
 model_navigator/api/package.py,sha256=BqPo9VD_alP4aMbvvQCdqGEZZ3YrQ1PNMcDH-B-uBC8,16279
 model_navigator/api/python.py,sha256=n3Pdc_2TK9Q1yYui4R2rLh8ImC3ezhHnh-n0K1Hcom0,4795
@@ -36,15 +36,15 @@
 model_navigator/commands/correctness/correctness_script.py,sha256=Ejdk8rM7_wPxP5gwIkryOVghKMzCUrqF9L2J8V9kKF0,4733
 model_navigator/commands/data_dump/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/data_dump/samples.py,sha256=SH_4Aejt16bN6JoQPd-sVa4wwFJKtkGjudK9PhBG3RA,10740
 model_navigator/commands/export/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/export/jax.py,sha256=O-4Ua4GnulFDC8DJhtjh40rYgEy0OHqKgkRgPpn_0RE,3611
 model_navigator/commands/export/tf.py,sha256=SX7-VJJSUJ86BCSZsz7ZLsi2B4OHnrk5du7-7zLb8FY,5598
 model_navigator/commands/export/torch.py,sha256=uCYN6IaJrO8nmOiCcapQ09V6JXDqU9hobR72_UTdeF8,9156
-model_navigator/commands/export/exporters/__init__.py,sha256=ZkOuCGTEqfxCY1PilU3DJV4IMMuMpTEEm2KsCmmcoMQ,1056
+model_navigator/commands/export/exporters/__init__.py,sha256=LuxcLIWjhUsVOjVvWhE5m3mdrlBIuDK-vjuYpZ-gNbI,1058
 model_navigator/commands/export/exporters/jax2savedmodel.py,sha256=LSr8I4mRHpwYZNDCs3IfUAyk3n89951bjA1JM_rnQks,3945
 model_navigator/commands/export/exporters/keras2savedmodel.py,sha256=oG4BqcklEmTtpwd3tlyKhNBub41VrQBqiiTfRKZaU6Q,3171
 model_navigator/commands/export/exporters/savedmodel2savedmodel.py,sha256=sdE76nSyXD8i_OfePhOEFBiMQFSOsVRiFf8bu26SoaE,3122
 model_navigator/commands/export/exporters/torch2onnx.py,sha256=sTj6uVxFfr-avTjSWC9RXayQhyPkyvjY1YWJhXFrQxc,3077
 model_navigator/commands/export/exporters/torch2torchscript.py,sha256=UdBcw1TVoaj85Tg6ww-MhkGkHB15ZfbJf6x9szJ3PXE,2728
 model_navigator/commands/find_max_batch_size/__init__.py,sha256=-j67tQs-RhZGWwXSqmRZ7OqR7NOdNRjg4RhBgvOhBhg,715
 model_navigator/commands/find_max_batch_size/find_max_batch_size.py,sha256=UWXtr4rSQvqx7c_K-f-3Zd_ENE4-dXXZQnhlPj2p3mo,7156
@@ -134,12 +134,12 @@
 model_navigator/utils/common.py,sha256=zDD3FCSPJsig7GK2EcqzKX-q2umzO34xg4a8tL7iuxw,14509
 model_navigator/utils/dataloader.py,sha256=r549fsb5tq7ZQpnKFw4Zk9Mgc8WKzwP4wZHlpWXNj1g,8132
 model_navigator/utils/devices.py,sha256=pGjRBByJqFjG6dyJ0H2E6GJA7hIgF6rgeINLNdS27kU,3902
 model_navigator/utils/enums.py,sha256=T-G5VV5CqimxpctOqPaCvVoAwx-pp10Eeo0rKlWoVGU,1308
 model_navigator/utils/environment.py,sha256=MnpdF5eCx2DJpHtaq8fUSky0hdT03qTJrGnJDhCnFhM,6163
 model_navigator/utils/format_helpers.py,sha256=3UGJhNTFZiMorbMQrciDzJgfFW2nvLMroNmeqC8FlGs,4096
 model_navigator/utils/module.py,sha256=BX9Da3b-tOHvOFb4Ffts0Qc1i9hbgwreGbScqq_DINY,2330
-triton_model_navigator-0.6.2.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
-triton_model_navigator-0.6.2.dist-info/METADATA,sha256=axM9Gs2j56BXrAXmn2YdshVD0bkM_rq5Q3EFskp4xLU,10798
-triton_model_navigator-0.6.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-triton_model_navigator-0.6.2.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
-triton_model_navigator-0.6.2.dist-info/RECORD,,
+triton_model_navigator-0.6.3.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
+triton_model_navigator-0.6.3.dist-info/METADATA,sha256=5GJ4FwcdsPQVVtI9tX3MYSgEqgr_f0bNfWD9cDFdB0E,10798
+triton_model_navigator-0.6.3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+triton_model_navigator-0.6.3.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
+triton_model_navigator-0.6.3.dist-info/RECORD,,
```

