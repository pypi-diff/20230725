# Comparing `tmp/jaxonnxruntime-0.1.0.tar.gz` & `tmp/jaxonnxruntime-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxonnxruntime-0.1.0.tar", last modified: Tue Jun 20 22:59:15 2023, max compression
+gzip compressed data, was "jaxonnxruntime-0.2.0.tar", last modified: Tue Jul 25 15:39:09 2023, max compression
```

## Comparing `jaxonnxruntime-0.1.0.tar` & `jaxonnxruntime-0.2.0.tar`

### file list

```diff
@@ -1,116 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.935574 jaxonnxruntime-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.939574 jaxonnxruntime-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.939574 jaxonnxruntime-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.935574 jaxonnxruntime-0.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.939574 jaxonnxruntime-0.1.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/docs/_static/css/jaxonnxruntime_theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.939574 jaxonnxruntime-0.1.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/docs/examples/jaxonnxruntime-python-api.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.935574 jaxonnxruntime-0.1.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.939574 jaxonnxruntime-0.1.0/examples/imagenet/
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/examples/imagenet/imagenet_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.943574 jaxonnxruntime-0.1.0/jaxonnxruntime/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/call_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.943574 jaxonnxruntime-0.1.0/jaxonnxruntime/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/core/onnx_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/core/onnx_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/core/onnx_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/abs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/averagepool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/batchnormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/ceil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/constantofshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/div.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/equal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/gemm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/globalaveragepool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/if_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/less.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/lessorequal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/lrn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/maxpool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/mul.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/neg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/nonzero.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/onehot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/or_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/pow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reciprocal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reducemax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reducemean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reducesum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sqrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/squeeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/tanh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/unsqueeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/where.py
--rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.943574 jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-20 22:59:15.000000 jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-20 22:59:15.000000 jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:59:15.000000 jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 22:59:15.000000 jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 22:59:15.000000 jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/call_onnx_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/core/handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/core/onnx_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/core/onnx_node_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/tests/onnx_ops/
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/onnx_ops/dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/onnx_ops/onehot_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/onnx_ops_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/run_all_tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tools/analyze_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tools/op_code_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.930083 jaxonnxruntime-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.910083 jaxonnxruntime-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.914083 jaxonnxruntime-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.914083 jaxonnxruntime-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-25 15:39:09.930083 jaxonnxruntime-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.914083 jaxonnxruntime-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.914083 jaxonnxruntime-0.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.914083 jaxonnxruntime-0.2.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/docs/_static/css/jaxonnxruntime_theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/docs/adding_a_new_op.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.914083 jaxonnxruntime-0.2.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/docs/examples/jaxonnxruntime-python-api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.914083 jaxonnxruntime-0.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.914083 jaxonnxruntime-0.2.0/examples/imagenet/
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/examples/imagenet/imagenet_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.914083 jaxonnxruntime-0.2.0/jaxonnxruntime/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/call_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/config_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.918083 jaxonnxruntime-0.2.0/jaxonnxruntime/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/core/onnx_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/core/onnx_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/core/onnx_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.914083 jaxonnxruntime-0.2.0/jaxonnxruntime/experimental/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.918083 jaxonnxruntime-0.2.0/jaxonnxruntime/experimental/custom_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/experimental/custom_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/experimental/custom_ops/zeros_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/experimental/custom_ops/zeros_like_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.926083 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/abs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/acos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/acosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/and_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/argmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/argmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/asin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/asinh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/atan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/atanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/averagepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/batchnormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/bitshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/castlike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/constantofshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/cos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/cosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/div.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/einsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/erf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/gatherelements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/gemm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/globalaveragepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/if_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/less.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/lessorequal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/logsoftmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/lrn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/maxpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/mul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/nonzero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/onehot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/or_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/pow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/reciprocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/reducemax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/reducemean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/reducesum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/selu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/sin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/sinh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/softplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/trilu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/unsqueeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/jaxonnxruntime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.918083 jaxonnxruntime-0.2.0/jaxonnxruntime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-25 15:39:09.000000 jaxonnxruntime-0.2.0/jaxonnxruntime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-25 15:39:09.000000 jaxonnxruntime-0.2.0/jaxonnxruntime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:39:09.000000 jaxonnxruntime-0.2.0/jaxonnxruntime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-25 15:39:09.000000 jaxonnxruntime-0.2.0/jaxonnxruntime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 15:39:09.000000 jaxonnxruntime-0.2.0/jaxonnxruntime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:39:09.930083 jaxonnxruntime-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.926083 jaxonnxruntime-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/tests/call_onnx_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.930083 jaxonnxruntime-0.2.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/tests/core/handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/tests/core/onnx_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/tests/core/onnx_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/tests/core/onnx_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.930083 jaxonnxruntime-0.2.0/tests/onnx_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/tests/onnx_ops/dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/tests/onnx_ops/onehot_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/tests/onnx_ops_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2979 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/tests/run_all_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:39:09.930083 jaxonnxruntime-0.2.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/tools/analyze_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-25 15:38:48.000000 jaxonnxruntime-0.2.0/tools/op_code_generator.py
```

### Comparing `jaxonnxruntime-0.1.0/.github/workflows/build.yml` & `jaxonnxruntime-0.2.0/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     name: Run Tests
     needs: [cancel-previous, pre-commit, commit-count, test-import]
     runs-on: ubuntu-20.04-16core
     strategy:
       matrix:
         python-version: ['3.10']
         test-type: [doctest, pytest]
+        onnx-version: ['1.12.0', '1.14.0']
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       id: setup_python
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
@@ -107,14 +108,17 @@
         python3 -m venv venv
         venv/bin/python3 -m pip install .[all]
         venv/bin/python3 -m pip install .[testing]
         venv/bin/python3 -m pip install -r docs/requirements.txt
     - name: Install Jaxonnxruntime
       run: |
         venv/bin/python3 -m pip install -e .[all]
+    - name: Test with onnx==${{ matrix.onnx-version }}
+      run: |
+        venv/bin/python3 -m pip install onnx==${{ matrix.onnx-version }}
     - name: Cached mypy cache
       id: mypy_cache
       uses: actions/cache@v3
       if: matrix.test-type == 'mypy'
       with:
         path: .mypy_cache
         key: mypy-${{ steps.setup_python.outputs.python-version }}-${{ steps.date_key.outputs.DATE }}
```

### Comparing `jaxonnxruntime-0.1.0/.github/workflows/pythonpublish.yml` & `jaxonnxruntime-0.2.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/.pre-commit-config.yaml` & `jaxonnxruntime-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/LICENSE` & `jaxonnxruntime-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/PKG-INFO` & `jaxonnxruntime-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxonnxruntime
-Version: 0.1.0
+Version: 0.2.0
 Summary: Jaxonnxruntime: JAX based ONNX Runtime.
 Author-email: Jaxonnxruntime team <jaxonnxruntime-dev@google.com>
 Project-URL: homepage, https://github.com/google/jaxonnxruntime
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -31,12 +31,20 @@
 
 - We follow most of the interface definitions by `onnx.backend` [here](https://onnx.ai/onnx/api/backend.html).
 
 - Please check a brief example on model conversion and forward calling in [`examples/imagenet/imagenet_main.py`](https://github.com/google/jaxonnxruntime/blob/main/examples/imagenet/imagenet_main.py).
 
 ## Contributions and Discussions
 
+We believe that collaboration is the key to building remarkable software, and we wholeheartedly welcome contributions from developers like you.
+You can make a real impact and help shape the future of our project with contributions such as
+[implementing new operators](https://github.com/google/jaxonnxruntime/blob/main/docs/adding_a_new_op.rst) and increasing support for more ML models.
+
+Our contributors will have a chance to earn [Google Open Source Peer Bonus](https://opensource.google/documentation/reference/growing/peer-bonus), so that your valuable contributions won't go unnoticed.
+Your hard work will be rewarded both by the community and by Google.
+Together, let's create an amazing library and foster a supportive environment for open-source enthusiasts.
+
 Thank you for taking the time to contribute! Please see [the contribution guidelines](https://github.com/google/jaxonnxruntime/blob/main/contributing.md).
 
 ## License
 
 This project is licensed under the [Apache License](https://github.com/google/jaxonnxruntime/blob/main/LICENSE).
```

### Comparing `jaxonnxruntime-0.1.0/contributing.md` & `jaxonnxruntime-0.2.0/contributing.md`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/docs/conf.py` & `jaxonnxruntime-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/docs/examples/jaxonnxruntime-python-api.py` & `jaxonnxruntime-0.2.0/docs/examples/jaxonnxruntime-python-api.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/docs/index.rst` & `jaxonnxruntime-0.2.0/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 ******************************
 Jaxonnxruntime
 ******************************
 
 
 .. div:: sd-text-left sd-font-italic
 
-   JAX based ONNX backend
-
-
-----
+JAX based ONNX backend
+------------------------------
 
 `Jaxonnxruntime` is focused on creating a JAX-based backend for the ONNX format. The benefits of using ONNX include interoperability and ease of hardware access, while JAX provides a similar API to Numpy and allows for performance speed-ups through jit compilation.
 
 `Jaxonnxruntime` implements the backend by re-writing the ONNX operator implementations in the "JAX programming way" and interpreting all data structures as PyTree. The user will be able to run the jit function on the run_model function for performance speed-up and apply other Jax transformations.
+
+.. toctree::
+   :maxdepth: 2
+   :caption: Getting Started
+
+   adding_a_new_op
```

### Comparing `jaxonnxruntime-0.1.0/examples/imagenet/imagenet_main.py` & `jaxonnxruntime-0.2.0/examples/imagenet/imagenet_main.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/__init__.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """JAX based onnxruntime."""
 # pylint: disable=useless-import-alias
 # PEP 484: import <name> as <name> is required for names to be exported.
-from .config import config as config
+from .config_class import config as config
 from .version import __version__ as __version__
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/backend.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,10 +154,11 @@
       device: The name of the device to check support for.
 
     Returns:
       True if the backend supports the specified device, False otherwise.
     """
     return True
 
-
+prepare = Backend.prepare
 run_model = Backend.run_model
 run = Backend.run_model
+supports_device = Backend.supports_device
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/call_onnx.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/call_onnx.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,37 +24,58 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Convert ONNX model into jax function."""
 
 import logging
-from typing import Any, Callable, Dict, Sequence, Type, Tuple, Union
+from typing import Any, Callable, Dict, Sequence, Tuple, Type, Union
 
+import jax
+from jaxonnxruntime import config
 from jaxonnxruntime import onnx_ops  # pylint: disable=unused-import
 from jaxonnxruntime.core import handler as onnx_handler
 from jaxonnxruntime.core import onnx_graph
 from jaxonnxruntime.core import onnx_node
 from jaxonnxruntime.core import onnx_utils
+
 import onnx
 from onnx import defs
 from onnx.helper import make_opsetid
 
+
 OnnxNode = onnx_node.OnnxNode
 OnnxGraph = onnx_graph.OnnxGraph
 Handler = onnx_handler.Handler
 
 logger = logging.getLogger(__name__)
 
 
 def call_onnx_model(
-    model: onnx.ModelProto, inputs: Union[Sequence[Any], Dict[str, Any]]
+    model: onnx.ModelProto,
+    inputs: Union[Sequence[Any], Dict[str, Any]],
+    rename_tensors: bool = False,
 ) -> Tuple[Callable[..., Any], Any]:
-  """Convert ONNX.ModelProto to jax_func with model parameters."""
+  """Convert an ONNX.ModelProto to a JAX function with model parameters and sample input.
+
+  Args:
+    model: The ONNX model to convert.
+    inputs: The sample input(s) for the model. It can be either a sequence of
+      inputs or a dictionary mapping input names to values.
+    rename_tensors: Indicates whether to rename all onnx.TensorProto name with
+      unique id `tensor_{id}`. Default is False.
+
+  Returns:
+    model_func, model_params: A tuple containing the JAX function  and the
+    model_params as PyTree.
+  """
+
   graph = model.graph
+  if rename_tensors:
+    graph = onnx_utils.sanitize_tensor_names_in_graph(graph)
   if model.ir_version < 3:
     opset = [make_opsetid(defs.ONNX_DOMAIN, 1)]
   else:
     opset = model.opset_import
   model_params = {
       n.name: onnx_utils.valueinfoproto_asarray(n) for n in graph.initializer
   }
@@ -75,19 +96,16 @@
   """Convert ONNX.GraphProto to jax_func with ONNX.GraphProto.initializer as parameters."""
   tensor_ref_dict = build_ref_dict(graph)
   graph_helper = OnnxGraph(graph)
 
   # step 1: Trace those static info
   jit_func_dict = {}
   onnx_node_dict = {}
-  opset = (
-    [make_opsetid(defs.ONNX_DOMAIN, defs.onnx_opset_version())]
-    if opset is None
-    else opset
-  )
+  if opset is None:
+    opset = [make_opsetid(defs.ONNX_DOMAIN, defs.onnx_opset_version())]
   handlers = _get_all_handlers(opset)
   node_execute_order_list = graph_helper.topological_sort()
 
   logger.info('Start tracing the jax_func model to get some static info')
   for node_proto in node_execute_order_list:
     node = OnnxNode(node_proto, graph_helper)
     onnx_node_dict[node.name] = node
@@ -97,15 +115,19 @@
       raise ValueError(
           'Fail to get the input tensor of node input names'
           f'{node.inputs + node.subgraph_inputs}, the node proto is'
           f'{node.node_proto}.'
       ) from e
     jit_func = _get_jit_func(node, node_inputs, handlers=handlers)
     jit_func_dict[node.name] = jit_func
-    outputs = jit_func(*node_inputs, **node.attrs_dict)
+
+    if config.jaxort_experimental_support_abtract_input_shape:
+      outputs = jax.eval_shape(jit_func, *node_inputs, **node.attrs_dict)
+    else:
+      outputs = jit_func(*node_inputs, **node.attrs_dict)
     outputs = outputs if isinstance(outputs, Sequence) else [outputs]
 
     for name, output in zip(node.outputs, outputs):
       tensor_dict[name] = output
 
   input_names = onnx_utils.get_graph_input(graph)
 
@@ -199,23 +221,32 @@
               'Please use handler.register_op decorator to register it.'
           ),
           handler.__name__,
       )
 
     domain = handler.DOMAIN
     opset_dict = dict([(o.domain, o.version) for o in opset])
+    if handler.DOMAIN not in opset_dict:
+      raise ValueError(
+          f'handler.DOMAIN {handler.DOMAIN} is not in opset_dict {opset_dict}'
+      )
     version = opset_dict[handler.DOMAIN]
     since_version = handler.get_since_version(version)
     handler.SINCE_VERSION = since_version
     handlers.setdefault(domain, {})[handler.OP_TYPE] = handler
 
   return handlers
 
 
-def _get_jit_func(node, inputs, handlers, **kwargs):
+def _get_jit_func(
+    node: OnnxNode,
+    inputs: list[Any],
+    handlers: Dict[str, Dict[str, type[Handler]]],
+    **kwargs,
+):
   """Get the JAX node implementation."""
   handler = (
       handlers[node.domain].get(node.op_type, None)
       if node.domain in handlers
       else None
   )
   if handler:
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/config.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/config_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -459,7 +459,18 @@
     help=(
         'The onnx If operator can have dynamic output shape, which cannot '
         'be supported by jax.jit. We have to manually manipulate the output '
         'shape if there is a mismatch between the outputs of else_branch and '
         'then_branch, as is the case for LLaMA.'
     ),
 )
+
+jaxort_experimental_support_abtract_input_shape = config.define_bool_state(
+    name='jaxort_experimental_support_abtract_input_shape',
+    default=False,
+    help=(
+        'Default behaviour is that call_onnx require real model input to'
+        ' tracethe JAX function. If `jaxort_support_abtract_input_shape`, users'
+        ' onlyneed provide input abstract shape and dtype info. Here we use'
+        ' `jax.eval_shape`function to deduce the output shape and dtype'
+    ),
+)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/core/__init__.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/core/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/core/handler.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/relu.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,79 +21,61 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Defines a Handler class and a decorator to register ONNX ops."""
-import logging
-
-from typing import Any, Sequence
-from onnx import defs
-
-logger = logging.getLogger(__name__)
-
-OnnxNode = Any
-JaxFunc = Any
-
-
-class Handler:
-  """Base class for ONNX op."""
-
-  DOMAIN: str = ""  # Domain of the op
-  OP_TYPE: str = ""  # Type of the op
-  SINCE_VERSION: int = 0  # Version since which the op is available
+"""Define ONNX Relu operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
+from collections.abc import Callable, Sequence
+import functools
+import inspect
+from typing import Any
+
+import jax
+from jax import jit
+from jaxonnxruntime.core import handler
+from jaxonnxruntime.core import onnx_node
+
+
+@handler.register_op("Relu")
+class Relu(handler.Handler):
+  """Implementation of the ONNX Relu operator."""
 
   @classmethod
-  def get_since_version(cls, version: int) -> int:
-    """Get the SINCE_VERSION based on the VERSION of the ONNX opset being used."""
-    domain = cls.DOMAIN
-    op_type = cls.OP_TYPE
-    since_version = 1
-    try:
-      since_version = defs.get_schema(
-          op_type,
-          domain=domain,
-          max_inclusive_version=version,
-      ).since_version
-    except Exception:  # pylint: disable=broad-except
-      logger.warning(
-          (
-              "Fail to get since_version of %s in domain %s "
-              "with max_inclusive_version= %d. Set to 1."
-          ),
-          op_type,
-          domain,
-          version,
-      )
-    return since_version
+  def _prepare(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
+  ):
+    sig = inspect.signature(onnx_jax_impl)
+    kwparams = [
+        param.name
+        for param in sig.parameters.values()
+        if param.kind == inspect.Parameter.KEYWORD_ONLY
+    ]
+    for name in kwparams:
+      node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def handle(cls, node: OnnxNode, inputs: Sequence[Any], **kwargs) -> Any:
-    ver_handle = getattr(cls, "version_{}".format(cls.SINCE_VERSION), None)
-    if ver_handle:
-      return ver_handle(node, inputs, **kwargs)  # pylint: disable=not-callable
-
-    raise NotImplementedError(
-        "{} version {} is not implemented.".format(
-            node.op_type, cls.SINCE_VERSION
-        )
-    )
+  def version_6(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_6 Relu op."""
+    cls._prepare(node, inputs, onnx_relu)
+    return onnx_relu
 
   @classmethod
-  def _prepare(
-      cls, node: OnnxNode, inputs: Sequence[Any], onnx_jax_impl: JaxFunc
-  ) -> None:
-    """The abstract method to rewwrite the node.attrs_dict."""
-    raise NotImplementedError
-
-
-def register_op(op_type: str, domain: str = "") -> Any:
-  """Register op into specific domain. default value "" is ai.onnx domain."""
+  def version_14(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_14 Relu op."""
+    cls._prepare(node, inputs, onnx_relu)
+    return onnx_relu
 
-  def deco(cls):
-    setattr(cls, "DOMAIN", domain)
-    setattr(cls, "OP_TYPE", op_type)
-    return cls
 
-  return deco
+@functools.partial(jit, static_argnames=())
+def onnx_relu(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Relu for more details."""
+  assert len(input_args) == 1
+  x = input_args[0]
+  return jax.nn.relu(x)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/core/onnx_graph.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/core/onnx_graph.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,17 +22,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Wrap the onnx.GraphProto as OnnxGraph class and provide useful graph manipulation methods."""
+
 import collections
 from typing import Any, List, Sequence
 
+import jax
+from jaxonnxruntime.core import onnx_utils
+
 import onnx
 
 
 class OnnxGraph:
   """Graph class wrapper of ONNX.GraphProto.
 
   Attributes:
@@ -47,26 +51,29 @@
     name: The name of the ONNX graph.
     value_info_dict: A dictionary containing all the value_info in the graph,
       indexed by their names.
     metadata: A dictionary containing the metadata of the graph.
   """
 
   def __init__(self, graph_proto: onnx.GraphProto):
-    self.graph_proto = graph_proto
-    self.node_dict = {}
+    self.graph_proto: onnx.GraphProto = graph_proto
+    self.node_dict: dict[str, onnx.NodeProto] = {}
     for index, nd in enumerate(graph_proto.node):
       node_name = f"node_{index}"
       nd.name = node_name
       self.node_dict[node_name] = nd
-    self.initializer_dict = {ts.name: ts for ts in graph_proto.initializer}
-    self.input = [proto.name for proto in graph_proto.input]
-    self.output = [proto.name for proto in graph_proto.output]
-    self.doc_string = graph_proto.doc_string
-    self.name = graph_proto.name
-    self.value_info_dict = {
+    self.initializer_dict: dict[str, jax.Array] = {
+        ts.name: onnx_utils.valueinfoproto_asarray(ts)
+        for ts in graph_proto.initializer
+    }
+    self.input: list[str] = [proto.name for proto in graph_proto.input]
+    self.output: list[str] = [proto.name for proto in graph_proto.output]
+    self.doc_string: str = graph_proto.doc_string
+    self.name: str = graph_proto.name
+    self.value_info_dict: dict[str, onnx.ValueInfoProto] = {
         **{proto.name: proto for proto in graph_proto.input},
         **{proto.name: proto for proto in graph_proto.output},
         **{proto.name: proto for proto in graph_proto.value_info},
     }
     self.metadata: dict[str, Any] = {}
     self._initialize_metadata()
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/core/onnx_node.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/core/onnx_node.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/core/onnx_utils.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/core/handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,83 +21,91 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""onnx utility functions collection."""
-from typing import Any, Dict, Optional, Sequence, Union
-from jax import numpy as jnp
-import onnx
-from onnx import numpy_helper
-
-
-def tensor_dtype_to_jnp_dtype(
-    tensor_type: onnx.TensorProto.DataType,
-) -> jnp.dtype:
-  """Convert onnx.TensorProto.DataType to jnp.dtype."""
-  if tensor_type is onnx.TensorProto.BFLOAT16:
-    return jnp.bfloat16
-  if onnx.__version__ < '1.14.0':
-    np_type = onnx.mapping.TENSOR_TYPE_TO_NP_TYPE[tensor_type]
-  else:
-    np_type = onnx.helper.tensor_dtype_to_np_dtype(tensor_type)
-  return jnp.dtype(np_type)
-
-
-def get_shape_and_dtype_from_val_info(
-    value_info: onnx.ValueInfoProto,
-) -> tuple[list[int], jnp.dtype]:
-  """Get jax numpy shape and dtype from onnx.ValueInfoProto."""
-  type_proto = value_info.type
-  dtype = tensor_dtype_to_jnp_dtype(type_proto.tensor_type.elem_type)
-  shape = [dim.dim_value for dim in type_proto.tensor_type.shape.dim]
-
-  return shape, dtype
-
-
-def contain_subgraph(node: Any) -> bool:
-  """Check if the node contains subgraph (control flow)."""
-  return node.op_type in ("If", "Loop")
-
-
-def get_graph_input(graph: onnx.GraphProto) -> list[str]:
-  """Returns unique non-node input names."""
-  real_input: list[str] = []
-  output_list: list[str] = []
-  initializers: list[str] = [ts.name for ts in graph.initializer]
-  for node in graph.node:
-    output_list.extend(list(node.output))
-  for node in graph.node:
-    real_input.extend(
-        i for i in node.input if i not in initializers and i not in output_list
+"""Defines a Handler class and a decorator to register ONNX ops."""
+
+from collections.abc import Sequence
+import inspect
+import logging
+from typing import Any
+
+from onnx import defs
+
+
+logger = logging.getLogger(__name__)
+
+OnnxNode = Any
+JaxFunc = Any
+
+
+class Handler:
+  """Base class for ONNX op."""
+
+  DOMAIN: str = ""  # Domain of the op
+  OP_TYPE: str = ""  # Type of the op
+  SINCE_VERSION: int = 0  # Version since which the op is available
+
+  @classmethod
+  def get_since_version(cls, version: int) -> int:
+    """Get the SINCE_VERSION based on the VERSION of the ONNX opset being used."""
+    domain = cls.DOMAIN
+    op_type = cls.OP_TYPE
+    since_version = 1
+    try:
+      since_version = defs.get_schema(
+          op_type,
+          domain=domain,
+          max_inclusive_version=version,
+      ).since_version
+    except Exception:  # pylint: disable=broad-except
+      logger.warning(
+          (
+              "Fail to get since_version of %s in domain %s "
+              "with max_inclusive_version= %d. Set to 1."
+          ),
+          op_type,
+          domain,
+          version,
+      )
+    return since_version
+
+  @classmethod
+  def handle(cls, node: OnnxNode, inputs: Sequence[Any], **kwargs) -> Any:
+    """Return the jax class version member depending on OnnxNode verison."""
+    ver_handle = getattr(cls, "version_{}".format(cls.SINCE_VERSION), None)
+    if ver_handle:
+      return ver_handle(node, inputs, **kwargs)  # pylint: disable=not-callable
+
+    # Get all the methods that start with "version_"
+    class_methods = inspect.getmembers(cls, predicate=inspect.ismethod)
+    version_methods = [
+        method_name
+        for method_name, _ in class_methods
+        if method_name.startswith("version_")
+    ]
+
+    raise NotImplementedError(
+        f"{node.op_type} version {cls.SINCE_VERSION} is not implemented."
+        f" Only have those versions: {version_methods}."
     )
 
-  # Sometimes input name is empty string(""), which should be removed.
-  # We also need to remove duplicates.
-  unique_real_input = []
-  for item in real_input:
-    if item not in unique_real_input and item != "":  # pylint: disable=g-explicit-bool-comparison
-      unique_real_input.append(item)
-  return unique_real_input
-
-
-def valueinfoproto_asarray(proto: Any):
-  """Convert onnx.ValueInfoProto to jaxlib.xla_extension.ArrayImpl."""
-  return jnp.asarray(numpy_helper.to_array(proto).reshape(tuple(proto.dims)))
-
-
-def maybe_convert_to_dict(
-    inputs: Union[Sequence[Any], Dict[str, Any]],
-    input_names: Optional[Sequence[Any]] = None,
-):
-  """Convert inputs to a dictionary with input_names as keys."""
-  if isinstance(inputs, dict):
-    return inputs
-  elif isinstance(inputs, Sequence):
-    if input_names is None:
-      raise ValueError("Should provide input names if `inputs` is a Sequence!")
-    assert len(inputs) == len(input_names)
-    return dict(zip(input_names, inputs))
-  else:
-    raise NotImplementedError("Please use inputs of type dict or Sequence!")
+  @classmethod
+  def _prepare(
+      cls, node: OnnxNode, inputs: Sequence[Any], onnx_jax_impl: JaxFunc
+  ) -> None:
+    """The abstract method to rewwrite the node.attrs_dict."""
+    raise NotImplementedError
+
+
+def register_op(op_type: str, domain: str = "") -> Any:
+  """Register op into specific domain. default value "" is ai.onnx domain."""
+
+  def deco(cls):
+    setattr(cls, "DOMAIN", domain)
+    setattr(cls, "OP_TYPE", op_type)
+    return cls
+
+  return deco
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/abs.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/abs.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,22 @@
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_1 Abs op."""
     cls._prepare(node, inputs, onnx_abs)
     return onnx_abs
 
   @classmethod
+  def version_6(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_6 Abs op."""
+    cls._prepare(node, inputs, onnx_abs)
+    return onnx_abs
+
+  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_13 Abs op."""
     cls._prepare(node, inputs, onnx_abs)
     return onnx_abs
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/add.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/exp.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Add operator."""
+"""Define ONNX Exp operator."""
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Add")
-class Add(handler.Handler):
-  """Implementation of the ONNX Add operator."""
+@handler.register_op("Exp")
+class Exp(handler.Handler):
+  """Implementation of the ONNX Exp operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,29 +51,29 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_7(
+  def version_6(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_7 Add op."""
-    cls._prepare(node, inputs, onnx_add)
-    return onnx_add
+    """ONNX version_6 Exp op."""
+    cls._prepare(node, inputs, onnx_exp)
+    return onnx_exp
 
   @classmethod
-  def version_14(
+  def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_14 Add op."""
-    cls._prepare(node, inputs, onnx_add)
-    return onnx_add
+    """ONNX version_13 Exp op."""
+    cls._prepare(node, inputs, onnx_exp)
+    return onnx_exp
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_add(*input_args):
-  """The internal jax impl for onnx Add op."""
-  assert len(input_args) == 2
-  a, b = input_args
-  return jnp.add(a, b)
+def onnx_exp(*input_args):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Exp."""
+  assert len(input_args) == 1
+  x = input_args[0]
+  return jnp.exp(x)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/averagepool.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/averagepool.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/batchnormalization.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/batchnormalization.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/cast.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/cast.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,24 +22,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Define ONNX Cast operator."""
+
 from collections.abc import Callable, Sequence
 import functools
-from typing import Any
-from jax import jit
+from typing import Any, Optional
+
+import jax
+from jax import numpy as jnp
 from jaxonnxruntime import config
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 from jaxonnxruntime.core import onnx_utils
+
 import onnx
 
+
 register_op = handler.register_op
 Handler = handler.Handler
 OnnxNode = onnx_node.OnnxNode
 
 
 @handler.register_op("Cast")
 class Cast(handler.Handler):
@@ -51,24 +56,25 @@
   ):
     node.attrs_dict["to"] = node.attrs.get("to", int)
     if node.context_graph.value_info_dict.get(node.inputs[0]) is not None:
       tensor_proto = node.context_graph.value_info_dict.get(node.inputs[0])
       from_type = onnx_utils.tensor_dtype_to_jnp_dtype(
           tensor_proto.type.tensor_type.elem_type
       )
-    elif node.context_graph.initializer_dict.get(node.inputs[0]) is not None:
-      tensor_proto = node.context_graph.initializer_dict.get(node.inputs[0])
-      from_type = onnx_utils.tensor_dtype_to_jnp_dtype(tensor_proto.data_type)
-    else:
-      if config.jaxort_only_allow_initializers_as_static_args:
+    elif config.jaxort_only_allow_initializers_as_static_args:
+      if node.context_graph.initializer_dict.get(node.inputs[0]) is not None:
+        tensor_proto = node.context_graph.initializer_dict.get(node.inputs[0])
+        from_type = onnx_utils.tensor_dtype_to_jnp_dtype(tensor_proto.data_type)
+      else:
         raise ValueError(
-            f"{node.inputs[0]} is not constant but used as a static argument "
-            "when `jax.jit` the `Cast` operator. "
-            "The jitted function gives wrong results if its value changes."
+            "`config.jaxort_only_allow_initializers_as_static_args = True but "
+            f"{node.inputs[0]} tensor is not constant. We can not use it"
+            "a static argument of the `Cast` operator. "
         )
+    else:
       from_type = inputs[0].dtype
     node.attrs_dict["from_type"] = from_type
 
   @classmethod
   def version_9(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
@@ -89,16 +95,21 @@
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_19 Cast op."""
     cls._prepare(node, inputs, onnx_cast)
     return onnx_cast
 
 
-@functools.partial(jit, static_argnames=("to", "from_type"))
-def onnx_cast(x, *, to, from_type=None):
+@functools.partial(jax.jit, static_argnames=("to", "from_type"))
+def onnx_cast(
+    x: jax.Array,
+    *,
+    to: onnx.TensorProto.DataType,
+    from_type: Optional[jnp.dtype],
+) -> jax.Array:
   """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Cast for more details."""
   if from_type is onnx.TensorProto.STRING or to is onnx.TensorProto.STRING:
     raise NotImplementedError(
         "Cast JAX version do not support STRING type yet."
     )
   to_type = onnx_utils.tensor_dtype_to_jnp_dtype(to)
   try:
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/ceil.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/ceil.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/concat.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/concat.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/constant.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/flatten.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,93 +21,75 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Constant operator."""
+"""Define ONNX Flatten operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
+import inspect
 from typing import Any
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
-import onnx
+import numpy as np
 
 
-def _asarray(proto):
-  return jnp.asarray(
-      onnx.numpy_helper.to_array(proto).reshape(tuple(proto.dims))
-  )
-
-
-@handler.register_op('Constant')
-class Constant(handler.Handler):
-  """Implementation of the ONNX Constant operator."""
+@handler.register_op("Flatten")
+class Flatten(handler.Handler):
+  """Implementation of the ONNX Flatten operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    attr_to_dtype = {
-        'value_int': jnp.int64,
-        'value_ints': jnp.int64,
-        'value_float': jnp.float32,
-        'value_floats': jnp.float32,
-    }
-
-    matched = 0
-    if 'value_string' in node.attrs:
-      node.attrs_dict['value'] = node.attrs['value_string']
-      matched = matched + 1
-    elif 'value_strings' in node.attrs:
-      node.attrs_dict['value'] = node.attrs['value_strings']
-      matched = matched + 1
-    elif 'value' in node.attrs:
-      node.attrs_dict['value'] = _asarray(node.attrs['value'])
-      matched = matched + 1
-    else:
-      for item in attr_to_dtype:
-        if item in node.attrs:
-          node.attrs_dict['value'] = jnp.array(
-              node.attrs[item], dtype=attr_to_dtype[item]
-          )
-        matched = matched + 1
-
-    assert (
-        matched == 1
-    ), f'Should only provide one of value attributes, but get {matched}'
+    sig = inspect.signature(onnx_jax_impl)
+    kwparams = [
+        param.name
+        for param in sig.parameters.values()
+        if param.kind == inspect.Parameter.KEYWORD_ONLY
+    ]
+    for name in kwparams:
+      node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_9(
+  def version_1(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_9 Constant op."""
-    cls._prepare(node, inputs, onnx_constant)
-    return onnx_constant
+    """ONNX version_1 Flatten op."""
+    cls._prepare(node, inputs, onnx_flatten)
+    return onnx_flatten
 
   @classmethod
-  def version_13(
+  def version_11(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Constant op."""
-    cls._prepare(node, inputs, onnx_constant)
-    return onnx_constant
+    """ONNX version_11 Flatten op."""
+    cls._prepare(node, inputs, onnx_flatten)
+    return onnx_flatten
 
   @classmethod
-  def version_19(
+  def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_19 Constant op."""
-    cls._prepare(node, inputs, onnx_constant)
-    return onnx_constant
+    """ONNX version_13 Flatten op."""
+    cls._prepare(node, inputs, onnx_flatten)
+    return onnx_flatten
 
 
-@functools.partial(jit, static_argnames=())
-def onnx_constant(*input_args, value):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Constant."""
-  assert len(input_args) == 0
-  return value
+@functools.partial(jit, static_argnames="axis")
+def onnx_flatten(*input_args, axis):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Flatten for more details."""
+  axis = 1 if axis is None else axis
+  assert len(input_args) == 1
+  x = input_args[0]
+  dim = len(x.shape)
+  assert axis < dim and axis >= -dim, f"axis should with [{-dim}, {dim}]"
+  new_shape = (
+      (1, -1) if axis == 0 else (-1, np.prod(x.shape[axis:]).astype(int))
+  )
+  return jnp.reshape(x, new_shape)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/constantofshape.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/constantofshape.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/conv.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/conv.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/div.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/sum.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Div operator."""
+"""Define ONNX Sum operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Div")
-class Div(handler.Handler):
-  """Implementation of the ONNX Div operator."""
+@handler.register_op("Sum")
+class Sum(handler.Handler):
+  """Implementation of the ONNX Sum operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,42 +53,35 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_7(
+  def version_6(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_7 Div op."""
-    cls._prepare(node, inputs, onnx_div)
-    return onnx_div
+    """ONNX version_6 Sum op."""
+    cls._prepare(node, inputs, onnx_sum)
+    return onnx_sum
 
   @classmethod
-  def version_13(
+  def version_8(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Div op."""
-    cls._prepare(node, inputs, onnx_div)
-    return onnx_div
+    """ONNX version_8 Sum op."""
+    cls._prepare(node, inputs, onnx_sum)
+    return onnx_sum
 
   @classmethod
-  def version_14(
+  def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_14 Div op."""
-    cls._prepare(node, inputs, onnx_div)
-    return onnx_div
+    """ONNX version_13 Sum op."""
+    cls._prepare(node, inputs, onnx_sum)
+    return onnx_sum
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_div(*input_args):
-  """The internal jax impl for onnx Div op."""
-  assert len(input_args) == 2
-  x, y = input_args
-  if jnp.issubdtype(x.dtype, jnp.integer) and jnp.issubdtype(
-      y.dtype, jnp.integer
-  ):
-    return jnp.floor_divide(x, y)
-  else:
-    return jnp.true_divide(x, y)
+def onnx_sum(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sum for more details."""
+  return jnp.sum(jnp.array(input_args), axis=0)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/dropout.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/dropout.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/equal.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/tanh.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,31 +21,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Equal operator."""
-# pylint: disable=unused-argument
-# pylint: disable=g-explicit-length-test
+"""Define ONNX Tanh operator."""
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Equal")
-class Equal(handler.Handler):
-  """Implementation of the ONNX Equal operator."""
+@handler.register_op("Tanh")
+class Tanh(handler.Handler):
+  """Implementation of the ONNX Tanh operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -53,28 +51,29 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_13(
+  def version_6(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Equal op."""
-    cls._prepare(node, inputs, onnx_equal)
-    return onnx_equal
+    """ONNX version_6 Tanh op."""
+    cls._prepare(node, inputs, onnx_tanh)
+    return onnx_tanh
 
   @classmethod
-  def version_19(
+  def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_19 Equal op."""
-    cls._prepare(node, inputs, onnx_equal)
-    return onnx_equal
+    """ONNX version_13 Tanh op."""
+    cls._prepare(node, inputs, onnx_tanh)
+    return onnx_tanh
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_equal(*input_args):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Equal for more details."""
-  assert len(input_args) == 2
-  return jnp.equal(input_args[0], input_args[1])
+def onnx_tanh(*input_args):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Tanh."""
+  assert len(input_args) == 1
+  x = input_args[0]
+  return jnp.tanh(x)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/exp.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/sqrt.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Exp operator."""
+"""Define ONNX Sqrt operator."""
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Exp")
-class Exp(handler.Handler):
-  """Implementation of the ONNX Exp operator."""
+@handler.register_op("Sqrt")
+class Sqrt(handler.Handler):
+  """Implementation of the ONNX Sqrt operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,21 +51,28 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_6(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_6 Sqrt op."""
+    cls._prepare(node, inputs, onnx_sqrt)
+    return onnx_sqrt
+
+  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Exp op."""
-    cls._prepare(node, inputs, onnx_exp)
-    return onnx_exp
+    """ONNX version_13 Sqrt op."""
+    cls._prepare(node, inputs, onnx_sqrt)
+    return onnx_sqrt
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_exp(*input_args):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Exp."""
+def onnx_sqrt(*input_args):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sqrt."""
   assert len(input_args) == 1
-  x = input_args[0]
-  return jnp.exp(x)
+  return jnp.sqrt(*input_args)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/expand.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/expand.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,15 +50,19 @@
     if config.jaxort_only_allow_initializers_as_static_args:
       if node.inputs[1] not in node.context_graph.initializer_dict:
         raise ValueError(
             f"{node.inputs[1]} is not constant but used as a static argument "
             "`shape` when `jax.jit` the `Expand` operator. "
             "The jitted function gives wrong results if its value changes."
         )
-    node.attrs_dict["shape"] = tuple(inputs[1].tolist())
+      node.attrs_dict["shape"] = tuple(
+          node.context_graph.initializer_dict[node.inputs[1]].tolist()
+      )
+    else:
+      node.attrs_dict["shape"] = tuple(inputs[1].tolist())
 
   @classmethod
   def version_8(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_8 Expand op."""
     cls._prepare(node, inputs, onnx_expand)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/flatten.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/max.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,67 +21,64 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Flatten operator."""
+"""Define ONNX Max operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
+
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
-import numpy as np
 
 
-@handler.register_op("Flatten")
-class Flatten(handler.Handler):
-  """Implementation of the ONNX Flatten operator."""
+@handler.register_op("Max")
+class Max(handler.Handler):
+  """Implementation of the ONNX Max operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
         param.name
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
+    node.attrs_dict["arg_num"] = len(node.inputs)
 
   @classmethod
-  def version_1(
+  def version_6(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_1 Flatten op."""
-    cls._prepare(node, inputs, onnx_flatten)
-    return onnx_flatten
+    """ONNX version_6 Max op."""
+    cls._prepare(node, inputs, onnx_max)
+    return onnx_max
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Flatten op."""
-    cls._prepare(node, inputs, onnx_flatten)
-    return onnx_flatten
-
-
-@functools.partial(jit, static_argnames="axis")
-def onnx_flatten(*input_args, axis):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Flatten for more details."""
-  axis = 1 if axis is None else axis
-  assert len(input_args) == 1
-  x = input_args[0]
-  dim = len(x.shape)
-  assert axis < dim and axis >= -dim, f"axis should with [{-dim}, {dim}]"
-  new_shape = (
-      (1, -1) if axis == 0 else (-1, np.prod(x.shape[axis:]).astype(int))
-  )
-  return jnp.reshape(x, new_shape)
+    """ONNX version_13 Max op."""
+    cls._prepare(node, inputs, onnx_max)
+    return onnx_max
+
+
+@functools.partial(jit, static_argnames=("arg_num",))
+def onnx_max(*input_args, arg_num):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Max for more details."""
+  assert len(input_args) == arg_num
+  res = input_args[0]
+  for i in range(arg_num):
+    res = jnp.maximum(res, input_args[i])
+  return res
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/gather.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/gather.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/gemm.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/less.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Gemm operator."""
+"""Define ONNX Less operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
-from typing import Any, Optional
+from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('Gemm')
-class Gemm(handler.Handler):
-  """Implementation of the ONNX Gemm operator."""
+@handler.register_op("Less")
+class Less(handler.Handler):
+  """Implementation of the ONNX Less operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,59 +53,28 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_7(
-      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
-  ) -> Callable[..., Any]:
-    """ONNX version_7 Gemm op."""
-    cls._prepare(node, inputs, onnx_gemm)
-    return onnx_gemm
-
-  @classmethod
   def version_9(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_9 Gemm op."""
-    cls._prepare(node, inputs, onnx_gemm)
-    return onnx_gemm
+    """ONNX version_9 Less op."""
+    cls._prepare(node, inputs, onnx_less)
+    return onnx_less
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Gemm op."""
-    cls._prepare(node, inputs, onnx_gemm)
-    return onnx_gemm
-
-
-@functools.partial(jit, static_argnames=('alpha', 'beta', 'transA', 'transB'))
-def onnx_gemm(
-    *input_args,
-    alpha: Optional[float] = None,
-    beta: Optional[float] = None,
-    transA: Optional[int] = None,
-    transB: Optional[int] = None
-):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Gemm."""
-  assert len(input_args) == 3 or len(input_args) == 2
-  if len(input_args) == 2:
-    a, b = input_args
-    c = 0
-  else:
-    a, b, c = input_args
-
-  alpha = 1.0 if not alpha else alpha
-  beta = 1.0 if not beta else beta
-  transA = 0 if not transA else transA
-  transB = 0 if not transB else transB
-
-  if transA == 1:
-    a = jnp.transpose(a)
-  if transB == 1:
-    b = jnp.transpose(b)
+    """ONNX version_13 Less op."""
+    cls._prepare(node, inputs, onnx_less)
+    return onnx_less
+
 
-    # Compute the matrix multiplicat
-  return alpha * jnp.dot(a, b) + beta * c
+@functools.partial(jit, static_argnames=())
+def onnx_less(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Less for more details."""
+  assert len(input_args) == 2
+  return jnp.less(input_args[0], input_args[1])
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/globalaveragepool.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/globalaveragepool.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/identity.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/transpose.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,30 +21,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Identity operator."""
-# pylint: disable=unused-argument
-# pylint: disable=g-explicit-length-test
+"""Define ONNX Transpose operator."""
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
+from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Identity")
-class Identity(handler.Handler):
-  """Implementation of the ONNX Identity operator."""
+@handler.register_op("Transpose")
+class Transpose(handler.Handler):
+  """Implementation of the ONNX Transpose operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -55,32 +54,26 @@
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
   def version_1(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_1 Identity op."""
-    cls._prepare(node, inputs, onnx_identity)
-    return onnx_identity
+    """ONNX version_1 Transpose op."""
+    cls._prepare(node, inputs, onnx_transpose)
+    return onnx_transpose
 
   @classmethod
-  def version_16(
+  def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_16 Identity op."""
-    cls._prepare(node, inputs, onnx_identity)
-    return onnx_identity
+    """ONNX version_13 Transpose op."""
+    cls._prepare(node, inputs, onnx_transpose)
+    return onnx_transpose
 
-  @classmethod
-  def version_19(
-      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
-  ) -> Callable[..., Any]:
-    """ONNX version_19 Identity op."""
-    cls._prepare(node, inputs, onnx_identity)
-    return onnx_identity
-
-@functools.partial(jit, static_argnames=())
-def onnx_identity(*input_args):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Identity for more details."""
+
+@functools.partial(jit, static_argnames="perm")
+def onnx_transpose(*input_args, perm):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Transpose."""
   assert len(input_args) == 1
-  return [input_args[0]]
+  x = input_args[0]
+  return jnp.transpose(x, perm)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/if_op.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/if_op.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,21 +59,37 @@
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_11 If op."""
     cls._prepare(node, inputs, onnx_if)
     return onnx_if
 
   @classmethod
+  def version_13(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_13 If op."""
+    cls._prepare(node, inputs, onnx_if)
+    return onnx_if
+
+  @classmethod
   def version_16(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_16 If op."""
     cls._prepare(node, inputs, onnx_if)
     return onnx_if
 
+  @classmethod
+  def version_19(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_19 If op."""
+    cls._prepare(node, inputs, onnx_if)
+    return onnx_if
+
 
 def flatten_subgraph(node, inputs):
   """Recursively construct the subgraphs for else and then branches."""
   from jaxonnxruntime.call_onnx import call_onnx_graph  # pylint: disable=g-import-not-at-top
 
   inp_start = 1
   subgraph_out_shape = None
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/leakyrelu.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/leakyrelu.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,22 @@
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
     node.attrs_dict["alpha"] = node.attrs.get("alpha", 0.01)
 
   @classmethod
+  def version_6(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_6 LeakyRelu op."""
+    cls._prepare(node, inputs, onnx_leakyrelu)
+    return onnx_leakyrelu
+
+  @classmethod
   def version_16(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_16 LeakyRelu op."""
     cls._prepare(node, inputs, onnx_leakyrelu)
     return onnx_leakyrelu
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/less.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/or_op.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Less operator."""
+"""Define ONNX Or operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Less")
-class Less(handler.Handler):
-  """Implementation of the ONNX Less operator."""
+@handler.register_op("Or")
+class Or(handler.Handler):
+  """Implementation of the ONNX Or operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -53,20 +53,20 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_13(
+  def version_7(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Less op."""
-    cls._prepare(node, inputs, onnx_less)
-    return onnx_less
+    """ONNX version_7 Or op."""
+    cls._prepare(node, inputs, onnx_or)
+    return onnx_or
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_less(*input_args):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Less for more details."""
+def onnx_or(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Or for more details."""
   assert len(input_args) == 2
-  return jnp.less(input_args[0], input_args[1])
+  return jnp.logical_or(input_args[0], input_args[1])
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/lessorequal.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/lessorequal.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/lrn.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/lrn.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/matmul.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/matmul.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,22 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_1(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_1 MatMul op."""
+    cls._prepare(node, inputs, onnx_matmul)
+    return onnx_matmul
+
+  @classmethod
   def version_9(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_9 MatMul op."""
     cls._prepare(node, inputs, onnx_matmul)
     return onnx_matmul
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/max.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/sigmoid.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,56 +21,60 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Max operator."""
+"""Define ONNX Sigmoid operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
+import jax
 from jax import jit
-from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Max")
-class Max(handler.Handler):
-  """Implementation of the ONNX Max operator."""
+@handler.register_op("Sigmoid")
+class Sigmoid(handler.Handler):
+  """Implementation of the ONNX Sigmoid operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
         param.name
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
-    node.attrs_dict["arg_num"] = len(node.inputs)
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Max op."""
-    cls._prepare(node, inputs, onnx_max)
-    return onnx_max
+    """ONNX version_13 Sigmoid op."""
+    cls._prepare(node, inputs, onnx_sigmoid)
+    return onnx_sigmoid
+
+  @classmethod
+  def version_6(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_6 Sigmoid op."""
+    cls._prepare(node, inputs, onnx_sigmoid)
+    return onnx_sigmoid
 
 
-@functools.partial(jit, static_argnames=("arg_num",))
-def onnx_max(*input_args, arg_num):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Max for more details."""
-  assert len(input_args) == arg_num
-  res = input_args[0]
-  for i in range(arg_num):
-    res = jnp.maximum(res, input_args[i])
-  return res
+@functools.partial(jit, static_argnames=())
+def onnx_sigmoid(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sigmoid for more details."""
+  assert len(input_args) == 1
+  return jax.nn.sigmoid(input_args[0])
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/maxpool.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/maxpool.py`

 * *Files 18% similar despite different names*

```diff
@@ -101,22 +101,46 @@
       }
       assert (
           pad_str_type in onnx_to_jax_pad_type
       ), f"Invalid auto_pad attribute: {pad_str_type}"
       node.attrs_dict["pads"] = onnx_to_jax_pad_type[pad_str_type]
 
   @classmethod
+  def version_1(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_1 MaxPool op."""
+    cls._prepare(node, inputs, onnx_maxpool)
+    return onnx_maxpool
+
+  @classmethod
   def version_8(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_8 MaxPool op."""
     cls._prepare(node, inputs, onnx_maxpool)
     return onnx_maxpool
 
   @classmethod
+  def version_10(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_10 MaxPool op."""
+    cls._prepare(node, inputs, onnx_maxpool)
+    return onnx_maxpool
+
+  @classmethod
+  def version_11(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_11 MaxPool op."""
+    cls._prepare(node, inputs, onnx_maxpool)
+    return onnx_maxpool
+
+  @classmethod
   def version_12(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_12 MaxPool op."""
     cls._prepare(node, inputs, onnx_maxpool)
     return onnx_maxpool
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/mul.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/sub.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Mul operator."""
+"""Define ONNX Sub operator."""
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Mul")
-class Mul(handler.Handler):
-  """Implementation of the ONNX Mul operator."""
+@handler.register_op("Sub")
+class Sub(handler.Handler):
+  """Implementation of the ONNX Sub operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,29 +51,45 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_6(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_6 Sub op."""
+    cls._prepare(node, inputs, onnx_sub)
+    return onnx_sub
+
+  @classmethod
   def version_7(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_7 Mul op."""
-    cls._prepare(node, inputs, onnx_mul)
-    return onnx_mul
+    """ONNX version_7 Sub op."""
+    cls._prepare(node, inputs, onnx_sub)
+    return onnx_sub
+
+  @classmethod
+  def version_13(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_13 Sub op."""
+    cls._prepare(node, inputs, onnx_sub)
+    return onnx_sub
 
   @classmethod
   def version_14(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_14 Mul op."""
-    cls._prepare(node, inputs, onnx_mul)
-    return onnx_mul
+    """ONNX version_14 Sub op."""
+    cls._prepare(node, inputs, onnx_sub)
+    return onnx_sub
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_mul(*input_args):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Mul."""
+def onnx_sub(*input_args):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sub."""
   assert len(input_args) == 2
   a, b = input_args
-  return jnp.multiply(a, b)
+  return jnp.subtract(a, b)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/neg.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/neg.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,22 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_6(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_6 Neg op."""
+    cls._prepare(node, inputs, onnx_neg)
+    return onnx_neg
+
+  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_13 Neg op."""
     cls._prepare(node, inputs, onnx_neg)
     return onnx_neg
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/nonzero.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/nonzero.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/onehot.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/onehot.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/or_op.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/sinh.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,44 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# Copyright 2023 The Jaxonnxruntime Authors.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-"""Define ONNX Or operator."""
+"""Define ONNX Sinh operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Or")
-class Or(handler.Handler):
-  """Implementation of the ONNX Or operator."""
+@handler.register_op("Sinh")
+class Sinh(handler.Handler):
+  """Implementation of the ONNX Sinh operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -53,20 +40,21 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_7(
+  def version_9(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_7 Or op."""
-    cls._prepare(node, inputs, onnx_or)
-    return onnx_or
+    """ONNX version_9 Sinh op."""
+    cls._prepare(node, inputs, onnx_sinh)
+    return onnx_sinh
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_or(*input_args):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Or for more details."""
-  assert len(input_args) == 2
-  return jnp.logical_or(input_args[0], input_args[1])
+def onnx_sinh(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sinh for more details."""
+  assert len(input_args) == 1
+  data = input_args[0]
+  return jnp.sinh(data)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/pad.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/slice.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,101 +21,83 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Pad operator."""
+"""Define ONNX Slice operator."""
 from collections.abc import Callable, Sequence
 import functools
 from typing import Any
-
 from jax import jit
-from jax import numpy as jnp
-from jaxonnxruntime import config
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('Pad')
-class Pad(handler.Handler):
-  """Implementation of the ONNX Pad operator."""
+@handler.register_op('Slice')
+class Slice(handler.Handler):
+  """Implementation of the ONNX Slice operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    node.attrs_dict['mode'] = node.attrs.get('mode', 'constant')
-
-    if config.jaxort_only_allow_initializers_as_static_args:
-      for index in range(1, len(node.inputs)):
-        if node.inputs[index] not in node.context_graph.initializer_dict:
-          raise ValueError(
-              f'{node.inputs[index]} is not constant but used as `pads`'
-              ' static argument during `jax.jit`. '
-              'the jitted function gives wrong results if its value changes'
-              'in another input.'
-          )
-    if len(inputs) >= 2:
-      node.attrs_dict['pads'] = tuple(inputs[1].tolist())
-
-    if len(inputs) >= 3:
-      node.attrs_dict['constant_value'] = inputs[2].item()
-    else:
-      node.attrs_dict['constant_value'] = 0.0
-
+    node.attrs_dict['starts'] = tuple(inputs[1].tolist())
+    node.attrs_dict['ends'] = tuple(inputs[2].tolist())
     if len(inputs) >= 4:
       node.attrs_dict['axes'] = tuple(inputs[3].tolist())
     else:
-      node.attrs_dict['axes'] = tuple(range(len(inputs[0].shape)))
+      node.attrs_dict['axes'] = None
+    if len(inputs) >= 5:
+      node.attrs_dict['steps'] = tuple(inputs[4].tolist())
+    else:
+      node.attrs_dict['steps'] = None
 
   @classmethod
-  def version_13(
+  def version_1(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_1 Slice op."""
+    cls._prepare(node, inputs, onnx_slice)
+    return onnx_slice
+
+  @classmethod
+  def version_10(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Pad op."""
-    cls._prepare(node, inputs, onnx_pad)
-    return onnx_pad
+    """ONNX version_10 Slice op."""
+    cls._prepare(node, inputs, onnx_slice)
+    return onnx_slice
 
   @classmethod
-  def version_19(
+  def version_11(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_19 Pad op."""
-    cls._prepare(node, inputs, onnx_pad)
-    return onnx_pad
-
-
-@functools.partial(
-    jit, static_argnames=('pads', 'constant_value', 'mode', 'axes')
-)
-def onnx_pad(
-    *input_args,
-    pads: Sequence[int],
-    constant_value: Any,
-    mode: str,
-    axes: Sequence[int],
-):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Pad."""
+    """ONNX version_11 Slice op."""
+    cls._prepare(node, inputs, onnx_slice)
+    return onnx_slice
+
+  @classmethod
+  def version_13(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_13 Slice op."""
+    cls._prepare(node, inputs, onnx_slice)
+    return onnx_slice
+
+
+@functools.partial(jit, static_argnames=('starts', 'ends', 'axes', 'steps'))
+def onnx_slice(*input_args, starts, ends, axes, steps):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Slice."""
   x = input_args[0]
-  input_rank = x.ndim
-  axes = [axis if axis >= 0 else axis + input_rank for axis in axes]
-  num_axes = len(axes)
-  if num_axes * 2 != jnp.size(pads):
-    raise ValueError(
-        'The number of elements in raw_pads should be 2 * len(axis)'
-        f'pads = {pads}, axis = {axes}'
-    )
-
-  # re-order to np.pad accepted order ((x1_begin, x1_end), (x2_begin, x2_end))
-  pad_width = []
-  for _ in range(input_rank):
-    pad_width += [[0, 0]]
-
-  for i in range(num_axes):
-    axis = axes[i]
-    pad_width[axis] = [pads[i], pads[i + num_axes]]
-
-  if mode == 'constant':
-    return jnp.pad(x, pad_width, mode, constant_values=constant_value)
-  return jnp.pad(x, pad_width, mode)
+  if axes is None:
+    axes = tuple(range(len(starts)))
+  if steps is None:
+    steps = [1] * len(starts)
+  slices = tuple(
+      slice(start, end, step) for start, end, step in zip(starts, ends, steps)
+  )
+  sub_indx = [slice(None)] * len(x.shape)
+  for i, axis in enumerate(axes):
+    sub_indx[axis] = slices[i]
+  return x[tuple(sub_indx)]
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/pow.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/shape.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Pow operator."""
+"""Define ONNX Shape operator."""
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Pow")
-class Pow(handler.Handler):
-  """Implementation of the ONNX Pow operator."""
+@handler.register_op('Shape')
+class Shape(handler.Handler):
+  """Implementation of the ONNX Shape operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,35 +51,46 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_7(
+  def version_1(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_7 Pow op."""
-    cls._prepare(node, inputs, onnx_pow)
-    return onnx_pow
+    """ONNX version_1 Shape op."""
+    cls._prepare(node, inputs, onnx_shape)
+    return onnx_shape
 
   @classmethod
-  def version_12(
+  def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_12 Pow op."""
-    cls._prepare(node, inputs, onnx_pow)
-    return onnx_pow
+    """ONNX version_13 Shape op."""
+    cls._prepare(node, inputs, onnx_shape)
+    return onnx_shape
 
   @classmethod
   def version_15(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_15 Pow op."""
-    cls._prepare(node, inputs, onnx_pow)
-    return onnx_pow
+    """ONNX version_15 Shape op."""
+    cls._prepare(node, inputs, onnx_shape)
+    return onnx_shape
+
+  @classmethod
+  def version_19(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_19 Shape op."""
+    cls._prepare(node, inputs, onnx_shape)
+    return onnx_shape
 
 
-@functools.partial(jit, static_argnames=())
-def onnx_pow(a, b):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Pow."""
-  return jnp.power(a, b).astype(a.dtype)
+@functools.partial(jit, static_argnames=('start', 'end'))
+def onnx_shape(*input_args, start=None, end=None):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Shape."""
+  assert len(input_args) == 1
+  x = input_args[0]
+  dims = x.shape[start:end]
+  return jnp.asarray(dims)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/range.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/equal.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,55 +21,68 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Range operator."""
+"""Define ONNX Equal operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
+import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
-from jaxonnxruntime import config
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Range")
-class Range(handler.Handler):
-  """Implementation of the ONNX Range operator."""
+@handler.register_op("Equal")
+class Equal(handler.Handler):
+  """Implementation of the ONNX Equal operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    if config.jaxort_only_allow_initializers_as_static_args:
-      for inp in node.inputs[1:]:
-        if inp not in node.context_graph.initializer_dict:
-          raise ValueError(
-              f"{inp} is not constant but used as a static argument "
-              "when `jax.jit` the `Range` operator. "
-              "The jitted function gives wrong results if its value changes."
-          )
-    node.attrs_dict["start"] = inputs[0].item()
-    node.attrs_dict["limit"] = inputs[1].item()
-    node.attrs_dict["delta"] = inputs[2].item()
-    node.attrs_dict["dtype"] = inputs[0].dtype
+    sig = inspect.signature(onnx_jax_impl)
+    kwparams = [
+        param.name
+        for param in sig.parameters.values()
+        if param.kind == inspect.Parameter.KEYWORD_ONLY
+    ]
+    for name in kwparams:
+      node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
   def version_11(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_11 Range op."""
-    cls._prepare(node, inputs, onnx_range)
-    return onnx_range
+    """ONNX version_11 Equal op."""
+    cls._prepare(node, inputs, onnx_equal)
+    return onnx_equal
+
+  @classmethod
+  def version_13(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_13 Equal op."""
+    cls._prepare(node, inputs, onnx_equal)
+    return onnx_equal
+
+  @classmethod
+  def version_19(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_19 Equal op."""
+    cls._prepare(node, inputs, onnx_equal)
+    return onnx_equal
 
 
-@functools.partial(jit, static_argnames=("start", "limit", "delta", "dtype"))
-def onnx_range(*_, start, limit, delta, dtype):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Range for more details."""
-  return jnp.arange(start, stop=limit, step=delta, dtype=dtype)
+@functools.partial(jit, static_argnames=())
+def onnx_equal(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Equal for more details."""
+  assert len(input_args) == 2
+  return jnp.equal(input_args[0], input_args[1])
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reciprocal.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/reciprocal.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reducemax.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/reducemax.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Define ONNX ReduceMax operator."""
 from collections.abc import Callable, Sequence
 import functools
-import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
@@ -41,30 +40,23 @@
 class ReduceMax(handler.Handler):
   """Implementation of the ONNX ReduceMax operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    sig = inspect.signature(onnx_jax_impl)
-    kwparams = [
-        param.name
-        for param in sig.parameters.values()
-        if param.kind == inspect.Parameter.KEYWORD_ONLY
-    ]
-    for name in kwparams:
-      node.attrs_dict[name] = node.attrs.get(name, None)
-
+    node.attrs_dict['axes'] = node.attrs.get('axes')
     if len(inputs) >= 2:
       node.attrs_dict['axes'] = tuple(inputs[1].tolist())
       node.attrs_dict['axes'] = (
           None if len(node.attrs_dict['axes']) == 0 else node.attrs_dict['axes']
       )
-    node.attrs_dict['keepdims'] = (
-        True if node.attrs_dict['keepdims'] == 1 else False
+    node.attrs_dict['keepdims'] = node.attrs.get('keepdims', 1)
+    node.attrs_dict['noop_with_empty_axes'] = node.attrs.get(
+        'noop_with_empty_axes', 0
     )
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_13 ReduceMax op."""
@@ -76,18 +68,22 @@
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_18 ReduceMax op."""
     cls._prepare(node, inputs, onnx_reducemax)
     return onnx_reducemax
 
 
-@functools.partial(jit, static_argnames=('axes', 'keepdims'))
+@functools.partial(
+    jit, static_argnames=('axes', 'keepdims', 'noop_with_empty_axes')
+)
 def onnx_reducemax(
-    *input_args, axes=None, keepdims=False, noop_with_empty_axes=None
+    *input_args,
+    axes=None,
+    keepdims=1,
+    noop_with_empty_axes=0,
 ):
   """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#ReduceSum."""
   assert len(input_args) == 1 or len(input_args) == 2
   data = input_args[0]
-  noop_with_empty_axes = 0 if not noop_with_empty_axes else noop_with_empty_axes
-  if noop_with_empty_axes != 0:
+  if axes is None and noop_with_empty_axes > 0:
     return data
-  return jnp.max(data, axis=axes, keepdims=keepdims)
+  return jnp.max(data, axis=axes, keepdims=keepdims > 0)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reducemean.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/reducemean.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Define ONNX ReduceMean operator."""
 from collections.abc import Callable, Sequence
 import functools
-import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
@@ -41,30 +40,23 @@
 class ReduceMean(handler.Handler):
   """Implementation of the ONNX ReduceMean operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    sig = inspect.signature(onnx_jax_impl)
-    kwparams = [
-        param.name
-        for param in sig.parameters.values()
-        if param.kind == inspect.Parameter.KEYWORD_ONLY
-    ]
-    for name in kwparams:
-      node.attrs_dict[name] = node.attrs.get(name, None)
-
+    node.attrs_dict['axes'] = node.attrs.get('axes')
     if len(inputs) >= 2:
       node.attrs_dict['axes'] = tuple(inputs[1].tolist())
       node.attrs_dict['axes'] = (
           None if len(node.attrs_dict['axes']) == 0 else node.attrs_dict['axes']
       )
-    node.attrs_dict['keepdims'] = (
-        True if node.attrs_dict['keepdims'] == 1 else False
+    node.attrs_dict['keepdims'] = node.attrs.get('keepdims', 1)
+    node.attrs_dict['noop_with_empty_axes'] = node.attrs.get(
+        'noop_with_empty_axes', 0
     )
 
   @classmethod
   def version_1(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_1 ReduceMean op."""
@@ -92,18 +84,22 @@
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_18 ReduceMean op."""
     cls._prepare(node, inputs, onnx_reducemean)
     return onnx_reducemean
 
 
-@functools.partial(jit, static_argnames=('axes', 'keepdims'))
+@functools.partial(
+    jit, static_argnames=('axes', 'keepdims', 'noop_with_empty_axes')
+)
 def onnx_reducemean(
-    *input_args, axes=None, keepdims=False, noop_with_empty_axes=None
+    *input_args,
+    axes=None,
+    keepdims=1,
+    noop_with_empty_axes=0,
 ):
   """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#ReduceSum."""
   assert len(input_args) == 1 or len(input_args) == 2
   data = input_args[0]
-  noop_with_empty_axes = 0 if not noop_with_empty_axes else noop_with_empty_axes
-  if noop_with_empty_axes != 0:
+  if axes is None and noop_with_empty_axes > 0:
     return data
-  return jnp.mean(data, axis=axes, keepdims=keepdims)
+  return jnp.mean(data, axis=axes, keepdims=keepdims > 0)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reducesum.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/reducesum.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Define ONNX ReduceSum operator."""
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
-import inspect
 from typing import Any
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
@@ -41,47 +40,50 @@
 class ReduceSum(handler.Handler):
   """Implementation of the ONNX ReduceSum operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    sig = inspect.signature(onnx_jax_impl)
-    kwparams = [
-        param.name
-        for param in sig.parameters.values()
-        if param.kind == inspect.Parameter.KEYWORD_ONLY
-    ]
-    for name in kwparams:
-      node.attrs_dict[name] = node.attrs.get(name, None)
-
+    node.attrs_dict['axes'] = node.attrs.get('axes')
     if len(inputs) >= 2:
       node.attrs_dict['axes'] = tuple(inputs[1].tolist())
       node.attrs_dict['axes'] = (
           None if len(node.attrs_dict['axes']) == 0 else node.attrs_dict['axes']
       )
-    node.attrs_dict['keepdims'] = (
-        True if node.attrs_dict['keepdims'] == 1 else False
+    node.attrs_dict['keepdims'] = node.attrs.get('keepdims', 1)
+    node.attrs_dict['noop_with_empty_axes'] = node.attrs.get(
+        'noop_with_empty_axes', 0
     )
 
   @classmethod
+  def version_1(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_1 ReduceSum op."""
+    cls._prepare(node, inputs, onnx_reducesum)
+    return onnx_reducesum
+
+  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_13 ReduceSum op."""
     cls._prepare(node, inputs, onnx_reducesum)
     return onnx_reducesum
 
 
 @functools.partial(
     jit, static_argnames=('axes', 'keepdims', 'noop_with_empty_axes')
 )
 def onnx_reducesum(
-    *input_args, axes=None, keepdims=False, noop_with_empty_axes=None
+    *input_args,
+    axes=None,
+    keepdims=1,
+    noop_with_empty_axes=0,
 ):
   """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#ReduceSum."""
   assert len(input_args) == 1 or len(input_args) == 2
   data = input_args[0]
-  noop_with_empty_axes = 0 if not noop_with_empty_axes else noop_with_empty_axes
-  if noop_with_empty_axes != 0:
+  if axes is None and noop_with_empty_axes > 0:
     return data
-  return jnp.sum(data, axis=axes, keepdims=keepdims)
+  return jnp.sum(data, axis=axes, keepdims=keepdims > 0)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/relu.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/atan.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,44 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# Copyright 2023 The Jaxonnxruntime Authors.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-"""Define ONNX Relu operator."""
+"""Define ONNX Atan operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
-import jax
 from jax import jit
+from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Relu")
-class Relu(handler.Handler):
-  """Implementation of the ONNX Relu operator."""
+@handler.register_op("Atan")
+class Atan(handler.Handler):
+  """Implementation of the ONNX Atan operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -53,29 +40,21 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_6(
-      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
-  ) -> Callable[..., Any]:
-    """ONNX version_6 Relu op."""
-    cls._prepare(node, inputs, onnx_relu)
-    return onnx_relu
-
-  @classmethod
-  def version_14(
+  def version_7(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_14 Relu op."""
-    cls._prepare(node, inputs, onnx_relu)
-    return onnx_relu
+    """ONNX version_7 Atan op."""
+    cls._prepare(node, inputs, onnx_atan)
+    return onnx_atan
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_relu(*input_args):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Relu for more details."""
+def onnx_atan(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Atan for more details."""
   assert len(input_args) == 1
-  x = input_args[0]
-  return jax.nn.relu(x)
+  data = input_args[0]
+  return jnp.arctan(data)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reshape.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/reshape.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,26 +49,38 @@
       if node.inputs[1] not in node.context_graph.initializer_dict:
         raise ValueError(
             f'{node.inputs[1]} is not constant but used as `shape` of Reshape'
             ' static argument during `jax.jit`. '
             'the jitted function gives wrong results if its value changes '
             'in another input.'
         )
-    node.attrs_dict['shape'] = tuple(inputs[1].tolist())
+      node.attrs_dict['shape'] = tuple(
+          node.context_graph.initializer_dict[node.inputs[1]].tolist()
+      )
+    else:
+      node.attrs_dict['shape'] = tuple(inputs[1].tolist())
     node.attrs_dict['allowzero'] = node.attrs.get('allowzero', 0)
 
   @classmethod
   def version_5(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_5 Reshape op."""
     cls._prepare(node, inputs, onnx_reshape)
     return onnx_reshape
 
   @classmethod
+  def version_13(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_13 Reshape op."""
+    cls._prepare(node, inputs, onnx_reshape)
+    return onnx_reshape
+
+  @classmethod
   def version_14(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_14 Reshape op."""
     cls._prepare(node, inputs, onnx_reshape)
     return onnx_reshape
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/shape.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/where.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Shape operator."""
+"""Define ONNX Where operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('Shape')
-class Shape(handler.Handler):
-  """Implementation of the ONNX Shape operator."""
+@handler.register_op("Where")
+class Where(handler.Handler):
+  """Implementation of the ONNX Where operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,38 +53,29 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_1(
+  def version_9(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_1 Shape op."""
-    cls._prepare(node, inputs, onnx_shape)
-    return onnx_shape
+    """ONNX version_9 Where op."""
+    cls._prepare(node, inputs, onnx_where)
+    return onnx_where
 
   @classmethod
-  def version_15(
+  def version_16(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_15 Shape op."""
-    cls._prepare(node, inputs, onnx_shape)
-    return onnx_shape
-
-  @classmethod
-  def version_19(
-      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
-  ) -> Callable[..., Any]:
-    """ONNX version_19 Shape op."""
-    cls._prepare(node, inputs, onnx_shape)
-    return onnx_shape
+    """ONNX version_16 Where op."""
+    cls._prepare(node, inputs, onnx_where)
+    return onnx_where
 
 
-@functools.partial(jit, static_argnames=('start', 'end'))
-def onnx_shape(*input_args, start=None, end=None):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Shape."""
-  assert len(input_args) == 1
-  x = input_args[0]
-  dims = x.shape[start:end]
-  return jnp.asarray(dims)
+@functools.partial(jit, static_argnames=())
+def onnx_where(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Where for more details."""
+  assert len(input_args) == 3
+  cond, x, y = input_args
+  return jnp.where(cond, x, y)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sigmoid.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/acos.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,44 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# Copyright 2023 The Jaxonnxruntime Authors.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-"""Define ONNX Sigmoid operator."""
+"""Define ONNX Acos operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
-import jax
 from jax import jit
+from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Sigmoid")
-class Sigmoid(handler.Handler):
-  """Implementation of the ONNX Sigmoid operator."""
+@handler.register_op("Acos")
+class Acos(handler.Handler):
+  """Implementation of the ONNX Acos operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -53,20 +40,21 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_13(
+  def version_7(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Sigmoid op."""
-    cls._prepare(node, inputs, onnx_sigmoid)
-    return onnx_sigmoid
+    """ONNX version_7 Acos op."""
+    cls._prepare(node, inputs, onnx_acos)
+    return onnx_acos
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_sigmoid(*input_args):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sigmoid for more details."""
+def onnx_acos(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Acos for more details."""
   assert len(input_args) == 1
-  return jax.nn.sigmoid(input_args[0])
+  data = input_args[0]
+  return jnp.arccos(data)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/slice.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/mul.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,75 +21,75 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Slice operator."""
+"""Define ONNX Mul operator."""
 from collections.abc import Callable, Sequence
 import functools
+import inspect
 from typing import Any
+
 from jax import jit
+from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('Slice')
-class Slice(handler.Handler):
-  """Implementation of the ONNX Slice operator."""
+@handler.register_op("Mul")
+class Mul(handler.Handler):
+  """Implementation of the ONNX Mul operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    node.attrs_dict['starts'] = tuple(inputs[1].tolist())
-    node.attrs_dict['ends'] = tuple(inputs[2].tolist())
-    if len(inputs) >= 4:
-      node.attrs_dict['axes'] = tuple(inputs[3].tolist())
-    else:
-      node.attrs_dict['axes'] = None
-    if len(inputs) >= 5:
-      node.attrs_dict['steps'] = tuple(inputs[4].tolist())
-    else:
-      node.attrs_dict['steps'] = None
+    sig = inspect.signature(onnx_jax_impl)
+    kwparams = [
+        param.name
+        for param in sig.parameters.values()
+        if param.kind == inspect.Parameter.KEYWORD_ONLY
+    ]
+    for name in kwparams:
+      node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_10(
+  def version_6(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_10 Slice op."""
-    cls._prepare(node, inputs, onnx_slice)
-    return onnx_slice
+    """ONNX version_6 Mul op."""
+    cls._prepare(node, inputs, onnx_mul)
+    return onnx_mul
 
   @classmethod
-  def version_11(
+  def version_7(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_11 Slice op."""
-    cls._prepare(node, inputs, onnx_slice)
-    return onnx_slice
+    """ONNX version_7 Mul op."""
+    cls._prepare(node, inputs, onnx_mul)
+    return onnx_mul
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Slice op."""
-    cls._prepare(node, inputs, onnx_slice)
-    return onnx_slice
-
-
-@functools.partial(jit, static_argnames=('starts', 'ends', 'axes', 'steps'))
-def onnx_slice(*input_args, starts, ends, axes, steps):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Slice."""
-  x = input_args[0]
-  if axes is None:
-    axes = tuple(range(len(starts)))
-  if steps is None:
-    steps = [1] * len(starts)
-  slices = tuple(
-      slice(start, end, step) for start, end, step in zip(starts, ends, steps)
-  )
-  sub_indx = [slice(None)] * len(x.shape)
-  for i, axis in enumerate(axes):
-    sub_indx[axis] = slices[i]
-  return x[tuple(sub_indx)]
+    """ONNX version_13 Mul op."""
+    cls._prepare(node, inputs, onnx_mul)
+    return onnx_mul
+
+  @classmethod
+  def version_14(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_14 Mul op."""
+    cls._prepare(node, inputs, onnx_mul)
+    return onnx_mul
+
+
+@functools.partial(jit, static_argnames=())
+def onnx_mul(*input_args):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Mul."""
+  assert len(input_args) == 2
+  a, b = input_args
+  return jnp.multiply(a, b)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/softmax.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/softmax.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/split.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/div.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,86 +21,80 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Split operator."""
+"""Define ONNX Div operator."""
 from collections.abc import Callable, Sequence
 import functools
+import inspect
 from typing import Any
 
 from jax import jit
-from jax import lax
+from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('Split')
-class Split(handler.Handler):
-  """Implementation of the ONNX Split operator."""
+@handler.register_op("Div")
+class Div(handler.Handler):
+  """Implementation of the ONNX Div operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    node.attrs_dict['axis'] = (
-        0 if 'axis' not in node.attrs else node.attrs['axis']
-    )
-    node.attrs_dict['num_output'] = node.len_outputs
-    if len(inputs) >= 2:
-      node.attrs_dict['split'] = tuple(inputs[1].tolist())
+    sig = inspect.signature(onnx_jax_impl)
+    kwparams = [
+        param.name
+        for param in sig.parameters.values()
+        if param.kind == inspect.Parameter.KEYWORD_ONLY
+    ]
+    for name in kwparams:
+      node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_2(
+  def version_6(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_2 Split op."""
-    cls._prepare(node, inputs, onnx_split)
-    return onnx_split
+    """ONNX version_7 Div op."""
+    cls._prepare(node, inputs, onnx_div)
+    return onnx_div
 
   @classmethod
-  def version_11(
+  def version_7(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_11 Split op."""
-    cls._prepare(node, inputs, onnx_split)
-    return onnx_split
+    """ONNX version_7 Div op."""
+    cls._prepare(node, inputs, onnx_div)
+    return onnx_div
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Split op."""
-    cls._prepare(node, inputs, onnx_split)
-    return onnx_split
+    """ONNX version_13 Div op."""
+    cls._prepare(node, inputs, onnx_div)
+    return onnx_div
 
   @classmethod
-  def version_18(
+  def version_14(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_18 Split op."""
-    cls._prepare(node, inputs, onnx_split)
-    return onnx_split
-
-
-@functools.partial(jit, static_argnames=('split', 'axis', 'num_output'))
-def onnx_split(*input_args, num_output, split=None, axis=0):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Split for more details."""
-
-  x = input_args[0]
-  if split is None:
-    split = [x.shape[axis] // num_output] * num_output
-  starts = []
-  ends = []
-  starts.append([0] * x.ndim)
-  for idx in range(1, num_output):
-    st = [0] * x.ndim
-    st[axis] = sum(split[:idx])
-    starts.append(st)
-    en = list(x.shape)
-    en[axis] = sum(split[:idx])
-    ends.append(en)
-  ends.append(list(x.shape))
+    """ONNX version_14 Div op."""
+    cls._prepare(node, inputs, onnx_div)
+    return onnx_div
 
-  return [lax.slice(x, start, end) for start, end in zip(starts, ends)]
+
+@functools.partial(jit, static_argnames=())
+def onnx_div(*input_args):
+  """The internal jax impl for onnx Div op."""
+  assert len(input_args) == 2
+  x, y = input_args
+  if jnp.issubdtype(x.dtype, jnp.integer) and jnp.issubdtype(
+      y.dtype, jnp.integer
+  ):
+    return jnp.floor_divide(x, y)
+  else:
+    return jnp.true_divide(x, y)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sqrt.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/log.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,42 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# Copyright 2023 The Jaxonnxruntime Authors.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-"""Define ONNX Sqrt operator."""
+"""Define ONNX Log operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Sqrt")
-class Sqrt(handler.Handler):
-  """Implementation of the ONNX Sqrt operator."""
+@handler.register_op("Log")
+class Log(handler.Handler):
+  """Implementation of the ONNX Log operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,28 +40,21 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_6(
-      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
-  ) -> Callable[..., Any]:
-    """ONNX version_6 Sqrt op."""
-    cls._prepare(node, inputs, onnx_sqrt)
-    return onnx_sqrt
-
-  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Sqrt op."""
-    cls._prepare(node, inputs, onnx_sqrt)
-    return onnx_sqrt
+    """ONNX version_13 Log op."""
+    cls._prepare(node, inputs, onnx_log)
+    return onnx_log
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_sqrt(*input_args):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sqrt."""
+def onnx_log(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Log for more details."""
   assert len(input_args) == 1
-  return jnp.sqrt(*input_args)
+  data = input_args[0]
+  return jnp.log(data)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/squeeze.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/squeeze.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sub.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/cos.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,42 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# Copyright 2023 The Jaxonnxruntime Authors.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-"""Define ONNX Sub operator."""
+"""Define ONNX Cos operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Sub")
-class Sub(handler.Handler):
-  """Implementation of the ONNX Sub operator."""
+@handler.register_op("Cos")
+class Cos(handler.Handler):
+  """Implementation of the ONNX Cos operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -54,34 +43,18 @@
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
   def version_7(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_7 Sub op."""
-    cls._prepare(node, inputs, onnx_sub)
-    return onnx_sub
-
-  @classmethod
-  def version_13(
-      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
-  ) -> Callable[..., Any]:
-    """ONNX version_13 Sub op."""
-    cls._prepare(node, inputs, onnx_sub)
-    return onnx_sub
-
-  @classmethod
-  def version_14(
-      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
-  ) -> Callable[..., Any]:
-    """ONNX version_14 Sub op."""
-    cls._prepare(node, inputs, onnx_sub)
-    return onnx_sub
+    """ONNX version_7 Cos op."""
+    cls._prepare(node, inputs, onnx_cos)
+    return onnx_cos
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_sub(*input_args):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sub."""
-  assert len(input_args) == 2
-  a, b = input_args
-  return jnp.subtract(a, b)
+def onnx_cos(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Cos for more details."""
+  assert len(input_args) == 1
+  data = input_args[0]
+  return jnp.cos(data)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sum.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/acosh.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,44 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# Copyright 2023 The Jaxonnxruntime Authors.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-"""Define ONNX Sum operator."""
+"""Define ONNX Acosh operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Sum")
-class Sum(handler.Handler):
-  """Implementation of the ONNX Sum operator."""
+@handler.register_op("Acosh")
+class Acosh(handler.Handler):
+  """Implementation of the ONNX Acosh operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -53,27 +40,21 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_8(
-      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
-  ) -> Callable[..., Any]:
-    """ONNX version_8 Sum op."""
-    cls._prepare(node, inputs, onnx_sum)
-    return onnx_sum
-
-  @classmethod
-  def version_13(
+  def version_9(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Sum op."""
-    cls._prepare(node, inputs, onnx_sum)
-    return onnx_sum
+    """ONNX version_9 Acosh op."""
+    cls._prepare(node, inputs, onnx_acosh)
+    return onnx_acosh
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_sum(*input_args):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sum for more details."""
-  return jnp.sum(jnp.array(input_args), axis=0)
+def onnx_acosh(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Acosh for more details."""
+  assert len(input_args) == 1
+  data = input_args[0]
+  return jnp.arccosh(data)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/tanh.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/sin.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,42 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# Copyright 2023 The Jaxonnxruntime Authors.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-"""Define ONNX Tanh operator."""
+"""Define ONNX Sin operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Tanh")
-class Tanh(handler.Handler):
-  """Implementation of the ONNX Tanh operator."""
+@handler.register_op("Sin")
+class Sin(handler.Handler):
+  """Implementation of the ONNX Sin operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,29 +40,21 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_6(
-      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
-  ) -> Callable[..., Any]:
-    """ONNX version_6 Tanh op."""
-    cls._prepare(node, inputs, onnx_tanh)
-    return onnx_tanh
-
-  @classmethod
-  def version_13(
+  def version_7(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Tanh op."""
-    cls._prepare(node, inputs, onnx_tanh)
-    return onnx_tanh
+    """ONNX version_7 Sin op."""
+    cls._prepare(node, inputs, onnx_sin)
+    return onnx_sin
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_tanh(*input_args):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Tanh."""
+def onnx_sin(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sin for more details."""
   assert len(input_args) == 1
-  x = input_args[0]
-  return jnp.tanh(x)
+  data = input_args[0]
+  return jnp.sin(data)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/transpose.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/pow.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Transpose operator."""
+"""Define ONNX Pow operator."""
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Transpose")
-class Transpose(handler.Handler):
-  """Implementation of the ONNX Transpose operator."""
+@handler.register_op("Pow")
+class Pow(handler.Handler):
+  """Implementation of the ONNX Pow operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,29 +51,43 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_1(
+  def version_7(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_1 Transpose op."""
-    cls._prepare(node, inputs, onnx_transpose)
-    return onnx_transpose
+    """ONNX version_7 Pow op."""
+    cls._prepare(node, inputs, onnx_pow)
+    return onnx_pow
+
+  @classmethod
+  def version_12(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_12 Pow op."""
+    cls._prepare(node, inputs, onnx_pow)
+    return onnx_pow
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Transpose op."""
-    cls._prepare(node, inputs, onnx_transpose)
-    return onnx_transpose
+    """ONNX version_13 Pow op."""
+    cls._prepare(node, inputs, onnx_pow)
+    return onnx_pow
+
+  @classmethod
+  def version_15(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_15 Pow op."""
+    cls._prepare(node, inputs, onnx_pow)
+    return onnx_pow
 
 
-@functools.partial(jit, static_argnames="perm")
-def onnx_transpose(*input_args, perm):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Transpose."""
-  assert len(input_args) == 1
-  x = input_args[0]
-  return jnp.transpose(x, perm)
+@functools.partial(jit, static_argnames=())
+def onnx_pow(a, b):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Pow."""
+  return jnp.power(a, b).astype(a.dtype)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/unsqueeze.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/unsqueeze.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/where.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/onnx_ops/cosh.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,44 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# Copyright 2023 The Jaxonnxruntime Authors.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-"""Define ONNX Where operator."""
+"""Define ONNX Cosh operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Where")
-class Where(handler.Handler):
-  """Implementation of the ONNX Where operator."""
+@handler.register_op("Cosh")
+class Cosh(handler.Handler):
+  """Implementation of the ONNX Cosh operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -53,21 +40,21 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_16(
+  def version_9(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_16 Where op."""
-    cls._prepare(node, inputs, onnx_where)
-    return onnx_where
+    """ONNX version_9 Cosh op."""
+    cls._prepare(node, inputs, onnx_cosh)
+    return onnx_cosh
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_where(*input_args):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Where for more details."""
-  assert len(input_args) == 3
-  cond, x, y = input_args
-  return jnp.where(cond, x, y)
+def onnx_cosh(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Cosh for more details."""
+  assert len(input_args) == 1
+  data = input_args[0]
+  return jnp.cosh(data)
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/runner.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,14 @@
 from jaxonnxruntime.backend import Backend
 import numpy as np
 
 import onnx
 from onnx import numpy_helper
 
 
-jax.config.update('jax_enable_x64', True)
-jax.config.update('jax_numpy_rank_promotion', 'warn')
-
-
 class TestItem:
 
   def __init__(
       self,
       func: Callable[..., Any],
       proto: list[Optional[Union[onnx.ModelProto, onnx.NodeProto]]],
   ) -> None:
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime/version.py` & `jaxonnxruntime-0.2.0/jaxonnxruntime/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Current jaxonnxruntime version at head on Github."""
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/PKG-INFO` & `jaxonnxruntime-0.2.0/jaxonnxruntime.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxonnxruntime
-Version: 0.1.0
+Version: 0.2.0
 Summary: Jaxonnxruntime: JAX based ONNX Runtime.
 Author-email: Jaxonnxruntime team <jaxonnxruntime-dev@google.com>
 Project-URL: homepage, https://github.com/google/jaxonnxruntime
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -31,12 +31,20 @@
 
 - We follow most of the interface definitions by `onnx.backend` [here](https://onnx.ai/onnx/api/backend.html).
 
 - Please check a brief example on model conversion and forward calling in [`examples/imagenet/imagenet_main.py`](https://github.com/google/jaxonnxruntime/blob/main/examples/imagenet/imagenet_main.py).
 
 ## Contributions and Discussions
 
+We believe that collaboration is the key to building remarkable software, and we wholeheartedly welcome contributions from developers like you.
+You can make a real impact and help shape the future of our project with contributions such as
+[implementing new operators](https://github.com/google/jaxonnxruntime/blob/main/docs/adding_a_new_op.rst) and increasing support for more ML models.
+
+Our contributors will have a chance to earn [Google Open Source Peer Bonus](https://opensource.google/documentation/reference/growing/peer-bonus), so that your valuable contributions won't go unnoticed.
+Your hard work will be rewarded both by the community and by Google.
+Together, let's create an amazing library and foster a supportive environment for open-source enthusiasts.
+
 Thank you for taking the time to contribute! Please see [the contribution guidelines](https://github.com/google/jaxonnxruntime/blob/main/contributing.md).
 
 ## License
 
 This project is licensed under the [Apache License](https://github.com/google/jaxonnxruntime/blob/main/LICENSE).
```

### Comparing `jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/SOURCES.txt` & `jaxonnxruntime-0.2.0/jaxonnxruntime.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,97 +1,130 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 contributing.md
 pylintrc
 pyproject.toml
+.github/ISSUE_TEMPLATE/feature_request.yml
 .github/workflows/build.yml
 .github/workflows/pythonpublish.yml
+docs/adding_a_new_op.rst
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 docs/_static/css/jaxonnxruntime_theme.css
 docs/examples/jaxonnxruntime-python-api.py
 examples/imagenet/imagenet_main.py
 jaxonnxruntime/__init__.py
 jaxonnxruntime/backend.py
 jaxonnxruntime/call_onnx.py
-jaxonnxruntime/config.py
+jaxonnxruntime/config_class.py
 jaxonnxruntime/runner.py
 jaxonnxruntime/version.py
 jaxonnxruntime.egg-info/PKG-INFO
 jaxonnxruntime.egg-info/SOURCES.txt
 jaxonnxruntime.egg-info/dependency_links.txt
 jaxonnxruntime.egg-info/requires.txt
 jaxonnxruntime.egg-info/top_level.txt
 jaxonnxruntime/core/__init__.py
 jaxonnxruntime/core/handler.py
 jaxonnxruntime/core/onnx_graph.py
 jaxonnxruntime/core/onnx_node.py
 jaxonnxruntime/core/onnx_utils.py
+jaxonnxruntime/experimental/custom_ops/__init__.py
+jaxonnxruntime/experimental/custom_ops/zeros_like.py
+jaxonnxruntime/experimental/custom_ops/zeros_like_test.py
 jaxonnxruntime/onnx_ops/__init__.py
 jaxonnxruntime/onnx_ops/abs.py
+jaxonnxruntime/onnx_ops/acos.py
+jaxonnxruntime/onnx_ops/acosh.py
 jaxonnxruntime/onnx_ops/add.py
+jaxonnxruntime/onnx_ops/and_op.py
+jaxonnxruntime/onnx_ops/argmax.py
+jaxonnxruntime/onnx_ops/argmin.py
+jaxonnxruntime/onnx_ops/asin.py
+jaxonnxruntime/onnx_ops/asinh.py
+jaxonnxruntime/onnx_ops/atan.py
+jaxonnxruntime/onnx_ops/atanh.py
 jaxonnxruntime/onnx_ops/averagepool.py
 jaxonnxruntime/onnx_ops/batchnormalization.py
+jaxonnxruntime/onnx_ops/bitshift.py
 jaxonnxruntime/onnx_ops/cast.py
+jaxonnxruntime/onnx_ops/castlike.py
 jaxonnxruntime/onnx_ops/ceil.py
+jaxonnxruntime/onnx_ops/clip.py
 jaxonnxruntime/onnx_ops/concat.py
 jaxonnxruntime/onnx_ops/constant.py
 jaxonnxruntime/onnx_ops/constantofshape.py
 jaxonnxruntime/onnx_ops/conv.py
+jaxonnxruntime/onnx_ops/cos.py
+jaxonnxruntime/onnx_ops/cosh.py
 jaxonnxruntime/onnx_ops/div.py
 jaxonnxruntime/onnx_ops/dropout.py
+jaxonnxruntime/onnx_ops/einsum.py
 jaxonnxruntime/onnx_ops/equal.py
+jaxonnxruntime/onnx_ops/erf.py
 jaxonnxruntime/onnx_ops/exp.py
 jaxonnxruntime/onnx_ops/expand.py
 jaxonnxruntime/onnx_ops/flatten.py
 jaxonnxruntime/onnx_ops/gather.py
+jaxonnxruntime/onnx_ops/gatherelements.py
 jaxonnxruntime/onnx_ops/gemm.py
 jaxonnxruntime/onnx_ops/globalaveragepool.py
 jaxonnxruntime/onnx_ops/identity.py
 jaxonnxruntime/onnx_ops/if_op.py
 jaxonnxruntime/onnx_ops/leakyrelu.py
 jaxonnxruntime/onnx_ops/less.py
 jaxonnxruntime/onnx_ops/lessorequal.py
+jaxonnxruntime/onnx_ops/log.py
+jaxonnxruntime/onnx_ops/logsoftmax.py
 jaxonnxruntime/onnx_ops/lrn.py
 jaxonnxruntime/onnx_ops/matmul.py
 jaxonnxruntime/onnx_ops/max.py
 jaxonnxruntime/onnx_ops/maxpool.py
+jaxonnxruntime/onnx_ops/min.py
 jaxonnxruntime/onnx_ops/mul.py
 jaxonnxruntime/onnx_ops/neg.py
 jaxonnxruntime/onnx_ops/nonzero.py
 jaxonnxruntime/onnx_ops/onehot.py
 jaxonnxruntime/onnx_ops/or_op.py
 jaxonnxruntime/onnx_ops/pad.py
 jaxonnxruntime/onnx_ops/pow.py
+jaxonnxruntime/onnx_ops/prelu.py
 jaxonnxruntime/onnx_ops/range.py
 jaxonnxruntime/onnx_ops/reciprocal.py
 jaxonnxruntime/onnx_ops/reducemax.py
 jaxonnxruntime/onnx_ops/reducemean.py
 jaxonnxruntime/onnx_ops/reducesum.py
 jaxonnxruntime/onnx_ops/relu.py
 jaxonnxruntime/onnx_ops/reshape.py
+jaxonnxruntime/onnx_ops/selu.py
 jaxonnxruntime/onnx_ops/shape.py
 jaxonnxruntime/onnx_ops/sigmoid.py
+jaxonnxruntime/onnx_ops/sin.py
+jaxonnxruntime/onnx_ops/sinh.py
 jaxonnxruntime/onnx_ops/slice.py
 jaxonnxruntime/onnx_ops/softmax.py
+jaxonnxruntime/onnx_ops/softplus.py
 jaxonnxruntime/onnx_ops/split.py
 jaxonnxruntime/onnx_ops/sqrt.py
 jaxonnxruntime/onnx_ops/squeeze.py
 jaxonnxruntime/onnx_ops/sub.py
 jaxonnxruntime/onnx_ops/sum.py
 jaxonnxruntime/onnx_ops/tanh.py
+jaxonnxruntime/onnx_ops/topk.py
 jaxonnxruntime/onnx_ops/transpose.py
+jaxonnxruntime/onnx_ops/trilu.py
 jaxonnxruntime/onnx_ops/unsqueeze.py
 jaxonnxruntime/onnx_ops/where.py
 tests/call_onnx_test.py
 tests/onnx_ops_test.py
 tests/run_all_tests.sh
 tests/core/handler_test.py
 tests/core/onnx_graph_test.py
 tests/core/onnx_node_test.py
+tests/core/onnx_utils_test.py
 tests/onnx_ops/dropout_test.py
 tests/onnx_ops/onehot_test.py
 tools/analyze_model.py
 tools/op_code_generator.py
```

### Comparing `jaxonnxruntime-0.1.0/pylintrc` & `jaxonnxruntime-0.2.0/pylintrc`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/pyproject.toml` & `jaxonnxruntime-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/tests/call_onnx_test.py` & `jaxonnxruntime-0.2.0/tests/call_onnx_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from absl.testing import absltest
+import jax
 from jaxonnxruntime import call_onnx
+from jaxonnxruntime import config_class
 import numpy as np
 
 import onnx
 
 ValueInfoProto = onnx.ValueInfoProto
 TypeProto = onnx.TypeProto
 GraphProto = onnx.GraphProto
@@ -67,10 +69,19 @@
     )
     model_proto = ModelProto(graph=graph_def, producer_name='onnx-example')
     jax_func, model_params = call_onnx.call_onnx_model(model_proto, [x])
     results = jax_func(model_params, [x])
     expect = [np.array([2.0, 1.0, 3.0], dtype=np.float32)]
     np.testing.assert_array_equal(results, expect)
 
+    with config_class.jaxort_experimental_support_abtract_input_shape(True):
+      x = np.array([-2.0, -8.0, 3.0], dtype=np.float32)
+      jax_func, model_params = call_onnx.call_onnx_model(
+          model_proto, [jax.ShapeDtypeStruct(x.shape, x.dtype)]
+      )
+      results = jax_func(model_params, [x])
+      expect = [np.array([2.0, 8.0, 3.0], dtype=np.float32)]
+      np.testing.assert_array_equal(results, expect)
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `jaxonnxruntime-0.1.0/tests/core/handler_test.py` & `jaxonnxruntime-0.2.0/tests/core/handler_test.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/tests/core/onnx_graph_test.py` & `jaxonnxruntime-0.2.0/tests/core/onnx_graph_test.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/tests/core/onnx_node_test.py` & `jaxonnxruntime-0.2.0/tests/core/onnx_node_test.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/tests/onnx_ops/dropout_test.py` & `jaxonnxruntime-0.2.0/tests/onnx_ops/dropout_test.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/tests/onnx_ops/onehot_test.py` & `jaxonnxruntime-0.2.0/tests/onnx_ops/onehot_test.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/tests/onnx_ops_test.py` & `jaxonnxruntime-0.2.0/tests/onnx_ops_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,25 +14,30 @@
 
 """ONNX node test."""
 
 import collections
 from typing import Any
 
 from absl.testing import absltest
+import jax
 from jaxonnxruntime import config
 from jaxonnxruntime import runner
 from jaxonnxruntime.backend import Backend as JaxBackend  # pylint: disable=g-importing-member
 
 
+jax.config.update('jax_enable_x64', True)
+jax.config.update('jax_numpy_rank_promotion', 'warn')
 config.update('jaxort_only_allow_initializers_as_static_args', False)
 
 
 class Runner(runner.Runner):
 
-  def __init__(self, backend: JaxBackend, parent_module: Any = None) -> None:
+  def __init__(
+      self, backend: type(JaxBackend), parent_module: Any = None
+  ) -> None:
     self.backend = backend
     self._parent_module = parent_module
     self._include_patterns = set()  # type: ignore[var-annotated]
     self._exclude_patterns = set()  # type: ignore[var-annotated]
     self._xfail_patterns = set()  # type: ignore[var-annotated]
     self._test_items = collections.defaultdict(dict)  # type: ignore[var-annotated]
 
@@ -55,74 +60,124 @@
 
 backend_test = Runner(JaxBackend, __name__)
 expect_fail_patterns = []
 include_patterns = []
 exclude_patterns = []
 
 include_patterns.append('test_abs_')
+include_patterns.append('test_acos_')
+include_patterns.append('test_acosh_')
 include_patterns.append('test_add_')
+include_patterns.append('test_and_')
+include_patterns.append('test_argmax_')
+include_patterns.append('test_argmin_')
+include_patterns.append('test_asin_')
+include_patterns.append('test_asinh_')
+include_patterns.append('test_atan_')
+include_patterns.append('test_atanh_')
 include_patterns.append('test_averagepool_')
 include_patterns.append('test_batchnormalization_')
+include_patterns.append('test_bitshift_')
 include_patterns.append('test_cast_')
+include_patterns.append('test_castlike_')
 include_patterns.append('test_ceil_')
+include_patterns.append('test_clip_')
 include_patterns.append('test_concat_')
 include_patterns.append('test_constant_')
 include_patterns.append('test_constantofshape_')
 include_patterns.append('test_conv_')
+include_patterns.append('test_cos_')
+include_patterns.append('test_cosh_')
 include_patterns.append('test_div_')
 include_patterns.append('test_dropout_')
+include_patterns.append('test_einsum_')
 include_patterns.append('test_equal_')
+include_patterns.append('test_erf_')
 include_patterns.append('test_exp_')
 include_patterns.append('test_expand_')
 include_patterns.append('test_flatten_')
 include_patterns.append('test_gather_')
+include_patterns.append('test_gather_elements_')
 include_patterns.append('test_gemm_')
 include_patterns.append('test_globalaveragepool_')
 include_patterns.append('test_identity_')
 include_patterns.append('test_if_')
 include_patterns.append('test_leakyrelu_')
 include_patterns.append('test_less_')
 include_patterns.append('test_lessorequal_')
+include_patterns.append('test_log_')
+include_patterns.append('test_logsoftmax_')
 include_patterns.append('test_lrn_')
 include_patterns.append('test_matmul_')
 include_patterns.append('test_max_')
 include_patterns.append('test_maxpool_')
+include_patterns.append('test_min_')
 include_patterns.append('test_mul_')
 include_patterns.append('test_neg_')
 include_patterns.append('test_onehot_')
 include_patterns.append('test_or_')
 include_patterns.append('test_pow_')
+include_patterns.append('test_prelu_')
 include_patterns.append('test_range_')
 include_patterns.append('test_reciprocal_')
 include_patterns.append('test_reduce_max_')
 include_patterns.append('test_reduce_mean_')
 include_patterns.append('test_reduce_sum_')
 include_patterns.append('test_relu_')
 include_patterns.append('test_reshape_')
+include_patterns.append('test_selu_')
 include_patterns.append('test_shape_')
 include_patterns.append('test_sigmoid_')
+include_patterns.append('test_sin_')
+include_patterns.append('test_sinh_')
 include_patterns.append('test_slice_')
 include_patterns.append('test_softmax_')
+include_patterns.append('test_softplus_')
 include_patterns.append('test_split_')
 include_patterns.append('test_sqrt_')
 include_patterns.append('test_sub_')
 include_patterns.append('test_sum_')
 include_patterns.append('test_squeeze_')
 include_patterns.append('test_tanh_')
+include_patterns.append('test_top_k_')
 include_patterns.append('test_transpose_')
+include_patterns.append('test_tri')
 include_patterns.append('test_unsqueeze_')
 include_patterns.append('test_where_')
 
 
 # TODO(johnqiangzhang): should modify onnx.numpy_helper.to_array to support load
 # bfloat16.
 exclude_patterns.append('test_cast_FLOAT_to_BFLOAT16')
+exclude_patterns.append('test_castlike_FLOAT_to_BFLOAT16')
 # Not implement yet
-exclude_patterns.append('test_gather_elements_')
-exclude_patterns.append('test_reduce_sum_square_')
+exclude_patterns.append('test_gather_elements_')  # Op GatherElements
+exclude_patterns.append('test_reduce_sum_square_')  # Op ReduceSumSquare
+exclude_patterns.append('test_leakyrelu_default_expanded_cpu')  # Op CastLike
+exclude_patterns.append('test_leakyrelu_example_expanded_cpu')  # Op CastLlike
+exclude_patterns.append('test_leakyrelu_expanded_cpu')  # Op CastLike
+exclude_patterns.append('test_relu_expanded_ver18_cpu')  # Op CastLike
+exclude_patterns.append('test_split_to_sequence_1_cpu')  # Op SplitToSequence
+exclude_patterns.append('test_split_to_sequence_2_cpu')  # Op SplitToSequence
+exclude_patterns.append(
+    'test_split_to_sequence_nokeepdims_cpu'
+)  # Op SplitToSequence
+# Clip: In ONNX's def, the Clip op's input `min` and `max` are optional.
+# The input name list would be ['data', 'min', 'max'].
+# In the test cases below, when `min` is not given, its name is set to
+# be an empty string. But this is not compatible with jaxonnxruntime,
+# as we don't handle placeholder as input names if the actual input data is
+# missing. There will be a mismatch between the length of input name list and
+# input data list. Therefore, we only include test cases with all three inputs,
+# and with the first two inputs. Test cases with input name list
+# ['data', '', 'max'] are excluded.
+exclude_patterns.append('test_clip_default_inbounds_')
+exclude_patterns.append('test_clip_default_int8_inbounds_')
+exclude_patterns.append('test_clip_default_int8_max_')
+exclude_patterns.append('test_clip_default_max_')
 # Need more debug
 exclude_patterns.append('test_softmax_axis_0_expanded_cpu')
 exclude_patterns.append('test_softmax_axis_1_expanded_cpu')
 exclude_patterns.append('test_softmax_axis_2_expanded_cpu')
 exclude_patterns.append('test_softmax_default_axis_expanded_cpu')
 exclude_patterns.append('test_softmax_large_number_expanded_cpu')
 exclude_patterns.append('test_softmax_negative_axis_expanded_cpu')
@@ -156,14 +211,35 @@
     'test_cast_no_saturate_FLOAT16_to_FLOAT8E4M3FN_cpu',
     'test_cast_no_saturate_FLOAT16_to_FLOAT8E5M2FNUZ_cpu',
     'test_cast_no_saturate_FLOAT16_to_FLOAT8E5M2_cpu',
     'test_cast_no_saturate_FLOAT_to_FLOAT8E4M3FNUZ_cpu',
     'test_cast_no_saturate_FLOAT_to_FLOAT8E4M3FN_cpu',
     'test_cast_no_saturate_FLOAT_to_FLOAT8E5M2FNUZ_cpu',
     'test_cast_no_saturate_FLOAT_to_FLOAT8E5M2_cpu',
+    # castlike
+    'test_castlike_FLOAT_to_STRING',
+    'test_castlike_STRING_to_FLOAT',
+    'test_castlike_FLOAT16_to_FLOAT8E4M3FNUZ_',
+    'test_castlike_FLOAT16_to_FLOAT8E4M3FNUZ_',
+    'test_castlike_FLOAT16_to_FLOAT8E4M3FN_',
+    'test_castlike_FLOAT16_to_FLOAT8E5M2FNUZ_',
+    'test_castlike_FLOAT16_to_FLOAT8E5M2_',
+    'test_castlike_FLOAT_to_FLOAT8E4M3FNUZ_',
+    'test_castlike_FLOAT_to_FLOAT8E4M3FN_',
+    'test_castlike_FLOAT_to_FLOAT8E5M2FNUZ_',
+    'test_castlike_FLOAT_to_FLOAT8E5M2_',
+    'test_castlike_no_saturate_FLOAT16_to_FLOAT8E4M3FNUZ_',
+    'test_castlike_no_saturate_FLOAT16_to_FLOAT8E4M3FN_',
+    'test_castlike_no_saturate_FLOAT16_to_FLOAT8E5M2FNUZ_',
+    'test_castlike_no_saturate_FLOAT16_to_FLOAT8E5M2_',
+    'test_castlike_no_saturate_FLOAT_to_FLOAT8E4M3FNUZ_',
+    'test_castlike_no_saturate_FLOAT_to_FLOAT8E4M3FN_',
+    'test_castlike_no_saturate_FLOAT_to_FLOAT8E5M2FNUZ_',
+    'test_castlike_no_saturate_FLOAT_to_FLOAT8E5M2_',
+    'test_castlike_.*_expanded_',
     # others
     'test_maxpool_2d_ceil_',
     'test_averagepool_2d_ceil_',
     'test_averagepool_2d_dilations_',
     'test_nonzero_',
     # np.object is not valid type for jax.array
     'test_equal_string_',
```

### Comparing `jaxonnxruntime-0.1.0/tests/run_all_tests.sh` & `jaxonnxruntime-0.2.0/tests/run_all_tests.sh`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 case $flag in
   --with-cov)
   PYTEST_OPTS+="--cov=jaxonnxruntime --cov-report=xml --cov-report=term --cov-config=pyproject.toml"
   ;;
   --help)
   echo "Usage:"
   echo "  --with-cov: Also generate pytest coverage."
+  echo "  --no-doctest: disable doctest pytest."
+  echo "  --no-pytest: disable pytest."
+  echo "  --no-mypy: disable mypy check."
+  echo "  --use-venv: use python virtual env."
+
   exit
   ;;
   --no-doctest)
   RUN_DOCTEST=false
   ;;
   --no-pytest)
   RUN_PYTEST=false
@@ -73,15 +78,15 @@
 if $RUN_DOCTEST; then
   echo "=== RUNNING DOCTESTS ==="
   # test doctest
   sphinx-build -M doctest docs docs/_build -T
   # test build html
   sphinx-build -M html docs docs/_build -T
   # test docstrings
-  pytest -n auto jaxonnxruntime --doctest-modules --suppress-no-test-exit-code
+  pytest -n auto jaxonnxruntime --doctest-modules --suppress-no-test-exit-code --ignore=jaxonnxruntime/experimental/ --ignore=jaxonnxruntime/examples
 fi
 
 # check that jaxonnxruntime is running on editable mode
 # (i.e. no notebook installed jaxonnxruntime from pypi)
 echo "=== CHECKING JAXONNXRUNTIME IS EDITABLE ==="
 assert_error="jaxonnxruntime is not running on editable mode."
 (cd docs; python -c "import jaxonnxruntime; assert 'site-packages' not in jaxonnxruntime.__file__, \"$assert_error\"";cd -)
```

### Comparing `jaxonnxruntime-0.1.0/tools/analyze_model.py` & `jaxonnxruntime-0.2.0/tools/analyze_model.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.1.0/tools/op_code_generator.py` & `jaxonnxruntime-0.2.0/tools/op_code_generator.py`

 * *Files 23% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 import functools
 import inspect
 from collections.abc import Callable, Sequence
 from typing import Any
 
-from jax import jit
+import jax
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
 @handler.register_op("{op_name}")
 class {op_name}(handler.Handler):
@@ -68,67 +68,108 @@
     \"\"\"ONNX version_{version} {op_name} op.\"\"\"
     cls._prepare(node, inputs, onnx_{op_name_lower})
     return onnx_{op_name_lower}
 """
 
 template_tail = """
 
-@functools.partial(jit, static_argnames=())
+@functools.partial(jax.jit, static_argnames=())
 def onnx_{op_name_lower}(*input_args):
   \"\"\"https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#{op_name} for more details.\"\"\"
   # TODO({username}): add the implementation here.
-  # Then update the onnx_ops_teset.py to include it,
-  # `include_patterns.append('test_{op_name_lower}_')`.
   return input_args
 """
 
-root_dir = os.path.dirname(os.path.realpath(onnx_ops.__file__))
-op_schema_set = {
-    str(op_schema.name) for op_schema in onnx.defs.get_all_schemas()
-}
+onnx_ops_root_dir = os.path.dirname(os.path.realpath(onnx_ops.__file__))
+
+
+def get_schema_dict():
+  res_dict = {}
+  for schema in onnx.defs.get_all_schemas_with_history():
+    if schema.name not in res_dict:
+      res_dict[schema.name] = []
+    res_dict[schema.name].append(schema)
+  return res_dict
 
 
 def update_onnx_ops_init_file(op_name):
   """Update onnx_ops/__init_.py with the created op."""
-  init_py_file = os.path.join(root_dir, '__init__.py')
+  init_py_file = os.path.join(onnx_ops_root_dir, '__init__.py')
   with open(init_py_file, 'r') as f:
     existing_imports = f.read()
 
   new_import = f'from . import {op_name.lower()} as {op_name.lower()}'
   if new_import in existing_imports:
     logging.info('Already have %s in onnx_ops/__init__.py.', op_name)
     return
 
   # Split the existing imports.
   initial_imports = existing_imports.split('from . import ')[0]
   onnx_op_imports = existing_imports[len(initial_imports) :]
 
   # Add the new import statement.
-  onnx_op_imports += f'\nfrom . import {op_name.lower()}'
+  onnx_op_imports += new_import
 
   # Replace and sort the ONNX op imports.
   pattern = r'from \. import .*'
   sorted_imports = sorted(re.findall(pattern, onnx_op_imports))
   sorted_imports_str = '\n'.join(sorted_imports)
 
   # Write the sorted import statements to the file
   with open(init_py_file, 'w') as f:
     f.write(initial_imports + sorted_imports_str)
     f.write('\n')
 
 
+def update_onnx_ops_test_file(op_name):
+  """enable those tests under test/onnx_ops_test.py with the created op."""
+  py_file = os.path.join(
+      os.path.realpath(onnx_ops_root_dir), '../tests/onnx_ops_test.py'
+  )
+  with open(py_file, 'r') as f:
+    source_code = f.read()
+
+  lines = source_code.splitlines()
+  start, end = None, None
+  include_patterns_lines = []
+  for i, line in enumerate(lines):
+    if 'include_patterns.append' in line:
+      include_patterns_lines.append(line)
+      if not start:
+        start = i
+      end = i + 1
+  logging.info('start = %s ,end = %s', start, end)
+  if f'test_{op_name.lower()}_' not in include_patterns_lines:
+    include_patterns_lines.append(
+        f"include_patterns.append('test_{op_name.lower()}_')"
+    )
+  else:
+    logging.info('Already have test %s in onnx_models_test.py.', op_name)
+    return
+
+  include_patterns_lines = sorted(include_patterns_lines)
+
+  modified_code = '\n'.join(
+      lines[0:start] + include_patterns_lines + lines[end:]
+  )
+
+  with open(py_file, 'w') as f:
+    f.write(modified_code)
+
+
 def main(args):
   # get the version list for the ONNX operator
   op_name = args.op_name
-  if str(op_name) not in op_schema_set:
+  op_schema_dict = get_schema_dict()
+  if str(op_name) not in op_schema_dict:
     raise ValueError(
-        f'ONNX {op_name} is not ONNX op list {sorted(op_schema_set)}?.'
+        f'ONNX {op_name} is not ONNX op list {sorted(op_schema_dict.keys())}?.'
     )
-  schema = onnx.defs.get_schema(op_name)
-  versions = [schema.since_version] if schema else []
+  schemas = op_schema_dict[str(op_name)]
+  versions = [schema.since_version for schema in schemas]
   username = os.environ['USER']
 
   # Render the template and create new op file under onnx_ops folder.
   code = template_head.format(
       op_name=op_name, op_name_lower=op_name.lower(), username=username
   )
   for version in versions:
@@ -137,19 +178,25 @@
     )
   code += template_tail.format(
       op_name_lower=op_name.lower(),
       op_name=op_name,
       username=username,
   )
   logging.info('Genereate new code=\n%s', code)
-  op_def_path = os.path.join(root_dir, f'{op_name.lower()}.py')
-  with open(op_def_path, 'w') as f:
-    f.write(code)
+  op_def_path = os.path.join(onnx_ops_root_dir, f'{op_name.lower()}.py')
+  if os.path.exists(op_def_path):
+    logging.error(
+        'file %s already exists. Please delete it first.', op_def_path
+    )
+  else:
+    with open(op_def_path, 'w') as f:
+      f.write(code)
 
   # Update the onnx_ops/__init__.py by adding this new op.
   update_onnx_ops_init_file(op_name)
+  update_onnx_ops_test_file(op_name)
 
 
 if __name__ == '__main__':
   parser = argparse.ArgumentParser(description='Generate ONNX op Python code.')
   parser.add_argument('op_name', type=str, help='name of the ONNX op')
   main(parser.parse_args())
```

