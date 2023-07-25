# Comparing `tmp/periflow_client-0.1.0.tar.gz` & `tmp/periflow_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periflow_client-0.1.0.tar", max compression
+gzip compressed data, was "periflow_client-0.1.1.tar", max compression
```

## Comparing `periflow_client-0.1.0.tar` & `periflow_client-0.1.1.tar`

### file list

```diff
@@ -1,80 +1,81 @@
--rw-r--r--   0        0        0     3567 2023-07-20 12:32:34.224062 periflow_client-0.1.0/LICENSE
--rw-r--r--   0        0        0      820 2023-07-20 12:32:34.262789 periflow_client-0.1.0/periflow/__init__.py
--rw-r--r--   0        0        0     4410 2023-07-20 12:32:34.262864 periflow_client-0.1.0/periflow/auth.py
--rw-r--r--   0        0        0      188 2023-07-20 12:32:34.262945 periflow_client-0.1.0/periflow/cli/__init__.py
--rw-r--r--   0        0        0    18967 2023-07-20 12:32:34.263041 periflow_client-0.1.0/periflow/cli/checkpoint.py
--rw-r--r--   0        0        0    10321 2023-07-20 12:32:34.263102 periflow_client-0.1.0/periflow/cli/credential.py
--rw-r--r--   0        0        0    18509 2023-07-20 12:32:34.263198 periflow_client-0.1.0/periflow/cli/deployment.py
--rw-r--r--   0        0        0     5700 2023-07-20 12:32:34.263272 periflow_client-0.1.0/periflow/cli/group.py
--rw-r--r--   0        0        0     2445 2023-07-20 12:32:34.263329 periflow_client-0.1.0/periflow/cli/key.py
--rw-r--r--   0        0        0     6063 2023-07-20 12:32:34.263407 periflow_client-0.1.0/periflow/cli/main.py
--rw-r--r--   0        0        0     9491 2023-07-20 12:32:34.263483 periflow_client-0.1.0/periflow/cli/project.py
--rw-r--r--   0        0        0     1536 2023-07-20 12:32:34.263563 periflow_client-0.1.0/periflow/cli/vm.py
--rw-r--r--   0        0        0      125 2023-07-20 12:32:34.263645 periflow_client-0.1.0/periflow/client/__init__.py
--rw-r--r--   0        0        0    15578 2023-07-20 12:32:34.263735 periflow_client-0.1.0/periflow/client/base.py
--rw-r--r--   0        0        0     2651 2023-07-20 12:32:34.263798 periflow_client-0.1.0/periflow/client/checkpoint.py
--rw-r--r--   0        0        0     2603 2023-07-20 12:32:34.263898 periflow_client-0.1.0/periflow/client/credential.py
--rw-r--r--   0        0        0     7402 2023-07-20 12:32:34.263972 periflow_client-0.1.0/periflow/client/deployment.py
--rw-r--r--   0        0        0     3069 2023-07-20 12:32:34.264036 periflow_client-0.1.0/periflow/client/file.py
--rw-r--r--   0        0        0     5904 2023-07-20 12:32:34.264109 periflow_client-0.1.0/periflow/client/group.py
--rw-r--r--   0        0        0     3581 2023-07-20 12:32:34.264158 periflow_client-0.1.0/periflow/client/project.py
--rw-r--r--   0        0        0     7361 2023-07-20 12:32:34.264235 periflow_client-0.1.0/periflow/client/user.py
--rw-r--r--   0        0        0       98 2023-07-20 12:32:34.264311 periflow_client-0.1.0/periflow/cloud/__init__.py
--rw-r--r--   0        0        0     9622 2023-07-20 12:32:34.264393 periflow_client-0.1.0/periflow/cloud/storage.py
--rw-r--r--   0        0        0      107 2023-07-20 12:32:34.264482 periflow_client-0.1.0/periflow/configurator/__init__.py
--rw-r--r--   0        0        0     1587 2023-07-20 12:32:34.264550 periflow_client-0.1.0/periflow/configurator/base.py
--rw-r--r--   0        0        0     4067 2023-07-20 12:32:34.264648 periflow_client-0.1.0/periflow/configurator/credential.py
--rw-r--r--   0        0        0     3112 2023-07-20 12:32:34.264715 periflow_client-0.1.0/periflow/configurator/deployment.py
--rw-r--r--   0        0        0     1753 2023-07-20 12:32:34.264778 periflow_client-0.1.0/periflow/context.py
--rw-r--r--   0        0        0      105 2023-07-20 12:32:34.264853 periflow_client-0.1.0/periflow/converter/__init__.py
--rw-r--r--   0        0        0    15051 2023-07-20 12:58:47.707975 periflow_client-0.1.0/periflow/converter/base.py
--rw-r--r--   0        0        0     5020 2023-07-20 12:32:34.265037 periflow_client-0.1.0/periflow/converter/interface.py
--rw-r--r--   0        0        0     2397 2023-07-20 12:32:34.265101 periflow_client-0.1.0/periflow/converter/maps.py
--rw-r--r--   0        0        0    13345 2023-07-20 12:32:34.265241 periflow_client-0.1.0/periflow/converter/models/blenderbot.py
--rw-r--r--   0        0        0     8689 2023-07-20 12:32:34.265314 periflow_client-0.1.0/periflow/converter/models/bloom.py
--rw-r--r--   0        0        0     7252 2023-07-20 12:32:34.265389 periflow_client-0.1.0/periflow/converter/models/codegen.py
--rw-r--r--   0        0        0     9706 2023-07-20 12:32:34.265458 periflow_client-0.1.0/periflow/converter/models/falcon.py
--rw-r--r--   0        0        0     7060 2023-07-20 12:32:34.265533 periflow_client-0.1.0/periflow/converter/models/gpt2.py
--rw-r--r--   0        0        0    10454 2023-07-20 12:32:34.265601 periflow_client-0.1.0/periflow/converter/models/gpt_neox.py
--rw-r--r--   0        0        0     7122 2023-07-20 12:32:34.265672 periflow_client-0.1.0/periflow/converter/models/gptj.py
--rw-r--r--   0        0        0     7704 2023-07-20 12:32:34.265761 periflow_client-0.1.0/periflow/converter/models/llama.py
--rw-r--r--   0        0        0     7316 2023-07-20 12:32:34.265844 periflow_client-0.1.0/periflow/converter/models/mpt.py
--rw-r--r--   0        0        0     9390 2023-07-20 12:32:34.265915 periflow_client-0.1.0/periflow/converter/models/opt.py
--rw-r--r--   0        0        0    12615 2023-07-20 12:32:34.265998 periflow_client-0.1.0/periflow/converter/models/t5.py
--rw-r--r--   0        0        0     4456 2023-07-20 12:32:34.266070 periflow_client-0.1.0/periflow/converter/utils.py
--rw-r--r--   0        0        0     3013 2023-07-20 12:32:34.266136 periflow_client-0.1.0/periflow/enums.py
--rw-r--r--   0        0        0     5404 2023-07-20 12:32:34.266214 periflow_client-0.1.0/periflow/errors.py
--rw-r--r--   0        0        0     9505 2023-07-20 12:32:34.266322 periflow_client-0.1.0/periflow/formatter.py
--rw-r--r--   0        0        0      660 2023-07-20 12:32:34.266385 periflow_client-0.1.0/periflow/logging.py
--rw-r--r--   0        0        0       92 2023-07-20 12:32:34.266497 periflow_client-0.1.0/periflow/schema/__init__.py
--rw-r--r--   0        0        0       96 2023-07-20 12:32:34.266643 periflow_client-0.1.0/periflow/schema/api/__init__.py
--rw-r--r--   0        0        0       99 2023-07-20 12:32:34.266768 periflow_client-0.1.0/periflow/schema/api/v1/__init__.py
--rw-r--r--   0        0        0     2828 2023-07-20 12:32:34.266844 periflow_client-0.1.0/periflow/schema/api/v1/completion.py
--rw-r--r--   0        0        0      101 2023-07-20 12:32:34.266958 periflow_client-0.1.0/periflow/schema/resource/__init__.py
--rw-r--r--   0        0        0      104 2023-07-20 12:32:34.267053 periflow_client-0.1.0/periflow/schema/resource/v1/__init__.py
--rw-r--r--   0        0        0     3890 2023-07-20 12:32:34.267126 periflow_client-0.1.0/periflow/schema/resource/v1/attributes.py
--rw-r--r--   0        0        0     2353 2023-07-20 12:32:34.267192 periflow_client-0.1.0/periflow/schema/resource/v1/checkpoint.py
--rw-r--r--   0        0        0     1358 2023-07-20 12:32:34.267258 periflow_client-0.1.0/periflow/schema/resource/v1/credential.py
--rw-r--r--   0        0        0     2027 2023-07-20 12:32:34.267312 periflow_client-0.1.0/periflow/schema/resource/v1/deployment.py
--rw-r--r--   0        0        0       88 2023-07-20 12:32:34.267397 periflow_client-0.1.0/periflow/sdk/__init__.py
--rw-r--r--   0        0        0      102 2023-07-20 12:32:34.267511 periflow_client-0.1.0/periflow/sdk/api/__init__.py
--rw-r--r--   0        0        0     5799 2023-07-20 12:32:34.267596 periflow_client-0.1.0/periflow/sdk/api/base.py
--rw-r--r--   0        0        0    25709 2023-07-20 12:32:34.267670 periflow_client-0.1.0/periflow/sdk/api/completion.py
--rw-r--r--   0        0        0     1836 2023-07-20 12:32:34.267758 periflow_client-0.1.0/periflow/sdk/init.py
--rw-r--r--   0        0        0      112 2023-07-20 12:32:34.267862 periflow_client-0.1.0/periflow/sdk/resource/__init__.py
--rw-r--r--   0        0        0      733 2023-07-20 12:32:34.267911 periflow_client-0.1.0/periflow/sdk/resource/base.py
--rw-r--r--   0        0        0    31343 2023-07-20 12:32:34.268025 periflow_client-0.1.0/periflow/sdk/resource/checkpoint.py
--rw-r--r--   0        0        0     4036 2023-07-20 12:32:34.268103 periflow_client-0.1.0/periflow/sdk/resource/credential.py
--rw-r--r--   0        0        0    17378 2023-07-20 12:32:34.268217 periflow_client-0.1.0/periflow/sdk/resource/deployment.py
--rw-r--r--   0        0        0       97 2023-07-20 12:32:34.268333 periflow_client-0.1.0/periflow/utils/__init__.py
--rw-r--r--   0        0        0     4232 2023-07-20 12:32:34.268415 periflow_client-0.1.0/periflow/utils/format.py
--rw-r--r--   0        0        0    14539 2023-07-20 12:32:34.268558 periflow_client-0.1.0/periflow/utils/fs.py
--rw-r--r--   0        0        0      770 2023-07-20 12:32:34.268623 periflow_client-0.1.0/periflow/utils/maps.py
--rw-r--r--   0        0        0      666 2023-07-20 12:32:34.268678 periflow_client-0.1.0/periflow/utils/prompt.py
--rw-r--r--   0        0        0     2265 2023-07-20 12:32:34.268742 periflow_client-0.1.0/periflow/utils/request.py
--rw-r--r--   0        0        0     1384 2023-07-20 12:32:34.268808 periflow_client-0.1.0/periflow/utils/testing.py
--rw-r--r--   0        0        0     1485 2023-07-20 12:32:34.268869 periflow_client-0.1.0/periflow/utils/url.py
--rw-r--r--   0        0        0     3552 2023-07-20 12:32:34.268951 periflow_client-0.1.0/periflow/utils/validate.py
--rw-r--r--   0        0        0     1513 2023-07-20 12:32:34.269017 periflow_client-0.1.0/periflow/utils/version.py
--rw-r--r--   0        0        0     3167 2023-07-20 12:59:05.280230 periflow_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1401 1970-01-01 00:00:00.000000 periflow_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3501 2023-07-25 04:03:34.042855 periflow_client-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7948 2023-07-20 12:32:34.224165 periflow_client-0.1.1/README.md
+-rw-r--r--   0        0        0      820 2023-07-20 12:32:34.262789 periflow_client-0.1.1/periflow/__init__.py
+-rw-r--r--   0        0        0     4410 2023-07-20 12:32:34.262864 periflow_client-0.1.1/periflow/auth.py
+-rw-r--r--   0        0        0      188 2023-07-20 12:32:34.262945 periflow_client-0.1.1/periflow/cli/__init__.py
+-rw-r--r--   0        0        0    19009 2023-07-25 03:49:51.897018 periflow_client-0.1.1/periflow/cli/checkpoint.py
+-rw-r--r--   0        0        0    10321 2023-07-20 12:32:34.263102 periflow_client-0.1.1/periflow/cli/credential.py
+-rw-r--r--   0        0        0    18875 2023-07-25 03:49:56.899224 periflow_client-0.1.1/periflow/cli/deployment.py
+-rw-r--r--   0        0        0     5700 2023-07-20 12:32:34.263272 periflow_client-0.1.1/periflow/cli/group.py
+-rw-r--r--   0        0        0     2445 2023-07-20 12:32:34.263329 periflow_client-0.1.1/periflow/cli/key.py
+-rw-r--r--   0        0        0     6077 2023-07-25 04:03:34.043963 periflow_client-0.1.1/periflow/cli/main.py
+-rw-r--r--   0        0        0     9491 2023-07-20 12:32:34.263483 periflow_client-0.1.1/periflow/cli/project.py
+-rw-r--r--   0        0        0     1676 2023-07-25 03:49:56.899466 periflow_client-0.1.1/periflow/cli/vm.py
+-rw-r--r--   0        0        0      125 2023-07-20 12:32:34.263645 periflow_client-0.1.1/periflow/client/__init__.py
+-rw-r--r--   0        0        0    15578 2023-07-20 12:32:34.263735 periflow_client-0.1.1/periflow/client/base.py
+-rw-r--r--   0        0        0     2651 2023-07-20 12:32:34.263798 periflow_client-0.1.1/periflow/client/checkpoint.py
+-rw-r--r--   0        0        0     2603 2023-07-20 12:32:34.263898 periflow_client-0.1.1/periflow/client/credential.py
+-rw-r--r--   0        0        0     7402 2023-07-20 12:32:34.263972 periflow_client-0.1.1/periflow/client/deployment.py
+-rw-r--r--   0        0        0     3069 2023-07-20 12:32:34.264036 periflow_client-0.1.1/periflow/client/file.py
+-rw-r--r--   0        0        0     5904 2023-07-20 12:32:34.264109 periflow_client-0.1.1/periflow/client/group.py
+-rw-r--r--   0        0        0     3581 2023-07-20 12:32:34.264158 periflow_client-0.1.1/periflow/client/project.py
+-rw-r--r--   0        0        0     7361 2023-07-20 12:32:34.264235 periflow_client-0.1.1/periflow/client/user.py
+-rw-r--r--   0        0        0       98 2023-07-20 12:32:34.264311 periflow_client-0.1.1/periflow/cloud/__init__.py
+-rw-r--r--   0        0        0     9622 2023-07-20 12:32:34.264393 periflow_client-0.1.1/periflow/cloud/storage.py
+-rw-r--r--   0        0        0      107 2023-07-20 12:32:34.264482 periflow_client-0.1.1/periflow/configurator/__init__.py
+-rw-r--r--   0        0        0     1587 2023-07-20 12:32:34.264550 periflow_client-0.1.1/periflow/configurator/base.py
+-rw-r--r--   0        0        0     4067 2023-07-20 12:32:34.264648 periflow_client-0.1.1/periflow/configurator/credential.py
+-rw-r--r--   0        0        0     3112 2023-07-20 12:32:34.264715 periflow_client-0.1.1/periflow/configurator/deployment.py
+-rw-r--r--   0        0        0     1753 2023-07-20 12:32:34.264778 periflow_client-0.1.1/periflow/context.py
+-rw-r--r--   0        0        0      105 2023-07-20 12:32:34.264853 periflow_client-0.1.1/periflow/converter/__init__.py
+-rw-r--r--   0        0        0    15051 2023-07-20 12:58:47.707975 periflow_client-0.1.1/periflow/converter/base.py
+-rw-r--r--   0        0        0     5020 2023-07-20 12:32:34.265037 periflow_client-0.1.1/periflow/converter/interface.py
+-rw-r--r--   0        0        0     2397 2023-07-20 12:32:34.265101 periflow_client-0.1.1/periflow/converter/maps.py
+-rw-r--r--   0        0        0    13345 2023-07-20 12:32:34.265241 periflow_client-0.1.1/periflow/converter/models/blenderbot.py
+-rw-r--r--   0        0        0     8689 2023-07-20 12:32:34.265314 periflow_client-0.1.1/periflow/converter/models/bloom.py
+-rw-r--r--   0        0        0     7252 2023-07-20 12:32:34.265389 periflow_client-0.1.1/periflow/converter/models/codegen.py
+-rw-r--r--   0        0        0     9706 2023-07-20 12:32:34.265458 periflow_client-0.1.1/periflow/converter/models/falcon.py
+-rw-r--r--   0        0        0     7060 2023-07-20 12:32:34.265533 periflow_client-0.1.1/periflow/converter/models/gpt2.py
+-rw-r--r--   0        0        0    10454 2023-07-20 12:32:34.265601 periflow_client-0.1.1/periflow/converter/models/gpt_neox.py
+-rw-r--r--   0        0        0     7122 2023-07-20 12:32:34.265672 periflow_client-0.1.1/periflow/converter/models/gptj.py
+-rw-r--r--   0        0        0     7916 2023-07-25 03:49:51.897974 periflow_client-0.1.1/periflow/converter/models/llama.py
+-rw-r--r--   0        0        0     7316 2023-07-20 12:32:34.265844 periflow_client-0.1.1/periflow/converter/models/mpt.py
+-rw-r--r--   0        0        0     9390 2023-07-20 12:32:34.265915 periflow_client-0.1.1/periflow/converter/models/opt.py
+-rw-r--r--   0        0        0    12615 2023-07-20 12:32:34.265998 periflow_client-0.1.1/periflow/converter/models/t5.py
+-rw-r--r--   0        0        0     4456 2023-07-20 12:32:34.266070 periflow_client-0.1.1/periflow/converter/utils.py
+-rw-r--r--   0        0        0     3318 2023-07-25 03:49:56.899802 periflow_client-0.1.1/periflow/enums.py
+-rw-r--r--   0        0        0     5404 2023-07-20 12:32:34.266214 periflow_client-0.1.1/periflow/errors.py
+-rw-r--r--   0        0        0     9505 2023-07-20 12:32:34.266322 periflow_client-0.1.1/periflow/formatter.py
+-rw-r--r--   0        0        0      660 2023-07-20 12:32:34.266385 periflow_client-0.1.1/periflow/logging.py
+-rw-r--r--   0        0        0       92 2023-07-20 12:32:34.266497 periflow_client-0.1.1/periflow/schema/__init__.py
+-rw-r--r--   0        0        0       96 2023-07-20 12:32:34.266643 periflow_client-0.1.1/periflow/schema/api/__init__.py
+-rw-r--r--   0        0        0       99 2023-07-20 12:32:34.266768 periflow_client-0.1.1/periflow/schema/api/v1/__init__.py
+-rw-r--r--   0        0        0     2828 2023-07-20 12:32:34.266844 periflow_client-0.1.1/periflow/schema/api/v1/completion.py
+-rw-r--r--   0        0        0      101 2023-07-20 12:32:34.266958 periflow_client-0.1.1/periflow/schema/resource/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-20 12:32:34.267053 periflow_client-0.1.1/periflow/schema/resource/v1/__init__.py
+-rw-r--r--   0        0        0     3912 2023-07-25 03:49:51.898529 periflow_client-0.1.1/periflow/schema/resource/v1/attributes.py
+-rw-r--r--   0        0        0     2353 2023-07-20 12:32:34.267192 periflow_client-0.1.1/periflow/schema/resource/v1/checkpoint.py
+-rw-r--r--   0        0        0     1358 2023-07-20 12:32:34.267258 periflow_client-0.1.1/periflow/schema/resource/v1/credential.py
+-rw-r--r--   0        0        0     2027 2023-07-20 12:32:34.267312 periflow_client-0.1.1/periflow/schema/resource/v1/deployment.py
+-rw-r--r--   0        0        0       88 2023-07-20 12:32:34.267397 periflow_client-0.1.1/periflow/sdk/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-20 12:32:34.267511 periflow_client-0.1.1/periflow/sdk/api/__init__.py
+-rw-r--r--   0        0        0     5799 2023-07-20 12:32:34.267596 periflow_client-0.1.1/periflow/sdk/api/base.py
+-rw-r--r--   0        0        0    25709 2023-07-20 12:32:34.267670 periflow_client-0.1.1/periflow/sdk/api/completion.py
+-rw-r--r--   0        0        0     1836 2023-07-20 12:32:34.267758 periflow_client-0.1.1/periflow/sdk/init.py
+-rw-r--r--   0        0        0      112 2023-07-20 12:32:34.267862 periflow_client-0.1.1/periflow/sdk/resource/__init__.py
+-rw-r--r--   0        0        0      733 2023-07-20 12:32:34.267911 periflow_client-0.1.1/periflow/sdk/resource/base.py
+-rw-r--r--   0        0        0    31401 2023-07-25 03:49:51.898894 periflow_client-0.1.1/periflow/sdk/resource/checkpoint.py
+-rw-r--r--   0        0        0     4036 2023-07-20 12:32:34.268103 periflow_client-0.1.1/periflow/sdk/resource/credential.py
+-rw-r--r--   0        0        0    17719 2023-07-25 03:49:56.900175 periflow_client-0.1.1/periflow/sdk/resource/deployment.py
+-rw-r--r--   0        0        0       97 2023-07-20 12:32:34.268333 periflow_client-0.1.1/periflow/utils/__init__.py
+-rw-r--r--   0        0        0     4232 2023-07-20 12:32:34.268415 periflow_client-0.1.1/periflow/utils/format.py
+-rw-r--r--   0        0        0    14539 2023-07-20 12:32:34.268558 periflow_client-0.1.1/periflow/utils/fs.py
+-rw-r--r--   0        0        0     1303 2023-07-25 03:49:56.900640 periflow_client-0.1.1/periflow/utils/maps.py
+-rw-r--r--   0        0        0      666 2023-07-20 12:32:34.268678 periflow_client-0.1.1/periflow/utils/prompt.py
+-rw-r--r--   0        0        0     2265 2023-07-20 12:32:34.268742 periflow_client-0.1.1/periflow/utils/request.py
+-rw-r--r--   0        0        0     1384 2023-07-20 12:32:34.268808 periflow_client-0.1.1/periflow/utils/testing.py
+-rw-r--r--   0        0        0     1485 2023-07-20 12:32:34.268869 periflow_client-0.1.1/periflow/utils/url.py
+-rw-r--r--   0        0        0     3552 2023-07-20 12:32:34.268951 periflow_client-0.1.1/periflow/utils/validate.py
+-rw-r--r--   0        0        0     1513 2023-07-20 12:32:34.269017 periflow_client-0.1.1/periflow/utils/version.py
+-rw-r--r--   0        0        0     3339 2023-07-25 04:03:34.044242 periflow_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9600 1970-01-01 00:00:00.000000 periflow_client-0.1.1/PKG-INFO
```

### Comparing `periflow_client-0.1.0/LICENSE` & `periflow_client-0.1.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright (c) 2022-present, FriendliAI Inc. All rights reserved.
-
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
```

### Comparing `periflow_client-0.1.0/periflow/__init__.py` & `periflow_client-0.1.1/periflow/__init__.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/auth.py` & `periflow_client-0.1.1/periflow/auth.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/cli/checkpoint.py` & `periflow_client-0.1.1/periflow/cli/checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,15 @@
 
     # llama
     model_type: llama
     dtype: fp16
     head_size: 128
     rotary_dim: 128
     num_heads: 32
+    num_kv_heads: 32
     num_layers: 32
     ff_intermediate_size: 11008
     max_length: 2048
     vocab_size: 32000
     eos_token: 1
 
     # opt
@@ -506,14 +507,15 @@
 
     # llama
     model_type: llama
     dtype: fp16
     head_size: 128
     rotary_dim: 128
     num_heads: 32
+    num_kv_heads: 32
     num_layers: 32
     ff_intermediate_size: 11008
     max_length: 2048
     vocab_size: 32000
     eos_token: 1
 
     # opt
```

### Comparing `periflow_client-0.1.0/periflow/cli/credential.py` & `periflow_client-0.1.1/periflow/cli/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/cli/deployment.py` & `periflow_client-0.1.1/periflow/cli/deployment.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from uuid import UUID
 
 import typer
 import yaml
 from dateutil.parser import parse
 
 from periflow.client.user import UserGroupProjectClient
-from periflow.enums import CloudType, DeploymentSecurityLevel, DeploymentType, GpuType
+from periflow.enums import CloudType, DeploymentSecurityLevel, DeploymentType, VMType
 from periflow.errors import (
     AuthenticationError,
     EntityTooLargeError,
     InvalidConfigError,
     LowServicePlanError,
 )
 from periflow.formatter import PanelFormatter, TableFormatter
@@ -32,14 +32,17 @@
 
 app = typer.Typer(
     no_args_is_help=True,
     context_settings={"help_option_names": ["-h", "--help"]},
     add_completion=False,
 )
 
+DEFAULT_MAX_BATCH_SIZE = 256
+DEFAULT_MAX_TOKEN_COUNT = 8192
+
 deployment_panel = PanelFormatter(
     name="Deployment Overview",
     fields=[
         "deployment_id",
         "config.name",
         "description",
         "config.deployment_type",
@@ -54,14 +57,16 @@
         "start",
         "end",
         "security_level",
         "config.infrequest_log",
         "endpoint",
         "config.cloud",
         "config.region",
+        "config.orca_config.max_batch_size",
+        "config.orca_config.max_token_count",
     ],
     headers=[
         "ID",
         "Name",
         "Description",
         "Type",
         "Ckpt ID",
@@ -75,39 +80,39 @@
         "Start",
         "End",
         "Security Level",
         "Logging",
         "Endpoint",
         "Cloud",
         "Region",
+        "Max batch size",
+        "Max token count",
     ],
     extra_fields=["error"],
     extra_headers=["error"],
     substitute_exact_match_only=False,
 )
 
 deployment_table = TableFormatter(
     name="Deployments",
     fields=[
         "deployment_id",
         "config.name",
-        "description",
         "status",
         "ready_replicas",
         "vms",
         "config.vm.gpu_type",
         "config.total_gpus",
         "start",
         "config.cloud",
         "config.region",
     ],
     headers=[
         "ID",
         "Name",
-        "Description",
         "Status",
         "#Ready",
         "VM Type",
         "GPU Type",
         "#GPUs",
         "Start",
         "Cloud",
@@ -119,30 +124,28 @@
 )
 
 deployment_org_table = TableFormatter(
     name="Deployments",
     fields=[
         "deployment_id",
         "config.name",
-        "description",
         "status",
         "ready_replicas",
         "vms",
         "config.vm.gpu_type",
         "config.total_gpus",
         "start",
         "config.cloud",
         "config.region",
         "config.project_id",
         "project_name",
     ],
     headers=[
         "ID",
         "Name",
-        "Description",
         "Status",
         "#Ready",
         "VM Type",
         "GPU Type",
         "#GPUs",
         "Start",
         "Cloud",
@@ -409,21 +412,21 @@
 def create(
     checkpoint_id: UUID = typer.Option(
         ..., "--checkpoint-id", "-i", help="Checkpoint id to deploy."
     ),
     deployment_name: str = typer.Option(
         ..., "--name", "-n", help="The name of deployment. "
     ),
-    gpu_type: GpuType = typer.Option(
-        ..., "--gpu-type", "-g", help="The GPU type for the deployment."
+    vm_type: VMType = typer.Option(
+        ..., "--vm-type", "-v", help="The VM type for the deployment."
     ),
     cloud: CloudType = typer.Option(..., "--cloud", "-c", help="Type of cloud."),
     region: str = typer.Option(..., "--region", "-r", help="Region of cloud."),
-    config_file: typer.FileText = typer.Option(
-        ..., "--config-file", "-f", help="Path to configuration file."
+    config_file: Optional[typer.FileText] = typer.Option(
+        None, "--config-file", "-f", help="Path to configuration file."
     ),
     deployment_type: DeploymentType = typer.Option(
         DeploymentType.PROD, "--type", "-t", help="Type of deployment."
     ),
     description: Optional[str] = typer.Option(
         None, "--description", "-d", help="Deployment description."
     ),
@@ -471,15 +474,15 @@
 
     :::tip
     To turn off the deployment autoscaling, set `--min-replicas` and
     `--max-replicas` to the same value.
     :::
 
     :::tip
-    Use `pf vm list -s deployment` to find available cloud, region, and gpu-type.
+    Use `pf vm list` to find available vm-type, cloud, region, and gpu-type.
     :::
 
     The default request-response configuration, such as stop tokens or bad words, is
     defined in a YAML file. The path of that file is passed to the `-drc` option.
     The format of the file is as follows.
 
     ```json
@@ -494,29 +497,38 @@
     :::caution
     Both `bad_words` and `bad_word_tokens` cannot be set at the same time. Also, both
     `stop` and `stop_tokens` cannot be set at the same time.
     :::
 
     """
     default_request_config = None
-    try:
-        config: Dict[str, Any] = yaml.safe_load(config_file)
-        if default_request_config_file is not None:
-            default_request_config = yaml.safe_load(default_request_config_file)
-    except yaml.YAMLError as e:
-        secho_error_and_exit(f"Error occurred while parsing engine config file... {e}")
+    config: Dict[str, Any] = {}
+    if config_file:
+        try:
+            config = yaml.safe_load(config_file)
+            if default_request_config_file is not None:
+                default_request_config = yaml.safe_load(default_request_config_file)
+        except yaml.YAMLError as e:
+            secho_error_and_exit(
+                f"Error occurred while parsing engine config file... {e}"
+            )
+    else:
+        config["orca_config"] = {
+            "max_batch_size": DEFAULT_MAX_BATCH_SIZE,
+            "max_token_count": DEFAULT_MAX_TOKEN_COUNT,
+        }
 
     try:
         deployment = DeploymentAPI.create(
             checkpoint_id=checkpoint_id,
             name=deployment_name,
             deployment_type=deployment_type,
-            gpu_type=gpu_type,
             cloud=cloud,
             region=region,
+            vm_type=vm_type,
             config=config,
             description=description,
             default_request_config=default_request_config,
             security_level=security_level,
             logging=logging,
             min_replicas=min_replicas,
             max_replicas=max_replicas,
```

### Comparing `periflow_client-0.1.0/periflow/cli/group.py` & `periflow_client-0.1.1/periflow/cli/group.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/cli/key.py` & `periflow_client-0.1.1/periflow/cli/key.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/cli/main.py` & `periflow_client-0.1.1/periflow/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from periflow.utils.format import secho_error_and_exit
 from periflow.utils.request import DEFAULT_REQ_TIMEOUT
 from periflow.utils.url import get_training_uri
 from periflow.utils.validate import validate_cli_version
 from periflow.utils.version import get_installed_version
 
 app = typer.Typer(
-    help="Welcome to PeriFlow 🤗",
+    help="Supercharge Generative AI Serving 🚀",
     no_args_is_help=True,
     context_settings={"help_option_names": ["-h", "--help"]},
     add_completion=False,
     callback=validate_cli_version,
 )
 
 app.add_typer(credential.app, name="credential", help="Manage credentials")
```

### Comparing `periflow_client-0.1.0/periflow/cli/project.py` & `periflow_client-0.1.1/periflow/cli/project.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/cli/vm.py` & `periflow_client-0.1.1/periflow/cli/vm.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,26 +21,30 @@
     add_completion=False,
     deprecated=True,
 )
 
 serving_vm_formatter = TableFormatter(
     name="Serving VM instances",
     fields=[
-        "vm.name",
         "cloud",
+        "region",
         "gpu_type",
+        "vm.name",
         "vm.total_gpus",
-        "region",
+        "vm.vcpu",
+        "memory",
     ],
     headers=[
-        "VM",
         "Cloud",
-        "GPU",
-        "GPU Count",
         "Region",
+        "GPU type",
+        "VM type",
+        "GPU",
+        "vCPUs",
+        "Memory (GiB)",
     ],
 )
 
 
 # pylint: disable=redefined-builtin
 @app.command()
 def list():
@@ -50,13 +54,14 @@
 
     vm_dict_list = [
         {
             "cloud": nodegroup_list_dict["cloud"].upper(),
             "region": nodegroup_list_dict["region"],
             "vm": nodegroup["vm"],
             "gpu_type": nodegroup["vm"]["gpu_type"].upper(),
+            "memory": int(nodegroup["vm"]["cpu_memory"]),
         }
         for nodegroup_list_dict in response
         for nodegroup in nodegroup_list_dict["nodegroup_list"]
         if nodegroup["vm"]["gpu_type"] in [gpu_type.value for gpu_type in GpuType]
     ]
     serving_vm_formatter.render(vm_dict_list)
```

### Comparing `periflow_client-0.1.0/periflow/client/base.py` & `periflow_client-0.1.1/periflow/client/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/client/checkpoint.py` & `periflow_client-0.1.1/periflow/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/client/credential.py` & `periflow_client-0.1.1/periflow/client/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/client/deployment.py` & `periflow_client-0.1.1/periflow/client/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/client/file.py` & `periflow_client-0.1.1/periflow/client/file.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/client/group.py` & `periflow_client-0.1.1/periflow/client/group.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/client/project.py` & `periflow_client-0.1.1/periflow/client/project.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/client/user.py` & `periflow_client-0.1.1/periflow/client/user.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/cloud/storage.py` & `periflow_client-0.1.1/periflow/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/configurator/base.py` & `periflow_client-0.1.1/periflow/configurator/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/configurator/credential.py` & `periflow_client-0.1.1/periflow/configurator/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/configurator/deployment.py` & `periflow_client-0.1.1/periflow/configurator/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/context.py` & `periflow_client-0.1.1/periflow/context.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/base.py` & `periflow_client-0.1.1/periflow/converter/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/interface.py` & `periflow_client-0.1.1/periflow/converter/interface.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/maps.py` & `periflow_client-0.1.1/periflow/converter/maps.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/models/blenderbot.py` & `periflow_client-0.1.1/periflow/converter/models/blenderbot.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/models/bloom.py` & `periflow_client-0.1.1/periflow/converter/models/bloom.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/models/codegen.py` & `periflow_client-0.1.1/periflow/converter/models/codegen.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/models/falcon.py` & `periflow_client-0.1.1/periflow/converter/models/falcon.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/models/gpt2.py` & `periflow_client-0.1.1/periflow/converter/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/models/gpt_neox.py` & `periflow_client-0.1.1/periflow/converter/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/models/gptj.py` & `periflow_client-0.1.1/periflow/converter/models/gptj.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/models/llama.py` & `periflow_client-0.1.1/periflow/converter/models/llama.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,26 +67,26 @@
 
         q_weight = q_weight.reshape(
             self.decoder_num_attention_heads,
             self.decoder_head_size,
             self.decoder_hidden_size,
         )
         k_weight = k_weight.reshape(
-            self.decoder_num_attention_heads,
+            self.decoder_num_kv_attention_heads,
             self.decoder_head_size,
             self.decoder_hidden_size,
         )
         q_weight = convert_to_gpt_j_params(q_weight, self.rotary_dim)
         k_weight = convert_to_gpt_j_params(k_weight, self.rotary_dim)
         q_weight = q_weight.reshape(
             self.decoder_num_attention_heads * self.decoder_head_size,
             self.decoder_hidden_size,
         )
         k_weight = k_weight.reshape(
-            self.decoder_num_attention_heads * self.decoder_head_size,
+            self.decoder_num_kv_attention_heads * self.decoder_head_size,
             self.decoder_hidden_size,
         )
 
         qkv_weight = torch.cat([q_weight, k_weight, v_weight], dim=0)
         qkv_weight = qkv_weight.transpose(0, -1)
         return convert_tensor_to_np_array(qkv_weight, self.data_type)
 
@@ -104,14 +104,15 @@
         eos_token_id = self.get_eos_token_id()
         attr = {
             "model_type": self.model_type,
             "dtype": self.data_type.value,
             "head_size": self.decoder_head_size,
             "rotary_dim": self.rotary_dim,
             "num_heads": self.decoder_num_attention_heads,
+            "num_kv_heads": self.decoder_num_kv_attention_heads,
             "num_layers": self.decoder_layer_num,
             "ff_intermediate_size": config.intermediate_size,
             "max_length": config.max_position_embeddings,
             "vocab_size": config.vocab_size,
             "eos_token": eos_token_id if eos_token_id is not None else "FILL ME",
         }
         return attr
@@ -197,15 +198,18 @@
     def decoder_num_attention_heads(self) -> int:
         """The number of attention heads in LLaMA."""
         return cast(LlamaConfig, self.config).num_attention_heads
 
     @property
     def decoder_num_kv_attention_heads(self) -> int:
         """The number of key-value attention heads in LLaMA."""
-        return self.decoder_num_attention_heads
+        config = cast(LlamaConfig, self.config)
+        if config.num_key_value_heads is None:
+            return self.decoder_num_attention_heads
+        return config.num_key_value_heads
 
     @property
     def decoder_head_size(self) -> int:
         """The head size of LLaMA."""
         return self.decoder_hidden_size // self.decoder_num_attention_heads
 
     @property
```

### Comparing `periflow_client-0.1.0/periflow/converter/models/mpt.py` & `periflow_client-0.1.1/periflow/converter/models/mpt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/models/opt.py` & `periflow_client-0.1.1/periflow/converter/models/opt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/models/t5.py` & `periflow_client-0.1.1/periflow/converter/models/t5.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/converter/utils.py` & `periflow_client-0.1.1/periflow/converter/utils.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/enums.py` & `periflow_client-0.1.1/periflow/enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,26 @@
 
 
 class GpuType(str, Enum):
     """GPU types for deployment."""
 
     A10G = "a10g"
     A100 = "a100"
+    A100_80G = "a100-80g"
+
+
+class VMType(str, Enum):
+    """VM types for deployment."""
+
+    G5_XLARGE = "g5.xlarge"
+    A2_HIGHGPU_1G = "a2-highgpu-1g"
+    A2_ULTRAGPU_1G = "a2-ultragpu-1g"
+    A2_ULTRAGPU_2G = "a2-ultragpu-2g"
+    A2_ULTRAGPU_4G = "a2-ultragpu-4g"
+    A2_ULTRAGPU_8G = "a2-ultragpu-8g"
 
 
 class DeploymentType(str, Enum):
     """Deployment phase types."""
 
     DEV = "dev"
     PROD = "prod"
```

### Comparing `periflow_client-0.1.0/periflow/errors.py` & `periflow_client-0.1.1/periflow/errors.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/formatter.py` & `periflow_client-0.1.1/periflow/formatter.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/logging.py` & `periflow_client-0.1.1/periflow/logging.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/schema/api/v1/completion.py` & `periflow_client-0.1.1/periflow/schema/api/v1/completion.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/schema/resource/v1/attributes.py` & `periflow_client-0.1.1/periflow/schema/resource/v1/attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 class V1LlamaAttributes(V1CommonAttributes):
     """V1 LLaMA attributes schema."""
 
     model_type: Literal["llama"]
     head_size: int
     rotary_dim: int
     num_heads: int
+    num_kv_heads: int
     num_layers: int
     ff_intermediate_size: int
     max_length: int
     vocab_size: int
     eos_token: int
```

### Comparing `periflow_client-0.1.0/periflow/schema/resource/v1/checkpoint.py` & `periflow_client-0.1.1/periflow/schema/resource/v1/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/schema/resource/v1/credential.py` & `periflow_client-0.1.1/periflow/schema/resource/v1/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/schema/resource/v1/deployment.py` & `periflow_client-0.1.1/periflow/schema/resource/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/sdk/api/base.py` & `periflow_client-0.1.1/periflow/sdk/api/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/sdk/api/completion.py` & `periflow_client-0.1.1/periflow/sdk/api/completion.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/sdk/init.py` & `periflow_client-0.1.1/periflow/sdk/init.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/sdk/resource/base.py` & `periflow_client-0.1.1/periflow/sdk/resource/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/sdk/resource/checkpoint.py` & `periflow_client-0.1.1/periflow/sdk/resource/checkpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,14 +171,15 @@
 
             # llama
             model_type: llama
             dtype: fp16
             head_size: 128
             rotary_dim: 128
             num_heads: 32
+            num_kv_heads: 32
             num_layers: 32
             ff_intermediate_size: 11008
             max_length: 2048
             vocab_size: 32000
             eos_token: 1
 
             # opt
@@ -509,14 +510,15 @@
 
             # llama
             model_type: llama
             dtype: fp16
             head_size: 128
             rotary_dim: 128
             num_heads: 32
+            num_kv_heads: 32
             num_layers: 32
             ff_intermediate_size: 11008
             max_length: 2048
             vocab_size: 32000
             eos_token: 1
 
             # opt
```

### Comparing `periflow_client-0.1.0/periflow/sdk/resource/credential.py` & `periflow_client-0.1.1/periflow/sdk/resource/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/sdk/resource/deployment.py` & `periflow_client-0.1.1/periflow/sdk/resource/deployment.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,59 +28,60 @@
 from periflow.client.group import GroupClient
 from periflow.configurator.deployment import DRCConfigurator, OrcaDeploymentConfigurator
 from periflow.context import get_current_group_id, get_current_project_id
 from periflow.enums import (
     CloudType,
     DeploymentSecurityLevel,
     DeploymentType,
-    GpuType,
     ServiceTier,
+    VMType,
 )
 from periflow.errors import (
     AuthenticationError,
     EntityTooLargeError,
     InvalidConfigError,
     InvalidPathError,
     LowServicePlanError,
     NotFoundError,
 )
 from periflow.logging import logger
 from periflow.schema.resource.v1.deployment import V1Deployment
 from periflow.sdk.resource.base import ResourceAPI
 from periflow.utils.format import extract_datetime_part, extract_deployment_id_part
 from periflow.utils.fs import download_file, upload_file
+from periflow.utils.maps import cloud_vm_map, vm_num_gpu_map
 
 
 class Deployment(ResourceAPI[V1Deployment, str]):
     """Deployment resource API."""
 
     @staticmethod
     def create(
         checkpoint_id: UUID,
         name: str,
-        gpu_type: GpuType,
         cloud: CloudType,
         region: str,
+        vm_type: VMType,
         config: Dict[str, Any],
         deployment_type: DeploymentType = DeploymentType.PROD,
         description: Optional[str] = None,
         default_request_config: Optional[Dict[str, Any]] = None,
         security_level: DeploymentSecurityLevel = DeploymentSecurityLevel.PUBLIC,
         logging: bool = False,
         min_replicas: int = 1,
         max_replicas: int = 1,
     ) -> V1Deployment:
         """Creates a new deployment.
 
         Args:
             checkpoint_id (UUID): ID of checkpoint to deploy.
             name (str): The name of deployment.
-            gpu_type (GpuType): Type of GPU.
             cloud (CloudType): Type of cloud provider.
             region (str): Cloud region to create a deployment.
+            vm_type (VMType): Type of VM.
             config (Dict[str, Any]): Deployment configuration.
             deployment_type (DeploymentType, optional): Type of deployment. Defaults to DeploymentType.PROD.
             description (Optional[str], optional): Optional long description for the deployment. Defaults to None.
             default_request_config (Optional[Dict[str, Any]], optional): Default request configuration (e.g., stop words, bad words). Defaults to None.
             security_level (DeploymentSecurityLevel, optional): Security level of deployment endpoint. Defaults to DeploymentSecurityLevel.PUBLIC.
             logging (bool, optional): When True, enables request-response logging for the deployment if it is set. Defaults to False.
             min_replicas (int, optional): The number of minimum replicas. Defaults to 1.
@@ -175,14 +176,19 @@
             )
 
         if min_replicas > max_replicas:
             raise InvalidConfigError(
                 f"Should be min_replicas('{min_replicas}') <= max_replicas('{max_replicas}')."
             )
 
+        if vm_type not in cloud_vm_map[cloud]:
+            raise InvalidConfigError(
+                f"VM type {vm_type.value} is not supported in cloud {cloud.value}."
+            )
+
         deploy_configurator = OrcaDeploymentConfigurator(config=config)
         deploy_configurator.validate()
 
         if default_request_config is not None:
             drc_configurator = DRCConfigurator(config=default_request_config)
             drc_configurator.validate()
 
@@ -223,27 +229,30 @@
                         file_path=drc_file_path,
                         url=upload_url,
                         ctx=t,
                     )
                 file_client.make_misc_file_uploaded(misc_file_id=file_id)
                 config["orca_config"]["default_request_config_id"] = file_id
 
+        num_gpus = vm_num_gpu_map[vm_type]
+        config["orca_config"]["num_devices"] = num_gpus
+
         config["scaler_config"] = {}
         config["scaler_config"]["min_replica_count"] = min_replicas
         config["scaler_config"]["max_replica_count"] = max_replicas
 
         request_data = {
             "project_id": str(project_id),
             "model_id": str(checkpoint_id),
             "deployment_type": deployment_type.value,
             "name": name,
-            "vm": {"gpu_type": gpu_type.value},
+            "vm": {"name": vm_type.value},
             "cloud": cloud.value,
             "region": region,
-            "total_gpus": 1,
+            "total_gpus": num_gpus,
             "infrequest_perm_check": security_level
             == DeploymentSecurityLevel.PROTECTED,
             "infrequest_log": logging,
             **config,
         }
         if description:
             request_data["description"] = description
```

### Comparing `periflow_client-0.1.0/periflow/utils/format.py` & `periflow_client-0.1.1/periflow/utils/format.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/utils/fs.py` & `periflow_client-0.1.1/periflow/utils/fs.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/utils/prompt.py` & `periflow_client-0.1.1/periflow/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/utils/request.py` & `periflow_client-0.1.1/periflow/utils/request.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/utils/testing.py` & `periflow_client-0.1.1/periflow/utils/testing.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/utils/url.py` & `periflow_client-0.1.1/periflow/utils/url.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/utils/validate.py` & `periflow_client-0.1.1/periflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/periflow/utils/version.py` & `periflow_client-0.1.1/periflow/utils/version.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.0/pyproject.toml` & `periflow_client-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 [tool.poetry]
 name = "periflow-client"
-version = "0.1.0"
-description = "PeriFlow is a reliable, speedy, and efficient service for training and serving your own Generative AI models on any data of your choice."
+version = "0.1.1"
+description = "Client of PeriFlow, the fastest generative AI serving available."
+license = "Apache-2.0"
 authors = ["PeriFlow teams <eng@friendli.ai>"]
-packages = [{include = "periflow"}]
+packages = [
+    { include = "periflow" },
+]
+readme = "README.md"
+homepage = "https://docs.periflow.ai/"
+repository = "https://github.com/friendliai/periflow-client"
+documentation = "https://docs.periflow.ai/"
+keywords = ["generative-ai", "serving", "llm"]
 
 [tool.poetry.scripts]
 pf = "periflow.cli:app"
 
 [build-system]
 requires = ["poetry-core>=1.6.1"]
 build-backend = "poetry.core.masonry.api"
```

