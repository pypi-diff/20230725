# Comparing `tmp/alpaca_eval-0.2.5.tar.gz` & `tmp/alpaca_eval-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.2.5.tar", last modified: Mon Jul 24 17:25:59 2023, max compression
+gzip compressed data, was "alpaca_eval-0.2.6.tar", last modified: Tue Jul 25 11:38:24 2023, max compression
```

## Comparing `alpaca_eval-0.2.5.tar` & `alpaca_eval-0.2.6.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    66618 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.377300 alpaca_eval-0.2.5/example/
--rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/example/outputs.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.373300 alpaca_eval-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.381300 alpaca_eval-0.2.5/src/alpaca_eval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 17:25:43.000000 alpaca_eval-0.2.5/src/alpaca_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.381300 alpaca_eval-0.2.5/src/alpaca_eval/annotators/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/annotators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27986 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/annotators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/completion_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.381300 alpaca_eval-0.2.5/src/alpaca_eval/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/cohere.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/huggingface_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/huggingface_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/replicate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.381300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude_2/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/test/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/test/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.373300 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.377300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/airoboros-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/airoboros-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baichuan-13b-chat/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baichuan-13b-chat/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baichuan-13b-chat/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baize-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baize-v2-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/chatglm2-6b/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/chatglm2-6b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/chatglm2-6b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/claude-2/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/claude-2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/cohere/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/cohere/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/cohere-chat/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/minotaur-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-v2-w-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat8192-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/opencoderplus-15b/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/text_davinci_001/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/ultralm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14843 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.381300 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-24 17:25:59.000000 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-07-24 17:25:59.000000 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:25:59.000000 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 17:25:59.000000 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-24 17:25:59.000000 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 17:25:59.000000 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/tests/test_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/tests/test_decoders_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/tests/test_pairwise_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    66618 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.367686 alpaca_eval-0.2.6/example/
+-rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/example/outputs.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.339684 alpaca_eval-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.367686 alpaca_eval-0.2.6/src/alpaca_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-25 11:38:08.000000 alpaca_eval-0.2.6/src/alpaca_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.371686 alpaca_eval-0.2.6/src/alpaca_eval/annotators/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/annotators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28020 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/annotators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/completion_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.371686 alpaca_eval-0.2.6/src/alpaca_eval/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/huggingface_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/huggingface_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/replicate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.371686 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.371686 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.371686 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/test/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.347684 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.363686 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/airoboros-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/airoboros-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baichuan-13b-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baichuan-13b-chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baichuan-13b-chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baize-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baize-v2-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/chatglm2-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/chatglm2-6b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/chatglm2-6b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/claude-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/claude-2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/cohere/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/cohere/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/cohere-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/minotaur-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-v2-w-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat8192-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/opencoderplus-15b/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/ultralm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.371686 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-25 11:38:24.000000 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-07-25 11:38:24.000000 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:38:24.000000 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 11:38:24.000000 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-25 11:38:24.000000 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 11:38:24.000000 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/tests/test_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/tests/test_decoders_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/tests/test_pairwise_evaluator.py
```

### Comparing `alpaca_eval-0.2.5/LICENSE` & `alpaca_eval-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/PKG-INFO` & `alpaca_eval-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_eval
-Version: 0.2.5
+Version: 0.2.6
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.5 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.6 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
```

### Comparing `alpaca_eval-0.2.5/README.md` & `alpaca_eval-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/example/outputs.json` & `alpaca_eval-0.2.6/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/setup.py` & `alpaca_eval-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/analyze.py` & `alpaca_eval-0.2.6/src/alpaca_eval/analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/annotators/base.py` & `alpaca_eval-0.2.6/src/alpaca_eval/annotators/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         Temporary value to use for missing annotations when `is_store_missing_annotations` is True.
 
     annotation_type : type, optional
         Type to use for storing the annotations. If None, uses `self.DEFAULT_ANNOTATION_TYPE`.
     """
 
     DEFAULT_BASE_DIR = constants.EVALUATORS_CONFIG_DIR
-    ANNOTATOR_COLUMN = "annotator"
+    annotator_column = "annotator"
     TMP_MISSING_ANNOTATION = -1
     DEFAULT_ANNOTATION_TYPE = int
 
     def __init__(
         self,
         primary_keys: Sequence[str],
         annotators_config: Union[utils.AnyPath, list[dict[str, Any]]] = "claude",
@@ -90,15 +90,15 @@
         annotation_type: Optional[Type] = None,
     ):
         logging.info(f"Creating the annotator from `{annotators_config}`.")
         self.base_dir = Path(base_dir or self.DEFAULT_BASE_DIR)
         self.seed = seed
         self.is_avoid_reannotations = is_avoid_reannotations
         self.primary_keys = list(primary_keys)
-        self.all_keys = self.primary_keys + [self.ANNOTATOR_COLUMN]
+        self.all_keys = self.primary_keys + [self.annotator_column]
         self.other_keys_to_keep = list(other_keys_to_keep)
         self.is_store_missing_annotations = is_store_missing_annotations
         self.is_raise_if_missing_primary_keys = is_raise_if_missing_primary_keys
         self.annotation_type = annotation_type or self.DEFAULT_ANNOTATION_TYPE
 
         self.annotators_config = self._initialize_annotators_config(annotators_config)
         self.annotators = self._initialize_annotators()
@@ -205,22 +205,22 @@
         """Preprocess the examples to annotate. In particular takes care of filtering unnecessary examples."""
 
         df_to_annotate = utils.convert_to_dataframe(to_annotate)
         self._add_missing_primary_keys_(df_to_annotate)
 
         for c in self.other_keys_to_keep + [self.annotation_key]:
             if c in df_to_annotate.columns:
-                logging.warning(f"""{c} column is already in the dataframe. We will overwrite it.""")
+                logging.warning(f"{c} column is already in the dataframe. We will overwrite it.")
                 df_to_annotate[c] = None
 
         # remove duplicates because you only need to annotate one of them
         df_to_annotate = df_to_annotate.drop_duplicates(subset=self.primary_keys)
 
         # set the annotater for each example
-        df_to_annotate[self.ANNOTATOR_COLUMN] = df_to_annotate.apply(
+        df_to_annotate[self.annotator_column] = df_to_annotate.apply(
             lambda x: utils.random_seeded_choice(
                 # we add "annotator" at the beginning to not use the same seed for all tasks
                 seed="annotator" + "".join(x[self.random_seed_key]) + str(self.seed),
                 choices=list(self.annotators.keys()),
             ),
             axis=1,
         )
@@ -232,15 +232,15 @@
 
     def _annotate(self, df_to_annotate: pd.DataFrame, **decoding_kwargs) -> pd.DataFrame:
         """Annotate the examples."""
 
         df_annotated = df_to_annotate
         for annotator in self.annotators.keys():
             # only annotate examples that have not been annotated yet
-            curr_idcs = df_annotated[self.ANNOTATOR_COLUMN] == annotator
+            curr_idcs = df_annotated[self.annotator_column] == annotator
             if self.annotation_key in df_annotated.columns:
                 curr_idcs &= df_annotated[self.annotation_key].isna()
 
             logging.info(f"Annotating {curr_idcs.sum()} examples with {annotator}")
 
             # actual annotation
             curr_annotated = self.annotators[annotator](
@@ -567,19 +567,19 @@
         return df_annotated
 
     ######################
 
     ### Private methods ###
     def _search_fn_completion_parser(self, name: str) -> Callable:
         """Search for a completion parser by name."""
-        return getattr(completion_parsers, name)
+        return utils.get_module_attribute(completion_parsers, name)
 
     def _search_processor(self, name: str) -> Type["processors.BaseProcessor"]:
         """Search for a Processor class by name."""
-        return getattr(processors, name)
+        return utils.get_module_attribute(processors, name)
 
     def _get_prompt_template(self, prompt_template: utils.AnyPath):
         return utils.read_or_return(self.base_dir / prompt_template)
 
     def _make_prompts(
         self, df_to_annotate: pd.DataFrame, prompt_template: Optional[str] = None
     ) -> tuple[list[str], pd.DataFrame]:
```

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/annotators/pairwise_evaluator.py` & `alpaca_eval-0.2.6/src/alpaca_eval/annotators/pairwise_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,16 @@
             .apply(lambda x: x.drop_duplicates(["output"]))
             .reset_index(drop=True)
             .rename(columns={"output": "output_1"})
         )
 
         if len(df_to_annotate) != n_pre_drop:
             logging.warning(
-                f"""Filtered rows because of duplicate outputs for the same keys_to_sample_output_2=
-                {keys_to_sample_output_2}. {n_pre_drop} -> {len(df_to_annotate)}"""
+                f"Filtered rows because of duplicate outputs for the same keys_to_sample_output_2="
+                f"{keys_to_sample_output_2}. {n_pre_drop} -> {len(df_to_annotate)}"
             )
 
         # sample an output 2 for each output 1 that are different
         df_to_annotate["output_2"] = df_to_annotate.groupby(list(keys_to_sample_output_2))["output_1"].transform(
             lambda x: utils.random_derangement(x.values, seed=self.seed)
         )
 
@@ -225,18 +225,17 @@
             df_to_annotate = df_to_annotate.drop(columns="tmp_idx")
         else:
             # if you are taking the cartesian product, you can have undesired duplicates
             df_to_annotate = df_to_annotate.drop_duplicates()
 
             if not (len(outputs_1) == len(outputs_2) == len(df_to_annotate)):
                 logging.warning(
-                    f"""The length of outputs before and after merge are not the same. We have len(outputs_1)==
-                    {len(outputs_1)}, len(outputs_2)=={len(outputs_2)}, and len(df_annotated)=={len(df_to_annotate)}. 
-                    This means that there are missing examples or duplicates. We are taking a SQL inner join.
-                    """
+                    f"The length of outputs before and after merge are not the same. We have len(outputs_1)=="
+                    f"{len(outputs_1)}, len(outputs_2)=={len(outputs_2)}, and len(df_annotated)=={len(df_to_annotate)}."
+                    f" This means that there are missing examples or duplicates. We are taking a SQL inner join."
                 )
 
         out = self.__call__(df_to_annotate, **decoding_kwargs)
 
         return out
 
     def annotate_pairs(
@@ -343,14 +342,15 @@
         annotation_column: str = "preference",
         random_seed_column: Sequence[str] = ("instruction",),
         processors_to_kwargs: Optional[dict[str, dict]] = None,
         is_randomize_output_order: bool = True,
         **kwargs,
     ):
         processors_to_kwargs = processors_to_kwargs or {}
+        self.is_randomize_output_order = is_randomize_output_order
         if is_randomize_output_order:
             # swith output columns by default
             processors_to_kwargs["RandomSwitchTwoColumnsProcessor"] = dict(
                 two_columns_to_switch=["output_1", "output_2"],
                 replace_if_switch_kwargs={"preference": {1: 2, 2: 1}},
                 random_seed_columns=random_seed_column,
                 _switch_column="is_switched_outputs",  # backward compatibility
```

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.2.6/src/alpaca_eval/completion_parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import re
 from typing import Any
 
 import numpy as np
 
 from . import utils
 
+__all__ = ["regex_parser", "lmsys_parser", "ranking_parser", "json_parser", "eval_parser"]
+
 
 def regex_parser(completion: str, outputs_to_match: dict[str, Any]) -> list[Any]:
     r"""Parse a single batch of completions, by returning a sequence of keys in the order in which outputs_to_match
     was matched.
 
     Parameters
     ----------
```

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/constants.py` & `alpaca_eval-0.2.6/src/alpaca_eval/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.2.6/src/alpaca_eval/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.2.6/src/alpaca_eval/decoders/anthropic.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.2.6/src/alpaca_eval/decoders/cohere.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.2.6/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.2.6/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.2.6/src/alpaca_eval/decoders/openai.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/decoders/replicate.py` & `alpaca_eval-0.2.6/src/alpaca_eval/decoders/replicate.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv` & `alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/main.py` & `alpaca_eval-0.2.6/src/alpaca_eval/main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/metrics.py` & `alpaca_eval-0.2.6/src/alpaca_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt` & `alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/plotting.py` & `alpaca_eval-0.2.6/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/processors.py` & `alpaca_eval-0.2.6/src/alpaca_eval/processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import numpy as np
 import pandas as pd
 
 from . import utils
 
 DUMMY_EXAMPLE = dict(instruction="1+1=", output_1="2", input="", output_2="3")
+__all__ = ["RandomSwitchTwoColumnsProcessor", "PaddingForBatchesProcessor"]
 
 
 class BaseProcessor(abc.ABC):
     """Base class for a processor."""
 
     def __init__(self, seed: int = 123):
         self.seed = seed
@@ -88,15 +89,15 @@
         # `switch_column` used for backward compatibility
         if _switch_column is None:
             _switch_column = "_".join(["is_switch"] + list(two_columns_to_switch))
         self._switch_column = _switch_column
 
         if random_seed_columns is None:
             random_seed_columns = two_columns_to_switch
-        self.random_seed_columns = list(random_seed_columns)
+        self.random_seed_columns = sorted(list(random_seed_columns))
 
         super().__init__(**kwargs)
 
     def preprocess(self, df_to_annotate: pd.DataFrame) -> pd.DataFrame:
         """When preprocessing, we select the rows to switch and perform the switch."""
         df_to_annotate = df_to_annotate.copy()
```

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval/utils.py` & `alpaca_eval-0.2.6/src/alpaca_eval/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,7 +428,20 @@
     if name is None:
         try:
             assert len(model_outputs["generator"].unique()) == 1
             name = model_outputs["generator"].iloc[0]
         except:
             name = "Current model"
     return name
+
+
+def get_module_attribute(module, func_name):
+    """getattr but only if it's in __all__"""
+    if func_name in module.__all__:
+        return getattr(module, func_name)
+    elif hasattr(module, func_name):
+        raise AttributeError(
+            f"The function {func_name} is not allowed,add it to __all__ if needed."
+            f" Available functions: {module.__all__}"
+        )
+    else:
+        raise AttributeError(f"The function {func_name} does not exist. Available functions: {module.__all__}")
```

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval.egg-info/PKG-INFO` & `alpaca_eval-0.2.6/src/alpaca_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-eval
-Version: 0.2.5
+Version: 0.2.6
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.5 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.6 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
```

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.2.6/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/src/alpaca_eval.egg-info/requires.txt` & `alpaca_eval-0.2.6/src/alpaca_eval.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/tests/test_analyze.py` & `alpaca_eval-0.2.6/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/tests/test_decoders_unit.py` & `alpaca_eval-0.2.6/tests/test_decoders_unit.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/tests/test_main.py` & `alpaca_eval-0.2.6/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.5/tests/test_pairwise_evaluator.py` & `alpaca_eval-0.2.6/tests/test_pairwise_evaluator.py`

 * *Files identical despite different names*

