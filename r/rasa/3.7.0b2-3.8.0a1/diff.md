# Comparing `tmp/rasa-3.7.0b2.tar.gz` & `tmp/rasa-3.8.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa-3.7.0b2.tar", max compression
+gzip compressed data, was "rasa-3.8.0a1.tar", max compression
```

## Comparing `rasa-3.7.0b2.tar` & `rasa-3.8.0a1.tar`

### file list

```diff
@@ -1,317 +1,353 @@
--rw-r--r--   0        0        0    11352 2023-07-20 16:16:53.899925 rasa-3.7.0b2/LICENSE.txt
--rw-r--r--   0        0        0    21519 2023-07-20 16:16:53.899925 rasa-3.7.0b2/README.md
--rw-r--r--   0        0        0     9559 2023-07-20 16:16:54.075926 rasa-3.7.0b2/pyproject.toml
--rw-r--r--   0        0        0      280 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/__init__.py
--rw-r--r--   0        0        0     5441 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/__main__.py
--rw-r--r--   0        0        0     5314 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/api.py
--rw-r--r--   0        0        0      115 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/__init__.py
--rw-r--r--   0        0        0     2388 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/data.py
--rw-r--r--   0        0        0     5242 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/default_arguments.py
--rw-r--r--   0        0        0     2199 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/evaluate.py
--rw-r--r--   0        0        0     1499 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/export.py
--rw-r--r--   0        0        0     2685 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/interactive.py
--rw-r--r--   0        0        0     5674 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/run.py
--rw-r--r--   0        0        0      367 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/shell.py
--rw-r--r--   0        0        0     6853 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/test.py
--rw-r--r--   0        0        0     8279 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/train.py
--rw-r--r--   0        0        0      861 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/visualize.py
--rw-r--r--   0        0        0     1027 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/x.py
--rw-r--r--   0        0        0     9722 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/data.py
--rw-r--r--   0        0        0     7948 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/evaluate.py
--rw-r--r--   0        0        0     8204 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/export.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/actions/__init__.py
--rw-r--r--   0        0        0      742 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/actions/actions.py
--rw-r--r--   0        0        0     1505 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/config.yml
--rw-r--r--   0        0        0      998 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/credentials.yml
--rw-r--r--   0        0        0     1433 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/data/nlu.yml
--rw-r--r--   0        0        0      244 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/data/rules.yml
--rw-r--r--   0        0        0      542 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/data/stories.yml
--rw-r--r--   0        0        0      565 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/domain.yml
--rw-r--r--   0        0        0     1411 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/endpoints.yml
--rw-r--r--   0        0        0     1664 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/tests/test_stories.yml
--rw-r--r--   0        0        0     5943 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/interactive.py
--rw-r--r--   0        0        0     4196 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/run.py
--rw-r--r--   0        0        0     6846 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/scaffold.py
--rw-r--r--   0        0        0     4264 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/shell.py
--rw-r--r--   0        0        0     3118 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/telemetry.py
--rw-r--r--   0        0        0     8888 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/test.py
--rw-r--r--   0        0        0     7798 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/train.py
--rw-r--r--   0        0        0    12508 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/utils.py
--rw-r--r--   0        0        0     1256 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/visualize.py
--rw-r--r--   0        0        0     6785 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/x.py
--rw-r--r--   0        0        0     1172 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/constants.py
--rw-r--r--   0        0        0      123 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/core/actions/__init__.py
--rw-r--r--   0        0        0    48450 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/core/actions/action.py
--rw-r--r--   0        0        0       78 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/core/actions/constants.py
--rw-r--r--   0        0        0    26679 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/actions/forms.py
--rw-r--r--   0        0        0     3401 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/actions/loops.py
--rw-r--r--   0        0        0     6078 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/actions/two_stage_fallback.py
--rw-r--r--   0        0        0    20445 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/agent.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/brokers/__init__.py
--rw-r--r--   0        0        0     4398 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/brokers/broker.py
--rw-r--r--   0        0        0     1801 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/brokers/file.py
--rw-r--r--   0        0        0    12002 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/brokers/kafka.py
--rw-r--r--   0        0        0    14160 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/brokers/pika.py
--rw-r--r--   0        0        0     2754 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/brokers/sql.py
--rw-r--r--   0        0        0     1656 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/__init__.py
--rw-r--r--   0        0        0    11669 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/botframework.py
--rw-r--r--   0        0        0     2746 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/callback.py
--rw-r--r--   0        0        0    13331 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/channel.py
--rw-r--r--   0        0        0     8073 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/console.py
--rw-r--r--   0        0        0    15819 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/facebook.py
--rw-r--r--   0        0        0    11568 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/hangouts.py
--rw-r--r--   0        0        0     7743 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/mattermost.py
--rw-r--r--   0        0        0     4814 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/rasa_chat.py
--rw-r--r--   0        0        0     6957 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/rest.py
--rw-r--r--   0        0        0     5999 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/rocketchat.py
--rw-r--r--   0        0        0    24405 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/slack.py
--rw-r--r--   0        0        0    10163 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/socketio.py
--rw-r--r--   0        0        0    10630 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/telegram.py
--rw-r--r--   0        0        0     5938 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/twilio.py
--rw-r--r--   0        0        0    13181 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/twilio_voice.py
--rw-r--r--   0        0        0     4845 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/webexteams.py
--rw-r--r--   0        0        0     3047 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/constants.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/evaluation/__init__.py
--rw-r--r--   0        0        0     9154 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/evaluation/marker.py
--rw-r--r--   0        0        0    38043 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/evaluation/marker_base.py
--rw-r--r--   0        0        0    12086 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/evaluation/marker_stats.py
--rw-r--r--   0        0        0     3658 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/evaluation/marker_tracker_loader.py
--rw-r--r--   0        0        0      901 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/exceptions.py
--rw-r--r--   0        0        0    10220 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/exporter.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/featurizers/__init__.py
--rw-r--r--   0        0        0    17964 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/featurizers/precomputation.py
--rw-r--r--   0        0        0    15447 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/featurizers/single_state_featurizer.py
--rw-r--r--   0        0        0    43363 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/featurizers/tracker_featurizers.py
--rw-r--r--   0        0        0     3084 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/http_interpreter.py
--rw-r--r--   0        0        0     2018 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/jobs.py
--rw-r--r--   0        0        0     4719 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/lock.py
--rw-r--r--   0        0        0    11678 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/lock_store.py
--rw-r--r--   0        0        0    14821 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/migrate.py
--rw-r--r--   0        0        0      240 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/nlg/__init__.py
--rw-r--r--   0        0        0     3870 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/nlg/callback.py
--rw-r--r--   0        0        0     3285 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/nlg/generator.py
--rw-r--r--   0        0        0     2897 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/nlg/interpolator.py
--rw-r--r--   0        0        0     7503 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/nlg/response.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/policies/__init__.py
--rw-r--r--   0        0        0    12959 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/policies/ensemble.py
--rw-r--r--   0        0        0    19295 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/policies/memoization.py
--rw-r--r--   0        0        0    25038 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/policies/policy.py
--rw-r--r--   0        0        0    50315 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/policies/rule_policy.py
--rw-r--r--   0        0        0    86521 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/policies/ted_policy.py
--rw-r--r--   0        0        0    39329 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/policies/unexpected_intent_policy.py
--rw-r--r--   0        0        0    41906 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/processor.py
--rw-r--r--   0        0        0     9243 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/run.py
--rw-r--r--   0        0        0    48935 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/test.py
--rw-r--r--   0        0        0    58040 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/tracker_store.py
--rw-r--r--   0        0        0     3543 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/train.py
--rw-r--r--   0        0        0     3218 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/training/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/training/converters/__init__.py
--rw-r--r--   0        0        0     3889 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/training/converters/responses_prefix_converter.py
--rw-r--r--   0        0        0    59595 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/training/interactive.py
--rw-r--r--   0        0        0    13604 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/training/story_conflict.py
--rw-r--r--   0        0        0     3067 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/training/training.py
--rw-r--r--   0        0        0    10995 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/utils.py
--rw-r--r--   0        0        0     2125 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/visualize.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/__init__.py
--rw-r--r--   0        0        0    16744 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/caching.py
--rw-r--r--   0        0        0      469 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/constants.py
--rw-r--r--   0        0        0      437 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/exceptions.py
--rw-r--r--   0        0        0    22105 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/graph.py
--rw-r--r--   0        0        0     1384 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/loader.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/recipes/__init__.py
--rw-r--r--   0        0        0     1139 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/recipes/config_files/default_config.yml
--rw-r--r--   0        0        0     3244 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/recipes/default_components.py
--rw-r--r--   0        0        0    43587 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/recipes/default_recipe.py
--rw-r--r--   0        0        0     3301 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/recipes/graph_recipe.py
--rw-r--r--   0        0        0     3354 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/recipes/recipe.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/runner/__init__.py
--rw-r--r--   0        0        0     4302 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/runner/dask.py
--rw-r--r--   0        0        0     1672 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/runner/interface.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/storage/__init__.py
--rw-r--r--   0        0        0     9581 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/storage/local_model_storage.py
--rw-r--r--   0        0        0     3931 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/storage/resource.py
--rw-r--r--   0        0        0     6923 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/storage/storage.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/training/__init__.py
--rw-r--r--   0        0        0     6524 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/training/components.py
--rw-r--r--   0        0        0     1848 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/training/fingerprinting.py
--rw-r--r--   0        0        0    10516 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/training/graph_trainer.py
--rw-r--r--   0        0        0     5036 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/training/hooks.py
--rw-r--r--   0        0        0    22697 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/validation.py
--rw-r--r--   0        0        0     2132 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/graph_components/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/graph_components/converters/__init__.py
--rw-r--r--   0        0        0     1576 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/graph_components/converters/nlu_message_converter.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/graph_components/providers/__init__.py
--rw-r--r--   0        0        0     3832 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/domain_for_core_training_provider.py
--rw-r--r--   0        0        0     2571 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/domain_provider.py
--rw-r--r--   0        0        0     1294 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/forms_provider.py
--rw-r--r--   0        0        0     2119 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/nlu_training_data_provider.py
--rw-r--r--   0        0        0     1354 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/responses_provider.py
--rw-r--r--   0        0        0     1540 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/rule_only_provider.py
--rw-r--r--   0        0        0     1466 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/story_graph_provider.py
--rw-r--r--   0        0        0     1965 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/training_tracker_provider.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/validators/__init__.py
--rw-r--r--   0        0        0    22668 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/validators/default_recipe_validator.py
--rw-r--r--   0        0        0    12863 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/validators/finetuning_validator.py
--rw-r--r--   0        0        0     1782 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/jupyter.py
--rw-r--r--   0        0        0      101 2023-07-20 16:17:14.656082 rasa-3.7.0b2/rasa/keys
--rw-r--r--   0        0        0     3490 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/model.py
--rw-r--r--   0        0        0    14961 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/model_testing.py
--rw-r--r--   0        0        0    16836 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/model_training.py
--rw-r--r--   0        0        0      123 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/__init__.py
--rw-r--r--   0        0        0      118 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/__init__.py
--rw-r--r--   0        0        0      133 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/classifier.py
--rw-r--r--   0        0        0    71637 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/diet_classifier.py
--rw-r--r--   0        0        0     7150 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/fallback_classifier.py
--rw-r--r--   0        0        0     7581 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/keyword_intent_classifier.py
--rw-r--r--   0        0        0     7568 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/logistic_regression_classifier.py
--rw-r--r--   0        0        0     5559 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/mitie_intent_classifier.py
--rw-r--r--   0        0        0     1989 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/regex_message_handler.py
--rw-r--r--   0        0        0    11915 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/sklearn_intent_classifier.py
--rw-r--r--   0        0        0     2757 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/constants.py
--rw-r--r--   0        0        0     1317 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/convert.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/emulators/__init__.py
--rw-r--r--   0        0        0     1748 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/emulators/dialogflow.py
--rw-r--r--   0        0        0     1367 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/emulators/emulator.py
--rw-r--r--   0        0        0     3032 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/emulators/luis.py
--rw-r--r--   0        0        0      334 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/emulators/no_emulator.py
--rw-r--r--   0        0        0     1930 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/emulators/wit.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/__init__.py
--rw-r--r--   0        0        0    26499 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/crf_entity_extractor.py
--rw-r--r--   0        0        0     7685 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/duckling_entity_extractor.py
--rw-r--r--   0        0        0     7160 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/entity_synonyms.py
--rw-r--r--   0        0        0    17530 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/extractor.py
--rw-r--r--   0        0        0    10973 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/mitie_entity_extractor.py
--rw-r--r--   0        0        0     8289 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/regex_entity_extractor.py
--rw-r--r--   0        0        0     3366 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/spacy_entity_extractor.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/__init__.py
--rw-r--r--   0        0        0    17142 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py
--rw-r--r--   0        0        0     2433 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py
--rw-r--r--   0        0        0    30361 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py
--rw-r--r--   0        0        0     5861 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py
--rw-r--r--   0        0        0     4888 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py
--rw-r--r--   0        0        0     3347 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/featurizer.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/__init__.py
--rw-r--r--   0        0        0    33295 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py
--rw-r--r--   0        0        0    21810 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py
--rw-r--r--   0        0        0    10289 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py
--rw-r--r--   0        0        0      220 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/sparse_featurizer.py
--rw-r--r--   0        0        0      557 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/model.py
--rw-r--r--   0        0        0     8333 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/persistor.py
--rw-r--r--   0        0        0      803 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/run.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/selectors/__init__.py
--rw-r--r--   0        0        0    39012 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/selectors/response_selector.py
--rw-r--r--   0        0        0    67726 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/test.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/tokenizers/__init__.py
--rw-r--r--   0        0        0     5374 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/tokenizers/jieba_tokenizer.py
--rw-r--r--   0        0        0     2618 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/tokenizers/mitie_tokenizer.py
--rw-r--r--   0        0        0     2378 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/tokenizers/spacy_tokenizer.py
--rw-r--r--   0        0        0     8196 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     3750 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/tokenizers/whitespace_tokenizer.py
--rw-r--r--   0        0        0      928 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/__init__.py
--rw-r--r--   0        0        0    14703 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/bilou_utils.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/hugging_face/__init__.py
--rw-r--r--   0        0        0     3380 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/hugging_face/registry.py
--rw-r--r--   0        0        0     9143 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py
--rw-r--r--   0        0        0     3887 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/mitie_utils.py
--rw-r--r--   0        0        0     5386 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/pattern_utils.py
--rw-r--r--   0        0        0    11795 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/spacy_utils.py
--rw-r--r--   0        0        0     4921 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/plugin.py
--rw-r--r--   0        0        0    55589 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/server.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/__init__.py
--rw-r--r--   0        0        0     4337 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/constants.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/__init__.py
--rw-r--r--   0        0        0     4416 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/constants.py
--rw-r--r--   0        0        0     1366 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/conversation.py
--rw-r--r--   0        0        0    77445 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/domain.py
--rw-r--r--   0        0        0    66276 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/events.py
--rw-r--r--   0        0        0    35597 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/generator.py
--rw-r--r--   0        0        0     8286 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/slot_mappings.py
--rw-r--r--   0        0        0    16371 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/slots.py
--rw-r--r--   0        0        0    34744 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/trackers.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/__init__.py
--rw-r--r--   0        0        0     2895 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/loading.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/__init__.py
--rw-r--r--   0        0        0     4449 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/story_reader.py
--rw-r--r--   0        0        0     6671 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/story_step_builder.py
--rw-r--r--   0        0        0    32976 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/yaml_story_reader.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_writer/__init__.py
--rw-r--r--   0        0        0     2543 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_writer/story_writer.py
--rw-r--r--   0        0        0    14903 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_writer/yaml_story_writer.py
--rw-r--r--   0        0        0    29313 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/structures.py
--rw-r--r--   0        0        0     3500 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/visualization.html
--rw-r--r--   0        0        0    20341 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/core/training_data/visualization.py
--rw-r--r--   0        0        0     5479 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/data.py
--rw-r--r--   0        0        0     3633 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/importers/__init__.py
--rw-r--r--   0        0        0    21866 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/importers/importer.py
--rw-r--r--   0        0        0     7836 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/importers/multi_project.py
--rw-r--r--   0        0        0     3388 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/importers/rasa.py
--rw-r--r--   0        0        0      861 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/importers/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/__init__.py
--rw-r--r--   0        0        0     1388 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/constants.py
--rw-r--r--   0        0        0      188 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/interpreter.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/__init__.py
--rw-r--r--   0        0        0     6759 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/entities_parser.py
--rw-r--r--   0        0        0    14835 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/features.py
--rw-r--r--   0        0        0      453 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/__init__.py
--rw-r--r--   0        0        0     6123 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/dialogflow.py
--rw-r--r--   0        0        0     3014 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/luis.py
--rw-r--r--   0        0        0     4495 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/rasa.py
--rw-r--r--   0        0        0    22353 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/rasa_yaml.py
--rw-r--r--   0        0        0     8540 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/readerwriter.py
--rw-r--r--   0        0        0     1820 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/wit.py
--rw-r--r--   0        0        0     4258 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/loading.py
--rw-r--r--   0        0        0     1116 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/lookup_tables_parser.py
--rw-r--r--   0        0        0    16662 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/message.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/__init__.py
--rw-r--r--   0        0        0     2565 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/data_schema.py
--rw-r--r--   0        0        0     1179 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/nlu.yml
--rw-r--r--   0        0        0     1661 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/responses.yml
--rw-r--r--   0        0        0     1476 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/synonyms_parser.py
--rw-r--r--   0        0        0    28493 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/training_data.py
--rw-r--r--   0        0        0     7040 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/util.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/__init__.py
--rw-r--r--   0        0        0     2078 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/cli.py
--rw-r--r--   0        0        0     8731 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/common.py
--rw-r--r--   0        0        0    20606 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/io.py
--rw-r--r--   0        0        0      883 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/pykwalify_extensions.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/schemas/__init__.py
--rw-r--r--   0        0        0       27 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/schemas/config.yml
--rw-r--r--   0        0        0     3267 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/schemas/domain.yml
--rw-r--r--   0        0        0     5569 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/schemas/events.py
--rw-r--r--   0        0        0      998 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/schemas/model_config.yml
--rw-r--r--   0        0        0     4034 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/schemas/stories.yml
--rw-r--r--   0        0        0    10317 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/validation.py
--rw-r--r--   0        0        0    36273 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/telemetry.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/__init__.py
--rw-r--r--   0        0        0    19532 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/common.py
--rw-r--r--   0        0        0     1647 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/converter.py
--rw-r--r--   0        0        0     8796 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/endpoints.py
--rw-r--r--   0        0        0     7831 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/io.py
--rw-r--r--   0        0        0     2018 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/llm.py
--rw-r--r--   0        0        0     5036 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/log_utils.py
--rw-r--r--   0        0        0    12246 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/plotting.py
--rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/__init__.py
--rw-r--r--   0        0        0     4036 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/callback.py
--rw-r--r--   0        0        0     3140 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/constants.py
--rw-r--r--   0        0        0    19658 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/crf.py
--rw-r--r--   0        0        0    15526 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/data_generator.py
--rw-r--r--   0        0        0     5576 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/environment.py
--rw-r--r--   0        0        0      168 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/exceptions.py
--rw-r--r--   0        0        0    59263 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/layers.py
--rw-r--r--   0        0        0     3319 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/layers_utils.py
--rw-r--r--   0        0        0    10055 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/metrics.py
--rw-r--r--   0        0        0    34572 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/tensorflow/model_data.py
--rw-r--r--   0        0        0    18667 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/tensorflow/model_data_utils.py
--rw-r--r--   0        0        0    36004 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/tensorflow/models.py
--rw-r--r--   0        0        0    49066 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/tensorflow/rasa_layers.py
--rw-r--r--   0        0        0    25509 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/tensorflow/transformer.py
--rw-r--r--   0        0        0      204 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/tensorflow/types.py
--rw-r--r--   0        0        0    20999 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/train_utils.py
--rw-r--r--   0        0        0    17708 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/validator.py
--rw-r--r--   0        0        0      118 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/version.py
--rw-r--r--   0        0        0    28151 1970-01-01 00:00:00.000000 rasa-3.7.0b2/PKG-INFO
+-rw-r--r--   0        0        0    11352 2023-07-25 21:45:25.561717 rasa-3.8.0a1/LICENSE.txt
+-rw-r--r--   0        0        0    21519 2023-07-25 21:45:25.561717 rasa-3.8.0a1/README.md
+-rw-r--r--   0        0        0     9769 2023-07-25 21:45:25.901720 rasa-3.8.0a1/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-07-25 21:45:25.901720 rasa-3.8.0a1/rasa/__init__.py
+-rw-r--r--   0        0        0     5510 2023-07-25 21:45:25.901720 rasa-3.8.0a1/rasa/__main__.py
+-rw-r--r--   0        0        0     5314 2023-07-25 21:45:25.901720 rasa-3.8.0a1/rasa/api.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.901720 rasa-3.8.0a1/rasa/cdu/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.901720 rasa-3.8.0a1/rasa/cdu/command_generator/__init__.py
+-rw-r--r--   0        0        0     1717 2023-07-25 21:45:25.901720 rasa-3.8.0a1/rasa/cdu/command_generator/base.py
+-rw-r--r--   0        0        0     2828 2023-07-25 21:45:25.901720 rasa-3.8.0a1/rasa/cdu/command_generator/command_prompt_template.jinja2
+-rw-r--r--   0        0        0    10511 2023-07-25 21:45:25.901720 rasa-3.8.0a1/rasa/cdu/command_generator/llm_command_generator.py
+-rw-r--r--   0        0        0    11649 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cdu/command_processor.py
+-rw-r--r--   0        0        0     1722 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cdu/command_processor_component.py
+-rw-r--r--   0        0        0     3161 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cdu/commands.py
+-rw-r--r--   0        0        0     6725 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cdu/flow_stack.py
+-rw-r--r--   0        0        0      557 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cdu/nlu_command_adapter.py
+-rw-r--r--   0        0        0      115 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/arguments/__init__.py
+-rw-r--r--   0        0        0     2388 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/arguments/data.py
+-rw-r--r--   0        0        0     5242 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/arguments/default_arguments.py
+-rw-r--r--   0        0        0     2199 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/arguments/evaluate.py
+-rw-r--r--   0        0        0     1499 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/arguments/export.py
+-rw-r--r--   0        0        0     2685 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/arguments/interactive.py
+-rw-r--r--   0        0        0     5674 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/arguments/run.py
+-rw-r--r--   0        0        0      367 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/arguments/shell.py
+-rw-r--r--   0        0        0     6853 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/arguments/test.py
+-rw-r--r--   0        0        0     8279 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/arguments/train.py
+-rw-r--r--   0        0        0      861 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/arguments/visualize.py
+-rw-r--r--   0        0        0     1027 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/arguments/x.py
+-rw-r--r--   0        0        0     2004 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/chat.py
+-rw-r--r--   0        0        0     9722 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/data.py
+-rw-r--r--   0        0        0     7948 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/evaluate.py
+-rw-r--r--   0        0        0     8204 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/export.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project/actions/__init__.py
+-rw-r--r--   0        0        0      742 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project/actions/actions.py
+-rw-r--r--   0        0        0     1505 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project/config.yml
+-rw-r--r--   0        0        0      998 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project/credentials.yml
+-rw-r--r--   0        0        0     1433 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project/data/nlu.yml
+-rw-r--r--   0        0        0      244 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project/data/rules.yml
+-rw-r--r--   0        0        0      542 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project/data/stories.yml
+-rw-r--r--   0        0        0      702 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project/domain.yml
+-rw-r--r--   0        0        0     1411 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project/endpoints.yml
+-rw-r--r--   0        0        0     1664 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project/tests/test_stories.yml
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project_dm2/actions/__init__.py
+-rw-r--r--   0        0        0      742 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project_dm2/actions/actions.py
+-rw-r--r--   0        0        0      282 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project_dm2/config.yml
+-rw-r--r--   0        0        0      998 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project_dm2/credentials.yml
+-rw-r--r--   0        0        0     1203 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project_dm2/data/flows.yml
+-rw-r--r--   0        0        0      136 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project_dm2/data/nlu.yml
+-rw-r--r--   0        0        0     1138 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project_dm2/domain.yml
+-rw-r--r--   0        0        0      193 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project_dm2/e2e_tests/complete_request.yml
+-rw-r--r--   0        0        0      334 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project_dm2/e2e_tests/happy.yml
+-rw-r--r--   0        0        0     1409 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project_dm2/endpoints.yml
+-rw-r--r--   0        0        0     1664 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/initial_project_dm2/tests/test_stories.yml
+-rw-r--r--   0        0        0     5943 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/interactive.py
+-rw-r--r--   0        0        0     4196 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/run.py
+-rw-r--r--   0        0        0     7160 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/scaffold.py
+-rw-r--r--   0        0        0     4264 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/shell.py
+-rw-r--r--   0        0        0     3118 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/telemetry.py
+-rw-r--r--   0        0        0     8888 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/test.py
+-rw-r--r--   0        0        0     7798 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/train.py
+-rw-r--r--   0        0        0    12508 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/utils.py
+-rw-r--r--   0        0        0     1256 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/visualize.py
+-rw-r--r--   0        0        0     6785 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/cli/x.py
+-rw-r--r--   0        0        0     1172 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/constants.py
+-rw-r--r--   0        0        0      123 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/core/actions/__init__.py
+-rw-r--r--   0        0        0    48374 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/core/actions/action.py
+-rw-r--r--   0        0        0       78 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/core/actions/constants.py
+-rw-r--r--   0        0        0     2309 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/core/actions/flows.py
+-rw-r--r--   0        0        0    26679 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/core/actions/forms.py
+-rw-r--r--   0        0        0     3401 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/core/actions/loops.py
+-rw-r--r--   0        0        0     1062 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/core/actions/tests/test_flows.py
+-rw-r--r--   0        0        0     6078 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/core/actions/two_stage_fallback.py
+-rw-r--r--   0        0        0    20445 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/core/agent.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/core/brokers/__init__.py
+-rw-r--r--   0        0        0     4398 2023-07-25 21:45:25.905720 rasa-3.8.0a1/rasa/core/brokers/broker.py
+-rw-r--r--   0        0        0     1801 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/brokers/file.py
+-rw-r--r--   0        0        0    12127 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/brokers/kafka.py
+-rw-r--r--   0        0        0    14363 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/brokers/pika.py
+-rw-r--r--   0        0        0     2754 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/brokers/sql.py
+-rw-r--r--   0        0        0     1656 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/__init__.py
+-rw-r--r--   0        0        0    11669 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/botframework.py
+-rw-r--r--   0        0        0     2746 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/callback.py
+-rw-r--r--   0        0        0    13331 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/channel.py
+-rw-r--r--   0        0        0     5210 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/chat.html
+-rw-r--r--   0        0        0     8073 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/console.py
+-rw-r--r--   0        0        0    15819 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/facebook.py
+-rw-r--r--   0        0        0    11568 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/hangouts.py
+-rw-r--r--   0        0        0     7743 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/mattermost.py
+-rw-r--r--   0        0        0     4814 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/rasa_chat.py
+-rw-r--r--   0        0        0     6957 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/rest.py
+-rw-r--r--   0        0        0     5999 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/rocketchat.py
+-rw-r--r--   0        0        0    24405 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/slack.py
+-rw-r--r--   0        0        0    10621 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/socketio.py
+-rw-r--r--   0        0        0    10630 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/telegram.py
+-rw-r--r--   0        0        0     5938 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/twilio.py
+-rw-r--r--   0        0        0    13181 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/twilio_voice.py
+-rw-r--r--   0        0        0     4845 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/channels/webexteams.py
+-rw-r--r--   0        0        0     3047 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/constants.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/evaluation/__init__.py
+-rw-r--r--   0        0        0     9154 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/evaluation/marker.py
+-rw-r--r--   0        0        0    38043 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/evaluation/marker_base.py
+-rw-r--r--   0        0        0    12086 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/evaluation/marker_stats.py
+-rw-r--r--   0        0        0     3658 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/evaluation/marker_tracker_loader.py
+-rw-r--r--   0        0        0      901 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/exceptions.py
+-rw-r--r--   0        0        0    10220 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/exporter.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/featurizers/__init__.py
+-rw-r--r--   0        0        0    17964 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/featurizers/precomputation.py
+-rw-r--r--   0        0        0    15447 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/featurizers/single_state_featurizer.py
+-rw-r--r--   0        0        0    43363 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/featurizers/tracker_featurizers.py
+-rw-r--r--   0        0        0     3084 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/http_interpreter.py
+-rw-r--r--   0        0        0     2018 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/jobs.py
+-rw-r--r--   0        0        0     4719 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/lock.py
+-rw-r--r--   0        0        0    11678 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/lock_store.py
+-rw-r--r--   0        0        0    14821 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/migrate.py
+-rw-r--r--   0        0        0      240 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/nlg/__init__.py
+-rw-r--r--   0        0        0     5232 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/nlg/callback.py
+-rw-r--r--   0        0        0     8146 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/nlg/generator.py
+-rw-r--r--   0        0        0     2897 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/nlg/interpolator.py
+-rw-r--r--   0        0        0     5345 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/nlg/response.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/policies/__init__.py
+-rw-r--r--   0        0        0     2692 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/policies/default_flows.yml
+-rw-r--r--   0        0        0    12959 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/policies/ensemble.py
+-rw-r--r--   0        0        0    26256 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/policies/flow_policy.py
+-rw-r--r--   0        0        0    19295 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/policies/memoization.py
+-rw-r--r--   0        0        0    25546 2023-07-25 21:45:25.909720 rasa-3.8.0a1/rasa/core/policies/policy.py
+-rw-r--r--   0        0        0    50315 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/policies/rule_policy.py
+-rw-r--r--   0        0        0    86521 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/policies/ted_policy.py
+-rw-r--r--   0        0        0     2297 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/policies/test_flow_policy.py
+-rw-r--r--   0        0        0    39329 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/policies/unexpected_intent_policy.py
+-rw-r--r--   0        0        0    42336 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/processor.py
+-rw-r--r--   0        0        0     9567 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/run.py
+-rw-r--r--   0        0        0    48935 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/test.py
+-rw-r--r--   0        0        0    58040 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/tracker_store.py
+-rw-r--r--   0        0        0     3543 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/train.py
+-rw-r--r--   0        0        0     3218 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/training/converters/__init__.py
+-rw-r--r--   0        0        0     3889 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/training/converters/responses_prefix_converter.py
+-rw-r--r--   0        0        0    59595 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/training/interactive.py
+-rw-r--r--   0        0        0    13604 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/training/story_conflict.py
+-rw-r--r--   0        0        0     3067 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/training/training.py
+-rw-r--r--   0        0        0    10995 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/utils.py
+-rw-r--r--   0        0        0     2125 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/core/visualize.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/__init__.py
+-rw-r--r--   0        0        0    16478 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/caching.py
+-rw-r--r--   0        0        0      469 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/constants.py
+-rw-r--r--   0        0        0      437 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/exceptions.py
+-rw-r--r--   0        0        0    22105 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/graph.py
+-rw-r--r--   0        0        0     1384 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/loader.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/recipes/__init__.py
+-rw-r--r--   0        0        0     1139 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/recipes/config_files/default_config.yml
+-rw-r--r--   0        0        0     3350 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/recipes/default_components.py
+-rw-r--r--   0        0        0    45433 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/recipes/default_recipe.py
+-rw-r--r--   0        0        0     3301 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/recipes/graph_recipe.py
+-rw-r--r--   0        0        0     3354 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/recipes/recipe.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/runner/__init__.py
+-rw-r--r--   0        0        0     4302 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/runner/dask.py
+-rw-r--r--   0        0        0     1672 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/runner/interface.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/storage/__init__.py
+-rw-r--r--   0        0        0     9581 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/storage/local_model_storage.py
+-rw-r--r--   0        0        0     3931 2023-07-25 21:45:25.913720 rasa-3.8.0a1/rasa/engine/storage/resource.py
+-rw-r--r--   0        0        0     6923 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/engine/storage/storage.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/engine/training/__init__.py
+-rw-r--r--   0        0        0     6524 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/engine/training/components.py
+-rw-r--r--   0        0        0     1848 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/engine/training/fingerprinting.py
+-rw-r--r--   0        0        0    10516 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/engine/training/graph_trainer.py
+-rw-r--r--   0        0        0     5036 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/engine/training/hooks.py
+-rw-r--r--   0        0        0    22697 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/engine/validation.py
+-rw-r--r--   0        0        0     2132 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/converters/__init__.py
+-rw-r--r--   0        0        0     1576 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/converters/nlu_message_converter.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/providers/__init__.py
+-rw-r--r--   0        0        0     3832 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/providers/domain_for_core_training_provider.py
+-rw-r--r--   0        0        0     2571 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/providers/domain_provider.py
+-rw-r--r--   0        0        0     2942 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/providers/flows_provider.py
+-rw-r--r--   0        0        0     1294 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/providers/forms_provider.py
+-rw-r--r--   0        0        0     2119 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/providers/nlu_training_data_provider.py
+-rw-r--r--   0        0        0     1354 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/providers/responses_provider.py
+-rw-r--r--   0        0        0     1540 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/providers/rule_only_provider.py
+-rw-r--r--   0        0        0     1466 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/providers/story_graph_provider.py
+-rw-r--r--   0        0        0     1965 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/providers/training_tracker_provider.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/validators/__init__.py
+-rw-r--r--   0        0        0    22562 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/validators/default_recipe_validator.py
+-rw-r--r--   0        0        0    12863 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/graph_components/validators/finetuning_validator.py
+-rw-r--r--   0        0        0     1782 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/jupyter.py
+-rw-r--r--   0        0        0      101 2023-07-25 21:45:47.853881 rasa-3.8.0a1/rasa/keys
+-rw-r--r--   0        0        0     3490 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/model.py
+-rw-r--r--   0        0        0    14961 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/model_testing.py
+-rw-r--r--   0        0        0    16904 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/model_training.py
+-rw-r--r--   0        0        0      123 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/__init__.py
+-rw-r--r--   0        0        0      118 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/classifiers/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/classifiers/classifier.py
+-rw-r--r--   0        0        0    71637 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/classifiers/diet_classifier.py
+-rw-r--r--   0        0        0     7150 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/classifiers/fallback_classifier.py
+-rw-r--r--   0        0        0     7581 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/classifiers/keyword_intent_classifier.py
+-rw-r--r--   0        0        0     7568 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/classifiers/logistic_regression_classifier.py
+-rw-r--r--   0        0        0     5559 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/classifiers/mitie_intent_classifier.py
+-rw-r--r--   0        0        0     1989 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/classifiers/regex_message_handler.py
+-rw-r--r--   0        0        0    11915 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/classifiers/sklearn_intent_classifier.py
+-rw-r--r--   0        0        0     2757 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/constants.py
+-rw-r--r--   0        0        0     1317 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/convert.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/emulators/__init__.py
+-rw-r--r--   0        0        0     1748 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/emulators/dialogflow.py
+-rw-r--r--   0        0        0     1367 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/emulators/emulator.py
+-rw-r--r--   0        0        0     3032 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/emulators/luis.py
+-rw-r--r--   0        0        0      334 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/emulators/no_emulator.py
+-rw-r--r--   0        0        0     1930 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/emulators/wit.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/extractors/__init__.py
+-rw-r--r--   0        0        0    26499 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/extractors/crf_entity_extractor.py
+-rw-r--r--   0        0        0     7685 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/extractors/duckling_entity_extractor.py
+-rw-r--r--   0        0        0     7160 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/extractors/entity_synonyms.py
+-rw-r--r--   0        0        0    17530 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/extractors/extractor.py
+-rw-r--r--   0        0        0    10973 2023-07-25 21:45:25.917720 rasa-3.8.0a1/rasa/nlu/extractors/mitie_entity_extractor.py
+-rw-r--r--   0        0        0     8289 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/extractors/regex_entity_extractor.py
+-rw-r--r--   0        0        0     3366 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/extractors/spacy_entity_extractor.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/dense_featurizer/__init__.py
+-rw-r--r--   0        0        0    17142 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py
+-rw-r--r--   0        0        0     2433 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py
+-rw-r--r--   0        0        0    30361 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py
+-rw-r--r--   0        0        0     5861 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py
+-rw-r--r--   0        0        0     4888 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py
+-rw-r--r--   0        0        0     3347 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/featurizer.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/sparse_featurizer/__init__.py
+-rw-r--r--   0        0        0    33295 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py
+-rw-r--r--   0        0        0    21810 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py
+-rw-r--r--   0        0        0    10289 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py
+-rw-r--r--   0        0        0      220 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/featurizers/sparse_featurizer/sparse_featurizer.py
+-rw-r--r--   0        0        0      557 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/model.py
+-rw-r--r--   0        0        0     8333 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/persistor.py
+-rw-r--r--   0        0        0      803 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/run.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/selectors/__init__.py
+-rw-r--r--   0        0        0    39012 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/selectors/response_selector.py
+-rw-r--r--   0        0        0    67726 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/test.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/tokenizers/__init__.py
+-rw-r--r--   0        0        0     5374 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/tokenizers/jieba_tokenizer.py
+-rw-r--r--   0        0        0     2618 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/tokenizers/mitie_tokenizer.py
+-rw-r--r--   0        0        0     2378 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/tokenizers/spacy_tokenizer.py
+-rw-r--r--   0        0        0     8196 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     3750 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/tokenizers/whitespace_tokenizer.py
+-rw-r--r--   0        0        0      928 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/utils/__init__.py
+-rw-r--r--   0        0        0    14703 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/utils/bilou_utils.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/utils/hugging_face/__init__.py
+-rw-r--r--   0        0        0     3380 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/utils/hugging_face/registry.py
+-rw-r--r--   0        0        0     9143 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py
+-rw-r--r--   0        0        0     3887 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/utils/mitie_utils.py
+-rw-r--r--   0        0        0     5386 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/utils/pattern_utils.py
+-rw-r--r--   0        0        0    11795 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/nlu/utils/spacy_utils.py
+-rw-r--r--   0        0        0     4921 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/plugin.py
+-rw-r--r--   0        0        0    55720 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/server.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/shared/__init__.py
+-rw-r--r--   0        0        0     4406 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/shared/constants.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/shared/core/__init__.py
+-rw-r--r--   0        0        0     4853 2023-07-25 21:45:25.921720 rasa-3.8.0a1/rasa/shared/core/constants.py
+-rw-r--r--   0        0        0     1366 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/conversation.py
+-rw-r--r--   0        0        0    76046 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/domain.py
+-rw-r--r--   0        0        0    66732 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/events.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/flows/__init__.py
+-rw-r--r--   0        0        0    35957 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/flows/flow.py
+-rw-r--r--   0        0        0      120 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/flows/flows_yaml_schema.yml
+-rw-r--r--   0        0        0      674 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/flows/utils.py
+-rw-r--r--   0        0        0     2808 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/flows/yaml_flows_io.py
+-rw-r--r--   0        0        0    35597 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/generator.py
+-rw-r--r--   0        0        0     8286 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/slot_mappings.py
+-rw-r--r--   0        0        0    16371 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/slots.py
+-rw-r--r--   0        0        0    34744 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/trackers.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/training_data/__init__.py
+-rw-r--r--   0        0        0     2895 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/training_data/loading.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/training_data/story_reader/__init__.py
+-rw-r--r--   0        0        0     4449 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/training_data/story_reader/story_reader.py
+-rw-r--r--   0        0        0     6671 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/training_data/story_reader/story_step_builder.py
+-rw-r--r--   0        0        0    32976 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/training_data/story_reader/yaml_story_reader.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/training_data/story_writer/__init__.py
+-rw-r--r--   0        0        0     2543 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/training_data/story_writer/story_writer.py
+-rw-r--r--   0        0        0    14903 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/training_data/story_writer/yaml_story_writer.py
+-rw-r--r--   0        0        0    29313 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/training_data/structures.py
+-rw-r--r--   0        0        0     3500 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/training_data/visualization.html
+-rw-r--r--   0        0        0    20341 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/core/training_data/visualization.py
+-rw-r--r--   0        0        0     5479 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/data.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/engine/__init__.py
+-rw-r--r--   0        0        0      743 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/engine/caching.py
+-rw-r--r--   0        0        0     3633 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/importers/__init__.py
+-rw-r--r--   0        0        0    24941 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/importers/importer.py
+-rw-r--r--   0        0        0     7836 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/importers/multi_project.py
+-rw-r--r--   0        0        0     3803 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/importers/rasa.py
+-rw-r--r--   0        0        0     1215 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/importers/utils.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/nlu/__init__.py
+-rw-r--r--   0        0        0     1410 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/nlu/constants.py
+-rw-r--r--   0        0        0      188 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/nlu/interpreter.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/nlu/training_data/__init__.py
+-rw-r--r--   0        0        0     6759 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/nlu/training_data/entities_parser.py
+-rw-r--r--   0        0        0    14835 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/nlu/training_data/features.py
+-rw-r--r--   0        0        0      453 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/__init__.py
+-rw-r--r--   0        0        0     6123 2023-07-25 21:45:25.925720 rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/dialogflow.py
+-rw-r--r--   0        0        0     3014 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/luis.py
+-rw-r--r--   0        0        0     4495 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/rasa.py
+-rw-r--r--   0        0        0    22353 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/rasa_yaml.py
+-rw-r--r--   0        0        0     8540 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/readerwriter.py
+-rw-r--r--   0        0        0     1820 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/wit.py
+-rw-r--r--   0        0        0     4258 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/loading.py
+-rw-r--r--   0        0        0     1116 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/lookup_tables_parser.py
+-rw-r--r--   0        0        0    16662 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/message.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/schemas/__init__.py
+-rw-r--r--   0        0        0     2565 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/schemas/data_schema.py
+-rw-r--r--   0        0        0     1179 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/schemas/nlu.yml
+-rw-r--r--   0        0        0     1661 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/schemas/responses.yml
+-rw-r--r--   0        0        0     1476 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/synonyms_parser.py
+-rw-r--r--   0        0        0    28493 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/training_data.py
+-rw-r--r--   0        0        0     7040 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/nlu/training_data/util.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/__init__.py
+-rw-r--r--   0        0        0     2078 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/cli.py
+-rw-r--r--   0        0        0     8731 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/common.py
+-rw-r--r--   0        0        0    20606 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/io.py
+-rw-r--r--   0        0        0     5887 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/llm.py
+-rw-r--r--   0        0        0      883 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/pykwalify_extensions.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/schemas/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/schemas/config.yml
+-rw-r--r--   0        0        0     3286 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/schemas/domain.yml
+-rw-r--r--   0        0        0     5569 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/schemas/events.py
+-rw-r--r--   0        0        0      998 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/schemas/model_config.yml
+-rw-r--r--   0        0        0     4034 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/schemas/stories.yml
+-rw-r--r--   0        0        0    10317 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/shared/utils/validation.py
+-rw-r--r--   0        0        0    36273 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/telemetry.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/__init__.py
+-rw-r--r--   0        0        0    19638 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/common.py
+-rw-r--r--   0        0        0     1647 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/converter.py
+-rw-r--r--   0        0        0     8796 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/endpoints.py
+-rw-r--r--   0        0        0     7831 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/io.py
+-rw-r--r--   0        0        0     5036 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/log_utils.py
+-rw-r--r--   0        0        0    12246 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/plotting.py
+-rw-r--r--   0        0        0        0 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/__init__.py
+-rw-r--r--   0        0        0     4036 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/callback.py
+-rw-r--r--   0        0        0     3140 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/constants.py
+-rw-r--r--   0        0        0    19658 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/crf.py
+-rw-r--r--   0        0        0    15526 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/data_generator.py
+-rw-r--r--   0        0        0     5576 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/environment.py
+-rw-r--r--   0        0        0      168 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/exceptions.py
+-rw-r--r--   0        0        0    59263 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/layers.py
+-rw-r--r--   0        0        0     3319 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/layers_utils.py
+-rw-r--r--   0        0        0    10055 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/metrics.py
+-rw-r--r--   0        0        0    34572 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/model_data.py
+-rw-r--r--   0        0        0    18667 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/model_data_utils.py
+-rw-r--r--   0        0        0    36004 2023-07-25 21:45:25.929720 rasa-3.8.0a1/rasa/utils/tensorflow/models.py
+-rw-r--r--   0        0        0    49066 2023-07-25 21:45:25.933720 rasa-3.8.0a1/rasa/utils/tensorflow/rasa_layers.py
+-rw-r--r--   0        0        0    25509 2023-07-25 21:45:25.933720 rasa-3.8.0a1/rasa/utils/tensorflow/transformer.py
+-rw-r--r--   0        0        0      204 2023-07-25 21:45:25.933720 rasa-3.8.0a1/rasa/utils/tensorflow/types.py
+-rw-r--r--   0        0        0    20999 2023-07-25 21:45:25.933720 rasa-3.8.0a1/rasa/utils/train_utils.py
+-rw-r--r--   0        0        0    17708 2023-07-25 21:45:25.933720 rasa-3.8.0a1/rasa/validator.py
+-rw-r--r--   0        0        0      118 2023-07-25 21:45:25.933720 rasa-3.8.0a1/rasa/version.py
+-rw-r--r--   0        0        0    28229 1970-01-01 00:00:00.000000 rasa-3.8.0a1/PKG-INFO
```

### Comparing `rasa-3.7.0b2/LICENSE.txt` & `rasa-3.8.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/README.md` & `rasa-3.8.0a1/README.md`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/pyproject.toml` & `rasa-3.8.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 [tool.black]
 line-length = 88
 target-version = [ "py37", "py38", "py39", "py310",]
 exclude = "((.eggs | .git | .pytest_cache | build | dist))"
 
 [tool.poetry]
 name = "rasa"
-version = "3.7.0b2"
+version = "3.8.0a1"
 description = "Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants"
 authors = [ "Rasa Technologies GmbH <hi@rasa.com>",]
 maintainers = [ "Tom Bocklisch <tom@rasa.com>",]
 homepage = "https://rasa.com"
 repository = "https://github.com/rasahq/rasa"
 documentation = "https://rasa.com/docs"
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "License :: OSI Approved :: Apache Software License", "Topic :: Software Development :: Libraries",]
 keywords = [ "nlp", "machine-learning", "machine-learning-library", "bot", "bots", "botkit", "rasa conversational-agents", "conversational-ai", "chatbot", "chatbot-framework", "bot-framework",]
-include = [ "LICENSE.txt", "README.md", "rasa/shared/core/training_data/visualization.html", "rasa/cli/default_config.yml", "rasa/shared/importers/*", "rasa/utils/schemas/*", "rasa/keys",]
+include = [ "LICENSE.txt", "README.md", "rasa/shared/core/training_data/visualization.html", "rasa/cli/default_config.yml", "rasa/shared/importers/*", "rasa/utils/schemas/*", "rasa/keys", "rasa/core/channels/chat.html", "rasa/cdu/classifiers/command_prompt_template.jinja2",]
 readme = "README.md"
 license = "Apache-2.0"
 [[tool.poetry.source]]
 name = "internal repository mirroring psycopg binary for macos"
 url = "https://europe-west3-python.pkg.dev/rasa-releases/psycopg-binary/simple/"
 
 [tool.towncrier]
@@ -83,15 +83,15 @@
 
 [tool.ruff]
 ignore = [ "D100", "D104", "D105", "RUF001", "RUF002", "RUF003", "RUF005",]
 line-length = 88
 select = [ "D", "E", "F", "W", "RUF",]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8.1,<3.11"
 boto3 = "^1.26.136"
 requests = "^2.23"
 matplotlib = ">=3.1,<3.8"
 attrs = ">=19.3,<22.2"
 jsonpickle = ">=1.3,<3.1"
 redis = ">=4.5.3, <5.0"
 absl-py = ">=0.9,<1.5"
@@ -107,15 +107,14 @@
 webexteamssdk = ">=1.1.1,<1.7.0"
 mattermostwrapper = "~2.2"
 rocketchat_API = ">=0.6.31,<1.31.0"
 colorhash = ">=1.0.2,<1.3.0"
 jsonschema = ">=3.2,<4.18"
 packaging = ">=20.0,<21.0"
 pytz = ">=2019.1,<2023.0"
-rasa-sdk = "~3.7.0b1"
 colorclass = "~2.2"
 terminaltables = "~3.1.0"
 sanic = "~21.12"
 sanic-cors = "~2.0.0"
 sanic-jwt = "^1.6.0"
 sanic-routing = "^0.7.2"
 websockets = ">=10.0,<11.0"
@@ -145,16 +144,19 @@
 google-auth = "<3"
 CacheControl = "^0.12.9"
 randomname = "^0.1.5"
 pluggy = "^1.0.0"
 slack-sdk = "^3.19.2"
 confluent-kafka = ">=1.9.2,<3.0.0"
 portalocker = "^2.7.0"
+pypred = "^0.4.0"
 structlog = "^23.1.0"
 structlog-sentry = "^2.0.2"
+langchain = "^0.0.223"
+openai = "^0.27.8"
 [[tool.poetry.dependencies.tensorflow-io-gcs-filesystem]]
 version = "==0.31"
 markers = "sys_platform == 'win32'"
 
 [[tool.poetry.dependencies.tensorflow-io-gcs-filesystem]]
 version = "==0.32"
 markers = "sys_platform == 'linux'"
@@ -238,14 +240,18 @@
 log_cli_level = "WARNING"
 log_cli = true
 markers = [ "skip_on_windows", "skip_on_ci", "sequential", "category_cli", "category_core_featurizers", "category_policies", "category_nlu_featurizers", "category_nlu_predictors", "category_full_model_training", "category_other_unit_tests", "category_performance", "flaky",]
 timeout = 60
 timeout_func_only = true
 asyncio_mode = "auto"
 
+[tool.poetry.dependencies.rasa-sdk]
+version = "~3.8.0a1"
+allow-prereleases = true
+
 [tool.poetry.dependencies.tensorflow]
 version = "2.12.0"
 markers = "sys_platform != 'darwin' or platform_machine != 'arm64'"
 
 [tool.poetry.dependencies.tensorflow-intel]
 version = "2.12.0"
 markers = "sys_platform == 'win32'"
```

### Comparing `rasa-3.7.0b2/rasa/__main__.py` & `rasa-3.8.0a1/rasa/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from rasa.utils.log_utils import configure_structlog
 
 import rasa.telemetry
 import rasa.utils.io
 import rasa.utils.tensorflow.environment as tf_env
 from rasa import version
 from rasa.cli import (
+    chat,
     data,
     export,
     interactive,
     run,
     scaffold,
     shell,
     telemetry,
@@ -59,14 +60,15 @@
     parent_parsers = [parent_parser]
 
     subparsers = parser.add_subparsers(help="Rasa commands")
 
     scaffold.add_subparser(subparsers, parents=parent_parsers)
     run.add_subparser(subparsers, parents=parent_parsers)
     shell.add_subparser(subparsers, parents=parent_parsers)
+    chat.add_subparser(subparsers, parents=parent_parsers)
     train.add_subparser(subparsers, parents=parent_parsers)
     interactive.add_subparser(subparsers, parents=parent_parsers)
     telemetry.add_subparser(subparsers, parents=parent_parsers)
     test.add_subparser(subparsers, parents=parent_parsers)
     visualize.add_subparser(subparsers, parents=parent_parsers)
     data.add_subparser(subparsers, parents=parent_parsers)
     export.add_subparser(subparsers, parents=parent_parsers)
```

### Comparing `rasa-3.7.0b2/rasa/api.py` & `rasa-3.8.0a1/rasa/api.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/arguments/data.py` & `rasa-3.8.0a1/rasa/cli/arguments/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/arguments/default_arguments.py` & `rasa-3.8.0a1/rasa/cli/arguments/default_arguments.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/arguments/evaluate.py` & `rasa-3.8.0a1/rasa/cli/arguments/evaluate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/arguments/export.py` & `rasa-3.8.0a1/rasa/cli/arguments/export.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/arguments/interactive.py` & `rasa-3.8.0a1/rasa/cli/arguments/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/arguments/run.py` & `rasa-3.8.0a1/rasa/cli/arguments/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/arguments/test.py` & `rasa-3.8.0a1/rasa/cli/arguments/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/arguments/train.py` & `rasa-3.8.0a1/rasa/cli/arguments/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/arguments/visualize.py` & `rasa-3.8.0a1/rasa/cli/arguments/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/arguments/x.py` & `rasa-3.8.0a1/rasa/cli/arguments/x.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/data.py` & `rasa-3.8.0a1/rasa/cli/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/evaluate.py` & `rasa-3.8.0a1/rasa/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/export.py` & `rasa-3.8.0a1/rasa/cli/export.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/initial_project/actions/actions.py` & `rasa-3.8.0a1/rasa/cli/initial_project/actions/actions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/initial_project/config.yml` & `rasa-3.8.0a1/rasa/cli/initial_project/config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/initial_project/credentials.yml` & `rasa-3.8.0a1/rasa/cli/initial_project/credentials.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/initial_project/data/nlu.yml` & `rasa-3.8.0a1/rasa/cli/initial_project/data/nlu.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/initial_project/data/stories.yml` & `rasa-3.8.0a1/rasa/cli/initial_project/data/stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/initial_project/domain.yml` & `rasa-3.8.0a1/rasa/cli/initial_project/domain.yml`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,18 @@
   utter_cheer_up:
   - text: "Here is something to cheer you up:"
     image: "https://i.imgur.com/nGF1K8f.jpg"
 
   utter_did_that_help:
   - text: "Did that help you?"
 
+  utter_flow_continue_interrupted: 
+  - text: Let's continue with the previous topic {flow_name}.
+    metadata: {allow_variation: True}
+
   utter_happy:
   - text: "Great, carry on!"
 
   utter_goodbye:
   - text: "Bye"
 
   utter_iamabot:
```

### Comparing `rasa-3.7.0b2/rasa/cli/initial_project/endpoints.yml` & `rasa-3.8.0a1/rasa/cli/initial_project/endpoints.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/initial_project/tests/test_stories.yml` & `rasa-3.8.0a1/rasa/cli/initial_project/tests/test_stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/interactive.py` & `rasa-3.8.0a1/rasa/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/run.py` & `rasa-3.8.0a1/rasa/cli/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/scaffold.py` & `rasa-3.8.0a1/rasa/cli/scaffold.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,19 @@
         help="Automatically choose default options for prompts and suppress warnings.",
     )
     scaffold_parser.add_argument(
         "--init-dir",
         default=None,
         help="Directory where your project should be initialized.",
     )
-
+    scaffold_parser.add_argument(
+        "--dm2",
+        action="store_true",
+        help="Temporary. Whether to create a DM2 project or a classic one",
+    )
     scaffold_parser.set_defaults(func=run)
 
 
 def print_train_or_instructions(args: argparse.Namespace) -> None:
     """Train a model if the user wants to."""
     import questionary
     import rasa
@@ -123,29 +127,31 @@
                 "the project directory."
             )
 
 
 def init_project(args: argparse.Namespace, path: Text) -> None:
     """Inits project."""
     os.chdir(path)
-    create_initial_project(".")
+    create_initial_project(".", args.dm2)
     print(f"Created project directory at '{os.getcwd()}'.")
     print_train_or_instructions(args)
 
 
-def create_initial_project(path: Text) -> None:
+def create_initial_project(path: Text, is_dm2: bool = False) -> None:
     """Creates directory structure and templates for initial project."""
     from distutils.dir_util import copy_tree
 
-    copy_tree(scaffold_path(), path)
+    copy_tree(scaffold_path(is_dm2), path)
 
 
-def scaffold_path() -> Text:
+def scaffold_path(is_dm2: bool = False) -> Text:
     import pkg_resources
 
+    if is_dm2:
+        return pkg_resources.resource_filename(__name__, "initial_project_dm2")
     return pkg_resources.resource_filename(__name__, "initial_project")
 
 
 def print_cancel() -> None:
     print_success("Ok. You can continue setting up by running 'rasa init' 🙋🏽‍♀️")
     sys.exit(0)
```

### Comparing `rasa-3.7.0b2/rasa/cli/shell.py` & `rasa-3.8.0a1/rasa/cli/shell.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/telemetry.py` & `rasa-3.8.0a1/rasa/cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/test.py` & `rasa-3.8.0a1/rasa/cli/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/train.py` & `rasa-3.8.0a1/rasa/cli/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/utils.py` & `rasa-3.8.0a1/rasa/cli/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/visualize.py` & `rasa-3.8.0a1/rasa/cli/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/cli/x.py` & `rasa-3.8.0a1/rasa/cli/x.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/constants.py` & `rasa-3.8.0a1/rasa/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/actions/action.py` & `rasa-3.8.0a1/rasa/core/actions/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 import rasa.core
 from rasa.core.actions.constants import DEFAULT_SELECTIVE_DOMAIN, SELECTIVE_DOMAIN
 from rasa.core.constants import (
     DEFAULT_REQUEST_TIMEOUT,
     COMPRESS_ACTION_SERVER_REQUEST_ENV_NAME,
     DEFAULT_COMPRESS_ACTION_SERVER_REQUEST,
 )
-from rasa.core.nlg.callback import RESPONSE_ID_KEY
 from rasa.core.policies.policy import PolicyPrediction
 from rasa.nlu.constants import (
     RESPONSE_SELECTOR_DEFAULT_INTENT,
     RESPONSE_SELECTOR_PROPERTY_NAME,
     RESPONSE_SELECTOR_PREDICTION_KEY,
     RESPONSE_SELECTOR_UTTER_ACTION_KEY,
 )
 from rasa.plugin import plugin_manager
 from rasa.shared.constants import (
     DOCS_BASE_URL,
     DEFAULT_NLU_FALLBACK_INTENT_NAME,
     UTTER_PREFIX,
+    FLOW_PREFIX,
 )
 from rasa.shared.core import events
 from rasa.shared.core.constants import (
     USER_INTENT_OUT_OF_SCOPE,
     ACTION_LISTEN_NAME,
     ACTION_RESTART_NAME,
     ACTION_SEND_TEXT_NAME,
@@ -204,14 +204,18 @@
     # Users can override the form by defining an action with the same name as the form
     user_overrode_form_action = is_form and action_name_or_text in domain.user_actions
     if is_form and not user_overrode_form_action:
         from rasa.core.actions.forms import FormAction
 
         return FormAction(action_name_or_text, action_endpoint)
 
+    if action_name_or_text.startswith(FLOW_PREFIX):
+        from rasa.core.actions.flows import FlowTriggerAction
+
+        return FlowTriggerAction(action_name_or_text)
     return RemoteAction(action_name_or_text, action_endpoint)
 
 
 def create_bot_utterance(message: Dict[Text, Any]) -> BotUttered:
     """Create BotUttered event from message."""
     bot_message = BotUttered(
         text=message.pop("text", None),
@@ -306,23 +310,16 @@
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
         metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Simple run implementation uttering a (hopefully defined) response."""
-        response_ids_for_response = domain.response_ids_per_response.get(
-            self.utter_action, set()
-        )
-
-        response_id_list = list(response_ids_for_response)
-        response_id_list.sort()
-
         kwargs = {
-            RESPONSE_ID_KEY: response_id_list,
+            "domain_responses": domain.responses,
         }
 
         message = await nlg.generate(
             self.utter_action,
             tracker,
             output_channel.name(),
             **kwargs,
```

### Comparing `rasa-3.7.0b2/rasa/core/actions/forms.py` & `rasa-3.8.0a1/rasa/core/actions/forms.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/actions/loops.py` & `rasa-3.8.0a1/rasa/core/actions/loops.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/actions/two_stage_fallback.py` & `rasa-3.8.0a1/rasa/core/actions/two_stage_fallback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/agent.py` & `rasa-3.8.0a1/rasa/core/agent.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/brokers/broker.py` & `rasa-3.8.0a1/rasa/core/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/brokers/file.py` & `rasa-3.8.0a1/rasa/core/brokers/file.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/brokers/kafka.py` & `rasa-3.8.0a1/rasa/core/brokers/kafka.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import copy
 import os
 import json
 import logging
 import structlog
 import threading
 from asyncio import AbstractEventLoop
 from typing import Any, Text, List, Optional, Union, Dict, TYPE_CHECKING
@@ -236,18 +235,20 @@
             headers = [
                 (
                     "RASA_ENVIRONMENT",
                     bytes(self.rasa_environment, encoding=DEFAULT_ENCODING),
                 )
             ]
 
+        reduced_event = rasa.shared.core.events.remove_parse_data(event)
         structlogger.debug(
             "kafka.publish.event",
+            event_info="Logging a reduced version of the Kafka event",
             topic=self.topic,
-            rasa_event=copy.deepcopy(event),
+            rasa_event=reduced_event,
             partition_key=partition_key,
             headers=headers,
         )
 
         serialized_event = json.dumps(event).encode(DEFAULT_ENCODING)
 
         if self.producer is not None:
```

### Comparing `rasa-3.7.0b2/rasa/core/brokers/pika.py` & `rasa-3.8.0a1/rasa/core/brokers/pika.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import copy
 import json
 import logging
 import structlog
 import os
 import ssl
 from asyncio import AbstractEventLoop
 from collections import deque
@@ -294,28 +293,32 @@
 
     async def _publish(
         self, event: Dict[Text, Any], headers: Optional[Dict[Text, Text]] = None
     ) -> None:
         if self._exchange is None:
             return
 
+        reduced_event = rasa.shared.core.events.remove_parse_data(event)
+
         try:
             await self._exchange.publish(self._message(event, headers), "")
 
             structlogger.debug(
                 "pika.events.publish",
+                event_info="Logging a reduced version of the Pika event",
                 rabbitmq_exchange=RABBITMQ_EXCHANGE,
                 host=self.host,
-                rasa_event=copy.deepcopy(event),
+                rasa_event=reduced_event,
             )
         except Exception as e:
             structlogger.error(
                 "pika.events.publish.failed",
+                event_info="Logging a reduced version of the failed Pika event",
                 host=self.host,
-                rasa_event=copy.deepcopy(event),
+                rasa_event=reduced_event,
             )
             if self.should_keep_unpublished_messages:
                 self._unpublished_events.append(event)
 
             if self.raise_on_failure:
                 self.close()  # type: ignore[unused-coroutine]
                 raise e
```

### Comparing `rasa-3.7.0b2/rasa/core/brokers/sql.py` & `rasa-3.8.0a1/rasa/core/brokers/sql.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/__init__.py` & `rasa-3.8.0a1/rasa/core/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/botframework.py` & `rasa-3.8.0a1/rasa/core/channels/botframework.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/callback.py` & `rasa-3.8.0a1/rasa/core/channels/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/channel.py` & `rasa-3.8.0a1/rasa/core/channels/channel.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/console.py` & `rasa-3.8.0a1/rasa/core/channels/console.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/facebook.py` & `rasa-3.8.0a1/rasa/core/channels/facebook.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/hangouts.py` & `rasa-3.8.0a1/rasa/core/channels/hangouts.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/mattermost.py` & `rasa-3.8.0a1/rasa/core/channels/mattermost.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/rasa_chat.py` & `rasa-3.8.0a1/rasa/core/channels/rasa_chat.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/rest.py` & `rasa-3.8.0a1/rasa/core/channels/rest.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/rocketchat.py` & `rasa-3.8.0a1/rasa/core/channels/rocketchat.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/slack.py` & `rasa-3.8.0a1/rasa/core/channels/slack.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/socketio.py` & `rasa-3.8.0a1/rasa/core/channels/socketio.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,20 @@
 from sanic import Blueprint, response, Sanic
 from sanic.request import Request
 from sanic.response import HTTPResponse
 from socketio import AsyncServer
 
 logger = logging.getLogger(__name__)
 
+CHAT_TEMPLATE_PATH = "/chat.html"
+
 
 class SocketBlueprint(Blueprint):
+    """Blueprint for socketio connections."""
+
     def __init__(
         self, sio: AsyncServer, socketio_path: Text, *args: Any, **kwargs: Any
     ) -> None:
         """Creates a :class:`sanic.Blueprint` for routing socketio connenctions.
 
         :param sio: Instance of :class:`socketio.AsyncServer` class
         :param socketio_path: string indicating the route to accept requests on.
@@ -139,27 +143,27 @@
     @classmethod
     def from_credentials(cls, credentials: Optional[Dict[Text, Any]]) -> InputChannel:
         credentials = credentials or {}
         return cls(
             credentials.get("user_message_evt", "user_uttered"),
             credentials.get("bot_message_evt", "bot_uttered"),
             credentials.get("namespace"),
-            credentials.get("session_persistence", False),
+            credentials.get("session_persistence", True),
             credentials.get("socketio_path", "/socket.io"),
             credentials.get("jwt_key"),
             credentials.get("jwt_method", "HS256"),
             credentials.get("metadata_key", "metadata"),
         )
 
     def __init__(
         self,
         user_message_evt: Text = "user_uttered",
         bot_message_evt: Text = "bot_uttered",
         namespace: Optional[Text] = None,
-        session_persistence: bool = False,
+        session_persistence: bool = True,
         socketio_path: Optional[Text] = "/socket.io",
         jwt_key: Optional[Text] = None,
         jwt_method: Optional[Text] = "HS256",
         metadata_key: Optional[Text] = "metadata",
     ):
         """Creates a ``SocketIOInput`` object."""
         self.bot_message_evt = bot_message_evt
@@ -182,14 +186,20 @@
                 "workers or multiple Rasa Open Source instances. "
                 "Please use a different channel for external events in these "
                 "scenarios."
             )
             return None
         return SocketIOOutput(self.sio, self.bot_message_evt)
 
+    def chat_html_path(self) -> Text:
+        """Returns the path to the chat.html file."""
+        import pkg_resources
+
+        return pkg_resources.resource_filename(__name__, CHAT_TEMPLATE_PATH)
+
     def blueprint(
         self, on_new_message: Callable[[UserMessage], Awaitable[Any]]
     ) -> Blueprint:
         """Defines a Sanic blueprint."""
         # Workaround so that socketio works with requests from other origins.
         # https://github.com/miguelgrinberg/python-socketio/issues/205#issuecomment-493769183
         sio = AsyncServer(async_mode="sanic", cors_allowed_origins=[])
@@ -200,14 +210,18 @@
         # make sio object static to use in get_output_channel
         self.sio = sio
 
         @socketio_webhook.route("/", methods=["GET"])
         async def health(_: Request) -> HTTPResponse:
             return response.json({"status": "ok"})
 
+        @socketio_webhook.route("/chat.html", methods=["GET"])
+        async def chat(_: Request) -> HTTPResponse:
+            return await response.file(self.chat_html_path())
+
         @sio.on("connect", namespace=self.namespace)
         async def connect(sid: Text, environ: Dict, auth: Optional[Dict]) -> bool:
             if self.jwt_key:
                 jwt_payload = None
                 if auth and auth.get("token"):
                     jwt_payload = rasa.core.channels.channel.decode_bearer_token(
                         auth.get("token"), self.jwt_key, self.jwt_algorithm
```

### Comparing `rasa-3.7.0b2/rasa/core/channels/telegram.py` & `rasa-3.8.0a1/rasa/core/channels/telegram.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/twilio.py` & `rasa-3.8.0a1/rasa/core/channels/twilio.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/twilio_voice.py` & `rasa-3.8.0a1/rasa/core/channels/twilio_voice.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/channels/webexteams.py` & `rasa-3.8.0a1/rasa/core/channels/webexteams.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/constants.py` & `rasa-3.8.0a1/rasa/core/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/evaluation/marker.py` & `rasa-3.8.0a1/rasa/core/evaluation/marker.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/evaluation/marker_base.py` & `rasa-3.8.0a1/rasa/core/evaluation/marker_base.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/evaluation/marker_stats.py` & `rasa-3.8.0a1/rasa/core/evaluation/marker_stats.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/evaluation/marker_tracker_loader.py` & `rasa-3.8.0a1/rasa/core/evaluation/marker_tracker_loader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/exceptions.py` & `rasa-3.8.0a1/rasa/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/exporter.py` & `rasa-3.8.0a1/rasa/core/exporter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/featurizers/precomputation.py` & `rasa-3.8.0a1/rasa/core/featurizers/precomputation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/featurizers/single_state_featurizer.py` & `rasa-3.8.0a1/rasa/core/featurizers/single_state_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/featurizers/tracker_featurizers.py` & `rasa-3.8.0a1/rasa/core/featurizers/tracker_featurizers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/http_interpreter.py` & `rasa-3.8.0a1/rasa/core/http_interpreter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/jobs.py` & `rasa-3.8.0a1/rasa/core/jobs.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/lock.py` & `rasa-3.8.0a1/rasa/core/lock.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/lock_store.py` & `rasa-3.8.0a1/rasa/core/lock_store.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/migrate.py` & `rasa-3.8.0a1/rasa/core/migrate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/nlg/callback.py` & `rasa-3.8.0a1/rasa/core/nlg/callback.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import json
 import logging
-from typing import Text, Any, Dict, Optional
+from typing import List, Text, Any, Dict, Optional
 
 from rasa.core.constants import DEFAULT_REQUEST_TIMEOUT
-from rasa.core.nlg.generator import NaturalLanguageGenerator
+from rasa.core.nlg.generator import NaturalLanguageGenerator, ResponseVariationFilter
 from rasa.shared.core.trackers import DialogueStateTracker, EventVerbosity
 from rasa.shared.exceptions import RasaException
 from rasa.utils.endpoints import EndpointConfig
 
 logger = logging.getLogger(__name__)
 
 
@@ -15,14 +16,15 @@
 
     Used for validation of the response returned from the NLG endpoint.
     """
     return {
         "type": "object",
         "properties": {
             "text": {"type": "string"},
+            "id": {"type": ["string", "null"]},
             "buttons": {"type": ["array", "null"], "items": {"type": "object"}},
             "elements": {"type": ["array", "null"], "items": {"type": "object"}},
             "attachment": {"type": ["object", "null"]},
             "image": {"type": ["string", "null"]},
             "custom": {"type": "object"},
         },
     }
@@ -35,19 +37,19 @@
     utter_action: Text,
     tracker: DialogueStateTracker,
     output_channel: Text,
     **kwargs: Any,
 ) -> Dict[Text, Any]:
     """Create the json body for the NLG json body for the request."""
     tracker_state = tracker.current_state(EventVerbosity.ALL)
-    response_ids = kwargs.pop(RESPONSE_ID_KEY, [])
+    response_id = kwargs.pop("response_id", None)
 
     return {
         "response": utter_action,
-        "ids": response_ids,
+        "id": response_id,
         "arguments": kwargs,
         "tracker": tracker_state,
         "channel": {"name": output_channel},
     }
 
 
 class CallbackNaturalLanguageGenerator(NaturalLanguageGenerator):
@@ -67,25 +69,34 @@
         self,
         utter_action: Text,
         tracker: DialogueStateTracker,
         output_channel: Text,
         **kwargs: Any,
     ) -> Dict[Text, Any]:
         """Retrieve a named response from the domain using an endpoint."""
+        domain_responses = kwargs.pop("domain_responses")
+        response_id = self.fetch_response_id(
+            utter_action, tracker, output_channel, domain_responses
+        )
+        kwargs["response_id"] = response_id
+
         body = nlg_request_format(utter_action, tracker, output_channel, **kwargs)
 
         logger.debug(
             "Requesting NLG for {} from {}."
-            "".format(utter_action, self.nlg_endpoint.url)
+            "The request body is {}."
+            "".format(utter_action, self.nlg_endpoint.url, json.dumps(body))
         )
 
         response = await self.nlg_endpoint.request(
             method="post", json=body, timeout=DEFAULT_REQUEST_TIMEOUT
         )
 
+        logger.debug(f"Received NLG response: {json.dumps(response)}")
+
         if isinstance(response, dict) and self.validate_response(response):
             return response
         else:
             raise RasaException("NLG web endpoint returned an invalid response.")
 
     @staticmethod
     def validate_response(content: Optional[Dict[Text, Any]]) -> bool:
@@ -104,7 +115,33 @@
             raise RasaException(
                 f"{e.message}. Failed to validate NLG response from API, make sure "
                 f"your response from the NLG endpoint is valid. "
                 f"For more information about the format please consult the "
                 f"`nlg_response_format_spec` function from this same module: "
                 f"https://github.com/RasaHQ/rasa/blob/main/rasa/core/nlg/callback.py"
             )
+
+    @staticmethod
+    def fetch_response_id(
+        utter_action: Text,
+        tracker: DialogueStateTracker,
+        output_channel: Text,
+        domain_responses: Optional[Dict[Text, List[Dict[Text, Any]]]],
+    ) -> Optional[Text]:
+        """Fetch the response id for the utter action.
+
+        The response id is retrieved from the domain responses for the
+        utter action given the tracker state and channel.
+        """
+        if domain_responses is None:
+            logger.debug("Failed to fetch response id. Responses not provided.")
+            return None
+
+        response_filter = ResponseVariationFilter(domain_responses)
+        response_id = response_filter.get_response_variation_id(
+            utter_action, tracker, output_channel
+        )
+
+        if response_id is None:
+            logger.debug(f"Failed to fetch response id for action '{utter_action}'.")
+
+        return response_id
```

### Comparing `rasa-3.7.0b2/rasa/core/nlg/interpolator.py` & `rasa-3.8.0a1/rasa/core/nlg/interpolator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/nlg/response.py` & `rasa-3.8.0a1/rasa/core/nlg/response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import copy
 import logging
 
 from rasa.shared.core.trackers import DialogueStateTracker
 from typing import Text, Any, Dict, Optional, List
 
 from rasa.core.nlg import interpolator
-from rasa.core.nlg.generator import NaturalLanguageGenerator
-from rasa.shared.constants import RESPONSE_CONDITION, CHANNEL
+from rasa.core.nlg.generator import NaturalLanguageGenerator, ResponseVariationFilter
+from rasa.shared.constants import RESPONSE_CONDITION
 
 logger = logging.getLogger(__name__)
 
 
 class TemplatedNaturalLanguageGenerator(NaturalLanguageGenerator):
     """Natural language generator that generates messages based on responses.
 
@@ -22,90 +22,28 @@
         """Creates a Template Natural Language Generator.
 
         Args:
             responses: responses that will be used to generate messages.
         """
         self.responses = responses
 
-    def _matches_filled_slots(
-        self, filled_slots: Dict[Text, Any], response: Dict[Text, Any]
-    ) -> bool:
-        """Checks if the conditional response variation matches the filled slots."""
-        constraints = response.get(RESPONSE_CONDITION, [])
-        for constraint in constraints:
-            name = constraint["name"]
-            value = constraint["value"]
-            filled_slots_value = filled_slots.get(name)
-            if isinstance(filled_slots_value, str) and isinstance(value, str):
-                if filled_slots_value.casefold() != value.casefold():
-                    return False
-            elif filled_slots_value != value:
-                return False
-
-        return True
-
-    def _responses_for_utter_action(
-        self, utter_action: Text, output_channel: Text, filled_slots: Dict[Text, Any]
-    ) -> List[Dict[Text, Any]]:
-        """Returns array of responses that fit the channel, action and condition."""
-        default_responses = list(
-            filter(
-                lambda x: (x.get(RESPONSE_CONDITION) is None),
-                self.responses[utter_action],
-            )
-        )
-        conditional_responses = list(
-            filter(
-                lambda x: (
-                    x.get(RESPONSE_CONDITION)
-                    and self._matches_filled_slots(
-                        filled_slots=filled_slots, response=x
-                    )
-                ),
-                self.responses[utter_action],
-            )
-        )
-
-        conditional_channel = list(
-            filter(lambda x: (x.get(CHANNEL) == output_channel), conditional_responses)
-        )
-        conditional_no_channel = list(
-            filter(lambda x: (x.get(CHANNEL) is None), conditional_responses)
-        )
-        default_channel = list(
-            filter(lambda x: (x.get(CHANNEL) == output_channel), default_responses)
-        )
-        default_no_channel = list(
-            filter(lambda x: (x.get(CHANNEL) is None), default_responses)
-        )
-
-        if conditional_channel:
-            return conditional_channel
-
-        if default_channel:
-            return default_channel
-
-        if conditional_no_channel:
-            return conditional_no_channel
-
-        return default_no_channel
-
     # noinspection PyUnusedLocal
     def _random_response_for(
         self, utter_action: Text, output_channel: Text, filled_slots: Dict[Text, Any]
     ) -> Optional[Dict[Text, Any]]:
         """Select random response for the utter action from available ones.
 
         If channel-specific responses for the current output channel are given,
         only choose from channel-specific ones.
         """
         import numpy as np
 
         if utter_action in self.responses:
-            suitable_responses = self._responses_for_utter_action(
+            response_filter = ResponseVariationFilter(self.responses)
+            suitable_responses = response_filter.responses_for_utter_action(
                 utter_action, output_channel, filled_slots
             )
 
             if suitable_responses:
                 selected_response = np.random.choice(suitable_responses)
                 condition = selected_response.get(RESPONSE_CONDITION)
                 if condition:
```

### Comparing `rasa-3.7.0b2/rasa/core/policies/ensemble.py` & `rasa-3.8.0a1/rasa/core/policies/ensemble.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/policies/memoization.py` & `rasa-3.8.0a1/rasa/core/policies/memoization.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/policies/policy.py` & `rasa-3.8.0a1/rasa/core/policies/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 import abc
 import copy
 import logging
 from enum import Enum
 from pathlib import Path
+from rasa.cdu.flow_stack import FlowStack, StackFrameType
 from rasa.shared.core.events import Event
 from typing import (
     Any,
     List,
     Optional,
     Text,
     Dict,
@@ -101,14 +102,27 @@
         or both ML-based data and rule data, they need to override this method.
 
         Returns:
             The data type supported by this policy (ML-based training data).
         """
         return SupportedData.ML_DATA
 
+    @staticmethod
+    def supported_stack_frames() -> List[StackFrameType]:
+        """Returns the stack frames supported by the policy."""
+        return []
+
+    def supports_current_stack_frame(self, tracker: DialogueStateTracker) -> bool:
+        flow_stack = FlowStack.from_tracker(tracker)
+
+        if top_frame := flow_stack.top():
+            return top_frame.frame_type in self.supported_stack_frames()
+        else:
+            return True
+
     def __init__(
         self,
         config: Dict[Text, Any],
         model_storage: ModelStorage,
         resource: Resource,
         execution_context: ExecutionContext,
         featurizer: Optional[TrackerFeaturizer] = None,
```

### Comparing `rasa-3.7.0b2/rasa/core/policies/rule_policy.py` & `rasa-3.8.0a1/rasa/core/policies/rule_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/policies/ted_policy.py` & `rasa-3.8.0a1/rasa/core/policies/ted_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/policies/unexpected_intent_policy.py` & `rasa-3.8.0a1/rasa/core/policies/unexpected_intent_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/processor.py` & `rasa-3.8.0a1/rasa/core/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -716,18 +716,18 @@
 
         Returns:
             Parsed data extracted from the message.
         """
         if self.http_interpreter:
             parse_data = await self.http_interpreter.parse(message)
         else:
+            # Intent is not explicitly present. Pass message to graph.
             msg = YAMLStoryReader.unpack_regex_message(
                 message=Message({TEXT: message.text})
             )
-            # Intent is not explicitly present. Pass message to graph.
             if msg.data.get(INTENT) is None:
                 parse_data = self._parse_message_with_graph(
                     message, tracker, only_output_properties
                 )
             else:
                 parse_data = {
                     TEXT: "",
@@ -850,14 +850,16 @@
 
     async def _run_prediction_loop(
         self, output_channel: OutputChannel, tracker: DialogueStateTracker
     ) -> None:
         # keep taking actions decided by the policy until it chooses to 'listen'
         should_predict_another_action = True
 
+        tracker = self.run_command_processor(tracker)
+
         # action loop. predicts actions until we hit action listen
         while should_predict_another_action and self._should_handle_message(tracker):
             # this actually just calls the policy's method by the same name
             try:
                 action, prediction = self.predict_next_with_tracker_if_should(tracker)
             except ActionLimitReached:
                 logger.warning(
@@ -955,14 +957,25 @@
                 scheduler = await jobs.scheduler()
                 for scheduled_job in scheduler.get_jobs():
                     if event.cancels_job_with_name(
                         scheduled_job.name, tracker.sender_id
                     ):
                         scheduler.remove_job(scheduled_job.id)
 
+    def run_command_processor(
+        self, tracker: DialogueStateTracker
+    ) -> DialogueStateTracker:
+        target = "command_processor"
+        results = self.graph_runner.run(
+            inputs={PLACEHOLDER_TRACKER: tracker}, targets=[target]
+        )
+        events = results[target]
+        tracker.update_with_events(events, self.domain)
+        return tracker
+
     async def _run_action(
         self,
         action: rasa.core.actions.action.Action,
         tracker: DialogueStateTracker,
         output_channel: OutputChannel,
         nlg: NaturalLanguageGenerator,
         prediction: PolicyPrediction,
```

### Comparing `rasa-3.7.0b2/rasa/core/run.py` & `rasa-3.8.0a1/rasa/core/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import logging
 import uuid
 import os
 from functools import partial
-from typing import Any, List, Optional, Text, Union, Dict
+from typing import Any, Callable, List, Optional, Text, Tuple, Union, Dict
 
 import rasa.core.utils
 from rasa.plugin import plugin_manager
 from rasa.shared.exceptions import RasaException
 import rasa.shared.utils.common
 import rasa.utils
 import rasa.utils.common
@@ -92,14 +92,15 @@
     log_file: Optional[Text] = None,
     conversation_id: Optional[Text] = uuid.uuid4().hex,
     use_syslog: bool = False,
     syslog_address: Optional[Text] = None,
     syslog_port: Optional[int] = None,
     syslog_protocol: Optional[Text] = None,
     request_timeout: Optional[int] = None,
+    server_listeners: Optional[List[Tuple[Callable, Text]]] = None,
 ) -> Sanic:
     """Run the agent."""
     rasa.core.utils.configure_file_logging(
         logger, log_file, use_syslog, syslog_address, syslog_port, syslog_protocol
     )
 
     if enable_api:
@@ -143,14 +144,18 @@
 
             logger.info("Killing Sanic server now.")
             running_app.stop()  # kill the sanic server
             plugin_manager().hook.after_server_stop()
 
         app.add_task(run_cmdline_io)
 
+    if server_listeners:
+        for (listener, event) in server_listeners:
+            app.register_listener(listener, event)
+
     return app
 
 
 def serve_application(
     model_path: Optional[Text] = None,
     channel: Optional[Text] = None,
     interface: Optional[Text] = constants.DEFAULT_SERVER_INTERFACE,
@@ -172,14 +177,15 @@
     ssl_password: Optional[Text] = None,
     conversation_id: Optional[Text] = uuid.uuid4().hex,
     use_syslog: Optional[bool] = False,
     syslog_address: Optional[Text] = None,
     syslog_port: Optional[int] = None,
     syslog_protocol: Optional[Text] = None,
     request_timeout: Optional[int] = None,
+    server_listeners: Optional[List[Tuple[Callable, Text]]] = None,
 ) -> None:
     """Run the API entrypoint."""
     if not channel and not credentials:
         channel = "cmdline"
 
     input_channels = create_http_input_channels(channel, credentials)
 
@@ -197,14 +203,15 @@
         log_file=log_file,
         conversation_id=conversation_id,
         use_syslog=use_syslog,
         syslog_address=syslog_address,
         syslog_port=syslog_port,
         syslog_protocol=syslog_protocol,
         request_timeout=request_timeout,
+        server_listeners=server_listeners,
     )
 
     ssl_context = server.create_ssl_context(
         ssl_certificate, ssl_keyfile, ssl_ca_file, ssl_password
     )
     protocol = "https" if ssl_context else "http"
```

### Comparing `rasa-3.7.0b2/rasa/core/test.py` & `rasa-3.8.0a1/rasa/core/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/tracker_store.py` & `rasa-3.8.0a1/rasa/core/tracker_store.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/train.py` & `rasa-3.8.0a1/rasa/core/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/training/__init__.py` & `rasa-3.8.0a1/rasa/core/training/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/training/converters/responses_prefix_converter.py` & `rasa-3.8.0a1/rasa/core/training/converters/responses_prefix_converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/training/interactive.py` & `rasa-3.8.0a1/rasa/core/training/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/training/story_conflict.py` & `rasa-3.8.0a1/rasa/core/training/story_conflict.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/training/training.py` & `rasa-3.8.0a1/rasa/core/training/training.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/utils.py` & `rasa-3.8.0a1/rasa/core/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/core/visualize.py` & `rasa-3.8.0a1/rasa/core/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/caching.py` & `rasa-3.8.0a1/rasa/engine/caching.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import abc
 import logging
-import os
 import shutil
 from datetime import datetime
 from pathlib import Path
 from typing import Text, Any, Optional, Tuple, List
 
 from packaging import version
 from sqlalchemy.engine import URL
@@ -20,25 +19,22 @@
 import rasa.shared.utils.common
 from rasa.constants import MINIMUM_COMPATIBLE_VERSION
 import sqlalchemy as sa
 import sqlalchemy.orm
 from sqlalchemy.ext.declarative import declarative_base, DeclarativeMeta
 
 from rasa.engine.storage.storage import ModelStorage
+from rasa.shared.engine.caching import (
+    get_local_cache_location,
+    get_max_cache_size,
+    get_cache_database_name,
+)
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_CACHE_LOCATION = Path(".rasa", "cache")
-DEFAULT_CACHE_NAME = "cache.db"
-DEFAULT_CACHE_SIZE_MB = 1000
-
-CACHE_LOCATION_ENV = "RASA_CACHE_DIRECTORY"
-CACHE_DB_NAME_ENV = "RASA_CACHE_NAME"
-CACHE_SIZE_ENV = "RASA_MAX_CACHE_SIZE"
-
 
 class TrainingCache(abc.ABC):
     """Stores training results in a persistent cache.
 
     Used to minimize re-retraining when the data / config didn't change in between
     training runs.
     """
@@ -166,36 +162,32 @@
     def __init__(self) -> None:
         """Creates cache.
 
         The `Cache` setting can be configured via environment variables.
         """
         self._cache_location = LocalTrainingCache._get_cache_location()
 
-        self._max_cache_size = float(
-            os.environ.get(CACHE_SIZE_ENV, DEFAULT_CACHE_SIZE_MB)
-        )
-
-        self._cache_database_name = os.environ.get(
-            CACHE_DB_NAME_ENV, DEFAULT_CACHE_NAME
-        )
+        self._max_cache_size = get_max_cache_size()
+
+        self._cache_database_name = get_cache_database_name()
 
         if not self._cache_location.exists() and not self._is_disabled():
             logger.debug(
                 f"Creating caching directory '{self._cache_location}' because "
                 f"it doesn't exist yet."
             )
             self._cache_location.mkdir(parents=True)
 
         self._sessionmaker = self._create_database()
 
         self._drop_cache_entries_from_incompatible_versions()
 
     @staticmethod
     def _get_cache_location() -> Path:
-        return Path(os.environ.get(CACHE_LOCATION_ENV, DEFAULT_CACHE_LOCATION))
+        return get_local_cache_location()
 
     def _create_database(self) -> sqlalchemy.orm.sessionmaker:
         if self._is_disabled():
             # Use in-memory database as mock to avoid having to check `_is_disabled`
             # everywhere
             database = ""
         else:
```

### Comparing `rasa-3.7.0b2/rasa/engine/graph.py` & `rasa-3.8.0a1/rasa/engine/graph.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/loader.py` & `rasa-3.8.0a1/rasa/engine/loader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/recipes/config_files/default_config.yml` & `rasa-3.8.0a1/rasa/engine/recipes/config_files/default_config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/recipes/default_components.py` & `rasa-3.8.0a1/rasa/engine/recipes/default_components.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from rasa.nlu.classifiers.diet_classifier import DIETClassifier
 from rasa.nlu.classifiers.fallback_classifier import FallbackClassifier
 from rasa.nlu.classifiers.keyword_intent_classifier import KeywordIntentClassifier
+from rasa.cdu.command_generator.llm_command_generator import LLMCommandGenerator
 from rasa.nlu.classifiers.logistic_regression_classifier import (
     LogisticRegressionClassifier,
 )
 from rasa.nlu.classifiers.mitie_intent_classifier import MitieIntentClassifier
 from rasa.nlu.classifiers.sklearn_intent_classifier import SklearnIntentClassifier
 from rasa.nlu.extractors.crf_entity_extractor import CRFEntityExtractor
 from rasa.nlu.extractors.duckling_entity_extractor import DucklingEntityExtractor
@@ -41,14 +42,15 @@
     # Message Classifiers
     DIETClassifier,
     FallbackClassifier,
     KeywordIntentClassifier,
     MitieIntentClassifier,
     SklearnIntentClassifier,
     LogisticRegressionClassifier,
+    LLMCommandGenerator,
     # Response Selectors
     ResponseSelector,
     # Message Entity Extractors
     CRFEntityExtractor,
     DucklingEntityExtractor,
     EntitySynonymMapper,
     MitieEntityExtractor,
```

### Comparing `rasa-3.7.0b2/rasa/engine/recipes/default_recipe.py` & `rasa-3.8.0a1/rasa/engine/recipes/default_recipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 import dataclasses
 
 from rasa.core.featurizers.precomputation import (
     CoreFeaturizationInputConverter,
     CoreFeaturizationCollector,
 )
+from rasa.graph_components.providers.flows_provider import FlowsProvider
+from rasa.cdu.command_processor_component import CommandProcessorComponent
 from rasa.plugin import plugin_manager
 from rasa.shared.exceptions import FileNotFoundException
 from rasa.core.policies.ensemble import DefaultPolicyPredictionEnsemble
 
 from rasa.engine.graph import (
     GraphSchema,
     GraphComponent,
@@ -93,14 +95,15 @@
         MESSAGE_TOKENIZER = 0
         MESSAGE_FEATURIZER = 1
         INTENT_CLASSIFIER = 2
         ENTITY_EXTRACTOR = 3
         POLICY_WITHOUT_END_TO_END_SUPPORT = 4
         POLICY_WITH_END_TO_END_SUPPORT = 5
         MODEL_LOADER = 6
+        COMMAND_GENERATOR = 7
 
     name = "default.v1"
     _registered_components: Dict[Text, RegisteredComponent] = {}
 
     def __init__(self) -> None:
         """Creates recipe."""
         self._use_core = True
@@ -283,15 +286,25 @@
         cli_parameters: Dict[Text, Any],
     ) -> List[Text]:
         plugin_manager().hook.modify_default_recipe_graph_train_nodes(
             train_config=train_config,
             train_nodes=train_nodes,
             cli_parameters=cli_parameters,
         )
-
+        train_nodes["flows_provider"] = SchemaNode(
+            needs={
+                "importer": "finetuning_validator",
+            },
+            uses=FlowsProvider,
+            constructor_name="create",
+            fn="provide_train",
+            config={},
+            is_target=True,
+            is_input=True,
+        )
         persist_nlu_data = bool(cli_parameters.get("persist_nlu_training_data"))
         train_nodes["nlu_training_data_provider"] = SchemaNode(
             needs={"importer": "finetuning_validator"},
             uses=NLUTrainingDataProvider,
             constructor_name="create",
             fn="provide",
             config={
@@ -577,14 +590,25 @@
             needs={"importer": "finetuning_validator"},
             uses=StoryGraphProvider,
             constructor_name="create",
             fn="provide",
             config={"exclusion_percentage": cli_parameters.get("exclusion_percentage")},
             is_input=True,
         )
+        train_nodes["flows_provider"] = SchemaNode(
+            needs={
+                "importer": "finetuning_validator",
+            },
+            uses=FlowsProvider,
+            constructor_name="create",
+            fn="provide_train",
+            config={},
+            is_target=True,
+            is_input=True,
+        )
         train_nodes["training_tracker_provider"] = SchemaNode(
             needs={
                 "story_graph": "story_graph_provider",
                 "domain": "domain_for_core_training_provider",
             },
             uses=TrainingTrackerProvider,
             constructor_name="create",
@@ -715,14 +739,24 @@
         predict_config: Dict[Text, Any],
         predict_nodes: Dict[Text, SchemaNode],
         train_nodes: Dict[Text, SchemaNode],
     ) -> Text:
         plugin_manager().hook.modify_default_recipe_graph_predict_nodes(
             predict_nodes=predict_nodes
         )
+        # LLMFlowClassifier needs flows
+        predict_nodes["flows_provider"] = SchemaNode(
+            **DEFAULT_PREDICT_KWARGS,
+            needs={},
+            uses=FlowsProvider,
+            fn="provide_inference",
+            config={},
+            resource=Resource("flows_provider"),
+        )
+
         for idx, config in enumerate(predict_config["pipeline"]):
             component_name = config.pop("name")
             component = self._from_registry(component_name)
             component_name = f"{component_name}{idx}"
             if self.ComponentType.MODEL_LOADER in component.types:
                 predict_nodes[f"provide_{component_name}"] = SchemaNode(
                     **DEFAULT_PREDICT_KWARGS,
@@ -746,14 +780,15 @@
                     config,
                     from_resource=component.is_trainable,
                 )
             elif component.types.intersection(
                 {
                     self.ComponentType.INTENT_CLASSIFIER,
                     self.ComponentType.ENTITY_EXTRACTOR,
+                    self.ComponentType.COMMAND_GENERATOR,
                 }
             ):
                 if component.is_trainable:
                     last_run_node = self._add_nlu_predict_node_from_train(
                         predict_nodes,
                         component_name,
                         train_nodes,
@@ -835,22 +870,41 @@
             **DEFAULT_PREDICT_KWARGS,
             needs={},
             uses=DomainProvider,
             fn="provide_inference",
             config={},
             resource=Resource("domain_provider"),
         )
+        predict_nodes["flows_provider"] = SchemaNode(
+            **DEFAULT_PREDICT_KWARGS,
+            needs={},
+            uses=FlowsProvider,
+            fn="provide_inference",
+            config={},
+            resource=Resource("flows_provider"),
+        )
 
         node_with_e2e_features = None
 
         if "end_to_end_features_provider" in train_nodes:
             node_with_e2e_features = self._add_end_to_end_features_for_inference(
                 predict_nodes, preprocessors
             )
 
+        predict_nodes["command_processor"] = SchemaNode(
+            **DEFAULT_PREDICT_KWARGS,
+            needs=self._get_needs_from_args(
+                CommandProcessorComponent, "execute_commands"
+            ),
+            uses=CommandProcessorComponent,
+            fn="execute_commands",
+            config={},
+            resource=Resource("command_processor"),
+        )
+
         rule_policy_resource = None
         policies: List[Text] = []
 
         for idx, config in enumerate(predict_config["policies"]):
             component_name = config.pop("name")
             component = self._from_registry(component_name)
```

### Comparing `rasa-3.7.0b2/rasa/engine/recipes/graph_recipe.py` & `rasa-3.8.0a1/rasa/engine/recipes/graph_recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/recipes/recipe.py` & `rasa-3.8.0a1/rasa/engine/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/runner/dask.py` & `rasa-3.8.0a1/rasa/engine/runner/dask.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/runner/interface.py` & `rasa-3.8.0a1/rasa/engine/runner/interface.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/storage/local_model_storage.py` & `rasa-3.8.0a1/rasa/engine/storage/local_model_storage.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/storage/resource.py` & `rasa-3.8.0a1/rasa/engine/storage/resource.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/storage/storage.py` & `rasa-3.8.0a1/rasa/engine/storage/storage.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/training/components.py` & `rasa-3.8.0a1/rasa/engine/training/components.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/training/fingerprinting.py` & `rasa-3.8.0a1/rasa/engine/training/fingerprinting.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/training/graph_trainer.py` & `rasa-3.8.0a1/rasa/engine/training/graph_trainer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/training/hooks.py` & `rasa-3.8.0a1/rasa/engine/training/hooks.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/engine/validation.py` & `rasa-3.8.0a1/rasa/engine/validation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/exceptions.py` & `rasa-3.8.0a1/rasa/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/graph_components/converters/nlu_message_converter.py` & `rasa-3.8.0a1/rasa/graph_components/converters/nlu_message_converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/graph_components/providers/domain_for_core_training_provider.py` & `rasa-3.8.0a1/rasa/graph_components/providers/domain_for_core_training_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/graph_components/providers/domain_provider.py` & `rasa-3.8.0a1/rasa/graph_components/providers/domain_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/graph_components/providers/forms_provider.py` & `rasa-3.8.0a1/rasa/graph_components/providers/forms_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/graph_components/providers/nlu_training_data_provider.py` & `rasa-3.8.0a1/rasa/graph_components/providers/nlu_training_data_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/graph_components/providers/responses_provider.py` & `rasa-3.8.0a1/rasa/graph_components/providers/responses_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/graph_components/providers/rule_only_provider.py` & `rasa-3.8.0a1/rasa/graph_components/providers/rule_only_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/graph_components/providers/story_graph_provider.py` & `rasa-3.8.0a1/rasa/graph_components/providers/story_graph_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/graph_components/providers/training_tracker_provider.py` & `rasa-3.8.0a1/rasa/graph_components/providers/training_tracker_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/graph_components/validators/default_recipe_validator.py` & `rasa-3.8.0a1/rasa/graph_components/validators/default_recipe_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from rasa.shared.constants import (
     DEFAULT_CONFIG_PATH,
     DOCS_URL_COMPONENTS,
     DOCS_URL_DEFAULT_ACTIONS,
     DOCS_URL_POLICIES,
     DOCS_URL_RULES,
 )
-from rasa.shared.core.domain import Domain, InvalidDomain
+from rasa.shared.core.domain import Domain
 from rasa.shared.core.constants import (
     ACTION_BACK_NAME,
     ACTION_RESTART_NAME,
     USER_INTENT_BACK,
     USER_INTENT_RESTART,
 )
 from rasa.shared.exceptions import InvalidConfigException
@@ -379,15 +379,15 @@
             rasa.shared.utils.io.raise_warning(
                 "Found data for training policies but no policy was configured.",
                 docs=DOCS_URL_POLICIES,
             )
         if not self._policy_schema_nodes:
             return
         self._warn_if_no_rule_policy_is_contained()
-        self._raise_if_domain_contains_form_names_but_no_rule_policy_given(domain)
+        self._warn_if_domain_contains_form_names_but_no_rule_policy_given(domain)
         self._raise_if_a_rule_policy_is_incompatible_with_domain(domain)
         self._validate_policy_priorities()
         self._warn_if_rule_based_data_is_unused_or_missing(story_graph=story_graph)
 
     def _warn_if_no_rule_policy_is_contained(self) -> None:
         """Warns if there is no rule policy among the given policies."""
         if not any(node.uses == RulePolicy for node in self._policy_schema_nodes):
@@ -396,30 +396,26 @@
                 f"policy configuration. Default intents such as "
                 f"'{USER_INTENT_RESTART}' and '{USER_INTENT_BACK}' will "
                 f"not trigger actions '{ACTION_RESTART_NAME}' and "
                 f"'{ACTION_BACK_NAME}'.",
                 docs=DOCS_URL_DEFAULT_ACTIONS,
             )
 
-    def _raise_if_domain_contains_form_names_but_no_rule_policy_given(
+    def _warn_if_domain_contains_form_names_but_no_rule_policy_given(
         self, domain: Domain
     ) -> None:
-        """Validates that there exists a rule policy if forms are defined.
-
-        Raises:
-            `InvalidConfigException` if domain and rule policies do not match
-        """
+        """Validates that there exists a rule policy if forms are defined."""
         contains_rule_policy = any(
             schema_node
             for schema_node in self._graph_schema.nodes.values()
             if issubclass(schema_node.uses, RulePolicy)
         )
 
         if domain.form_names and not contains_rule_policy:
-            raise InvalidDomain(
+            rasa.shared.utils.io.raise_warning(
                 "You have defined a form action, but have not added the "
                 f"'{RulePolicy.__name__}' to your policy ensemble. "
                 f"Either remove all forms from your domain or add the "
                 f"'{RulePolicy.__name__}' to your policy configuration."
             )
 
     def _raise_if_a_rule_policy_is_incompatible_with_domain(
```

### Comparing `rasa-3.7.0b2/rasa/graph_components/validators/finetuning_validator.py` & `rasa-3.8.0a1/rasa/graph_components/validators/finetuning_validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/jupyter.py` & `rasa-3.8.0a1/rasa/jupyter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/model.py` & `rasa-3.8.0a1/rasa/model.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/model_testing.py` & `rasa-3.8.0a1/rasa/model_testing.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/model_training.py` & `rasa-3.8.0a1/rasa/model_training.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,14 +160,15 @@
         An instance of `TrainingResult`.
     """
     file_importer = TrainingDataImporter.load_from_config(
         config, domain, training_files, core_additional_arguments
     )
 
     stories = file_importer.get_stories()
+    flows = file_importer.get_flows()
     nlu_data = file_importer.get_nlu_data()
 
     training_type = TrainingType.BOTH
 
     if nlu_data.has_e2e_examples():
         rasa.shared.utils.common.mark_as_experimental_feature("end-to-end training")
         training_type = TrainingType.END_TO_END
@@ -184,17 +185,17 @@
         rasa.shared.utils.cli.print_warning(
             "Core training was skipped because no valid domain file was found. "
             "Only an NLU-model was created. Please specify a valid domain using "
             "the '--domain' argument or check if the provided domain file exists."
         )
         training_type = TrainingType.NLU
 
-    elif stories.is_empty():
+    elif stories.is_empty() and flows.is_empty():
         rasa.shared.utils.cli.print_warning(
-            "No stories present. Just a Rasa NLU model will be trained."
+            "No stories or flows present. Just a Rasa NLU model will be trained."
         )
         training_type = TrainingType.NLU
 
     # We will train nlu if there are any nlu example, including from e2e stories.
     elif nlu_data.contains_no_pure_nlu_data() and not nlu_data.has_e2e_examples():
         rasa.shared.utils.cli.print_warning(
             "No NLU data present. Just a Rasa Core model will be trained."
```

### Comparing `rasa-3.7.0b2/rasa/nlu/classifiers/diet_classifier.py` & `rasa-3.8.0a1/rasa/nlu/classifiers/diet_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/classifiers/fallback_classifier.py` & `rasa-3.8.0a1/rasa/nlu/classifiers/fallback_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/classifiers/keyword_intent_classifier.py` & `rasa-3.8.0a1/rasa/nlu/classifiers/keyword_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/classifiers/logistic_regression_classifier.py` & `rasa-3.8.0a1/rasa/nlu/classifiers/logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/classifiers/mitie_intent_classifier.py` & `rasa-3.8.0a1/rasa/nlu/classifiers/mitie_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/classifiers/regex_message_handler.py` & `rasa-3.8.0a1/rasa/nlu/classifiers/regex_message_handler.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/classifiers/sklearn_intent_classifier.py` & `rasa-3.8.0a1/rasa/nlu/classifiers/sklearn_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/constants.py` & `rasa-3.8.0a1/rasa/nlu/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/convert.py` & `rasa-3.8.0a1/rasa/nlu/convert.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/emulators/dialogflow.py` & `rasa-3.8.0a1/rasa/nlu/emulators/dialogflow.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/emulators/emulator.py` & `rasa-3.8.0a1/rasa/nlu/emulators/emulator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/emulators/luis.py` & `rasa-3.8.0a1/rasa/nlu/emulators/luis.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/emulators/wit.py` & `rasa-3.8.0a1/rasa/nlu/emulators/wit.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/extractors/crf_entity_extractor.py` & `rasa-3.8.0a1/rasa/nlu/extractors/crf_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/extractors/duckling_entity_extractor.py` & `rasa-3.8.0a1/rasa/nlu/extractors/duckling_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/extractors/entity_synonyms.py` & `rasa-3.8.0a1/rasa/nlu/extractors/entity_synonyms.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/extractors/extractor.py` & `rasa-3.8.0a1/rasa/nlu/extractors/extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/extractors/mitie_entity_extractor.py` & `rasa-3.8.0a1/rasa/nlu/extractors/mitie_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/extractors/regex_entity_extractor.py` & `rasa-3.8.0a1/rasa/nlu/extractors/regex_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/extractors/spacy_entity_extractor.py` & `rasa-3.8.0a1/rasa/nlu/extractors/spacy_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py` & `rasa-3.8.0a1/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py` & `rasa-3.8.0a1/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py` & `rasa-3.8.0a1/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py` & `rasa-3.8.0a1/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py` & `rasa-3.8.0a1/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/featurizers/featurizer.py` & `rasa-3.8.0a1/rasa/nlu/featurizers/featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py` & `rasa-3.8.0a1/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py` & `rasa-3.8.0a1/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py` & `rasa-3.8.0a1/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/model.py` & `rasa-3.8.0a1/rasa/nlu/model.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/persistor.py` & `rasa-3.8.0a1/rasa/nlu/persistor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/run.py` & `rasa-3.8.0a1/rasa/nlu/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/selectors/response_selector.py` & `rasa-3.8.0a1/rasa/nlu/selectors/response_selector.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/test.py` & `rasa-3.8.0a1/rasa/nlu/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/tokenizers/jieba_tokenizer.py` & `rasa-3.8.0a1/rasa/nlu/tokenizers/jieba_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/tokenizers/mitie_tokenizer.py` & `rasa-3.8.0a1/rasa/nlu/tokenizers/mitie_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/tokenizers/spacy_tokenizer.py` & `rasa-3.8.0a1/rasa/nlu/tokenizers/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/tokenizers/tokenizer.py` & `rasa-3.8.0a1/rasa/nlu/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/tokenizers/whitespace_tokenizer.py` & `rasa-3.8.0a1/rasa/nlu/tokenizers/whitespace_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/utils/__init__.py` & `rasa-3.8.0a1/rasa/nlu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/utils/bilou_utils.py` & `rasa-3.8.0a1/rasa/nlu/utils/bilou_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/utils/hugging_face/registry.py` & `rasa-3.8.0a1/rasa/nlu/utils/hugging_face/registry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py` & `rasa-3.8.0a1/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/utils/mitie_utils.py` & `rasa-3.8.0a1/rasa/nlu/utils/mitie_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/utils/pattern_utils.py` & `rasa-3.8.0a1/rasa/nlu/utils/pattern_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/nlu/utils/spacy_utils.py` & `rasa-3.8.0a1/rasa/nlu/utils/spacy_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/plugin.py` & `rasa-3.8.0a1/rasa/plugin.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/server.py` & `rasa-3.8.0a1/rasa/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,19 +323,14 @@
         trackers = [await processor.get_tracker(conversation_id)]
 
     if until_time is not None:
         trackers = [tracker.travel_back_in_time(until_time) for tracker in trackers]
         # keep only non-empty trackers
         trackers = [tracker for tracker in trackers if len(tracker.events)]
 
-    logger.debug(
-        f"Fetched trackers for {len(trackers)} conversation sessions "
-        f"for conversation ID {conversation_id}."
-    )
-
     story_steps = []
 
     more_than_one_story = len(trackers) > 1
 
     for i, tracker in enumerate(trackers, 1):
         tracker.sender_id = conversation_id
 
@@ -715,20 +710,28 @@
     @app.get("/conversations/<conversation_id:path>/tracker")
     @requires_auth(app, auth_token)
     @ensure_loaded_agent(app)
     async def retrieve_tracker(request: Request, conversation_id: Text) -> HTTPResponse:
         """Get a dump of a conversation's tracker including its events."""
         verbosity = event_verbosity_parameter(request, EventVerbosity.AFTER_RESTART)
         until_time = rasa.utils.endpoints.float_arg(request, "until")
-
-        tracker = await app.ctx.agent.processor.fetch_full_tracker_with_initial_session(
-            conversation_id,
-            output_channel=CollectingOutputChannel(),
+        should_start_session = rasa.utils.endpoints.bool_arg(
+            request, "start_session", default=True
         )
 
+        if should_start_session:
+            tracker = (
+                await app.ctx.agent.processor.fetch_full_tracker_with_initial_session(
+                    conversation_id,
+                    output_channel=CollectingOutputChannel(),
+                )
+            )
+        else:
+            tracker = await app.ctx.agent.processor.get_tracker(conversation_id)
+
         try:
             if until_time is not None:
                 tracker = tracker.travel_back_in_time(until_time)
 
             state = tracker.current_state(verbosity)
             return response.json(state)
         except Exception as e:
@@ -824,15 +827,14 @@
                 "ConversationError",
                 f"An unexpected error occurred. Error: {e}",
             )
 
     @app.get("/conversations/<conversation_id:path>/story")
     @requires_auth(app, auth_token)
     @ensure_loaded_agent(app)
-    @ensure_conversation_exists()
     async def retrieve_story(request: Request, conversation_id: Text) -> HTTPResponse:
         """Get an end-to-end story corresponding to this conversation."""
         until_time = rasa.utils.endpoints.float_arg(request, "until")
         fetch_all_sessions = rasa.utils.endpoints.bool_arg(
             request, "all_sessions", default=False
         )
```

### Comparing `rasa-3.7.0b2/rasa/shared/constants.py` & `rasa-3.8.0a1/rasa/shared/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
 DEFAULT_LOG_LEVEL = "INFO"
 ENV_LOG_LEVEL = "LOG_LEVEL"
 TCP_PROTOCOL = "TCP"
 
 DEFAULT_SENDER_ID = "default"
 UTTER_PREFIX = "utter_"
+FLOW_PREFIX = "flow_"
 
 ASSISTANT_ID_KEY = "assistant_id"
 ASSISTANT_ID_DEFAULT_VALUE = "placeholder_default"
 
 CONFIG_MANDATORY_COMMON_KEYS = [ASSISTANT_ID_KEY]
 CONFIG_AUTOCONFIGURABLE_KEYS_CORE = ["policies"]
 CONFIG_AUTOCONFIGURABLE_KEYS_NLU = ["pipeline"]
@@ -104,7 +105,9 @@
 
 DIAGNOSTIC_DATA = "diagnostic_data"
 
 RESPONSE_CONDITION = "condition"
 CHANNEL = "channel"
 
 OPENAI_API_KEY_ENV_VAR = "OPENAI_API_KEY"
+
+RASA_DEFAULT_FLOW_PATTERN_PREFIX = "pattern_"
```

### Comparing `rasa-3.7.0b2/rasa/shared/core/constants.py` & `rasa-3.8.0a1/rasa/shared/core/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 ACTION_BACK_NAME = "action_back"
 ACTION_TWO_STAGE_FALLBACK_NAME = "action_two_stage_fallback"
 ACTION_UNLIKELY_INTENT_NAME = "action_unlikely_intent"
 RULE_SNIPPET_ACTION_NAME = "..."
 ACTION_EXTRACT_SLOTS = "action_extract_slots"
 ACTION_VALIDATE_SLOT_MAPPINGS = "action_validate_slot_mappings"
 
+
 DEFAULT_ACTION_NAMES = [
     ACTION_LISTEN_NAME,
     ACTION_RESTART_NAME,
     ACTION_SESSION_START_NAME,
     ACTION_DEFAULT_FALLBACK_NAME,
     ACTION_DEACTIVATE_LOOP_NAME,
     ACTION_REVERT_FALLBACK_EVENTS_NAME,
@@ -74,23 +75,40 @@
 # Key to access data in the event metadata
 # It specifies if an event was caused by an external entity (e.g. a sensor).
 IS_EXTERNAL = "is_external"
 
 ACTION_NAME_SENDER_ID_CONNECTOR_STR = "__sender_id:"
 
 REQUESTED_SLOT = "requested_slot"
+FLOW_STACK_SLOT = "flow_stack"
+PREVIOUS_FLOW_SLOT = "rasa_previous_flow"
+CANCELLED_FLOW_SLOT = "rasa_cancelled_flow"
+CORRECTED_SLOTS_SLOT = "rasa_corrected_slots"
+RETURN_VALUE_SLOT = "return_value"
+
+FLOW_SLOT_NAMES = [
+    FLOW_STACK_SLOT,
+    PREVIOUS_FLOW_SLOT,
+    CANCELLED_FLOW_SLOT,
+    CORRECTED_SLOTS_SLOT,
+    RETURN_VALUE_SLOT,
+]
 
 # slots for knowledge base
 SLOT_LISTED_ITEMS = "knowledge_base_listed_objects"
 SLOT_LAST_OBJECT = "knowledge_base_last_object"
 SLOT_LAST_OBJECT_TYPE = "knowledge_base_last_object_type"
 DEFAULT_KNOWLEDGE_BASE_ACTION = "action_query_knowledge_base"
 
 DEFAULT_SLOT_NAMES = {
     REQUESTED_SLOT,
+    FLOW_STACK_SLOT,
+    PREVIOUS_FLOW_SLOT,
+    CANCELLED_FLOW_SLOT,
+    CORRECTED_SLOTS_SLOT,
     SESSION_START_METADATA_SLOT,
     SLOT_LISTED_ITEMS,
     SLOT_LAST_OBJECT,
     SLOT_LAST_OBJECT_TYPE,
 }
```

### Comparing `rasa-3.7.0b2/rasa/shared/core/conversation.py` & `rasa-3.8.0a1/rasa/shared/core/conversation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/core/domain.py` & `rasa-3.8.0a1/rasa/shared/core/domain.py`

 * *Files 3% similar despite different names*

```diff
@@ -235,15 +235,14 @@
             The instantiated `Domain` object.
         """
         duplicates = data.pop("duplicates", None)
         if duplicates:
             warn_about_duplicates_found_during_domain_merging(duplicates)
 
         responses = data.get(KEY_RESPONSES, {})
-        response_ids_per_response = cls._collect_response_ids(responses)
 
         domain_slots = data.get(KEY_SLOTS, {})
         if domain_slots:
             rasa.shared.core.slot_mappings.validate_slot_mappings(domain_slots)
         slots = cls.collect_slots(domain_slots)
         domain_actions = data.get(KEY_ACTIONS, [])
         actions = cls._collect_action_names(domain_actions)
@@ -266,15 +265,14 @@
             slots=slots,
             responses=responses,
             action_names=actions,
             forms=data.get(KEY_FORMS, {}),
             data=Domain._cleaned_data(data),
             action_texts=data.get(KEY_E2E_ACTIONS, []),
             session_config=session_config,
-            response_ids_per_response=response_ids_per_response,
             **additional_arguments,
         )
 
     @staticmethod
     def _get_session_config(session_config: Dict) -> SessionConfig:
         session_expiration_time_min = session_config.get(SESSION_EXPIRATION_TIME_KEY)
 
@@ -763,18 +761,18 @@
         self.overridden_default_intents = self._collect_overridden_default_intents(
             intents
         )
 
         self.form_names, self.forms, overridden_form_actions = self._initialize_forms(
             forms
         )
+
         action_names += overridden_form_actions
 
         self.responses = responses
-        self.response_ids_per_response = kwargs.get("response_ids_per_response", {})
 
         self.action_texts = action_texts if action_texts is not None else []
 
         data_copy = copy.deepcopy(data)
         self._data = self._preprocess_domain_dict(
             data_copy,
             store_entities_as_slots,
@@ -950,27 +948,53 @@
         the rest.
         """
         return RESPONSE_IDENTIFIER_DELIMITER in response[0]
 
     def _add_default_slots(self) -> None:
         """Sets up the default slots and slot values for the domain."""
         self._add_requested_slot()
+        self._add_flow_slots()
         self._add_knowledge_base_slots()
         self._add_categorical_slot_default_value()
         self._add_session_metadata_slot()
 
     def _add_categorical_slot_default_value(self) -> None:
         """Add a default value to all categorical slots.
 
         All unseen values found for the slot will be mapped to this default value
         for featurization.
         """
         for slot in [s for s in self.slots if isinstance(s, CategoricalSlot)]:
             slot.add_default_value()
 
+    def _add_flow_slots(self) -> None:
+        """Adds the slots needed for the conversation flows.
+
+        Add a slot called `flow_step_slot` to the list of slots. The value of
+        this slot will hold the name of the id of the next step in the flow.
+
+        Add a slot called `flow_stack_slot` to the list of slots. The value of
+        this slot will be a call stack of the flow ids.
+        """
+        from rasa.shared.core.constants import FLOW_SLOT_NAMES
+
+        slot_names = [slot.name for slot in self.slots]
+
+        for flow_slot in FLOW_SLOT_NAMES:
+            if flow_slot not in slot_names:
+                self.slots.append(
+                    AnySlot(flow_slot, mappings=[], influence_conversation=False)
+                )
+            else:
+                # TODO: figure out what to do here.
+                logger.warning(
+                    f"Slot {flow_slot} is reserved for Rasa internal usage, "
+                    f"but it already exists. 🤔"
+                )
+
     def _add_requested_slot(self) -> None:
         """Add a slot called `requested_slot` to the list of slots.
 
         The value of this slot will hold the name of the slot which the user
         needs to fill in next (either explicitly or implicitly) as part of a form.
         """
         if self.form_names and rasa.shared.core.constants.REQUESTED_SLOT not in [
@@ -1915,74 +1939,14 @@
                         action_names += [action_name]
 
             elif action.startswith("validate_"):
                 action_names += [action]
 
         return action_names
 
-    @staticmethod
-    def _collect_response_ids(
-        responses: Dict[Text, List[Dict[Text, Any]]]
-    ) -> Dict[Text, Set[Text]]:
-        """Collects all response ids.
-
-        Args:
-            responses: The responses to collect the ids from.
-
-        Returns:
-            A dictionary mapping the response names to the set of response ids.
-        """
-        response_ids: Set[Text] = set()
-        response_ids_per_response: Dict[Text, Set[Text]] = {}
-        for response_name, response_variations in responses.items():
-            response_ids_for_response = (
-                Domain._collect_response_ids_for_response_variations(
-                    response_variations
-                )
-            )
-
-            already_present_response_ids = response_ids_for_response.intersection(
-                response_ids
-            )
-
-            if len(already_present_response_ids) > 0:
-                rasa.shared.utils.io.raise_warning(
-                    f"Duplicate response ids "
-                    f"'{already_present_response_ids}' "
-                    f"defined in domain."
-                )
-
-            response_ids.update(response_ids_for_response)
-            response_ids_per_response[response_name] = response_ids_for_response
-        return response_ids_per_response
-
-    @staticmethod
-    def _collect_response_ids_for_response_variations(
-        response_variations: List[Dict[Text, Any]]
-    ) -> Set[Text]:
-        """Collects all response ids of a particular response key name.
-
-        Args:
-            response_variations: The responses variations to collect the ids from.
-
-        Returns:
-            A set of response ids.
-        """
-        response_ids = set()
-        for response_variation in response_variations:
-            response_variation_id = response_variation.get("id")
-            if response_variation_id:
-                if response_variation_id in response_ids:
-                    rasa.shared.utils.io.raise_warning(
-                        f"Duplicate response id '{response_variation_id}' "
-                        f"defined in domain."
-                    )
-                response_ids.add(response_variation_id)
-        return response_ids
-
 
 def warn_about_duplicates_found_during_domain_merging(
     duplicates: Dict[Text, List[Text]]
 ) -> None:
     """Emits warning about found duplicates while loading multiple domain paths."""
     message = ""
     for key in [
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rasa-3.7.0b2/rasa/shared/core/events.py` & `rasa-3.8.0a1/rasa/shared/core/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,31 @@
     return (
         isinstance(first, ActionExecuted)
         and first.action_name == ACTION_SESSION_START_NAME
         and isinstance(second, SessionStarted)
     )
 
 
+def remove_parse_data(event: Dict[Text, Any]) -> Dict[Text, Any]:
+    """Reduce event details to the minimum necessary to be structlogged.
+
+    Deletes the parse_data key from the event if it exists.
+
+    Args:
+        event: The event to be reduced.
+
+    Returns:
+        A reduced copy of the event.
+    """
+    reduced_event = copy.deepcopy(event)
+    if "parse_data" in reduced_event:
+        del reduced_event["parse_data"]
+    return reduced_event
+
+
 E = TypeVar("E", bound="Event")
 
 
 class Event(ABC):
     """Describes events in conversation and how the affect the conversation state.
 
     Immutable representation of everything which happened during a conversation of the
```

### Comparing `rasa-3.7.0b2/rasa/shared/core/generator.py` & `rasa-3.8.0a1/rasa/shared/core/generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/core/slot_mappings.py` & `rasa-3.8.0a1/rasa/shared/core/slot_mappings.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/core/slots.py` & `rasa-3.8.0a1/rasa/shared/core/slots.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/core/trackers.py` & `rasa-3.8.0a1/rasa/shared/core/trackers.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,18 +194,18 @@
         # maximum number of events to store
         self._max_event_history = max_event_history
         # list of previously seen events
         self.events = self._create_events([])
         # id of the source of the messages
         self.sender_id = sender_id
         # slots that can be filled in this domain
+        self.slots: Dict[str, Slot] = AnySlotDict()
         if slots is not None:
             self.slots = {slot.name: copy.copy(slot) for slot in slots}
-        else:
-            self.slots = AnySlotDict()
+
         # file source of the messages
         self.sender_source = sender_source
         # whether the tracker belongs to a rule-based data
         self.is_rule_tracker = is_rule_tracker
 
         ###
         # current state of the tracker - MUST be re-creatable by processing
```

### Comparing `rasa-3.7.0b2/rasa/shared/core/training_data/loading.py` & `rasa-3.8.0a1/rasa/shared/core/training_data/loading.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/story_reader.py` & `rasa-3.8.0a1/rasa/shared/core/training_data/story_reader/story_reader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/story_step_builder.py` & `rasa-3.8.0a1/rasa/shared/core/training_data/story_reader/story_step_builder.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/yaml_story_reader.py` & `rasa-3.8.0a1/rasa/shared/core/training_data/story_reader/yaml_story_reader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/core/training_data/story_writer/story_writer.py` & `rasa-3.8.0a1/rasa/shared/core/training_data/story_writer/story_writer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/core/training_data/story_writer/yaml_story_writer.py` & `rasa-3.8.0a1/rasa/shared/core/training_data/story_writer/yaml_story_writer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/core/training_data/structures.py` & `rasa-3.8.0a1/rasa/shared/core/training_data/structures.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/core/training_data/visualization.html` & `rasa-3.8.0a1/rasa/shared/core/training_data/visualization.html`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/core/training_data/visualization.py` & `rasa-3.8.0a1/rasa/shared/core/training_data/visualization.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/data.py` & `rasa-3.8.0a1/rasa/shared/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/exceptions.py` & `rasa-3.8.0a1/rasa/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/importers/importer.py` & `rasa-3.8.0a1/rasa/shared/importers/importer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from abc import ABC, abstractmethod
 from functools import reduce
 from typing import Text, Optional, List, Dict, Set, Any, Tuple, Type, Union, cast
 import logging
 
+import pkg_resources
+
 import rasa.shared.constants
+from rasa.shared.core.flows.flow import FlowsList, QuestionFlowStep
 import rasa.shared.utils.common
 import rasa.shared.core.constants
 import rasa.shared.utils.io
 from rasa.shared.core.domain import (
+    KEY_FORMS,
     Domain,
     KEY_E2E_ACTIONS,
     KEY_INTENTS,
     KEY_RESPONSES,
     KEY_ACTIONS,
 )
 from rasa.shared.core.events import ActionExecuted, UserUttered
@@ -55,14 +59,25 @@
             exclusion_percentage: Amount of training data that should be excluded.
 
         Returns:
             `StoryGraph` containing all loaded stories.
         """
         ...
 
+    def get_flows(self) -> FlowsList:
+        """Retrieves the flows that should be used for training.
+
+        Default implementation returns an empty `FlowsList`. The default
+        implementation is required because of backwards compatibility.
+
+        Returns:
+            `FlowsList` containing all loaded flows.
+        """
+        return FlowsList(flows=[])
+
     def get_conversation_tests(self) -> StoryGraph:
         """Retrieves end-to-end conversation stories for testing.
 
         Returns:
             `StoryGraph` containing all loaded stories.
         """
         return self.get_stories()
@@ -136,15 +151,15 @@
         importer = TrainingDataImporter.load_from_config(
             config_path, domain_path, training_data_paths, args
         )
 
         if isinstance(importer, E2EImporter):
             # When we only train NLU then there is no need to enrich the data with
             # E2E data from Core training data.
-            importer = importer.importer
+            importer = importer._importer
 
         return NluDataImporter(importer)
 
     @staticmethod
     def load_from_dict(
         config: Optional[Dict] = None,
         config_path: Optional[Text] = None,
@@ -165,15 +180,17 @@
         ]
         importers = [importer for importer in importers if importer]
         if not importers:
             importers = [
                 RasaFileImporter(config_path, domain_path, training_data_paths)
             ]
 
-        return E2EImporter(ResponsesSyncImporter(CombinedDataImporter(importers)))
+        return E2EImporter(
+            FlowSyncImporter(ResponsesSyncImporter(CombinedDataImporter(importers)))
+        )
 
     @staticmethod
     def _importer_from_dict(
         importer_config: Dict,
         config_path: Text,
         domain_path: Optional[Text] = None,
         training_data_paths: Optional[List[Text]] = None,
@@ -285,14 +302,23 @@
         ]
 
         return reduce(
             lambda merged, other: merged.merge(other), stories, StoryGraph([])
         )
 
     @rasa.shared.utils.common.cached_method
+    def get_flows(self) -> FlowsList:
+        """Retrieves training stories / rules (see parent class for full docstring)."""
+        flow_lists = [importer.get_flows() for importer in self._importers]
+
+        return reduce(
+            lambda merged, other: merged.merge(other), flow_lists, FlowsList(flows=[])
+        )
+
+    @rasa.shared.utils.common.cached_method
     def get_conversation_tests(self) -> StoryGraph:
         """Retrieves conversation test stories (see parent class for full docstring)."""
         stories = [importer.get_conversation_tests() for importer in self._importers]
 
         return reduce(
             lambda merged, other: merged.merge(other), stories, StoryGraph([])
         )
@@ -314,35 +340,138 @@
                 "Auto-config for multiple importers is not supported; "
                 "using config as is."
             )
             return None
         return self._importers[0].get_config_file_for_auto_config()
 
 
-class ResponsesSyncImporter(TrainingDataImporter):
-    """Importer that syncs `responses` between Domain and NLU training data.
-
-    Synchronizes responses between Domain and NLU and
-    adds retrieval intent properties from the NLU training data
-    back to the Domain.
-    """
+class PassThroughImporter(TrainingDataImporter):
+    """Importer that passes through all calls to the actual importer."""
 
     def __init__(self, importer: TrainingDataImporter):
-        """Initializes the ResponsesSyncImporter."""
+        """Initializes the FlowSyncImporter."""
         self._importer = importer
 
     def get_config(self) -> Dict:
         """Retrieves model config (see parent class for full docstring)."""
         return self._importer.get_config()
 
-    @rasa.shared.utils.common.cached_method
+    def get_flows(self) -> FlowsList:
+        """Retrieves model flows (see parent class for full docstring)."""
+        return self._importer.get_flows()
+
     def get_config_file_for_auto_config(self) -> Optional[Text]:
         """Returns config file path for auto-config only if there is a single one."""
         return self._importer.get_config_file_for_auto_config()
 
+    def get_domain(self) -> Domain:
+        """Retrieves model domain (see parent class for full docstring)."""
+        return self._importer.get_domain()
+
+    def get_stories(self, exclusion_percentage: Optional[int] = None) -> StoryGraph:
+        """Retrieves training stories / rules (see parent class for full docstring)."""
+        return self._importer.get_stories(exclusion_percentage)
+
+    def get_conversation_tests(self) -> StoryGraph:
+        """Retrieves conversation test stories (see parent class for full docstring)."""
+        return self._importer.get_conversation_tests()
+
+    def get_nlu_data(self, language: Optional[Text] = "en") -> TrainingData:
+        """Updates NLU data with responses for retrieval intents from domain."""
+        return self._importer.get_nlu_data(language)
+
+
+DEFAULT_FLOW_FILE_NAME = "default_flows.yml"
+
+
+def load_default_flows() -> FlowsList:
+    """Loads the default flows from the file system."""
+    from rasa.shared.core.flows.yaml_flows_io import YAMLFlowsReader
+
+    default_flows_file = pkg_resources.resource_filename(
+        "rasa.core.policies", DEFAULT_FLOW_FILE_NAME
+    )
+
+    return YAMLFlowsReader.read_from_file(default_flows_file)
+
+
+def load_default_flows_domain() -> Domain:
+    """Loads the default flows from the file system."""
+    default_flows_file = pkg_resources.resource_filename(
+        "rasa.core.policies", DEFAULT_FLOW_FILE_NAME
+    )
+
+    return Domain.from_path(default_flows_file)
+
+
+class FlowSyncImporter(PassThroughImporter):
+    """Importer that syncs `flows` between Domain and flow training data."""
+
+    @rasa.shared.utils.common.cached_method
+    def get_flows(self) -> FlowsList:
+        flows = self._importer.get_flows()
+
+        if flows.is_empty():
+            # if there are no flows, we don't need to add the default flows either
+            return flows
+
+        default_flows = load_default_flows()
+
+        user_flow_ids = [flow.id for flow in flows.underlying_flows]
+        missing_default_flows = [
+            default_flow
+            for default_flow in default_flows.underlying_flows
+            if default_flow.id not in user_flow_ids
+        ]
+
+        return flows.merge(FlowsList(missing_default_flows))
+
+    @rasa.shared.utils.common.cached_method
+    def get_domain(self) -> Domain:
+        """Merge existing domain with properties of flows."""
+        domain = self._importer.get_domain()
+
+        flows = self.get_flows()
+
+        if flows.is_empty():
+            # if there are no flows, we don't need to add the default flows either
+            return domain
+
+        default_flows_domain = load_default_flows_domain()
+
+        flow_names = [
+            rasa.shared.constants.FLOW_PREFIX + flow.id
+            for flow in flows.underlying_flows
+        ]
+
+        all_question_steps = [
+            step
+            for flow in flows.underlying_flows
+            for step in flow.steps
+            if isinstance(step, QuestionFlowStep)
+        ]
+        forms = {}
+        for step in all_question_steps:
+            form_name = "question_" + step.question
+            forms[form_name] = {
+                rasa.shared.constants.REQUIRED_SLOTS_KEY: [step.question]
+            }
+
+        flow_domain = Domain.from_dict({KEY_ACTIONS: flow_names, KEY_FORMS: forms})
+        return domain.merge(flow_domain.merge(default_flows_domain))
+
+
+class ResponsesSyncImporter(PassThroughImporter):
+    """Importer that syncs `responses` between Domain and NLU training data.
+
+    Synchronizes responses between Domain and NLU and
+    adds retrieval intent properties from the NLU training data
+    back to the Domain.
+    """
+
     @rasa.shared.utils.common.cached_method
     def get_domain(self) -> Domain:
         """Merge existing domain with properties of retrieval intents in NLU data."""
         existing_domain = self._importer.get_domain()
         existing_nlu_data = self._importer.get_nlu_data()
 
         # Merge responses from NLU data with responses in the domain.
@@ -417,22 +546,14 @@
             {
                 KEY_INTENTS: retrieval_intent_properties,
                 KEY_RESPONSES: responses,
                 KEY_ACTIONS: action_names,
             }
         )
 
-    def get_stories(self, exclusion_percentage: Optional[int] = None) -> StoryGraph:
-        """Retrieves training stories / rules (see parent class for full docstring)."""
-        return self._importer.get_stories(exclusion_percentage)
-
-    def get_conversation_tests(self) -> StoryGraph:
-        """Retrieves conversation test stories (see parent class for full docstring)."""
-        return self._importer.get_conversation_tests()
-
     @rasa.shared.utils.common.cached_method
     def get_nlu_data(self, language: Optional[Text] = "en") -> TrainingData:
         """Updates NLU data with responses for retrieval intents from domain."""
         existing_nlu_data = self._importer.get_nlu_data(language)
         existing_domain = self._importer.get_domain()
 
         return existing_nlu_data.merge(
@@ -453,29 +574,25 @@
 
         Returns: TrainingData object with responses.
 
         """
         return TrainingData(responses=responses)
 
 
-class E2EImporter(TrainingDataImporter):
+class E2EImporter(PassThroughImporter):
     """Importer with the following functionality.
 
     - enhances the NLU training data with actions / user messages from the stories.
     - adds potential end-to-end bot messages from stories as actions to the domain
     """
 
-    def __init__(self, importer: TrainingDataImporter) -> None:
-        """Initializes the E2EImporter."""
-        self.importer = importer
-
     @rasa.shared.utils.common.cached_method
     def get_domain(self) -> Domain:
         """Retrieves model domain (see parent class for full docstring)."""
-        original = self.importer.get_domain()
+        original = self._importer.get_domain()
         e2e_domain = self._get_domain_with_e2e_actions()
 
         return original.merge(e2e_domain)
 
     def _get_domain_with_e2e_actions(self) -> Domain:
 
         stories = self.get_stories()
@@ -488,40 +605,22 @@
                     for event in story_step.events
                     if isinstance(event, ActionExecuted) and event.action_text
                 }
             )
 
         return Domain.from_dict({KEY_E2E_ACTIONS: list(additional_e2e_action_names)})
 
-    def get_stories(self, exclusion_percentage: Optional[int] = None) -> StoryGraph:
-        """Retrieves the stories that should be used for training.
-
-        See parent class for details.
-        """
-        return self.importer.get_stories(exclusion_percentage)
-
-    def get_conversation_tests(self) -> StoryGraph:
-        """Retrieves conversation test stories (see parent class for full docstring)."""
-        return self.importer.get_conversation_tests()
-
-    def get_config(self) -> Dict:
-        """Retrieves model config (see parent class for full docstring)."""
-        return self.importer.get_config()
-
-    @rasa.shared.utils.common.cached_method
-    def get_config_file_for_auto_config(self) -> Optional[Text]:
-        """Returns config file path for auto-config only if there is a single one."""
-        return self.importer.get_config_file_for_auto_config()
+        return self._importer.get_config_file_for_auto_config()
 
     @rasa.shared.utils.common.cached_method
     def get_nlu_data(self, language: Optional[Text] = "en") -> TrainingData:
         """Retrieves NLU training data (see parent class for full docstring)."""
         training_datasets = [
             _additional_training_data_from_default_actions(),
-            self.importer.get_nlu_data(language),
+            self._importer.get_nlu_data(language),
             self._additional_training_data_from_stories(),
         ]
 
         return reduce(
             lambda merged, other: merged.merge(other), training_datasets, TrainingData()
         )
```

### Comparing `rasa-3.7.0b2/rasa/shared/importers/multi_project.py` & `rasa-3.8.0a1/rasa/shared/importers/multi_project.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/importers/rasa.py` & `rasa-3.8.0a1/rasa/shared/importers/rasa.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import logging
 import os
 from typing import Dict, List, Optional, Text, Union
+from rasa.shared.core.flows.flow import FlowsList
 
 import rasa.shared.data
 import rasa.shared.utils.common
 import rasa.shared.utils.io
 from rasa.shared.core.training_data.structures import StoryGraph
 from rasa.shared.importers import utils
 from rasa.shared.importers.importer import TrainingDataImporter
 from rasa.shared.nlu.training_data.training_data import TrainingData
 from rasa.shared.core.domain import InvalidDomain, Domain
+import rasa.shared.core.flows.utils
 from rasa.shared.core.training_data.story_reader.yaml_story_reader import (
     YAMLStoryReader,
 )
 
 logger = logging.getLogger(__name__)
 
 
@@ -31,14 +33,17 @@
 
         self._nlu_files = rasa.shared.data.get_data_files(
             training_data_paths, rasa.shared.data.is_nlu_file
         )
         self._story_files = rasa.shared.data.get_data_files(
             training_data_paths, YAMLStoryReader.is_stories_file
         )
+        self._flow_files = rasa.shared.data.get_data_files(
+            training_data_paths, rasa.shared.core.flows.utils.is_flows_file
+        )
         self._conversation_test_files = rasa.shared.data.get_data_files(
             training_data_paths, YAMLStoryReader.is_test_stories_file
         )
 
         self.config_file = config_file
 
     def get_config(self) -> Dict:
@@ -57,14 +62,18 @@
 
     def get_stories(self, exclusion_percentage: Optional[int] = None) -> StoryGraph:
         """Retrieves training stories / rules (see parent class for full docstring)."""
         return utils.story_graph_from_paths(
             self._story_files, self.get_domain(), exclusion_percentage
         )
 
+    def get_flows(self) -> FlowsList:
+        """Retrieves training stories / rules (see parent class for full docstring)."""
+        return utils.flows_from_paths(self._flow_files)
+
     def get_conversation_tests(self) -> StoryGraph:
         """Retrieves conversation test stories (see parent class for full docstring)."""
         return utils.story_graph_from_paths(
             self._conversation_test_files, self.get_domain()
         )
 
     def get_nlu_data(self, language: Optional[Text] = "en") -> TrainingData:
```

### Comparing `rasa-3.7.0b2/rasa/shared/importers/utils.py` & `rasa-3.8.0a1/rasa/shared/importers/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Iterable, Text, Optional, List
 
 from rasa.shared.core.domain import Domain
+from rasa.shared.core.flows.flow import FlowsList
 from rasa.shared.core.training_data.structures import StoryGraph
 from rasa.shared.nlu.training_data.training_data import TrainingData
 
 
 def training_data_from_paths(paths: Iterable[Text], language: Text) -> TrainingData:
     from rasa.shared.nlu.training_data import loading
 
@@ -16,7 +17,17 @@
     files: List[Text], domain: Domain, exclusion_percentage: Optional[int] = None
 ) -> StoryGraph:
     """Returns the `StoryGraph` from paths."""
     from rasa.shared.core.training_data import loading
 
     story_steps = loading.load_data_from_files(files, domain, exclusion_percentage)
     return StoryGraph(story_steps)
+
+
+def flows_from_paths(files: List[Text]) -> FlowsList:
+    """Returns the flows from paths."""
+    from rasa.shared.core.flows.yaml_flows_io import YAMLFlowsReader
+
+    flows = FlowsList(flows=[])
+    for file in files:
+        flows = flows.merge(YAMLFlowsReader.read_from_file(file))
+    return flows
```

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/constants.py` & `rasa-3.8.0a1/rasa/shared/nlu/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 TEXT = "text"
 TEXT_TOKENS = "text_tokens"
 INTENT = "intent"
+COMMANDS = "commands"
 NOT_INTENT = "not_intent"
 RESPONSE = "response"
 RESPONSE_SELECTOR = "response_selector"
 INTENT_RESPONSE_KEY = "intent_response_key"
 ACTION_TEXT = "action_text"
 ACTION_NAME = "action_name"
 INTENT_NAME_KEY = "name"
```

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/entities_parser.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/entities_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/features.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/features.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/dialogflow.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/dialogflow.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/luis.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/luis.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/rasa.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/rasa.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/rasa_yaml.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/rasa_yaml.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/readerwriter.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/readerwriter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/wit.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/formats/wit.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/loading.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/loading.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/lookup_tables_parser.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/lookup_tables_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/message.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/message.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/data_schema.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/schemas/data_schema.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/nlu.yml` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/schemas/nlu.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/responses.yml` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/schemas/responses.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/synonyms_parser.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/synonyms_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/training_data.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/training_data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/nlu/training_data/util.py` & `rasa-3.8.0a1/rasa/shared/nlu/training_data/util.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/utils/cli.py` & `rasa-3.8.0a1/rasa/shared/utils/cli.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/utils/common.py` & `rasa-3.8.0a1/rasa/shared/utils/common.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/utils/io.py` & `rasa-3.8.0a1/rasa/shared/utils/io.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/utils/pykwalify_extensions.py` & `rasa-3.8.0a1/rasa/shared/utils/pykwalify_extensions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/utils/schemas/domain.yml` & `rasa-3.8.0a1/rasa/shared/utils/schemas/domain.yml`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         mapping:
           regex;([A-Za-z]+):
             type: map
             mapping:
               send_domain:
                 type: "bool"
   responses:
-    # see utils/schemas/responses.yml
+    # see shared/nlu/training_data/schemas/responses.yml
     include: responses
 
   slots:
     type: "map"
     allowempty: True
     mapping:
       regex;([A-Za-z]+):
```

### Comparing `rasa-3.7.0b2/rasa/shared/utils/schemas/events.py` & `rasa-3.8.0a1/rasa/shared/utils/schemas/events.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/utils/schemas/model_config.yml` & `rasa-3.8.0a1/rasa/shared/utils/schemas/model_config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/utils/schemas/stories.yml` & `rasa-3.8.0a1/rasa/shared/utils/schemas/stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/shared/utils/validation.py` & `rasa-3.8.0a1/rasa/shared/utils/validation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/telemetry.py` & `rasa-3.8.0a1/rasa/telemetry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/common.py` & `rasa-3.8.0a1/rasa/utils/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,18 @@
     # UserWarning which is always issued if the default value for
     # assistant_id key in config file is not changed
     (UserWarning, "is missing a unique value for the 'assistant_id' mandatory key.*"),
     (
         DeprecationWarning,
         "non-integer arguments to randrange\\(\\) have been deprecated since",
     ),
+    (
+        UserWarning,
+        "The utterance 'utter_flow_continue_interrupted' is not used*",
+    ),
 ]
 
 EXPECTED_WARNINGS.extend(EXPECTED_PILLOW_DEPRECATION_WARNINGS)
 PYTHON_LOGGING_SCHEMA_DOCS = (
     "https://docs.python.org/3/library/logging.config.html#dictionary-schema-details"
 )
```

### Comparing `rasa-3.7.0b2/rasa/utils/converter.py` & `rasa-3.8.0a1/rasa/utils/converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/endpoints.py` & `rasa-3.8.0a1/rasa/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/io.py` & `rasa-3.8.0a1/rasa/utils/io.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/log_utils.py` & `rasa-3.8.0a1/rasa/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/plotting.py` & `rasa-3.8.0a1/rasa/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/callback.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/constants.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/crf.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/crf.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/data_generator.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/data_generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/environment.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/environment.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/layers.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/layers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/layers_utils.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/layers_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/metrics.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/metrics.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/model_data.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/model_data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/model_data_utils.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/model_data_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/models.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/models.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/rasa_layers.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/rasa_layers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/tensorflow/transformer.py` & `rasa-3.8.0a1/rasa/utils/tensorflow/transformer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/utils/train_utils.py` & `rasa-3.8.0a1/rasa/utils/train_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/rasa/validator.py` & `rasa-3.8.0a1/rasa/validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b2/PKG-INFO` & `rasa-3.8.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: rasa
-Version: 3.7.0b2
+Version: 3.8.0a1
 Summary: Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants
 Home-page: https://rasa.com
 License: Apache-2.0
 Keywords: nlp,machine-learning,machine-learning-library,bot,bots,botkit,rasa conversational-agents,conversational-ai,chatbot,chatbot-framework,bot-framework
 Author: Rasa Technologies GmbH
 Author-email: hi@rasa.com
 Maintainer: Tom Bocklisch
 Maintainer-email: tom@rasa.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8.1,<3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: full
 Provides-Extra: gh-release-notes
 Provides-Extra: jieba
 Provides-Extra: metal
@@ -45,38 +44,41 @@
 Requires-Dist: fbmessenger (>=6.0.0,<6.1.0)
 Requires-Dist: github3.py (>=3.2.0,<3.3.0) ; extra == "gh-release-notes"
 Requires-Dist: google-auth (<3)
 Requires-Dist: jieba (>=0.39,<0.43) ; extra == "jieba" or extra == "full"
 Requires-Dist: joblib (>=0.15.1,<1.3.0)
 Requires-Dist: jsonpickle (>=1.3,<3.1)
 Requires-Dist: jsonschema (>=3.2,<4.18)
+Requires-Dist: langchain (>=0.0.223,<0.0.224)
 Requires-Dist: matplotlib (>=3.1,<3.8)
 Requires-Dist: mattermostwrapper (>=2.2,<2.3)
 Requires-Dist: networkx (>=2.4,<2.7)
 Requires-Dist: numpy (==1.22.3) ; sys_platform == "Windows" and platform_python_implementation != "PyPy" and python_version == "3.10"
 Requires-Dist: numpy (>=1.19.2,<1.22.0) ; python_full_version >= "3.7.0" and python_full_version < "3.8.0"
 Requires-Dist: numpy (>=1.19.2,<1.25.0) ; python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: packaging (>=20.0,<21.0)
 Requires-Dist: pluggy (>=1.0.0,<2.0.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: prompt-toolkit (>=3.0,<3.0.29)
 Requires-Dist: protobuf (>=4.23.3,<4.23.4)
 Requires-Dist: psycopg2-binary (>=2.8.2,<2.10.0)
 Requires-Dist: pydantic (<1.10.10)
 Requires-Dist: pydot (>=1.4,<1.5)
 Requires-Dist: pykwalify (>=1.7,<1.9)
 Requires-Dist: pymongo[srv,tls] (>=3.8,<4.4)
+Requires-Dist: pypred (>=0.4.0,<0.5.0)
 Requires-Dist: python-dateutil (>=2.8,<2.9)
 Requires-Dist: python-engineio (>=4,<6,!=5.0.0)
 Requires-Dist: python-socketio (>=4.4,<6)
 Requires-Dist: pytz (>=2019.1,<2023.0)
 Requires-Dist: pyyaml (>=6.0)
 Requires-Dist: questionary (>=1.5.1,<1.11.0)
 Requires-Dist: randomname (>=0.1.5,<0.2.0)
-Requires-Dist: rasa-sdk (>=3.7.0b1,<3.8.0)
+Requires-Dist: rasa-sdk (>=3.8.0a1,<3.9.0)
 Requires-Dist: redis (>=4.5.3,<5.0)
 Requires-Dist: regex (>=2020.6,<2022.11)
 Requires-Dist: requests (>=2.23,<3.0)
 Requires-Dist: rocketchat_API (>=0.6.31,<1.31.0)
 Requires-Dist: ruamel.yaml (>=0.16.5,<0.17.22)
 Requires-Dist: sanic (>=21.12,<21.13)
 Requires-Dist: sanic-cors (>=2.0.0,<2.1.0)
```

