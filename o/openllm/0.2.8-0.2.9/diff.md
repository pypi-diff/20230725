# Comparing `tmp/openllm-0.2.8.tar.gz` & `tmp/openllm-0.2.9.tar.gz`

## Comparing `openllm-0.2.8.tar` & `openllm-0.2.9.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.8/.gitattributes
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 openllm-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.8/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0    14307 2020-02-02 00:00:00.000000 openllm-0.2.8/CHANGELOG.md
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.8/CITATION.cff
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.8/DEVELOPMENT.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.8/nightly-requirements-gpu.txt
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.8/nightly-requirements.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.8/package.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.8/pyoxidizer.bzl
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.8/taplo.toml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/__about__.py
--rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/__main__.py
--rw-r--r--   0        0        0    90120 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_configuration.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_generation.py
--rw-r--r--   0        0        0    69548 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_llm.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_prompt.py
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_quantisation.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_schema.py
--rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_service.py
--rw-r--r--   0        0        0    19111 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_strategies.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_types.py
--rw-r--r--   0        0        0    89468 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/cli.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/client.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/py.typed
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/testing.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0    12608 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/bundle/oci/Dockerfile-builder
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/bundle/oci/Dockerfile-vllm
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/bundle/oci/__init__.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0    10520 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/modeling_vllm_auto.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/baichuan/__init__.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/baichuan/configuration_baichuan.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/baichuan/modeling_baichuan.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/gpt_neox/configuration_gpt_neox.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/gpt_neox/modeling_gpt_neox.py
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/llama/configuration_llama.py
--rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/llama/modeling_llama.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/llama/modeling_vllm_llama.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/mpt/__init__.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/mpt/configuration_mpt.py
--rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/mpt/modeling_mpt.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/opt/__init__.py
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/opt/configuration_opt.py
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/opt/modeling_flax_opt.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/opt/modeling_opt.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/opt/modeling_tf_opt.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/opt/modeling_vllm_opt.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/__init__.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/_meta.yml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/falcon_tuned.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/features.py
--rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/llama2_qlora.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/opt_tuned.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/serialisation/ggml.py
--rw-r--r--   0        0        0    15916 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/serialisation/transformers.py
--rw-r--r--   0        0        0    16946 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    19722 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_pt_and_triton_objects.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_vllm_objects.py
--rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/representation.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0    13366 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/client_test.py
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/configuration_test.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models_test.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/package_test.py
--rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/strategies_test.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/__init__.py
--rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/conftest.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/flan_t5_test.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/opt_test.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.8/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.8/LICENSE.md
--rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.8/README.md
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 openllm-0.2.8/hatch.toml
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 openllm-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    30106 2020-02-02 00:00:00.000000 openllm-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.9/.gitattributes
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 openllm-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.9/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0    14392 2020-02-02 00:00:00.000000 openllm-0.2.9/CHANGELOG.md
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.9/CITATION.cff
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.9/DEVELOPMENT.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.9/nightly-requirements-gpu.txt
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.9/nightly-requirements.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.9/package.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.9/pyoxidizer.bzl
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.9/taplo.toml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/__about__.py
+-rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/__main__.py
+-rw-r--r--   0        0        0    90120 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/_configuration.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/_generation.py
+-rw-r--r--   0        0        0    69548 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/_llm.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/_schema.py
+-rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/_service.py
+-rw-r--r--   0        0        0    19111 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/_types.py
+-rw-r--r--   0        0        0    88106 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/cli.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/client.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/py.typed
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/testing.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0    12608 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/bundle/oci/Dockerfile-builder
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/bundle/oci/Dockerfile-vllm
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/bundle/oci/__init__.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0    10520 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/auto/modeling_vllm_auto.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/baichuan/__init__.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/baichuan/configuration_baichuan.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/baichuan/modeling_baichuan.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/gpt_neox/configuration_gpt_neox.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/gpt_neox/modeling_gpt_neox.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/llama/configuration_llama.py
+-rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/llama/modeling_llama.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/llama/modeling_vllm_llama.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/mpt/__init__.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/mpt/configuration_mpt.py
+-rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/mpt/modeling_mpt.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/opt/__init__.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/opt/configuration_opt.py
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/opt/modeling_flax_opt.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/opt/modeling_opt.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/opt/modeling_tf_opt.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/opt/modeling_vllm_opt.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/playground/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/playground/__init__.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/playground/_meta.yml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/playground/falcon_tuned.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/playground/features.py
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/playground/llama2_qlora.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/playground/opt_tuned.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/serialisation/ggml.py
+-rw-r--r--   0        0        0    15916 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/serialisation/transformers.py
+-rw-r--r--   0        0        0    16946 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    19722 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/dummy_pt_and_triton_objects.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/dummy_vllm_objects.py
+-rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm/utils/representation.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0    13366 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.9/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/client_test.py
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/configuration_test.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/conftest.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/models_test.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/package_test.py
+-rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/strategies_test.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/models/__init__.py
+-rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/models/conftest.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/models/flan_t5_test.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/models/opt_test.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.9/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.9/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.9/LICENSE.md
+-rw-r--r--   0        0        0    24883 2020-02-02 00:00:00.000000 openllm-0.2.9/README.md
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 openllm-0.2.9/hatch.toml
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 openllm-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    30309 2020-02-02 00:00:00.000000 openllm-0.2.9/PKG-INFO
```

### Comparing `openllm-0.2.8/.pre-commit-config.yaml` & `openllm-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/ADDING_NEW_MODEL.md` & `openllm-0.2.9/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/CHANGELOG.md` & `openllm-0.2.9/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.2.9](https://github.com/bentoml/openllm/tree/v0.2.9)
+No significant changes.
+
+
 ## [0.2.8](https://github.com/bentoml/openllm/tree/v0.2.8)
 
 ### Features
 
 - APIs for LLMService are now provisional based on the capabilities of the LLM.
 
   The following APIs are considered provisional:
```

### Comparing `openllm-0.2.8/CITATION.cff` & `openllm-0.2.9/CITATION.cff`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/DEVELOPMENT.md` & `openllm-0.2.9/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/nightly-requirements.txt` & `openllm-0.2.9/nightly-requirements.txt`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/package.json` & `openllm-0.2.9/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.2.9'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.2.8",
+    "version": "0.2.9",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.2.8/pyoxidizer.bzl` & `openllm-0.2.9/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/__about__.py` & `openllm-0.2.9/src/openllm/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.2.8"
+__version__ = "0.2.9"
```

### Comparing `openllm-0.2.8/src/openllm/__init__.py` & `openllm-0.2.9/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/__main__.py` & `openllm-0.2.9/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/_configuration.py` & `openllm-0.2.9/src/openllm/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/_generation.py` & `openllm-0.2.9/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/_llm.py` & `openllm-0.2.9/src/openllm/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/_prompt.py` & `openllm-0.2.9/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/_quantisation.py` & `openllm-0.2.9/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/_schema.py` & `openllm-0.2.9/src/openllm/_schema.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/_service.py` & `openllm-0.2.9/src/openllm/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/_strategies.py` & `openllm-0.2.9/src/openllm/_strategies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/_types.py` & `openllm-0.2.9/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/cli.py` & `openllm-0.2.9/src/openllm/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,82 +149,65 @@
  ╚═════╝ ╚═╝     ╚══════╝╚═╝  ╚═══╝╚══════╝╚══════╝╚═╝     ╚═╝
 """
 
 
 _AnyCallable = t.Callable[..., t.Any]
 FC = t.TypeVar("FC", bound=t.Union[_AnyCallable, click.Command])
 
-
-def parse_device_callback(
-    ctx: click.Context, param: click.Parameter, value: tuple[tuple[str], ...] | None
-) -> TupleStr | None:
-    if value is None:
-        return value
-
-    if not LazyType(TupleStr).isinstance(value):
-        ctx.fail(f"{param} only accept multiple values, not {type(value)} (value: {value})")
-
+def parse_device_callback(ctx: click.Context, param: click.Parameter, value: tuple[tuple[str], ...] | None) -> TupleStr | None:
+    if value is None: return value
+    if not LazyType(TupleStr).isinstance(value): ctx.fail(f"{param} only accept multiple values, not {type(value)} (value: {value})")
     el: TupleStr = tuple(i for k in value for i in k)
-
     # NOTE: --device all is a special case
-    if len(el) == 1 and el[0] == "all":
-        return tuple(map(str, available_devices()))
-
+    if len(el) == 1 and el[0] == "all": return tuple(map(str, available_devices()))
     return el
 
-
 def _echo(text: t.Any, fg: str = "green", _with_style: bool = True, **attrs: t.Any) -> None:
     call = click.echo
     if _with_style:
         attrs["fg"] = fg if not get_debug_mode() else None
         call = click.secho
     call(text, **attrs)
 
-
 def output_option(f: _AnyCallable, *, factory: t.Any = click) -> t.Callable[[FC], FC]:
     return factory.option(
         "-o",
         "--output",
         "output",
         type=click.Choice(["json", "pretty", "porcelain"]),
         default="pretty",
         help="Showing output type.",
         show_default=True,
         envvar="OPENLLM_OUTPUT",
         show_envvar=True,
     )(f)
 
-
 def machine_option(factory: t.Any) -> t.Callable[[FC], FC]:
     return factory.option("--machine", is_flag=True, default=False, hidden=True)
 
-
 def model_id_option(factory: t.Any, model_env: EnvVarMixin | None = None) -> t.Callable[[FC], FC]:
     envvar = None
-    if model_env is not None:
-        envvar = model_env.model_id
+    if model_env is not None: envvar = model_env.model_id
     return factory.option(
         "--model-id",
         type=click.STRING,
         default=None,
         help="Optional model_id name or path for (fine-tune) weight.",
         envvar=envvar,
         show_envvar=True if envvar is not None else False,
     )
 
-
 def model_version_option(factory: t.Any) -> t.Callable[[FC], FC]:
     return factory.option(
         "--model-version",
         type=click.STRING,
         default=None,
         help="Optional model version to save for this model. It will be inferred automatically from model-id.",
     )
 
-
 def workers_per_resource_callback(ctx: click.Context, param: click.Parameter, value: str | None) -> str | None:
     if value is None: return value
     value = inflection.underscore(value)
     if value in {"round_robin", "conserved"}: return value
     else:
         try: float(value)  # type: ignore[arg-type]
         except ValueError: ctx.fail(f"'workers_per_resource' only accept '{_wpr_strategies}' as possible strategies, otherwise pass in float.")
@@ -237,48 +220,41 @@
 
     **Note**: ``--workers-per-resource`` will also accept the following strategies:
 
     - ``round_robin``: Similar behaviour when setting ``--workers-per-resource 1``. This is useful for smaller models.
 
     - ``conserved``: This will determine the number of available GPU resources, and only assign one worker for the LLMRunner. For example, if ther are 4 GPUs available, then ``conserved`` is equivalent to ``--workers-per-resource 0.25``.
     """
-    if build:
-        help_str += """\n
+    if build: help_str += """\n
     **Note**: The workers value passed into 'build' will determine how the LLM can
     be provisioned in Kubernetes as well as in standalone container. This will
     ensure it has the same effect with 'openllm start --workers ...'"""
     return factory.option("--workers-per-resource", default=None, help=help_str, callback=workers_per_resource_callback, type=str, required=False)
 
 
 def quantize_option(factory: t.Any, build: bool = False, model_env: EnvVarMixin | None = None) -> t.Callable[[FC], FC]:
     envvar = None
-    if model_env is not None:
-        envvar = model_env.quantize
-    help_str = (
-        "Running this model in quantized mode." if not build else "Set quantization mode for serving in deployment."
-    )
+    if model_env is not None: envvar = model_env.quantize
+    help_str = "Running this model in quantized mode." if not build else "Set quantization mode for serving in deployment."
     help_str += "\nNOTE: Quantization is only available for PyTorch models. "
     return factory.option(
         "--quantise",
         "--quantize",
         "quantize",
         type=click.Choice(["int8", "int4", "gptq"]),
         default=None,
         help=help_str,
         envvar=envvar,
         show_envvar=True if envvar is not None else False,
     )
 
 
-def bettertransformer_option(
-    factory: t.Any, build: bool = False, model_env: EnvVarMixin | None = None
-) -> t.Callable[[FC], FC]:
+def bettertransformer_option(factory: t.Any, build: bool = False, model_env: EnvVarMixin | None = None) -> t.Callable[[FC], FC]:
     envvar = None
-    if model_env is not None:
-        envvar = model_env.bettertransformer
+    if model_env is not None: envvar = model_env.bettertransformer
     return factory.option(
         "--bettertransformer",
         is_flag=True,
         default=None,
         help="Apply FasterTransformer wrapper to serve model. This will applies during serving time."
         if not build
         else "Set defaul environment variable whether to serve this model with FasterTransformer in build time.",
@@ -296,47 +272,36 @@
         default="safetensors",
         help="Serialisation format to save the model in. Default is safetensors, which is similar to `safe_serialization=True`. If the weight is not yet supported my safetensors, make sure to pass in '--serialisation legacy'",
         show_default=True,
         show_envvar=True,
         envvar="OPENLLM_SERIALIZATION",
     )
 
-
 _adapter_mapping_key = "adapter_map"
 def _id_callback(ctx: click.Context, _: click.Parameter, value: tuple[str, ...] | None) -> None:
-    if not value:
-        return None
-    if _adapter_mapping_key not in ctx.params:
-        ctx.params[_adapter_mapping_key] = {}
+    if not value: return None
+    if _adapter_mapping_key not in ctx.params: ctx.params[_adapter_mapping_key] = {}
     for v in value:
         adapter_id, *adapter_name = v.rsplit(":", maxsplit=1)
-        try:
-            # try to resolve the full path if users pass in relative,
-            # currently only support one level of resolve path.
-            adapter_id = resolve_user_filepath(adapter_id, os.getcwd())
-        except FileNotFoundError:
-            pass
+        # try to resolve the full path if users pass in relative,
+        # currently only support one level of resolve path with current directory
+        try: adapter_id = resolve_user_filepath(adapter_id, os.getcwd())
+        except FileNotFoundError: pass
         ctx.params[_adapter_mapping_key][adapter_id] = adapter_name[0] if len(adapter_name) > 0 else None
     return None
 
-
 @attr.define
 class CliContext:
     cloud_context: str | None = attr.field(default=None, converter=attr.converters.default_if_none("default"))
     def with_options(self, **attrs: t.Any) -> t.Self: return attr.evolve(self, **attrs)
 
-
 class OpenLLMCommandGroup(BentoMLCommandGroup):
     NUMBER_OF_COMMON_PARAMS = 5  # parameters in common_params + 1 faked group option header
     @staticmethod
     def common_params(f: FC) -> t.Callable[[FC], FC]:
-        """This is not supposed to be used with unprocessed click function.
-
-        This should be used a the last currying from common_params -> usage_tracking -> exception_handling.
-        """
         # The following logics is similar to one of BentoMLCommandGroup
 
         from bentoml._internal.configuration import DEBUG_ENV_VAR
         from bentoml._internal.configuration import QUIET_ENV_VAR
 
         @cog.optgroup.group("Global options")
         @cog.optgroup.option("-q", "--quiet", envvar=QUIET_ENV_VAR, is_flag=True, default=False, help="Suppress all output.")
@@ -350,28 +315,21 @@
             if quiet:
                 set_quiet_mode(True)
                 if debug: logger.warning("'--quiet' passed; ignoring '--verbose/--debug'")
             elif debug: set_debug_mode(True)
             configure_logging()
             return f(*args, **attrs)
         return wrapper
-
     @staticmethod
     def usage_tracking(func: _AnyCallable, group: click.Group, **attrs: t.Any) -> _AnyCallable:
-        """This is not supposed to be used with unprocessed click function.
-
-        This should be used a the last currying from common_params -> usage_tracking -> exception_handling.
-        """
         command_name = attrs.get("name", func.__name__)
-
         @functools.wraps(func)
         def wrapper(do_not_track: bool, *args: P.args, **attrs: P.kwargs) -> t.Any:
             if do_not_track:
                 with analytics.set_bentoml_tracking(): return func(*args, **attrs)
-
             start_time = time.time_ns()
             with analytics.set_bentoml_tracking():
                 assert group.name is not None, "group.name should not be None"
                 event = analytics.OpenllmCliEvent(cmd_group=group.name, cmd_name=command_name)
                 try:
                     return_value = func(*args, **attrs)
                     duration_in_ms = (time.time_ns() - start_time) / 1e6
@@ -381,58 +339,47 @@
                 except Exception as e:
                     duration_in_ms = (time.time_ns() - start_time) / 1e6
                     event.duration_in_ms = duration_in_ms
                     event.error_type = type(e).__name__
                     event.return_code = 2 if isinstance(e, KeyboardInterrupt) else 1
                     analytics.track(event)
                     raise
-
         return wrapper
-
     @staticmethod
     def exception_handling(func: _AnyCallable, group: click.Group, **attrs: t.Any) -> ClickFunctionWrapper[..., t.Any]:
-        """This is not supposed to be used with unprocessed click function.
-
-        This should be used a the last currying from common_params -> usage_tracking -> exception_handling.
-        """
         command_name = attrs.get("name", func.__name__)
-
         @functools.wraps(func)
         def wrapper(*args: P.args, **attrs: P.kwargs) -> t.Any:
             try: return func(*args, **attrs)
             except OpenLLMException as err:
                 raise click.ClickException(click.style(f"[{group.name}] '{command_name}' failed: " + err.message, fg="red")) from err
             except KeyboardInterrupt: pass
         return t.cast("ClickFunctionWrapper[..., t.Any]", wrapper)
-
     def get_command(self, ctx: click.Context, cmd_name: str) -> click.Command | None:
         cmd_name = self.resolve_alias(cmd_name)
         _mapping = {"start": _cached_http, "start-grpc": _cached_grpc}
         if ctx.command.name in _mapping:
             try: return _mapping[ctx.command.name][cmd_name]
             except KeyError:
                 # TODO: support start from a bento
                 try:
                     bentoml.get(cmd_name)
                     raise click.ClickException(f"'openllm start {cmd_name}' is currently disabled for the time being. Please let us know if you need this feature by opening an issue on GitHub.")
                 except bentoml.exceptions.NotFound: pass
                 raise click.BadArgumentUsage(f"{cmd_name} is not a valid model identifier supported by OpenLLM.") from None
         return super().get_command(ctx, cmd_name)
-
     def list_commands(self, ctx: click.Context) -> list[str]:
         if ctx.command.name in {"start", "start-grpc"}: return list(openllm.CONFIG_MAPPING.keys())
         return super().list_commands(ctx)
-
     @override
     def command(self, *args: t.Any, **attrs: t.Any):
         """Override the default 'cli.command' with supports for aliases for given command, and it wraps the implementation with common parameters."""
         if "context_settings" not in attrs: attrs["context_settings"] = {}
         if "max_content_width" not in attrs["context_settings"]: attrs["context_settings"]["max_content_width"] = 120
         aliases = attrs.pop("aliases", None)
-
         def wrapper(f: _AnyCallable) -> click.Command:
             name = f.__name__.lower()
             if name.endswith("_command"): name = name[:-8]
             name = name.replace("_", "-")
             attrs.setdefault("help", inspect.getdoc(f))
             attrs.setdefault("name", name)
 
@@ -451,15 +398,14 @@
             if aliases is not None:
                 assert cmd.name
                 self._commands[cmd.name] = aliases
                 self._aliases.update({alias: cmd.name for alias in aliases})
             return cmd
         return wrapper
 
-
 @click.group(cls=OpenLLMCommandGroup, context_settings=_CONTEXT_SETTINGS, name="openllm")
 @click.version_option(__version__, "--version", "-v")
 def cli() -> None:
     """\b
      ██████╗ ██████╗ ███████╗███╗   ██╗██╗     ██╗     ███╗   ███╗
     ██╔═══██╗██╔══██╗██╔════╝████╗  ██║██║     ██║     ████╗ ████║
     ██║   ██║██████╔╝█████╗  ██╔██╗ ██║██║     ██║     ██╔████╔██║
@@ -468,43 +414,39 @@
      ╚═════╝ ╚═╝     ╚══════╝╚═╝  ╚═══╝╚══════╝╚══════╝╚═╝     ╚═╝.
 
     \b
     An open platform for operating large language models in production.
     Fine-tune, serve, deploy, and monitor any LLMs with ease.
     """  # noqa: D205
 
-
 @cli.group(cls=OpenLLMCommandGroup, context_settings=_CONTEXT_SETTINGS, name="start", aliases=["start-http"])
 def start_command() -> None:
     """Start any LLM as a REST server.
 
     \b
     ```bash
     $ openllm <start|start-http> <model_name> --<options> ...
     ```
     """
 
-
 @cli.group(cls=OpenLLMCommandGroup, context_settings=_CONTEXT_SETTINGS, name="start-grpc")
 def start_grpc_command() -> None:
     """Start any LLM as a gRPC server.
 
     \b
     ```bash
     $ openllm start-grpc <model_name> --<options> ...
     ```
     """
 
-
 # NOTE: A list of bentoml option that is not needed for parsing.
 # NOTE: User shouldn't set '--working-dir', as OpenLLM will setup this.
 # NOTE: production is also deprecated
 _IGNORED_OPTIONS = {"working_dir", "production", "protocol_version"}
 
-
 def parse_serve_args(serve_grpc: bool) -> t.Callable[[t.Callable[..., openllm.LLMConfig]], t.Callable[[FC], FC]]:
     """Parsing `bentoml serve|serve-grpc` click.Option to be parsed via `openllm start`."""
     from bentoml_cli.cli import cli
 
     command = "serve" if not serve_grpc else "serve-grpc"
     group = cog.optgroup.group(
         f"Start a {'HTTP' if not serve_grpc else 'gRPC'} server options",
@@ -525,18 +467,15 @@
             # type can be determine from default value
             attrs.pop("type")
             param_decls = (*attrs.pop("opts"), *attrs.pop("secondary_opts"))
             f = cog.optgroup.option(*param_decls, **attrs)(f)
         return group(f)
     return decorator
 
-
-_http_server_args = parse_serve_args(False)
-_grpc_server_args = parse_serve_args(True)
-
+_http_server_args, _grpc_server_args = parse_serve_args(False), parse_serve_args(True)
 
 def start_decorator(llm_config: openllm.LLMConfig, serve_grpc: bool = False) -> t.Callable[[_AnyCallable], t.Callable[[FC], FC]]:
     opts = [
         llm_config.to_click_options,
         _http_server_args if not serve_grpc else _grpc_server_args,
         cog.optgroup.group("General LLM Options", help="The following options are related to running the LLM Server."),
         model_id_option(cog.optgroup, model_env=llm_config["env"]),
@@ -562,15 +501,14 @@
     - safetensors: Using safetensors instead of pickling (safetensors required) [default]
 
     - legacy: using default torch load behaviour.
 
     The following are currently being worked on:
 
     - DeepSpeed Inference: [link](https://www.deepspeed.ai/inference/)
-
       """,
         ),
         cog.optgroup.option("--device", type=dantic.CUDA, multiple=True, envvar="CUDA_VISIBLE_DEVICES", callback=parse_device_callback, help=f"Assign GPU devices (if available) for {llm_config['model_name']}.", show_envvar=True),
         cog.optgroup.option("--runtime", type=click.Choice(["ggml", "transformers"]), default="transformers", help="The runtime to use for the given model. Default is transformers."),
         quantize_option(cog.optgroup, model_env=llm_config["env"]),
         bettertransformer_option(cog.optgroup, model_env=llm_config["env"]),
         serialisation_option(cog.optgroup),
@@ -591,23 +529,19 @@
 
     ```
     """,
         ),
         cog.optgroup.option("--adapter-id", default=None, help="Optional name or path for given LoRA adapter" + f" to wrap '{llm_config['model_name']}'", multiple=True, callback=_id_callback, metavar="[PATH | [remote/][adapter_name:]adapter_id][, ...]"),
         click.option("--return-process", is_flag=True, default=False, help="Internal use only.", hidden=True),
     ]
-
     def decorator(f: _AnyCallable) -> _AnyCallable:
-        for opt in reversed(opts):
-            f = opt(f)
+        for opt in reversed(opts): f = opt(f)
         return f
-
     return decorator
 
-
 def parse_config_options(
     config: openllm.LLMConfig,
     server_timeout: int,
     workers_per_resource: float,
     device: tuple[str, ...] | None,
     environ: DictStrAny,
 ) -> DictStrAny:
@@ -616,15 +550,14 @@
     if device:
         if len(device) > 1: _bentoml_config_options_opts.extend([f'runners."llm-{config["start_name"]}-runner".resources."nvidia.com/gpu"[{idx}]={dev}' for idx, dev in enumerate(device)])
         else: _bentoml_config_options_opts.append(f'runners."llm-{config["start_name"]}-runner".resources."nvidia.com/gpu"=[{device[0]}]')
     _bentoml_config_options_env += " " if _bentoml_config_options_env else "" + " ".join(_bentoml_config_options_opts)
     environ["BENTOML_CONFIG_OPTIONS"] = _bentoml_config_options_env
     return environ
 
-
 _wpr_strategies = {"round_robin", "conserved"}
 
 def start_command_factory(model: str, _context_settings: DictStrAny | None = None, _serve_grpc: bool = False) -> click.Command:
     """Generate a 'click.Command' for any given LLM.
 
     Args:
         model: The name of the model or the ``bentoml.Bento`` instance.
@@ -685,51 +618,50 @@
         runtime: t.Literal["ggml", "transformers"],
         fast: bool,
         serialisation_format: t.Literal["safetensors", "legacy"],
         adapter_id: str | None,
         return_process: bool,
         **attrs: t.Any,
     ) -> openllm.LLMConfig | subprocess.Popen[bytes]:
-        if serialisation_format == "safetensors" and quantize is not None:
-            if os.getenv("OPENLLM_SERIALIZATION_WARNING", str(True)).upper() in ENV_VARS_TRUE_VALUES:
-                _echo(
-                    f"'--quantize={quantize}' might not work with 'safetensors' serialisation format. Use with caution!. To silence this warning, set \"OPENLLM_SERIALIZATION_WARNING=False\"\nNote: You can always fallback to '--serialisation legacy' when running quantisation.",
-                    fg="yellow",
-                )
+        if serialisation_format == "safetensors" and quantize is not None and os.getenv("OPENLLM_SERIALIZATION_WARNING", str(True)).upper() in ENV_VARS_TRUE_VALUES:
+            _echo(f"'--quantize={quantize}' might not work with 'safetensors' serialisation format. Use with caution!. To silence this warning, set \"OPENLLM_SERIALIZATION_WARNING=False\"\nNote: You can always fallback to '--serialisation legacy' when running quantisation.", fg="yellow")
         adapter_map: dict[str, str | None] | None = attrs.pop(_adapter_mapping_key, None)
         config, server_attrs = llm_config.model_validate_click(**attrs)
         server_timeout = first_not_none(server_timeout, default=config["timeout"])
-
         server_attrs.update({"working_dir": os.path.dirname(__file__), "timeout": server_timeout})
         if _serve_grpc: server_attrs["grpc_protocol_version"] = "v1"
         # NOTE: currently, theres no development args in bentoml.Server. To be fixed upstream.
         development = server_attrs.pop("development")
         server_attrs.setdefault("production", not development)
         wpr: t.Any = first_not_none(workers_per_resource, default=config["workers_per_resource"])
 
         if isinstance(wpr, str):
             if wpr == "round_robin": wpr = 1.0
             elif wpr == "conserved":
-                available_gpu = device if device else available_devices()
-                wpr = 1.0 if len(available_gpu) == 0 else float(1 / len(available_gpu))
+                if device and device_count() == 0:
+                    _echo("--device will have no effect as there is no GPUs available", fg="yellow")
+                    wpr = 1.0
+                else:
+                    available_gpu = len(device) if device else device_count()
+                    wpr = 1.0 if available_gpu == 0 else float(1 / available_gpu)
             else: wpr = float(wpr)
 
         # Create a new model env to work with the envvar during CLI invocation
         env = EnvVarMixin(config["model_name"], config.default_implementation(), model_id=model_id, bettertransformer=bettertransformer, quantize=quantize, runtime=runtime)
         prerequisite_check(ctx, config, quantize, adapter_map, int(1 / wpr))
 
         # NOTE: This is to set current configuration
         start_env = os.environ.copy()
         start_env = parse_config_options(config, server_timeout, wpr, device, start_env)
         if fast and not get_quiet_mode(): _echo(f"Fast mode is enabled. Make sure the model is available in local store before 'start': 'openllm import {model}{'--model-id ' + model_id if model_id else ''}'", fg="yellow")
 
         start_env.update(
             {
                 "OPENLLM_MODEL": model,
-                "BENTOML_DEBUG": str(not get_quiet_mode()),
+                "BENTOML_DEBUG": str(get_debug_mode()),
                 "BENTOML_HOME": os.getenv("BENTOML_HOME", BentoMLContainer.bentoml_home.get()),
                 "OPENLLM_ADAPTER_MAP": orjson.dumps(adapter_map).decode(),
                 "OPENLLM_SERIALIZATION": serialisation_format,
                 env.model_id: env.model_id_value,
                 env.runtime: env.runtime_value,
                 env.framework: env.framework_value,
             }
@@ -773,98 +705,59 @@
             else: next_step(model, adapter_map)
 
         # NOTE: Return the configuration for telemetry purposes.
         return config
 
     return start_cmd
 
-
 def noop_command(llm_config: openllm.LLMConfig, _serve_grpc: bool, **command_attrs: t.Any) -> click.Command:
     context_settings = command_attrs.pop("context_settings", {})
     context_settings.update({"ignore_unknown_options": True, "allow_extra_args": True})
     command_attrs["context_settings"] = context_settings
     group = start_command if not _serve_grpc else start_grpc_command
     # NOTE: The model requires GPU, therefore we will return a dummy command
     @group.command(**command_attrs)
     def noop(**_: t.Any) -> openllm.LLMConfig:
         _echo("No GPU available, therefore this command is disabled", fg="red")
         analytics.track_start_init(llm_config)
         return llm_config
-
     return noop
 
-
-def prerequisite_check(
-    ctx: click.Context,
-    llm_config: openllm.LLMConfig,
-    quantize: t.LiteralString | None,
-    adapter_map: dict[str, str | None] | None,
-    num_workers: int,
-) -> None:
+def prerequisite_check(ctx: click.Context, llm_config: openllm.LLMConfig, quantize: t.LiteralString | None, adapter_map: dict[str, str | None] | None, num_workers: int) -> None:
     if quantize:
         if device_count() < 1:
             _echo("Quantization requires at least 1 GPU (got None)", fg="red")
             ctx.exit(1)
+        if llm_config.default_implementation() == "vllm":
+            _echo("Quantization is not yet supported with vLLM", fg="red")
+            ctx.exit(1)
 
     if adapter_map and not is_peft_available():
-        _echo(
-            "Using adapter requires 'peft' to be available. Make sure to install with 'pip install \"openllm[fine-tune]\"'",
-            fg="red",
-        )
+        _echo("Using adapter requires 'peft' to be available. Make sure to install with 'pip install \"openllm[fine-tune]\"'", fg="red")
         ctx.exit(1)
 
     requirements = llm_config["requirements"]
     if requirements is not None and len(requirements) > 0:
         missing_requirements = [i for i in requirements if importlib.util.find_spec(inflection.underscore(i)) is None]
-        if len(missing_requirements) > 0:
-            _echo(
-                f"Make sure to have the following dependencies available: {missing_requirements}",
-                fg="yellow",
-            )
-
-    if num_workers > 1 and device_count() < num_workers:
-        raise click.BadOptionUsage(
-            "workers_per_resource",
-            f"# of workers is infered to {num_workers} GPUs per runner worker, while there are only"
-            f"'{device_count()}' for inference. (Tip: Try again using '--workers-per-resource={1/device_count()}')",
-            ctx=ctx,
-        )
+        if len(missing_requirements) > 0: _echo(f"Make sure to have the following dependencies available: {missing_requirements}", fg="yellow")
 
+    if num_workers > 1 and device_count() < num_workers: raise click.BadOptionUsage("workers_per_resource", f"# of workers is infered to {num_workers} GPUs per runner worker, while there are only '{device_count()}' for inference. (Tip: Try again using '--workers-per-resource={1/device_count()}')", ctx=ctx)
 
 @cli.command(name="import", aliases=["download"])
-@click.argument(
-    "model",
-    type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]),
-)
-@click.argument(
-    "model_id",
-    type=click.STRING,
-    default=None,
-    metavar="Optional[REMOTE_REPO/MODEL_ID | /path/to/local/model]",
-    required=False,
-)
+@click.argument("model", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]))
+@click.argument("model_id", type=click.STRING, default=None, metavar="Optional[REMOTE_REPO/MODEL_ID | /path/to/local/model]", required=False)
 @click.argument("converter", envvar="CONVERTER", type=click.STRING, default=None, required=False, metavar=None)
 @model_version_option(click)
-@click.option(
-    "--runtime",
-    type=click.Choice(["ggml", "transformers"]),
-    default="transformers",
-    help="The runtime to use for the given model. Default is transformers.",
-)
+@click.option("--runtime", type=click.Choice(["ggml", "transformers"]), default="transformers", help="The runtime to use for the given model. Default is transformers.")
 @output_option
 @quantize_option(click)
 @machine_option(click)
-@click.option(
-    "--implementation",
-    type=click.Choice(["pt", "tf", "flax", "vllm"]),
-    default=None,
-    help="The implementation for saving this LLM.",
-)
+@click.option("--implementation", type=click.Choice(["pt", "tf", "flax", "vllm"]), default=None, help="The implementation for saving this LLM.")
 @serialisation_option(click)
-def download_models_command(
+def import_command(
     model: str,
     model_id: str | None,
     converter: str | None,
     model_version: str | None,
     output: OutputLiteral,
     runtime: t.Literal["ggml", "transformers"],
     machine: bool,
@@ -945,30 +838,27 @@
     except bentoml.exceptions.NotFound:
         if not machine and output == "pretty":
             msg = f"'{model}' does not exists in local store. Saving..."
             if model_id is not None: msg = f"'{model}' with 'model_id={model_id}' does not exists in local store. Saving..."
             _echo(msg, fg="yellow", nl=True)
         _ref = openllm.serialisation.get(llm, auto_import=True)
         if impl == "pt" and is_torch_available() and torch.cuda.is_available(): torch.cuda.empty_cache()
-    if machine:
-        # NOTE: We will prefix the tag with __tag__ and we can use regex to correctly
-        # get the tag from 'bentoml.bentos.build|build_bentofile'
-        _echo(f"__tag__:{_ref.tag}", fg="white")
+    # NOTE: We will prefix the tag with __tag__ and we can use regex to correctly
+    # get the tag from 'bentoml.bentos.build|build_bentofile'
+    if machine: _echo(f"__tag__:{_ref.tag}", fg="white")
     elif output == "pretty":
         if _previously_saved: _echo(f"{model} with 'model_id={model_id}' is already setup for framework '{impl}': {_ref.tag!s}", nl=True, fg="yellow")
         else: _echo(f"Saved model: {_ref.tag}")
     elif output == "json": _echo(orjson.dumps({"previously_setup": _previously_saved, "framework": impl, "tag": str(_ref.tag)}, option=orjson.OPT_INDENT_2).decode())
     else: _echo(_ref.tag)
     return _ref
 
-
 _cached_http = {key: start_command_factory(key, _context_settings=_CONTEXT_SETTINGS) for key in openllm.CONFIG_MAPPING}
 _cached_grpc = {key: start_command_factory(key, _context_settings=_CONTEXT_SETTINGS, _serve_grpc=True) for key in openllm.CONFIG_MAPPING}
 
-
 @overload
 def _start(
     model_name: str,
     /,
     model_id: str | None = ...,
     timeout: int = ...,
     workers_per_resource: t.Literal["conserved", "round_robin"] | float | None = ...,
@@ -1176,59 +1066,37 @@
         "--machine",
         "--runtime",
         runtime,
         "--serialisation",
         serialisation_format,
     ]
 
-    if quantize and bettertransformer:
-        raise OpenLLMException("'quantize' and 'bettertransformer' are currently mutually exclusive.")
-
-    if quantize:
-        args.extend(["--quantize", quantize])
-    if bettertransformer:
-        args.append("--bettertransformer")
-
-    if containerize and push:
-        raise OpenLLMException("'containerize' and 'push' are currently mutually exclusive.")
-    if push:
-        args.extend(["--push"])
-    if containerize:
-        args.extend(["--containerize"])
-
-    if model_id:
-        args.extend(["--model-id", model_id])
-    if build_ctx:
-        args.extend(["--build-ctx", build_ctx])
-    if enable_features:
-        args.extend([f"--enable-features={f}" for f in enable_features])
-    if workers_per_resource:
-        args.extend(["--workers-per-resource", str(workers_per_resource)])
-    if overwrite:
-        args.append("--overwrite")
-    if adapter_map:
-        args.extend([f"--adapter-id={k}{':'+v if v is not None else ''}" for k, v in adapter_map.items()])
-    if model_version:
-        args.extend(["--model-version", model_version])
-    if dockerfile_template:
-        args.extend(["--dockerfile-template", dockerfile_template])
-    if additional_args:
-        args.extend(additional_args)
+    if quantize and bettertransformer: raise OpenLLMException("'quantize' and 'bettertransformer' are currently mutually exclusive.")
+    if quantize: args.extend(["--quantize", quantize])
+    if bettertransformer: args.append("--bettertransformer")
+    if containerize and push: raise OpenLLMException("'containerize' and 'push' are currently mutually exclusive.")
+    if push: args.extend(["--push"])
+    if containerize: args.extend(["--containerize"])
+    if model_id: args.extend(["--model-id", model_id])
+    if build_ctx: args.extend(["--build-ctx", build_ctx])
+    if enable_features: args.extend([f"--enable-features={f}" for f in enable_features])
+    if workers_per_resource: args.extend(["--workers-per-resource", str(workers_per_resource)])
+    if overwrite: args.append("--overwrite")
+    if adapter_map: args.extend([f"--adapter-id={k}{':'+v if v is not None else ''}" for k, v in adapter_map.items()])
+    if model_version: args.extend(["--model-version", model_version])
+    if dockerfile_template: args.extend(["--dockerfile-template", dockerfile_template])
+    if additional_args: args.extend(additional_args)
 
-    try:
-        output = subprocess.check_output(args, env=os.environ.copy(), cwd=build_ctx or os.getcwd())
+    try: output = subprocess.check_output(args, env=os.environ.copy(), cwd=build_ctx or os.getcwd())
     except subprocess.CalledProcessError as e:
         logger.error("Exception caught while building %s", model_name, exc_info=e)
-        if e.stderr:
-            raise OpenLLMException(e.stderr.decode("utf-8")) from None
+        if e.stderr: raise OpenLLMException(e.stderr.decode("utf-8")) from None
         raise OpenLLMException(str(e)) from None
-
     return bentoml.get(_tag_parsing(output), _bento_store=bento_store)
 
-
 def _import_model(
     model_name: str,
     /,
     *,
     model_id: str | None = None,
     model_version: str | None = None,
     runtime: t.Literal["ggml", "transformers"] = "transformers",
@@ -1271,44 +1139,29 @@
         runtime,
         "--implementation",
         implementation,
         "--machine",
         "--serialisation",
         serialisation_format,
     ]
-    if model_id is not None:
-        args.append(model_id)
-    if model_version is not None:
-        args.extend(["--model-version", str(model_version)])
-    if additional_args is not None:
-        args.extend(additional_args)
-    if quantize is not None:
-        args.extend(["--quantize", quantize])
-    return download_models_command.main(args=args, standalone_mode=False)
+    if model_id is not None: args.append(model_id)
+    if model_version is not None: args.extend(["--model-version", str(model_version)])
+    if additional_args is not None: args.extend(additional_args)
+    if quantize is not None: args.extend(["--quantize", quantize])
+    return import_command.main(args=args, standalone_mode=False)
 
 
 def _list_models() -> DictStrAny:
     """List all available models within the local store."""
-    args = ["-o", "json", "--show-available", "--machine"]
-    return models_command.main(args=args, standalone_mode=False)
-
-
-start, start_grpc, build, import_model, list_models = (
-    codegen.gen_sdk(_start, _serve_grpc=False),
-    codegen.gen_sdk(_start, _serve_grpc=True),
-    codegen.gen_sdk(_build),
-    codegen.gen_sdk(_import_model),
-    codegen.gen_sdk(_list_models),
-)
+    return models_command.main(args=["-o", "json", "--show-available", "--machine"], standalone_mode=False)
 
+start, start_grpc, build, import_model, list_models = codegen.gen_sdk(_start, _serve_grpc=False), codegen.gen_sdk(_start, _serve_grpc=True), codegen.gen_sdk(_build), codegen.gen_sdk(_import_model), codegen.gen_sdk(_list_models)
 
 @cli.command(context_settings={"token_normalize_func": inflection.underscore})
-@click.argument(
-    "model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()])
-)
+@click.argument("model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]))
 @model_id_option(click)
 @output_option
 @machine_option(click)
 @click.option("--overwrite", is_flag=True, help="Overwrite existing Bento for given LLM if it already exists.")
 @workers_per_resource_option(click, build=True)
 @cog.optgroup.group(cls=cog.MutuallyExclusiveOptionGroup, name="Optimisation options")
 @quantize_option(cog.optgroup, build=True)
@@ -1317,17 +1170,15 @@
     "--runtime",
     type=click.Choice(["ggml", "transformers"]),
     default="transformers",
     help="The runtime to use for the given model. Default is transformers.",
 )
 @click.option(
     "--enable-features",
-    help="Enable additional features for building this LLM Bento. Available: {}".format(
-        ", ".join(openllm.utils.OPTIONAL_DEPENDENCIES)
-    ),
+    help="Enable additional features for building this LLM Bento. Available: {}".format(", ".join(openllm.utils.OPTIONAL_DEPENDENCIES)),
     multiple=True,
     nargs=1,
     metavar="FEATURE[,FEATURE]",
 )
 @click.option(
     "--adapter-id",
     default=None,
@@ -1468,16 +1319,15 @@
                     quantize=quantize,
                     bettertransformer=bettertransformer,
                     extra_dependencies=enable_features,
                     build_ctx=build_ctx,
                     dockerfile_template=dockerfile_template_path,
                     runtime=runtime,
                 )
-    except Exception:
-        raise
+    except Exception: raise
 
     if machine: _echo(f"__tag__:{bento.tag}", fg="white")
     elif output == "pretty":
         if not get_quiet_mode():
             _echo("\n" + OPENLLM_FIGLET, fg="white")
             if not _previously_built: _echo(f"Successfully built {bento}.", fg="green")
             elif not overwrite: _echo(f"'{model_name}' already has a Bento built [{bento}]. To overwrite it pass '--overwrite'.", fg="yellow")
@@ -1555,32 +1405,27 @@
                 "installation": f'"openllm[{m}]"' if m in openllm.utils.OPTIONAL_DEPENDENCIES or config["requirements"] else "openllm",
             }
             converted.extend([normalise_model_name(i) for i in config["model_ids"]])
             if DEBUG:
                 try: openllm.AutoLLM.for_model(m, llm_config=config)
                 except Exception as e: failed_initialized.append((m, e))
 
-        ids_in_local_store: DictStrAny | None = None
+        ids_in_local_store = {k: [i for i in bentoml.models.list() if "framework" in i.info.labels and i.info.labels["framework"] == "openllm" and "model_name" in i.info.labels and i.info.labels["model_name"] == k] for k in json_data.keys()}
+        ids_in_local_store = {k: v for k, v in ids_in_local_store.items() if v}
         local_models: DictStrAny | None = None
         if show_available:
-            ids_in_local_store = {k: [i for i in bentoml.models.list() if "framework" in i.info.labels and i.info.labels["framework"] == "openllm" and "model_name" in i.info.labels and i.info.labels["model_name"] == k] for k in json_data.keys()}
-            ids_in_local_store = {k: v for k, v in ids_in_local_store.items() if v}
             local_models = {k: [str(i.tag) for i in val] for k, val in ids_in_local_store.items()}
 
         if machine:
-            if show_available:
-                assert ids_in_local_store
-                assert local_models
-                json_data["local"] = local_models
+            if show_available: json_data["local"] = local_models
             return json_data
         elif output == "pretty":
             import tabulate
 
             tabulate.PRESERVE_WHITESPACE = True
-
             # llm, architecture, url, model_id, installation, cpu, gpu, runtime_impl
             data: list[str | tuple[str, str, list[str], str, t.LiteralString, t.LiteralString, tuple[LiteralRuntime, ...]] ] = []
             for m, v in json_data.items():
                 data.extend(
                     [
                         (
                             m,
@@ -1621,27 +1466,21 @@
             if DEBUG and len(failed_initialized) > 0:
                 _echo("\nThe following models are supported but failed to initialize:\n")
                 for m, err in failed_initialized:
                     _echo(f"- {m}: ", fg="blue", nl=False)
                     _echo(err, fg="red")
 
             if show_available:
-                assert ids_in_local_store is not None
-                assert local_models
                 if len(ids_in_local_store) == 0:
                     _echo("No models available locally.")
                     ctx.exit(0)
-
                 _echo("The following are available in local store:", fg="magenta")
                 _echo(orjson.dumps(local_models, option=orjson.OPT_INDENT_2).decode(), fg="white")
         else:
-            if show_available:
-                assert ids_in_local_store
-                assert local_models
-                json_data["local"] = local_models
+            if show_available: json_data["local"] = local_models
             _echo(orjson.dumps(json_data, option=orjson.OPT_INDENT_2,).decode(), fg="white")
     ctx.exit(0)
 
 
 @cli.command()
 @click.argument("model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]), required=False)
 @click.option("-y", "--yes", "--assume-yes", is_flag=True, help="Skip confirmation when deleting a specific model")
@@ -1764,20 +1603,18 @@
         response = client.llm.postprocess_generate(prompt, res["responses"])
         _echo("\n\n==Responses==\n", fg="white")
         _echo(response, fg=generated_fg)
     elif output == "json": _echo(orjson.dumps(res, option=orjson.OPT_INDENT_2).decode(), fg="white")
     else: _echo(res["responses"], fg="white")
     ctx.exit(0)
 
-
 @cli.group(name="utils")
 def utils_command() -> None:
     """Utilities Subcommand group."""
 
-
 @utils_command.command()
 @click.pass_context
 def list_bentos(ctx: click.Context):
     """List available bentos built by OpenLLM."""
     _local_bentos = {str(i.tag): i.info.labels["start_name"] for i in bentoml.list() if "start_name" in i.info.labels}
     mapping = {k: [tag for tag, name in _local_bentos.items() if name == k] for k in tuple(inflection.dasherize(key) for key in openllm.CONFIG_MAPPING.keys())}
     mapping = {k: v for k, v in mapping.items() if v}
@@ -1792,16 +1629,14 @@
     """Dive into a BentoLLM. This is synonymous to cd $(b get <bento>:<tag> -o path)."""
     try: bentomodel = _bento_store.get(bento)
     except bentoml.exceptions.NotFound: ctx.fail(f"Bento {bento} not found. Make sure to call `openllm build first`")
     if "bundler" not in  bentomodel.info.labels or bentomodel.info.labels["bundler"] != "openllm.bundle": ctx.fail(f"Bento is either too old or not built with OpenLLM. Make sure to use ``openllm build {bentomodel.info.labels['start_name']}`` for correctness.")
     # copy and paste this into a new shell
     _echo(f"cd $(python -m bentoml get {bentomodel.tag!s} -o path)", fg="white")
 
-
-
 @overload
 def get_prompt(model_name: str, prompt: str, format: str | None, output: OutputLiteral, machine: t.Literal[True] = True) -> str: ...
 @overload
 def get_prompt(model_name: str, prompt: str, format: str | None, output: OutputLiteral, machine: t.Literal[False] = ...) -> None: ...
 @utils_command.command()
 @click.argument("model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]))
 @click.argument("prompt", type=click.STRING)
```

### Comparing `openllm-0.2.8/src/openllm/client.py` & `openllm-0.2.9/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/exceptions.py` & `openllm-0.2.9/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/testing.py` & `openllm-0.2.9/src/openllm/testing.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/bundle/__init__.py` & `openllm-0.2.9/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/bundle/_package.py` & `openllm-0.2.9/src/openllm/bundle/_package.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/bundle/oci/Dockerfile-builder` & `openllm-0.2.9/src/openllm/bundle/oci/Dockerfile-builder`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/bundle/oci/__init__.py` & `openllm-0.2.9/src/openllm/bundle/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/__init__.py` & `openllm-0.2.9/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/auto/__init__.py` & `openllm-0.2.9/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/auto/configuration_auto.py` & `openllm-0.2.9/src/openllm/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/auto/factory.py` & `openllm-0.2.9/src/openllm/models/auto/factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/auto/modeling_auto.py` & `openllm-0.2.9/src/openllm/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.2.9/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.2.9/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/auto/modeling_vllm_auto.py` & `openllm-0.2.9/src/openllm/models/auto/modeling_vllm_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/baichuan/__init__.py` & `openllm-0.2.9/src/openllm/models/baichuan/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/baichuan/configuration_baichuan.py` & `openllm-0.2.9/src/openllm/models/baichuan/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/baichuan/modeling_baichuan.py` & `openllm-0.2.9/src/openllm/models/baichuan/modeling_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/chatglm/__init__.py` & `openllm-0.2.9/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.2.9/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.2.9/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.2.9/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.2.9/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.2.9/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/falcon/__init__.py` & `openllm-0.2.9/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.2.9/src/openllm/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.2.9/src/openllm/models/falcon/modeling_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/flan_t5/__init__.py` & `openllm-0.2.9/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.2.9/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.2.9/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.2.9/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.2.9/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.2.9/src/openllm/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/gpt_neox/configuration_gpt_neox.py` & `openllm-0.2.9/src/openllm/models/gpt_neox/configuration_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/gpt_neox/modeling_gpt_neox.py` & `openllm-0.2.9/src/openllm/models/gpt_neox/modeling_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/llama/__init__.py` & `openllm-0.2.9/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/llama/configuration_llama.py` & `openllm-0.2.9/src/openllm/models/llama/configuration_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/llama/modeling_llama.py` & `openllm-0.2.9/src/openllm/models/llama/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/llama/modeling_vllm_llama.py` & `openllm-0.2.9/src/openllm/models/llama/modeling_vllm_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/mpt/__init__.py` & `openllm-0.2.9/src/openllm/models/mpt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/mpt/configuration_mpt.py` & `openllm-0.2.9/src/openllm/models/mpt/configuration_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/mpt/modeling_mpt.py` & `openllm-0.2.9/src/openllm/models/mpt/modeling_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/opt/__init__.py` & `openllm-0.2.9/src/openllm/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/opt/configuration_opt.py` & `openllm-0.2.9/src/openllm/models/opt/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/opt/modeling_flax_opt.py` & `openllm-0.2.9/src/openllm/models/opt/modeling_flax_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/opt/modeling_opt.py` & `openllm-0.2.9/src/openllm/models/opt/modeling_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/opt/modeling_tf_opt.py` & `openllm-0.2.9/src/openllm/models/opt/modeling_tf_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/opt/modeling_vllm_opt.py` & `openllm-0.2.9/src/openllm/models/opt/modeling_vllm_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/stablelm/__init__.py` & `openllm-0.2.9/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.2.9/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.2.9/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/starcoder/__init__.py` & `openllm-0.2.9/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.2.9/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.2.9/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/playground/__init__.py` & `openllm-0.2.9/src/openllm/playground/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/playground/_meta.yml` & `openllm-0.2.9/src/openllm/playground/_meta.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/playground/falcon_tuned.py` & `openllm-0.2.9/src/openllm/playground/falcon_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/playground/features.py` & `openllm-0.2.9/src/openllm/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/playground/llama2_qlora.py` & `openllm-0.2.9/src/openllm/playground/llama2_qlora.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/playground/opt_tuned.py` & `openllm-0.2.9/src/openllm/playground/opt_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/serialisation/__init__.py` & `openllm-0.2.9/src/openllm/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/serialisation/constants.py` & `openllm-0.2.9/src/openllm/serialisation/constants.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/serialisation/ggml.py` & `openllm-0.2.9/src/openllm/serialisation/ggml.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/serialisation/transformers.py` & `openllm-0.2.9/src/openllm/serialisation/transformers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/__init__.py` & `openllm-0.2.9/src/openllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/analytics.py` & `openllm-0.2.9/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/codegen.py` & `openllm-0.2.9/src/openllm/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/dantic.py` & `openllm-0.2.9/src/openllm/utils/dantic.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.2.9/src/openllm/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.2.9/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.2.9/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/dummy_pt_and_triton_objects.py` & `openllm-0.2.9/src/openllm/utils/dummy_pt_and_triton_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.2.9/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.2.9/src/openllm/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/dummy_vllm_objects.py` & `openllm-0.2.9/src/openllm/utils/dummy_vllm_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/import_utils.py` & `openllm-0.2.9/src/openllm/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/lazy.py` & `openllm-0.2.9/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm/utils/representation.py` & `openllm-0.2.9/src/openllm/utils/representation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm_client/__init__.py` & `openllm-0.2.9/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm_client/_prompt.py` & `openllm-0.2.9/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm_client/runtimes/__init__.py` & `openllm-0.2.9/src/openllm_client/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm_client/runtimes/base.py` & `openllm-0.2.9/src/openllm_client/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm_client/runtimes/grpc.py` & `openllm-0.2.9/src/openllm_client/runtimes/grpc.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/src/openllm_client/runtimes/http.py` & `openllm-0.2.9/src/openllm_client/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/__init__.py` & `openllm-0.2.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/client_test.py` & `openllm-0.2.9/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/configuration_test.py` & `openllm-0.2.9/tests/configuration_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/conftest.py` & `openllm-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/models_test.py` & `openllm-0.2.9/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/package_test.py` & `openllm-0.2.9/tests/package_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/strategies_test.py` & `openllm-0.2.9/tests/strategies_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/_strategies/__init__.py` & `openllm-0.2.9/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/_strategies/_configuration.py` & `openllm-0.2.9/tests/_strategies/_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         "default_id": st.text(min_size=1),
         "model_ids": st.lists(st.text(), min_size=1),
         "architecture": st.text(min_size=1),
         "url": st.text(),
         "requires_gpu": st.booleans(),
         "trust_remote_code": st.booleans(),
         "requirements": st.none() | st.lists(st.text(), min_size=1),
-        "default_implementation": st.dictionaries(["cpu", "nvidia.com/gpu"], ["vllm", "pt", "tf", "flax"]),
+        "default_implementation": st.dictionaries(st.sampled_from(["cpu", "nvidia.com/gpu"]), st.sampled_from(["vllm", "pt", "tf", "flax"])),
         "model_type": st.sampled_from(["causal_lm", "seq2seq_lm"]),
         "runtime": st.sampled_from(["transformers", "ggml"]),
         "name_type": st.sampled_from(["dasherize", "lowercase"]),
         "timeout": st.integers(min_value=3600),
         "workers_per_resource": st.one_of(st.integers(min_value=1), st.floats(min_value=0.1, max_value=1.0)),
     }
     return draw(st.builds(ModelSettings, **kwargs))
```

### Comparing `openllm-0.2.8/tests/models/__init__.py` & `openllm-0.2.9/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/models/conftest.py` & `openllm-0.2.9/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/models/flan_t5_test.py` & `openllm-0.2.9/tests/models/flan_t5_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/models/opt_test.py` & `openllm-0.2.9/tests/models/opt_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json` & `openllm-0.2.9/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json` & `openllm-0.2.9/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/models/__snapshots__/opt_test/test_opt_125m[container].json` & `openllm-0.2.9/tests/models/__snapshots__/opt_test/test_opt_125m[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/tests/models/__snapshots__/opt_test/test_opt_125m[local].json` & `openllm-0.2.9/tests/models/__snapshots__/opt_test/test_opt_125m[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/.gitignore` & `openllm-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/LICENSE.md` & `openllm-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/README.md` & `openllm-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ## 📖 Introduction
 
 With OpenLLM, you can run inference with any open-source large-language models,
 deploy to the cloud or on-premises, and build powerful AI apps.
 
 🚂 **State-of-the-art LLMs**: built-in supports a wide range of open-source LLMs
-and model runtime, including StableLM, Falcon, Dolly, Flan-T5, ChatGLM,
+and model runtime, including Llama 2， StableLM, Falcon, Dolly, Flan-T5, ChatGLM,
 StarCoder and more.
 
 🔥 **Flexible APIs**: serve LLMs over RESTful API or gRPC with one command,
 query via WebUI, CLI, our Python/Javascript client, or any HTTP client.
 
 ⛓️ **Freedom To Build**: First-class support for LangChain, BentoML and Hugging
 Face that allows you to easily create your own AI apps by composing LLMs with
@@ -86,17 +86,17 @@
 can experiment with the endpoints and sample input prompts.
 
 OpenLLM provides a built-in Python client, allowing you to interact with the
 model. In a different terminal window or a Jupyter Notebook, create a client to
 start interacting with the model:
 
 ```python
->>> import openllm
->>> client = openllm.client.HTTPClient('http://localhost:3000')
->>> client.query('Explain to me the difference between "further" and "farther"')
+import openllm
+client = openllm.client.HTTPClient('http://localhost:3000')
+client.query('Explain to me the difference between "further" and "farther"')
 ```
 
 You can also use the `openllm query` command to query the model from the
 terminal:
 
 ```bash
 export OPENLLM_ENDPOINT=http://localhost:3000
@@ -481,16 +481,17 @@
 [Adding a New Model Guide](https://github.com/bentoml/OpenLLM/blob/main/ADDING_NEW_MODEL.md)
 to see how you can do it yourself.
 
 ## ⚙️ Integrations
 
 OpenLLM is not just a standalone product; it's a building block designed to
 integrate with other powerful tools easily. We currently offer integration with
-[BentoML](https://github.com/bentoml/BentoML) and
-[LangChain](https://github.com/hwchase17/langchain).
+[BentoML](https://github.com/bentoml/BentoML),
+[LangChain](https://github.com/hwchase17/langchain),
+and [Transformers Agents](https://huggingface.co/docs/transformers/transformers_agents).
 
 ### BentoML
 
 OpenLLM models can be integrated as a
 [Runner](https://docs.bentoml.com/en/latest/concepts/runner.html) in your
 BentoML service. These runners have a `generate` method that takes a string as a
 prompt and returns a corresponding output string. This will allow you to plug
@@ -511,49 +512,14 @@
 
 @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str:
     answer = await llm_runner.generate(input_text)
     return answer
 ```
 
-### Hugging Face Agents
-
-OpenLLM seamlessly integrates with Hugging Face Agents.
-
-> **Warning** The HuggingFace Agent is still at experimental stage. It is
-> recommended to OpenLLM with `pip install -r nightly-requirements.txt` to get
-> the latest API update for HuggingFace agent.
-
-```python
-import transformers
-
-agent = transformers.HfAgent("http://localhost:3000/hf/agent")  # URL that runs the OpenLLM server
-
-agent.run("Is the following `text` positive or negative?", text="I don't like how this models is generate inputs")
-```
-
-> **Note** Only `starcoder` is currently supported with Agent integration. The
-> example above was also ran with four T4s on EC2 `g4dn.12xlarge`
-
-If you want to use OpenLLM client to ask questions to the running agent, you can
-also do so:
-
-```python
-import openllm
-
-client = openllm.client.HTTPClient("http://localhost:3000")
-
-client.ask_agent(
-    task="Is the following `text` positive or negative?",
-    text="What are you thinking about?",
-)
-```
-
-![Gif showing Agent integration](/assets/agent.gif)
-<br/>
 
 ### [LangChain](https://python.langchain.com/docs/ecosystem/integrations/openllm)
 
 To quickly start a local LLM with `langchain`, simply do the following:
 
 ```python
 from langchain.llms import OpenLLM
@@ -591,14 +557,53 @@
 def chat(input_text: str):
     return agent.run(input_text)
 ```
 
 > **Note** You can find out more examples under the
 > [examples](https://github.com/bentoml/OpenLLM/tree/main/examples) folder.
 
+
+### Transformers Agents
+
+OpenLLM seamlessly integrates with [Transformers Agents](https://huggingface.co/docs/transformers/transformers_agents).
+
+
+> **Warning** The Transformers Agent is still at an experimental stage. It is
+> recommended to install OpenLLM with `pip install -r nightly-requirements.txt` to get
+> the latest API update for HuggingFace agent.
+
+```python
+import transformers
+
+agent = transformers.HfAgent("http://localhost:3000/hf/agent")  # URL that runs the OpenLLM server
+
+agent.run("Is the following `text` positive or negative?", text="I don't like how this models is generate inputs")
+```
+
+> **Note** Only `starcoder` is currently supported with Agent integration. The
+> example above was also ran with four T4s on EC2 `g4dn.12xlarge`
+
+If you want to use OpenLLM client to ask questions to the running agent, you can
+also do so:
+
+```python
+import openllm
+
+client = openllm.client.HTTPClient("http://localhost:3000")
+
+client.ask_agent(
+    task="Is the following `text` positive or negative?",
+    text="What are you thinking about?",
+)
+```
+
+![Gif showing Agent integration](/assets/agent.gif)
+<br/>
+
+
 ## 🚀 Deploying to Production
 
 There are several ways to deploy your LLMs:
 
 ### 🐳 Docker container
 
 1. **Building a Bento**: With OpenLLM, you can easily build a Bento for a
@@ -614,19 +619,23 @@
    code, models, files, artefacts, and dependencies.
 
 2. **Containerize your Bento**
 
    ```bash
    bentoml containerize <name:version>
    ```
+   This generates a OCI-compatible docker image that can be deployed anywhere docker runs.
+   For best scalability and reliability of your LLM service in production, we recommend deploy
+   with BentoCloud。
+
 
 ### ☁️ BentoCloud
 
-Deploy your LLMs using [BentoCloud](https://www.bentoml.com/bento-cloud/), the
-production-ready platform for managing and deploying machine learning models.
+Deploy OpenLLM with [BentoCloud](https://www.bentoml.com/bento-cloud/), the
+the serverless cloud for shipping and scaling AI applications.
 
 1. **Create a BentoCloud account:** [sign up here](https://bentoml.com/cloud)
    for early access
 
 2. **Log into your BentoCloud account:**
 
    ```bash
@@ -650,36 +659,15 @@
    bentoml push <name:version>
    ```
 
 5. **Deploying a Bento**: Deploy your LLMs to BentoCloud with a single
    `bentoml deployment create` command following the
    [deployment instructions](https://docs.bentoml.com/en/latest/reference/cli.html#bentoml-deployment-create).
 
-Explore other options for deploying and hosting online ML services at
-[BentoML's Documentation](https://docs.bentoml.com/en/latest/concepts/deploy.html).
 
-## 🍇 Telemetry
-
-OpenLLM collects usage data to enhance user experience and improve the product.
-We only report OpenLLM's internal API calls and ensure maximum privacy by
-excluding sensitive information. We will never collect user code, model data, or
-stack traces. For usage tracking, check out the
-[code](./src/openllm/utils/analytics.py).
-
-You can opt out of usage tracking by using the `--do-not-track` CLI option:
-
-```bash
-openllm [command] --do-not-track
-```
-
-Or by setting the environment variable `OPENLLM_DO_NOT_TRACK=True`:
-
-```bash
-export OPENLLM_DO_NOT_TRACK=True
-```
 
 ## 👥 Community
 
 Engage with like-minded individuals passionate about LLMs, AI, and more on our
 [Discord](https://l.bentoml.com/join-openllm-discord)!
 
 OpenLLM is actively maintained by the BentoML team. Feel free to reach out and
@@ -692,14 +680,34 @@
 capabilities or have any questions, don't hesitate to reach out in our
 [discord channel](https://l.bentoml.com/join-openllm-discord).
 
 Checkout our
 [Developer Guide](https://github.com/bentoml/OpenLLM/blob/main/DEVELOPMENT.md)
 if you wish to contribute to OpenLLM's codebase.
 
+## 🍇 Telemetry
+
+OpenLLM collects usage data to enhance user experience and improve the product.
+We only report OpenLLM's internal API calls and ensure maximum privacy by
+excluding sensitive information. We will never collect user code, model data, or
+stack traces. For usage tracking, check out the
+[code](./src/openllm/utils/analytics.py).
+
+You can opt out of usage tracking by using the `--do-not-track` CLI option:
+
+```bash
+openllm [command] --do-not-track
+```
+
+Or by setting the environment variable `OPENLLM_DO_NOT_TRACK=True`:
+
+```bash
+export OPENLLM_DO_NOT_TRACK=True
+```
+
 ## 📔 Citation
 
 If you use OpenLLM in your research, we provide a [citation](./CITATION.cff) to
 use:
 
 ```bibtex
 @software{Pham_OpenLLM_Operating_LLMs_2023,
```

#### html2text {}

```diff
@@ -2,24 +2,25 @@
                           ****** ð¦¾ OpenLLM ******
                       [pypi_status][ci][Twitter][Discord]
   An open platform for operating large language models (LLMs) in production.
            Fine-tune, serve, deploy, and monitor any LLMs with ease.
 ## ð Introduction With OpenLLM, you can run inference with any open-source
 large-language models, deploy to the cloud or on-premises, and build powerful
 AI apps. ð **State-of-the-art LLMs**: built-in supports a wide range of
-open-source LLMs and model runtime, including StableLM, Falcon, Dolly, Flan-T5,
-ChatGLM, StarCoder and more. ð¥ **Flexible APIs**: serve LLMs over RESTful
-API or gRPC with one command, query via WebUI, CLI, our Python/Javascript
-client, or any HTTP client. âï¸ **Freedom To Build**: First-class support
-for LangChain, BentoML and Hugging Face that allows you to easily create your
-own AI apps by composing LLMs with other models and services. ð¯ **Streamline
-Deployment**: Automatically generate your LLM server Docker Images or deploy as
-serverless endpoint via [âï¸ BentoCloud](https://l.bentoml.com/bento-cloud).
-ð¤ï¸ **Bring your own LLM**: Fine-tune any LLM to suit your needs with
-`LLM.tuning()`. (Coming soon) ![Gif showing OpenLLM Intro](/assets/output.gif)
+open-source LLMs and model runtime, including Llama 2ï¼ StableLM, Falcon,
+Dolly, Flan-T5, ChatGLM, StarCoder and more. ð¥ **Flexible APIs**: serve LLMs
+over RESTful API or gRPC with one command, query via WebUI, CLI, our Python/
+Javascript client, or any HTTP client. âï¸ **Freedom To Build**: First-class
+support for LangChain, BentoML and Hugging Face that allows you to easily
+create your own AI apps by composing LLMs with other models and services. ð¯
+**Streamline Deployment**: Automatically generate your LLM server Docker Images
+or deploy as serverless endpoint via [âï¸ BentoCloud](https://l.bentoml.com/
+bento-cloud). ð¤ï¸ **Bring your own LLM**: Fine-tune any LLM to suit your
+needs with `LLM.tuning()`. (Coming soon) ![Gif showing OpenLLM Intro](/assets/
+output.gif)
 ## ðâ Getting Started To use OpenLLM, you need to have Python 3.8 (or
 newer) and `pip` installed on your system. We highly recommend using a Virtual
 Environment to prevent package conflicts. You can install OpenLLM using pip as
 follows: ```bash pip install openllm ``` To verify if it's installed correctly,
 run: ``` $ openllm -h Usage: openllm [OPTIONS] COMMAND [ARGS]...
 âââââââ âââââââ
 ââââââââââââ ââââââ âââ ââââ
@@ -40,28 +41,28 @@
 Fine-tune, serve, deploy, and monitor any LLMs with ease. ``` ### Starting an
 LLM Server To start an LLM server, use `openllm start`. For example, to start a
 [`OPT`](https://huggingface.co/docs/transformers/model_doc/opt) server, do the
 following: ```bash openllm start opt ``` Following this, a Web UI will be
 accessible at http://localhost:3000 where you can experiment with the endpoints
 and sample input prompts. OpenLLM provides a built-in Python client, allowing
 you to interact with the model. In a different terminal window or a Jupyter
-Notebook, create a client to start interacting with the model: ```python >>>
-import openllm >>> client = openllm.client.HTTPClient('http://localhost:3000')
->>> client.query('Explain to me the difference between "further" and
-"farther"') ``` You can also use the `openllm query` command to query the model
-from the terminal: ```bash export OPENLLM_ENDPOINT=http://localhost:3000
-openllm query 'Explain to me the difference between "further" and "farther"'
-``` Visit `http://localhost:3000/docs.json` for OpenLLM's API specification.
-Users can also specify different variants of the model to be served, by
-providing the `--model-id` argument, e.g.: ```bash openllm start flan-t5 --
-model-id google/flan-t5-large ``` Use the `openllm models` command to see the
-list of models and their variants supported in OpenLLM. ## ð§© Supported
-Models The following models are currently supported in OpenLLM. By default,
-OpenLLM doesn't include dependencies to run all models. The extra model-
-specific dependencies can be installed with the instructions below:
+Notebook, create a client to start interacting with the model: ```python import
+openllm client = openllm.client.HTTPClient('http://localhost:3000')
+client.query('Explain to me the difference between "further" and "farther"')
+``` You can also use the `openllm query` command to query the model from the
+terminal: ```bash export OPENLLM_ENDPOINT=http://localhost:3000 openllm query
+'Explain to me the difference between "further" and "farther"' ``` Visit `http:
+//localhost:3000/docs.json` for OpenLLM's API specification. Users can also
+specify different variants of the model to be served, by providing the `--
+model-id` argument, e.g.: ```bash openllm start flan-t5 --model-id google/flan-
+t5-large ``` Use the `openllm models` command to see the list of models and
+their variants supported in OpenLLM. ## ð§© Supported Models The following
+models are currently supported in OpenLLM. By default, OpenLLM doesn't include
+dependencies to run all models. The extra model-specific dependencies can be
+installed with the instructions below:
 Model     Architecture                    CPU GPU Model Ids              Installation
                                                       * thudm/chatglm-6b
                                                       * thudm/chatglm-
                                                         6b-int8          ```bash pip
                                                       * thudm/chatglm-   install
 chatglm   ChatGLMForConditionalGeneration ââ      6b-int4          "openllm
                                                       * thudm/chatglm2-  [chatglm]"
@@ -217,96 +218,98 @@
 tuning all models. > Currently, only OPT has fully adapters support. ###
 Integrating a New Model OpenLLM encourages contributions by welcoming users to
 incorporate their custom LLMs into the ecosystem. Check out [Adding a New Model
 Guide](https://github.com/bentoml/OpenLLM/blob/main/ADDING_NEW_MODEL.md) to see
 how you can do it yourself. ## âï¸ Integrations OpenLLM is not just a
 standalone product; it's a building block designed to integrate with other
 powerful tools easily. We currently offer integration with [BentoML](https://
-github.com/bentoml/BentoML) and [LangChain](https://github.com/hwchase17/
-langchain). ### BentoML OpenLLM models can be integrated as a [Runner](https://
-docs.bentoml.com/en/latest/concepts/runner.html) in your BentoML service. These
-runners have a `generate` method that takes a string as a prompt and returns a
-corresponding output string. This will allow you to plug and play any OpenLLM
-models with your existing ML workflow. ```python import bentoml import openllm
-model = "opt" llm_config = openllm.AutoConfig.for_model(model) llm_runner =
-openllm.Runner(model, llm_config=llm_config) svc = bentoml.Service( name=f"llm-
-opt-service", runners=[llm_runner] ) @svc.api(input=Text(), output=Text())
-async def prompt(input_text: str) -> str: answer = await llm_runner.generate
-(input_text) return answer ``` ### Hugging Face Agents OpenLLM seamlessly
-integrates with Hugging Face Agents. > **Warning** The HuggingFace Agent is
-still at experimental stage. It is > recommended to OpenLLM with `pip install -
+github.com/bentoml/BentoML), [LangChain](https://github.com/hwchase17/
+langchain), and [Transformers Agents](https://huggingface.co/docs/transformers/
+transformers_agents). ### BentoML OpenLLM models can be integrated as a
+[Runner](https://docs.bentoml.com/en/latest/concepts/runner.html) in your
+BentoML service. These runners have a `generate` method that takes a string as
+a prompt and returns a corresponding output string. This will allow you to plug
+and play any OpenLLM models with your existing ML workflow. ```python import
+bentoml import openllm model = "opt" llm_config = openllm.AutoConfig.for_model
+(model) llm_runner = openllm.Runner(model, llm_config=llm_config) svc =
+bentoml.Service( name=f"llm-opt-service", runners=[llm_runner] ) @svc.api
+(input=Text(), output=Text()) async def prompt(input_text: str) -> str: answer
+= await llm_runner.generate(input_text) return answer ``` ### [LangChain]
+(https://python.langchain.com/docs/ecosystem/integrations/openllm) To quickly
+start a local LLM with `langchain`, simply do the following: ```python from
+langchain.llms import OpenLLM llm = OpenLLM(model_name="dolly-v2",
+model_id='databricks/dolly-v2-7b', device_map='auto') llm("What is the
+difference between a duck and a goose? And why there are so many Goose in
+Canada?") ``` `langchain.llms.OpenLLM` has the capability to interact with
+remote OpenLLM Server. Given there is an OpenLLM server deployed elsewhere, you
+can connect to it by specifying its URL: ```python from langchain.llms import
+OpenLLM llm = OpenLLM(server_url='http://44.23.123.1:3000', server_type='grpc')
+llm("What is the difference between a duck and a goose? And why there are so
+many Goose in Canada?") ``` To integrate a LangChain agent with BentoML, you
+can do the following: ```python llm = OpenLLM( model_name='flan-t5',
+model_id='google/flan-t5-large', embedded=False, ) tools = load_tools(
+["serpapi", "llm-math"], llm=llm) agent = initialize_agent( tools, llm,
+agent=AgentType.ZERO_SHOT_REACT_DESCRIPTION ) svc = bentoml.Service("langchain-
+openllm", runners=[llm.runner]) @svc.api(input=Text(), output=Text()) def chat
+(input_text: str): return agent.run(input_text) ``` > **Note** You can find out
+more examples under the > [examples](https://github.com/bentoml/OpenLLM/tree/
+main/examples) folder. ### Transformers Agents OpenLLM seamlessly integrates
+with [Transformers Agents](https://huggingface.co/docs/transformers/
+transformers_agents). > **Warning** The Transformers Agent is still at an
+experimental stage. It is > recommended to install OpenLLM with `pip install -
 r nightly-requirements.txt` to get > the latest API update for HuggingFace
 agent. ```python import transformers agent = transformers.HfAgent("http://
 localhost:3000/hf/agent") # URL that runs the OpenLLM server agent.run("Is the
 following `text` positive or negative?", text="I don't like how this models is
 generate inputs") ``` > **Note** Only `starcoder` is currently supported with
 Agent integration. The > example above was also ran with four T4s on EC2
 `g4dn.12xlarge` If you want to use OpenLLM client to ask questions to the
 running agent, you can also do so: ```python import openllm client =
 openllm.client.HTTPClient("http://localhost:3000") client.ask_agent( task="Is
 the following `text` positive or negative?", text="What are you thinking
 about?", ) ``` ![Gif showing Agent integration](/assets/agent.gif)
-### [LangChain](https://python.langchain.com/docs/ecosystem/integrations/
-openllm) To quickly start a local LLM with `langchain`, simply do the
-following: ```python from langchain.llms import OpenLLM llm = OpenLLM
-(model_name="dolly-v2", model_id='databricks/dolly-v2-7b', device_map='auto')
-llm("What is the difference between a duck and a goose? And why there are so
-many Goose in Canada?") ``` `langchain.llms.OpenLLM` has the capability to
-interact with remote OpenLLM Server. Given there is an OpenLLM server deployed
-elsewhere, you can connect to it by specifying its URL: ```python from
-langchain.llms import OpenLLM llm = OpenLLM(server_url='http://44.23.123.1:
-3000', server_type='grpc') llm("What is the difference between a duck and a
-goose? And why there are so many Goose in Canada?") ``` To integrate a
-LangChain agent with BentoML, you can do the following: ```python llm = OpenLLM
-( model_name='flan-t5', model_id='google/flan-t5-large', embedded=False, )
-tools = load_tools(["serpapi", "llm-math"], llm=llm) agent = initialize_agent
-( tools, llm, agent=AgentType.ZERO_SHOT_REACT_DESCRIPTION ) svc =
-bentoml.Service("langchain-openllm", runners=[llm.runner]) @svc.api(input=Text
-(), output=Text()) def chat(input_text: str): return agent.run(input_text) ```
-> **Note** You can find out more examples under the > [examples](https://
-github.com/bentoml/OpenLLM/tree/main/examples) folder. ## ð Deploying to
-Production There are several ways to deploy your LLMs: ### ð³ Docker
-container 1. **Building a Bento**: With OpenLLM, you can easily build a Bento
-for a specific model, like `dolly-v2`, using the `build` command.: ```bash
-openllm build dolly-v2 ``` A [Bento](https://docs.bentoml.com/en/latest/
-concepts/bento.html#what-is-a-bento), in BentoML, is the unit of distribution.
-It packages your program's source code, models, files, artefacts, and
-dependencies. 2. **Containerize your Bento** ```bash bentoml containerize  ```
-### âï¸ BentoCloud Deploy your LLMs using [BentoCloud](https://
-www.bentoml.com/bento-cloud/), the production-ready platform for managing and
-deploying machine learning models. 1. **Create a BentoCloud account:** [sign up
-here](https://bentoml.com/cloud) for early access 2. **Log into your BentoCloud
-account:** ```bash bentoml cloud login --api-token  --endpoint  ``` > **Note**:
-Replace `` and `` with your > specific API token and the BentoCloud endpoint
-respectively. 3. **Bulding a Bento**: With OpenLLM, you can easily build a
-Bento for a specific model, such as `dolly-v2`: ```bash openllm build dolly-v2
-``` 4. **Pushing a Bento**: Push your freshly-built Bento service to BentoCloud
-via the `push` command: ```bash bentoml push  ``` 5. **Deploying a Bento**:
-Deploy your LLMs to BentoCloud with a single `bentoml deployment create`
-command following the [deployment instructions](https://docs.bentoml.com/en/
-latest/reference/cli.html#bentoml-deployment-create). Explore other options for
-deploying and hosting online ML services at [BentoML's Documentation](https://
-docs.bentoml.com/en/latest/concepts/deploy.html). ## ð Telemetry OpenLLM
-collects usage data to enhance user experience and improve the product. We only
-report OpenLLM's internal API calls and ensure maximum privacy by excluding
-sensitive information. We will never collect user code, model data, or stack
-traces. For usage tracking, check out the [code](./src/openllm/utils/
-analytics.py). You can opt out of usage tracking by using the `--do-not-track`
-CLI option: ```bash openllm [command] --do-not-track ``` Or by setting the
-environment variable `OPENLLM_DO_NOT_TRACK=True`: ```bash export
-OPENLLM_DO_NOT_TRACK=True ``` ## ð¥ Community Engage with like-minded
-individuals passionate about LLMs, AI, and more on our [Discord](https://
-l.bentoml.com/join-openllm-discord)! OpenLLM is actively maintained by the
-BentoML team. Feel free to reach out and join us in our pursuit to make LLMs
-more accessible and easy to use ð [Join our Slack community!](https://
-l.bentoml.com/join-slack) ## ð Contributing We welcome contributions! If
-you're interested in enhancing OpenLLM's capabilities or have any questions,
-don't hesitate to reach out in our [discord channel](https://l.bentoml.com/
-join-openllm-discord). Checkout our [Developer Guide](https://github.com/
-bentoml/OpenLLM/blob/main/DEVELOPMENT.md) if you wish to contribute to
-OpenLLM's codebase. ## ð Citation If you use OpenLLM in your research, we
-provide a [citation](./CITATION.cff) to use: ```bibtex @software
+## ð Deploying to Production There are several ways to deploy your LLMs: ###
+ð³ Docker container 1. **Building a Bento**: With OpenLLM, you can easily
+build a Bento for a specific model, like `dolly-v2`, using the `build`
+command.: ```bash openllm build dolly-v2 ``` A [Bento](https://
+docs.bentoml.com/en/latest/concepts/bento.html#what-is-a-bento), in BentoML, is
+the unit of distribution. It packages your program's source code, models,
+files, artefacts, and dependencies. 2. **Containerize your Bento** ```bash
+bentoml containerize  ``` This generates a OCI-compatible docker image that can
+be deployed anywhere docker runs. For best scalability and reliability of your
+LLM service in production, we recommend deploy with BentoCloudã ### âï¸
+BentoCloud Deploy OpenLLM with [BentoCloud](https://www.bentoml.com/bento-
+cloud/), the the serverless cloud for shipping and scaling AI applications. 1.
+**Create a BentoCloud account:** [sign up here](https://bentoml.com/cloud) for
+early access 2. **Log into your BentoCloud account:** ```bash bentoml cloud
+login --api-token  --endpoint  ``` > **Note**: Replace `` and `` with your >
+specific API token and the BentoCloud endpoint respectively. 3. **Bulding a
+Bento**: With OpenLLM, you can easily build a Bento for a specific model, such
+as `dolly-v2`: ```bash openllm build dolly-v2 ``` 4. **Pushing a Bento**: Push
+your freshly-built Bento service to BentoCloud via the `push` command: ```bash
+bentoml push  ``` 5. **Deploying a Bento**: Deploy your LLMs to BentoCloud with
+a single `bentoml deployment create` command following the [deployment
+instructions](https://docs.bentoml.com/en/latest/reference/cli.html#bentoml-
+deployment-create). ## ð¥ Community Engage with like-minded individuals
+passionate about LLMs, AI, and more on our [Discord](https://l.bentoml.com/
+join-openllm-discord)! OpenLLM is actively maintained by the BentoML team. Feel
+free to reach out and join us in our pursuit to make LLMs more accessible and
+easy to use ð [Join our Slack community!](https://l.bentoml.com/join-slack)
+## ð Contributing We welcome contributions! If you're interested in
+enhancing OpenLLM's capabilities or have any questions, don't hesitate to reach
+out in our [discord channel](https://l.bentoml.com/join-openllm-discord).
+Checkout our [Developer Guide](https://github.com/bentoml/OpenLLM/blob/main/
+DEVELOPMENT.md) if you wish to contribute to OpenLLM's codebase. ## ð
+Telemetry OpenLLM collects usage data to enhance user experience and improve
+the product. We only report OpenLLM's internal API calls and ensure maximum
+privacy by excluding sensitive information. We will never collect user code,
+model data, or stack traces. For usage tracking, check out the [code](./src/
+openllm/utils/analytics.py). You can opt out of usage tracking by using the `--
+do-not-track` CLI option: ```bash openllm [command] --do-not-track ``` Or by
+setting the environment variable `OPENLLM_DO_NOT_TRACK=True`: ```bash export
+OPENLLM_DO_NOT_TRACK=True ``` ## ð Citation If you use OpenLLM in your
+research, we provide a [citation](./CITATION.cff) to use: ```bibtex @software
 {Pham_OpenLLM_Operating_LLMs_2023, author = {Pham, Aaron and Yang, Chaoyu and
 Sheng, Sean and Zhao, Shenyang and Lee, Sauyon and Jiang, Bo and Dong, Fog and
 Guan, Xipeng and Ming, Frost}, license = {Apache-2.0}, month = jun, title = {
 {OpenLLM: Operating LLMs in production}}, url = {https://github.com/bentoml/
 OpenLLM}, year = {2023} } ```
```

### Comparing `openllm-0.2.8/hatch.toml` & `openllm-0.2.9/hatch.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/pyproject.toml` & `openllm-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.8/PKG-INFO` & `openllm-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.2.8
+Version: 0.2.9
 Summary: OpenLLM: Operating LLMs in production
 Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://discord.gg/openllm
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: GitHub, https://github.com/bentoml/openllm
 Project-URL: History, https://github.com/bentoml/openllm/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
@@ -146,15 +146,15 @@
 
 ## 📖 Introduction
 
 With OpenLLM, you can run inference with any open-source large-language models,
 deploy to the cloud or on-premises, and build powerful AI apps.
 
 🚂 **State-of-the-art LLMs**: built-in supports a wide range of open-source LLMs
-and model runtime, including StableLM, Falcon, Dolly, Flan-T5, ChatGLM,
+and model runtime, including Llama 2， StableLM, Falcon, Dolly, Flan-T5, ChatGLM,
 StarCoder and more.
 
 🔥 **Flexible APIs**: serve LLMs over RESTful API or gRPC with one command,
 query via WebUI, CLI, our Python/Javascript client, or any HTTP client.
 
 ⛓️ **Freedom To Build**: First-class support for LangChain, BentoML and Hugging
 Face that allows you to easily create your own AI apps by composing LLMs with
@@ -214,17 +214,17 @@
 can experiment with the endpoints and sample input prompts.
 
 OpenLLM provides a built-in Python client, allowing you to interact with the
 model. In a different terminal window or a Jupyter Notebook, create a client to
 start interacting with the model:
 
 ```python
->>> import openllm
->>> client = openllm.client.HTTPClient('http://localhost:3000')
->>> client.query('Explain to me the difference between "further" and "farther"')
+import openllm
+client = openllm.client.HTTPClient('http://localhost:3000')
+client.query('Explain to me the difference between "further" and "farther"')
 ```
 
 You can also use the `openllm query` command to query the model from the
 terminal:
 
 ```bash
 export OPENLLM_ENDPOINT=http://localhost:3000
@@ -609,16 +609,17 @@
 [Adding a New Model Guide](https://github.com/bentoml/OpenLLM/blob/main/ADDING_NEW_MODEL.md)
 to see how you can do it yourself.
 
 ## ⚙️ Integrations
 
 OpenLLM is not just a standalone product; it's a building block designed to
 integrate with other powerful tools easily. We currently offer integration with
-[BentoML](https://github.com/bentoml/BentoML) and
-[LangChain](https://github.com/hwchase17/langchain).
+[BentoML](https://github.com/bentoml/BentoML),
+[LangChain](https://github.com/hwchase17/langchain),
+and [Transformers Agents](https://huggingface.co/docs/transformers/transformers_agents).
 
 ### BentoML
 
 OpenLLM models can be integrated as a
 [Runner](https://docs.bentoml.com/en/latest/concepts/runner.html) in your
 BentoML service. These runners have a `generate` method that takes a string as a
 prompt and returns a corresponding output string. This will allow you to plug
@@ -639,49 +640,14 @@
 
 @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str:
     answer = await llm_runner.generate(input_text)
     return answer
 ```
 
-### Hugging Face Agents
-
-OpenLLM seamlessly integrates with Hugging Face Agents.
-
-> **Warning** The HuggingFace Agent is still at experimental stage. It is
-> recommended to OpenLLM with `pip install -r nightly-requirements.txt` to get
-> the latest API update for HuggingFace agent.
-
-```python
-import transformers
-
-agent = transformers.HfAgent("http://localhost:3000/hf/agent")  # URL that runs the OpenLLM server
-
-agent.run("Is the following `text` positive or negative?", text="I don't like how this models is generate inputs")
-```
-
-> **Note** Only `starcoder` is currently supported with Agent integration. The
-> example above was also ran with four T4s on EC2 `g4dn.12xlarge`
-
-If you want to use OpenLLM client to ask questions to the running agent, you can
-also do so:
-
-```python
-import openllm
-
-client = openllm.client.HTTPClient("http://localhost:3000")
-
-client.ask_agent(
-    task="Is the following `text` positive or negative?",
-    text="What are you thinking about?",
-)
-```
-
-![Gif showing Agent integration](/assets/agent.gif)
-<br/>
 
 ### [LangChain](https://python.langchain.com/docs/ecosystem/integrations/openllm)
 
 To quickly start a local LLM with `langchain`, simply do the following:
 
 ```python
 from langchain.llms import OpenLLM
@@ -719,14 +685,53 @@
 def chat(input_text: str):
     return agent.run(input_text)
 ```
 
 > **Note** You can find out more examples under the
 > [examples](https://github.com/bentoml/OpenLLM/tree/main/examples) folder.
 
+
+### Transformers Agents
+
+OpenLLM seamlessly integrates with [Transformers Agents](https://huggingface.co/docs/transformers/transformers_agents).
+
+
+> **Warning** The Transformers Agent is still at an experimental stage. It is
+> recommended to install OpenLLM with `pip install -r nightly-requirements.txt` to get
+> the latest API update for HuggingFace agent.
+
+```python
+import transformers
+
+agent = transformers.HfAgent("http://localhost:3000/hf/agent")  # URL that runs the OpenLLM server
+
+agent.run("Is the following `text` positive or negative?", text="I don't like how this models is generate inputs")
+```
+
+> **Note** Only `starcoder` is currently supported with Agent integration. The
+> example above was also ran with four T4s on EC2 `g4dn.12xlarge`
+
+If you want to use OpenLLM client to ask questions to the running agent, you can
+also do so:
+
+```python
+import openllm
+
+client = openllm.client.HTTPClient("http://localhost:3000")
+
+client.ask_agent(
+    task="Is the following `text` positive or negative?",
+    text="What are you thinking about?",
+)
+```
+
+![Gif showing Agent integration](/assets/agent.gif)
+<br/>
+
+
 ## 🚀 Deploying to Production
 
 There are several ways to deploy your LLMs:
 
 ### 🐳 Docker container
 
 1. **Building a Bento**: With OpenLLM, you can easily build a Bento for a
@@ -742,19 +747,23 @@
    code, models, files, artefacts, and dependencies.
 
 2. **Containerize your Bento**
 
    ```bash
    bentoml containerize <name:version>
    ```
+   This generates a OCI-compatible docker image that can be deployed anywhere docker runs.
+   For best scalability and reliability of your LLM service in production, we recommend deploy
+   with BentoCloud。
+
 
 ### ☁️ BentoCloud
 
-Deploy your LLMs using [BentoCloud](https://www.bentoml.com/bento-cloud/), the
-production-ready platform for managing and deploying machine learning models.
+Deploy OpenLLM with [BentoCloud](https://www.bentoml.com/bento-cloud/), the
+the serverless cloud for shipping and scaling AI applications.
 
 1. **Create a BentoCloud account:** [sign up here](https://bentoml.com/cloud)
    for early access
 
 2. **Log into your BentoCloud account:**
 
    ```bash
@@ -778,36 +787,15 @@
    bentoml push <name:version>
    ```
 
 5. **Deploying a Bento**: Deploy your LLMs to BentoCloud with a single
    `bentoml deployment create` command following the
    [deployment instructions](https://docs.bentoml.com/en/latest/reference/cli.html#bentoml-deployment-create).
 
-Explore other options for deploying and hosting online ML services at
-[BentoML's Documentation](https://docs.bentoml.com/en/latest/concepts/deploy.html).
 
-## 🍇 Telemetry
-
-OpenLLM collects usage data to enhance user experience and improve the product.
-We only report OpenLLM's internal API calls and ensure maximum privacy by
-excluding sensitive information. We will never collect user code, model data, or
-stack traces. For usage tracking, check out the
-[code](./src/openllm/utils/analytics.py).
-
-You can opt out of usage tracking by using the `--do-not-track` CLI option:
-
-```bash
-openllm [command] --do-not-track
-```
-
-Or by setting the environment variable `OPENLLM_DO_NOT_TRACK=True`:
-
-```bash
-export OPENLLM_DO_NOT_TRACK=True
-```
 
 ## 👥 Community
 
 Engage with like-minded individuals passionate about LLMs, AI, and more on our
 [Discord](https://l.bentoml.com/join-openllm-discord)!
 
 OpenLLM is actively maintained by the BentoML team. Feel free to reach out and
@@ -820,14 +808,34 @@
 capabilities or have any questions, don't hesitate to reach out in our
 [discord channel](https://l.bentoml.com/join-openllm-discord).
 
 Checkout our
 [Developer Guide](https://github.com/bentoml/OpenLLM/blob/main/DEVELOPMENT.md)
 if you wish to contribute to OpenLLM's codebase.
 
+## 🍇 Telemetry
+
+OpenLLM collects usage data to enhance user experience and improve the product.
+We only report OpenLLM's internal API calls and ensure maximum privacy by
+excluding sensitive information. We will never collect user code, model data, or
+stack traces. For usage tracking, check out the
+[code](./src/openllm/utils/analytics.py).
+
+You can opt out of usage tracking by using the `--do-not-track` CLI option:
+
+```bash
+openllm [command] --do-not-track
+```
+
+Or by setting the environment variable `OPENLLM_DO_NOT_TRACK=True`:
+
+```bash
+export OPENLLM_DO_NOT_TRACK=True
+```
+
 ## 📔 Citation
 
 If you use OpenLLM in your research, we provide a [citation](./CITATION.cff) to
 use:
 
 ```bibtex
 @software{Pham_OpenLLM_Operating_LLMs_2023,
```

