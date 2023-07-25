# Comparing `tmp/vocode_api-0.0.5a4.tar.gz` & `tmp/vocode_api-0.0.5a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocode_api-0.0.5a4.tar", max compression
+gzip compressed data, was "vocode_api-0.0.5a5.tar", max compression
```

## Comparing `vocode_api-0.0.5a4.tar` & `vocode_api-0.0.5a5.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     2777 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/README.md
--rw-r--r--   0        0        0      379 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/pyproject.toml
--rw-r--r--   0        0        0     4774 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/__init__.py
--rw-r--r--   0        0        0     2207 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/client.py
--rw-r--r--   0        0        0      348 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      224 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/environment.py
--rw-r--r--   0        0        0      170 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/py.typed
--rw-r--r--   0        0        0      220 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/actions/__init__.py
--rw-r--r--   0        0        0     9447 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/actions/client.py
--rw-r--r--   0        0        0       65 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/agents/__init__.py
--rw-r--r--   0        0        0     8903 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/agents/client.py
--rw-r--r--   0        0        0       65 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/calls/__init__.py
--rw-r--r--   0        0        0    10997 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/calls/client.py
--rw-r--r--   0        0        0       65 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/numbers/__init__.py
--rw-r--r--   0        0        0    10847 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/numbers/client.py
--rw-r--r--   0        0        0       65 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/usage/__init__.py
--rw-r--r--   0        0        0     2306 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/usage/client.py
--rw-r--r--   0        0        0       65 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/voices/__init__.py
--rw-r--r--   0        0        0     9397 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/voices/client.py
--rw-r--r--   0        0        0       65 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/webhooks/__init__.py
--rw-r--r--   0        0        0     8991 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/resources/webhooks/client.py
--rw-r--r--   0        0        0     6970 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/__init__.py
--rw-r--r--   0        0        0      837 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/action_type.py
--rw-r--r--   0        0        0     1045 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent.py
--rw-r--r--   0        0        0      321 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_actions_item.py
--rw-r--r--   0        0        0     1096 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_params.py
--rw-r--r--   0        0        0      409 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_params_actions_item.py
--rw-r--r--   0        0        0      332 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_params_voice.py
--rw-r--r--   0        0        0      177 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_params_webhook.py
--rw-r--r--   0        0        0     1360 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_update_params.py
--rw-r--r--   0        0        0      368 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_update_params_actions.py
--rw-r--r--   0        0        0      477 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_update_params_actions_agent_update_params_actions_item.py
--rw-r--r--   0        0        0      177 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_update_params_initial_message.py
--rw-r--r--   0        0        0      169 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_update_params_prompt.py
--rw-r--r--   0        0        0      445 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_update_params_voice.py
--rw-r--r--   0        0        0      246 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_update_params_webhook.py
--rw-r--r--   0        0        0      269 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_voice.py
--rw-r--r--   0        0        0      152 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/agent_webhook.py
--rw-r--r--   0        0        0      913 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/azure_voice.py
--rw-r--r--   0        0        0      873 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/azure_voice_params.py
--rw-r--r--   0        0        0     1197 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/azure_voice_update_params.py
--rw-r--r--   0        0        0      173 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/azure_voice_update_params_pitch.py
--rw-r--r--   0        0        0      172 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/azure_voice_update_params_rate.py
--rw-r--r--   0        0        0      177 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/azure_voice_update_params_voice_name.py
--rw-r--r--   0        0        0     1102 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/call.py
--rw-r--r--   0        0        0      143 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/call_agent.py
--rw-r--r--   0        0        0      832 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/call_status.py
--rw-r--r--   0        0        0      395 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/create_action_request.py
--rw-r--r--   0        0        0      320 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/create_action_response.py
--rw-r--r--   0        0        0      175 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/create_call_request_agent.py
--rw-r--r--   0        0        0      329 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/create_voice_request.py
--rw-r--r--   0        0        0      273 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/create_voice_response.py
--rw-r--r--   0        0        0      931 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/dtmf_action.py
--rw-r--r--   0        0        0      891 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/dtmf_action_params.py
--rw-r--r--   0        0        0      932 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/dtmf_action_update_params.py
--rw-r--r--   0        0        0      239 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/dtmf_action_update_params_config.py
--rw-r--r--   0        0        0      953 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/eleven_labs_voice.py
--rw-r--r--   0        0        0      913 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/eleven_labs_voice_params.py
--rw-r--r--   0        0        0     1455 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/eleven_labs_voice_update_params.py
--rw-r--r--   0        0        0      179 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/eleven_labs_voice_update_params_api_key.py
--rw-r--r--   0        0        0      190 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/eleven_labs_voice_update_params_similarity_boost.py
--rw-r--r--   0        0        0      184 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/eleven_labs_voice_update_params_stability.py
--rw-r--r--   0        0        0      180 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/eleven_labs_voice_update_params_voice_id.py
--rw-r--r--   0        0        0      736 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/empty_action_config.py
--rw-r--r--   0        0        0      942 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/end_conversation_action.py
--rw-r--r--   0        0        0      902 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/end_conversation_action_params.py
--rw-r--r--   0        0        0      977 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/end_conversation_action_update_params.py
--rw-r--r--   0        0        0      250 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/end_conversation_action_update_params_config.py
--rw-r--r--   0        0        0     1395 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/event_type.py
--rw-r--r--   0        0        0      317 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/get_action_response.py
--rw-r--r--   0        0        0      270 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/get_voice_response.py
--rw-r--r--   0        0        0      466 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/http_method.py
--rw-r--r--   0        0        0      843 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/http_validation_error.py
--rw-r--r--   0        0        0      323 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/list_actions_response_item.py
--rw-r--r--   0        0        0      276 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/list_voices_response_item.py
--rw-r--r--   0        0        0      900 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/phone_number.py
--rw-r--r--   0        0        0      157 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/phone_number_inbound_agent.py
--rw-r--r--   0        0        0      674 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/plan_type.py
--rw-r--r--   0        0        0      846 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/rime_voice.py
--rw-r--r--   0        0        0      806 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/rime_voice_params.py
--rw-r--r--   0        0        0      929 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/rime_voice_update_params.py
--rw-r--r--   0        0        0      174 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/rime_voice_update_params_speaker.py
--rw-r--r--   0        0        0      925 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/transfer_call_action.py
--rw-r--r--   0        0        0      965 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/transfer_call_action_update_params.py
--rw-r--r--   0        0        0      250 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/transfer_call_action_update_params_config.py
--rw-r--r--   0        0        0      760 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/transfer_call_config.py
--rw-r--r--   0        0        0      728 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/undefined.py
--rw-r--r--   0        0        0      443 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/update_action_request_body.py
--rw-r--r--   0        0        0      320 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/update_action_response.py
--rw-r--r--   0        0        0      203 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/update_number_request_inbound_agent.py
--rw-r--r--   0        0        0      390 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/update_voice_request_body.py
--rw-r--r--   0        0        0      273 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/update_voice_response.py
--rw-r--r--   0        0        0      866 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/usage.py
--rw-r--r--   0        0        0      869 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      907 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/voice_type.py
--rw-r--r--   0        0        0      921 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/webhook.py
--rw-r--r--   0        0        0      898 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/webhook_params.py
--rw-r--r--   0        0        0     1124 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/webhook_update_params.py
--rw-r--r--   0        0        0      214 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/webhook_update_params_method.py
--rw-r--r--   0        0        0      231 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/webhook_update_params_subscriptions.py
--rw-r--r--   0        0        0      168 2023-07-21 07:12:05.213288 vocode_api-0.0.5a4/src/vocode/types/webhook_update_params_url.py
--rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 vocode_api-0.0.5a4/PKG-INFO
+-rw-r--r--   0        0        0     2777 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/README.md
+-rw-r--r--   0        0        0      379 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/pyproject.toml
+-rw-r--r--   0        0        0     4780 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/__init__.py
+-rw-r--r--   0        0        0     2074 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/client.py
+-rw-r--r--   0        0        0      348 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/py.typed
+-rw-r--r--   0        0        0      220 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/actions/__init__.py
+-rw-r--r--   0        0        0     9264 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/agents/__init__.py
+-rw-r--r--   0        0        0     8814 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/agents/client.py
+-rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/calls/__init__.py
+-rw-r--r--   0        0        0    10806 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/calls/client.py
+-rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/numbers/__init__.py
+-rw-r--r--   0        0        0    10759 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/numbers/client.py
+-rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/usage/__init__.py
+-rw-r--r--   0        0        0     2159 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/usage/client.py
+-rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/voices/__init__.py
+-rw-r--r--   0        0        0     9214 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/voices/client.py
+-rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/webhooks/__init__.py
+-rw-r--r--   0        0        0     8808 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/webhooks/client.py
+-rw-r--r--   0        0        0     7085 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/__init__.py
+-rw-r--r--   0        0        0      837 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/action_type.py
+-rw-r--r--   0        0        0     1029 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent.py
+-rw-r--r--   0        0        0      316 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_actions_item.py
+-rw-r--r--   0        0        0     1096 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_params.py
+-rw-r--r--   0        0        0      384 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_params_actions_item.py
+-rw-r--r--   0        0        0      332 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_params_voice.py
+-rw-r--r--   0        0        0      177 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_params_webhook.py
+-rw-r--r--   0        0        0     1360 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params.py
+-rw-r--r--   0        0        0      368 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params_actions.py
+-rw-r--r--   0        0        0      477 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params_actions_agent_update_params_actions_item.py
+-rw-r--r--   0        0        0      177 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params_initial_message.py
+-rw-r--r--   0        0        0      169 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params_prompt.py
+-rw-r--r--   0        0        0      445 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params_voice.py
+-rw-r--r--   0        0        0      246 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params_webhook.py
+-rw-r--r--   0        0        0      264 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_voice.py
+-rw-r--r--   0        0        0      913 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/azure_voice.py
+-rw-r--r--   0        0        0      873 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/azure_voice_params.py
+-rw-r--r--   0        0        0     1197 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/azure_voice_update_params.py
+-rw-r--r--   0        0        0      173 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/azure_voice_update_params_pitch.py
+-rw-r--r--   0        0        0      172 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/azure_voice_update_params_rate.py
+-rw-r--r--   0        0        0      177 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/azure_voice_update_params_voice_name.py
+-rw-r--r--   0        0        0     1035 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/call.py
+-rw-r--r--   0        0        0      832 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/call_status.py
+-rw-r--r--   0        0        0      376 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/create_action_request.py
+-rw-r--r--   0        0        0      320 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/create_action_response.py
+-rw-r--r--   0        0        0      175 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/create_call_request_agent.py
+-rw-r--r--   0        0        0      329 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/create_voice_request.py
+-rw-r--r--   0        0        0      273 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/create_voice_response.py
+-rw-r--r--   0        0        0      931 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/dtmf_action.py
+-rw-r--r--   0        0        0      891 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/dtmf_action_params.py
+-rw-r--r--   0        0        0      932 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/dtmf_action_update_params.py
+-rw-r--r--   0        0        0      239 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/dtmf_action_update_params_config.py
+-rw-r--r--   0        0        0      953 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice.py
+-rw-r--r--   0        0        0      913 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_params.py
+-rw-r--r--   0        0        0     1455 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_update_params.py
+-rw-r--r--   0        0        0      179 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_update_params_api_key.py
+-rw-r--r--   0        0        0      190 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_update_params_similarity_boost.py
+-rw-r--r--   0        0        0      184 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_update_params_stability.py
+-rw-r--r--   0        0        0      180 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_update_params_voice_id.py
+-rw-r--r--   0        0        0      736 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/empty_action_config.py
+-rw-r--r--   0        0        0      942 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/end_conversation_action.py
+-rw-r--r--   0        0        0      902 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/end_conversation_action_params.py
+-rw-r--r--   0        0        0      977 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/end_conversation_action_update_params.py
+-rw-r--r--   0        0        0      250 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/end_conversation_action_update_params_config.py
+-rw-r--r--   0        0        0     1395 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/event_type.py
+-rw-r--r--   0        0        0      317 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/get_action_response.py
+-rw-r--r--   0        0        0      270 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/get_voice_response.py
+-rw-r--r--   0        0        0      466 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/http_method.py
+-rw-r--r--   0        0        0      843 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/http_validation_error.py
+-rw-r--r--   0        0        0      323 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/list_actions_response_item.py
+-rw-r--r--   0        0        0      276 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/list_voices_response_item.py
+-rw-r--r--   0        0        0      901 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/normalized_agent.py
+-rw-r--r--   0        0        0     1018 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/normalized_call.py
+-rw-r--r--   0        0        0      843 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/normalized_phone_number.py
+-rw-r--r--   0        0        0      860 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/phone_number.py
+-rw-r--r--   0        0        0      674 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/plan_type.py
+-rw-r--r--   0        0        0      846 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/rime_voice.py
+-rw-r--r--   0        0        0      806 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/rime_voice_params.py
+-rw-r--r--   0        0        0      929 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/rime_voice_update_params.py
+-rw-r--r--   0        0        0      174 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/rime_voice_update_params_speaker.py
+-rw-r--r--   0        0        0      925 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/transfer_call_action.py
+-rw-r--r--   0        0        0      885 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/transfer_call_action_params.py
+-rw-r--r--   0        0        0      965 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/transfer_call_action_update_params.py
+-rw-r--r--   0        0        0      250 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/transfer_call_action_update_params_config.py
+-rw-r--r--   0        0        0      760 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/transfer_call_config.py
+-rw-r--r--   0        0        0      728 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/undefined.py
+-rw-r--r--   0        0        0      443 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/update_action_request_body.py
+-rw-r--r--   0        0        0      320 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/update_action_response.py
+-rw-r--r--   0        0        0      203 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/update_number_request_inbound_agent.py
+-rw-r--r--   0        0        0      390 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/update_voice_request_body.py
+-rw-r--r--   0        0        0      273 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/update_voice_response.py
+-rw-r--r--   0        0        0      866 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/usage.py
+-rw-r--r--   0        0        0      869 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      907 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/voice_type.py
+-rw-r--r--   0        0        0      921 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/webhook.py
+-rw-r--r--   0        0        0      898 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/webhook_params.py
+-rw-r--r--   0        0        0     1124 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/webhook_update_params.py
+-rw-r--r--   0        0        0      214 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/webhook_update_params_method.py
+-rw-r--r--   0        0        0      231 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/webhook_update_params_subscriptions.py
+-rw-r--r--   0        0        0      168 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/webhook_update_params_url.py
+-rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 vocode_api-0.0.5a5/PKG-INFO
```

### Comparing `vocode_api-0.0.5a4/README.md` & `vocode_api-0.0.5a5/README.md`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/__init__.py` & `vocode_api-0.0.5a5/src/vocode/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .environment import VocodeEnvironment
 from .errors import UnprocessableEntityError
 from .resources import actions, agents, calls, numbers, usage, voices, webhooks
 from .types import (
     ActionType,
     Agent,
     AgentActionsItem,
     AgentParams,
@@ -15,23 +14,21 @@
     AgentUpdateParamsActions,
     AgentUpdateParamsActionsAgentUpdateParamsActionsItem,
     AgentUpdateParamsInitialMessage,
     AgentUpdateParamsPrompt,
     AgentUpdateParamsVoice,
     AgentUpdateParamsWebhook,
     AgentVoice,
-    AgentWebhook,
     AzureVoice,
     AzureVoiceParams,
     AzureVoiceUpdateParams,
     AzureVoiceUpdateParamsPitch,
     AzureVoiceUpdateParamsRate,
     AzureVoiceUpdateParamsVoiceName,
     Call,
-    CallAgent,
     CallStatus,
     CreateActionRequest,
     CreateActionResponse,
     CreateCallRequestAgent,
     CreateVoiceRequest,
     CreateVoiceResponse,
     DtmfAction,
@@ -53,22 +50,25 @@
     EventType,
     GetActionResponse,
     GetVoiceResponse,
     HttpMethod,
     HttpValidationError,
     ListActionsResponseItem,
     ListVoicesResponseItem,
+    NormalizedAgent,
+    NormalizedCall,
+    NormalizedPhoneNumber,
     PhoneNumber,
-    PhoneNumberInboundAgent,
     PlanType,
     RimeVoice,
     RimeVoiceParams,
     RimeVoiceUpdateParams,
     RimeVoiceUpdateParamsSpeaker,
     TransferCallAction,
+    TransferCallActionParams,
     TransferCallActionUpdateParams,
     TransferCallActionUpdateParamsConfig,
     TransferCallConfig,
     Undefined,
     UpdateActionRequestBody,
     UpdateActionResponse,
     UpdateNumberRequestInboundAgent,
@@ -98,23 +98,21 @@
     "AgentUpdateParamsActions",
     "AgentUpdateParamsActionsAgentUpdateParamsActionsItem",
     "AgentUpdateParamsInitialMessage",
     "AgentUpdateParamsPrompt",
     "AgentUpdateParamsVoice",
     "AgentUpdateParamsWebhook",
     "AgentVoice",
-    "AgentWebhook",
     "AzureVoice",
     "AzureVoiceParams",
     "AzureVoiceUpdateParams",
     "AzureVoiceUpdateParamsPitch",
     "AzureVoiceUpdateParamsRate",
     "AzureVoiceUpdateParamsVoiceName",
     "Call",
-    "CallAgent",
     "CallStatus",
     "CreateActionRequest",
     "CreateActionResponse",
     "CreateCallRequestAgent",
     "CreateVoiceRequest",
     "CreateVoiceResponse",
     "DtmfAction",
@@ -136,36 +134,38 @@
     "EventType",
     "GetActionResponse",
     "GetVoiceResponse",
     "HttpMethod",
     "HttpValidationError",
     "ListActionsResponseItem",
     "ListVoicesResponseItem",
+    "NormalizedAgent",
+    "NormalizedCall",
+    "NormalizedPhoneNumber",
     "PhoneNumber",
-    "PhoneNumberInboundAgent",
     "PlanType",
     "RimeVoice",
     "RimeVoiceParams",
     "RimeVoiceUpdateParams",
     "RimeVoiceUpdateParamsSpeaker",
     "TransferCallAction",
+    "TransferCallActionParams",
     "TransferCallActionUpdateParams",
     "TransferCallActionUpdateParamsConfig",
     "TransferCallConfig",
     "Undefined",
     "UnprocessableEntityError",
     "UpdateActionRequestBody",
     "UpdateActionResponse",
     "UpdateNumberRequestInboundAgent",
     "UpdateVoiceRequestBody",
     "UpdateVoiceResponse",
     "Usage",
     "ValidationError",
     "ValidationErrorLocItem",
-    "VocodeEnvironment",
     "VoiceType",
     "Webhook",
     "WebhookParams",
     "WebhookUpdateParams",
     "WebhookUpdateParamsMethod",
     "WebhookUpdateParamsSubscriptions",
     "WebhookUpdateParamsUrl",
```

### Comparing `vocode_api-0.0.5a4/src/vocode/client.py` & `vocode_api-0.0.5a5/src/vocode/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .environment import VocodeEnvironment
 from .resources.actions.client import ActionsClient, AsyncActionsClient
 from .resources.agents.client import AgentsClient, AsyncAgentsClient
 from .resources.calls.client import AsyncCallsClient, CallsClient
 from .resources.numbers.client import AsyncNumbersClient, NumbersClient
 from .resources.usage.client import AsyncUsageClient, UsageClient
 from .resources.voices.client import AsyncVoicesClient, VoicesClient
 from .resources.webhooks.client import AsyncWebhooksClient, WebhooksClient
 
 
 class Vocode:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
         self.numbers = NumbersClient(environment=self._environment, token=self._token)
         self.calls = CallsClient(environment=self._environment, token=self._token)
         self.usage = UsageClient(environment=self._environment, token=self._token)
         self.actions = ActionsClient(environment=self._environment, token=self._token)
         self.agents = AgentsClient(environment=self._environment, token=self._token)
         self.voices = VoicesClient(environment=self._environment, token=self._token)
         self.webhooks = WebhooksClient(environment=self._environment, token=self._token)
 
 
 class AsyncVocode:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
         self.numbers = AsyncNumbersClient(environment=self._environment, token=self._token)
         self.calls = AsyncCallsClient(environment=self._environment, token=self._token)
         self.usage = AsyncUsageClient(environment=self._environment, token=self._token)
         self.actions = AsyncActionsClient(environment=self._environment, token=self._token)
         self.agents = AsyncAgentsClient(environment=self._environment, token=self._token)
```

### Comparing `vocode_api-0.0.5a4/src/vocode/core/datetime_utils.py` & `vocode_api-0.0.5a5/src/vocode/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/core/jsonable_encoder.py` & `vocode_api-0.0.5a5/src/vocode/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/resources/actions/client.py` & `vocode_api-0.0.5a5/src/vocode/resources/actions/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,34 +6,33 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
-from ...environment import VocodeEnvironment
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.create_action_request import CreateActionRequest
 from ...types.create_action_response import CreateActionResponse
 from ...types.get_action_response import GetActionResponse
 from ...types.http_validation_error import HttpValidationError
 from ...types.list_actions_response_item import ListActionsResponseItem
 from ...types.update_action_request_body import UpdateActionRequestBody
 from ...types.update_action_response import UpdateActionResponse
 
 
 class ActionsClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
     def get_action(self, *, id: str) -> GetActionResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/actions"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -45,15 +44,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_actions(self) -> typing.List[ListActionsResponseItem]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions/list"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/actions/list"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[ListActionsResponseItem], _response.json())  # type: ignore
@@ -62,15 +61,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_action(self, *, request: CreateActionRequest) -> CreateActionResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions/create"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/actions/create"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -82,15 +81,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_action(self, *, id: str, request: UpdateActionRequestBody) -> UpdateActionResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions/update"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/actions/update"),
             params={"id": id},
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
@@ -102,23 +101,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncActionsClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
     async def get_action(self, *, id: str) -> GetActionResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/actions"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -131,15 +130,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_actions(self) -> typing.List[ListActionsResponseItem]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions/list"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/actions/list"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[ListActionsResponseItem], _response.json())  # type: ignore
@@ -149,15 +148,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_action(self, *, request: CreateActionRequest) -> CreateActionResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions/create"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/actions/create"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -170,15 +169,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_action(self, *, id: str, request: UpdateActionRequestBody) -> UpdateActionResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions/update"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/actions/update"),
                 params={"id": id},
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
```

### Comparing `vocode_api-0.0.5a4/src/vocode/resources/agents/client.py` & `vocode_api-0.0.5a5/src/vocode/resources/agents/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
-from ...environment import VocodeEnvironment
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.agent import Agent
 from ...types.agent_params import AgentParams
 from ...types.agent_update_params import AgentUpdateParams
 from ...types.http_validation_error import HttpValidationError
+from ...types.normalized_agent import NormalizedAgent
 
 
 class AgentsClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
     def get_agent(self, *, id: str) -> Agent:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/agents"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -39,35 +39,35 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list_agents(self) -> typing.List[Agent]:
+    def list_agents(self) -> typing.List[NormalizedAgent]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents/list"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/agents/list"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Agent], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[NormalizedAgent], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_agent(self, *, request: AgentParams) -> Agent:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents/create"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/agents/create"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -79,15 +79,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_agent(self, *, id: str, request: AgentUpdateParams) -> Agent:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents/update"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/agents/update"),
             params={"id": id},
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
@@ -99,23 +99,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAgentsClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
     async def get_agent(self, *, id: str) -> Agent:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/agents"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -124,37 +124,37 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list_agents(self) -> typing.List[Agent]:
+    async def list_agents(self) -> typing.List[NormalizedAgent]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents/list"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/agents/list"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Agent], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[NormalizedAgent], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_agent(self, *, request: AgentParams) -> Agent:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents/create"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/agents/create"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -167,15 +167,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_agent(self, *, id: str, request: AgentUpdateParams) -> Agent:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents/update"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/agents/update"),
                 params={"id": id},
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
```

### Comparing `vocode_api-0.0.5a4/src/vocode/resources/calls/client.py` & `vocode_api-0.0.5a5/src/vocode/resources/calls/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,47 +6,47 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
-from ...environment import VocodeEnvironment
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.call import Call
 from ...types.create_call_request_agent import CreateCallRequestAgent
 from ...types.http_validation_error import HttpValidationError
+from ...types.normalized_call import NormalizedCall
 
 
 class CallsClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
-    def list_calls(self) -> typing.List[Call]:
+    def list_calls(self) -> typing.List[NormalizedCall]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/list"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/calls/list"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Call], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[NormalizedCall], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_call(self, *, id: str) -> Call:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/calls"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -58,15 +58,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def end_call(self, *, id: str) -> Call:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/end"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/calls/end"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -75,19 +75,19 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_call(self, *, from_number: str, to_number: str, goal: str, agent: CreateCallRequestAgent) -> Call:
+    def create_call(self, *, from_number: str, to_number: str, agent: CreateCallRequestAgent) -> Call:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/create"),
-            json=jsonable_encoder({"from_number": from_number, "to_number": to_number, "goal": goal, "agent": agent}),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/calls/create"),
+            json=jsonable_encoder({"from_number": from_number, "to_number": to_number, "agent": agent}),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Call, _response.json())  # type: ignore
@@ -98,15 +98,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def recording(self, *, id: str) -> typing.Any:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/recording"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/calls/recording"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -117,41 +117,41 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncCallsClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
-    async def list_calls(self) -> typing.List[Call]:
+    async def list_calls(self) -> typing.List[NormalizedCall]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/list"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/calls/list"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Call], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[NormalizedCall], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_call(self, *, id: str) -> Call:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/calls"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -164,15 +164,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def end_call(self, *, id: str) -> Call:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/end"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/calls/end"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -181,22 +181,20 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_call(self, *, from_number: str, to_number: str, goal: str, agent: CreateCallRequestAgent) -> Call:
+    async def create_call(self, *, from_number: str, to_number: str, agent: CreateCallRequestAgent) -> Call:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/create"),
-                json=jsonable_encoder(
-                    {"from_number": from_number, "to_number": to_number, "goal": goal, "agent": agent}
-                ),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/calls/create"),
+                json=jsonable_encoder({"from_number": from_number, "to_number": to_number, "agent": agent}),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Call, _response.json())  # type: ignore
@@ -208,15 +206,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def recording(self, *, id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/recording"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/calls/recording"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
```

### Comparing `vocode_api-0.0.5a4/src/vocode/resources/numbers/client.py` & `vocode_api-0.0.5a5/src/vocode/resources/numbers/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,47 +6,47 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
-from ...environment import VocodeEnvironment
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
+from ...types.normalized_phone_number import NormalizedPhoneNumber
 from ...types.phone_number import PhoneNumber
 from ...types.update_number_request_inbound_agent import UpdateNumberRequestInboundAgent
 
 
 class NumbersClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
-    def list_numbers(self) -> typing.List[PhoneNumber]:
+    def list_numbers(self) -> typing.List[NormalizedPhoneNumber]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/list"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/list"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[PhoneNumber], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[NormalizedPhoneNumber], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_number(self, *, phone_number: str) -> PhoneNumber:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/numbers"),
             params={"phone_number": phone_number},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -58,15 +58,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def buy_number(self) -> PhoneNumber:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/buy"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/buy"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PhoneNumber, _response.json())  # type: ignore
@@ -75,15 +75,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_number(self, *, phone_number: str, inbound_agent: UpdateNumberRequestInboundAgent) -> PhoneNumber:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/update"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/update"),
             params={"phone_number": phone_number},
             json=jsonable_encoder({"inbound_agent": inbound_agent}),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
@@ -96,15 +96,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def cancel_number(self, *, phone_number: str) -> PhoneNumber:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/cancel"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/cancel"),
             params={"phone_number": phone_number},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -115,41 +115,41 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncNumbersClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
-    async def list_numbers(self) -> typing.List[PhoneNumber]:
+    async def list_numbers(self) -> typing.List[NormalizedPhoneNumber]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/list"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/list"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[PhoneNumber], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[NormalizedPhoneNumber], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_number(self, *, phone_number: str) -> PhoneNumber:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/numbers"),
                 params={"phone_number": phone_number},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -162,15 +162,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def buy_number(self) -> PhoneNumber:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/buy"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/buy"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PhoneNumber, _response.json())  # type: ignore
@@ -180,15 +180,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_number(self, *, phone_number: str, inbound_agent: UpdateNumberRequestInboundAgent) -> PhoneNumber:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/update"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/update"),
                 params={"phone_number": phone_number},
                 json=jsonable_encoder({"inbound_agent": inbound_agent}),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
@@ -202,15 +202,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def cancel_number(self, *, phone_number: str) -> PhoneNumber:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/cancel"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/cancel"),
                 params={"phone_number": phone_number},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
```

### Comparing `vocode_api-0.0.5a4/src/vocode/resources/usage/client.py` & `vocode_api-0.0.5a5/src/vocode/resources/usage/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
-from ...environment import VocodeEnvironment
 from ...types.usage import Usage
 
 
 class UsageClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
     def get_usage(self) -> Usage:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/usage"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/usage"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Usage, _response.json())  # type: ignore
@@ -32,23 +31,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncUsageClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
     async def get_usage(self) -> Usage:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/usage"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/usage"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Usage, _response.json())  # type: ignore
```

### Comparing `vocode_api-0.0.5a4/src/vocode/resources/voices/client.py` & `vocode_api-0.0.5a5/src/vocode/resources/voices/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,34 +6,33 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
-from ...environment import VocodeEnvironment
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.create_voice_request import CreateVoiceRequest
 from ...types.create_voice_response import CreateVoiceResponse
 from ...types.get_voice_response import GetVoiceResponse
 from ...types.http_validation_error import HttpValidationError
 from ...types.list_voices_response_item import ListVoicesResponseItem
 from ...types.update_voice_request_body import UpdateVoiceRequestBody
 from ...types.update_voice_response import UpdateVoiceResponse
 
 
 class VoicesClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
     def get_voice(self, *, id: str) -> GetVoiceResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/voices"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -45,15 +44,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_voices(self) -> typing.List[ListVoicesResponseItem]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices/list"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/voices/list"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[ListVoicesResponseItem], _response.json())  # type: ignore
@@ -62,15 +61,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_voice(self, *, request: CreateVoiceRequest) -> CreateVoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices/create"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/voices/create"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -82,15 +81,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_voice(self, *, id: str, request: UpdateVoiceRequestBody) -> UpdateVoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices/update"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/voices/update"),
             params={"id": id},
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
@@ -102,23 +101,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncVoicesClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
     async def get_voice(self, *, id: str) -> GetVoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/voices"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -131,15 +130,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_voices(self) -> typing.List[ListVoicesResponseItem]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices/list"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/voices/list"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[ListVoicesResponseItem], _response.json())  # type: ignore
@@ -149,15 +148,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_voice(self, *, request: CreateVoiceRequest) -> CreateVoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices/create"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/voices/create"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -170,15 +169,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_voice(self, *, id: str, request: UpdateVoiceRequestBody) -> UpdateVoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices/update"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/voices/update"),
                 params={"id": id},
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
```

### Comparing `vocode_api-0.0.5a4/src/vocode/resources/webhooks/client.py` & `vocode_api-0.0.5a5/src/vocode/resources/webhooks/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,31 +6,30 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
-from ...environment import VocodeEnvironment
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 from ...types.webhook import Webhook
 from ...types.webhook_params import WebhookParams
 from ...types.webhook_update_params import WebhookUpdateParams
 
 
 class WebhooksClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
     def get_webhook(self, *, id: str) -> Webhook:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -42,15 +41,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_webhooks(self) -> typing.List[Webhook]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks/list"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/list"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Webhook], _response.json())  # type: ignore
@@ -59,15 +58,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_webhook(self, *, request: WebhookParams) -> Webhook:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks/create"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/create"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -79,15 +78,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_webhook(self, *, id: str, request: WebhookUpdateParams) -> Webhook:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks/update"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/update"),
             params={"id": id},
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
@@ -99,23 +98,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncWebhooksClient:
-    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
+    def __init__(self, *, environment: str, token: str):
         self._environment = environment
         self._token = token
 
     async def get_webhook(self, *, id: str) -> Webhook:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -128,15 +127,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_webhooks(self) -> typing.List[Webhook]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks/list"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/list"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Webhook], _response.json())  # type: ignore
@@ -146,15 +145,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_webhook(self, *, request: WebhookParams) -> Webhook:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks/create"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/create"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -167,15 +166,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_webhook(self, *, id: str, request: WebhookUpdateParams) -> Webhook:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks/update"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/update"),
                 params={"id": id},
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
```

### Comparing `vocode_api-0.0.5a4/src/vocode/types/__init__.py` & `vocode_api-0.0.5a5/src/vocode/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,21 @@
     AgentUpdateParamsActionsAgentUpdateParamsActionsItem,
 )
 from .agent_update_params_initial_message import AgentUpdateParamsInitialMessage
 from .agent_update_params_prompt import AgentUpdateParamsPrompt
 from .agent_update_params_voice import AgentUpdateParamsVoice
 from .agent_update_params_webhook import AgentUpdateParamsWebhook
 from .agent_voice import AgentVoice
-from .agent_webhook import AgentWebhook
 from .azure_voice import AzureVoice
 from .azure_voice_params import AzureVoiceParams
 from .azure_voice_update_params import AzureVoiceUpdateParams
 from .azure_voice_update_params_pitch import AzureVoiceUpdateParamsPitch
 from .azure_voice_update_params_rate import AzureVoiceUpdateParamsRate
 from .azure_voice_update_params_voice_name import AzureVoiceUpdateParamsVoiceName
 from .call import Call
-from .call_agent import CallAgent
 from .call_status import CallStatus
 from .create_action_request import CreateActionRequest
 from .create_action_response import CreateActionResponse
 from .create_call_request_agent import CreateCallRequestAgent
 from .create_voice_request import CreateVoiceRequest
 from .create_voice_response import CreateVoiceResponse
 from .dtmf_action import DtmfAction
@@ -51,22 +49,25 @@
 from .event_type import EventType
 from .get_action_response import GetActionResponse
 from .get_voice_response import GetVoiceResponse
 from .http_method import HttpMethod
 from .http_validation_error import HttpValidationError
 from .list_actions_response_item import ListActionsResponseItem
 from .list_voices_response_item import ListVoicesResponseItem
+from .normalized_agent import NormalizedAgent
+from .normalized_call import NormalizedCall
+from .normalized_phone_number import NormalizedPhoneNumber
 from .phone_number import PhoneNumber
-from .phone_number_inbound_agent import PhoneNumberInboundAgent
 from .plan_type import PlanType
 from .rime_voice import RimeVoice
 from .rime_voice_params import RimeVoiceParams
 from .rime_voice_update_params import RimeVoiceUpdateParams
 from .rime_voice_update_params_speaker import RimeVoiceUpdateParamsSpeaker
 from .transfer_call_action import TransferCallAction
+from .transfer_call_action_params import TransferCallActionParams
 from .transfer_call_action_update_params import TransferCallActionUpdateParams
 from .transfer_call_action_update_params_config import TransferCallActionUpdateParamsConfig
 from .transfer_call_config import TransferCallConfig
 from .undefined import Undefined
 from .update_action_request_body import UpdateActionRequestBody
 from .update_action_response import UpdateActionResponse
 from .update_number_request_inbound_agent import UpdateNumberRequestInboundAgent
@@ -95,23 +96,21 @@
     "AgentUpdateParamsActions",
     "AgentUpdateParamsActionsAgentUpdateParamsActionsItem",
     "AgentUpdateParamsInitialMessage",
     "AgentUpdateParamsPrompt",
     "AgentUpdateParamsVoice",
     "AgentUpdateParamsWebhook",
     "AgentVoice",
-    "AgentWebhook",
     "AzureVoice",
     "AzureVoiceParams",
     "AzureVoiceUpdateParams",
     "AzureVoiceUpdateParamsPitch",
     "AzureVoiceUpdateParamsRate",
     "AzureVoiceUpdateParamsVoiceName",
     "Call",
-    "CallAgent",
     "CallStatus",
     "CreateActionRequest",
     "CreateActionResponse",
     "CreateCallRequestAgent",
     "CreateVoiceRequest",
     "CreateVoiceResponse",
     "DtmfAction",
@@ -133,22 +132,25 @@
     "EventType",
     "GetActionResponse",
     "GetVoiceResponse",
     "HttpMethod",
     "HttpValidationError",
     "ListActionsResponseItem",
     "ListVoicesResponseItem",
+    "NormalizedAgent",
+    "NormalizedCall",
+    "NormalizedPhoneNumber",
     "PhoneNumber",
-    "PhoneNumberInboundAgent",
     "PlanType",
     "RimeVoice",
     "RimeVoiceParams",
     "RimeVoiceUpdateParams",
     "RimeVoiceUpdateParamsSpeaker",
     "TransferCallAction",
+    "TransferCallActionParams",
     "TransferCallActionUpdateParams",
     "TransferCallActionUpdateParamsConfig",
     "TransferCallConfig",
     "Undefined",
     "UpdateActionRequestBody",
     "UpdateActionResponse",
     "UpdateNumberRequestInboundAgent",
```

### Comparing `vocode_api-0.0.5a4/src/vocode/types/action_type.py` & `vocode_api-0.0.5a5/src/vocode/types/action_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/agent.py` & `vocode_api-0.0.5a5/src/vocode/types/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .agent_actions_item import AgentActionsItem
 from .agent_voice import AgentVoice
-from .agent_webhook import AgentWebhook
+from .webhook import Webhook
 
 
 class Agent(pydantic.BaseModel):
     id: str
     user_id: str
     prompt: str
     actions: typing.List[AgentActionsItem]
     voice: AgentVoice
     initial_message: typing.Optional[str]
-    webhook: typing.Optional[AgentWebhook]
+    webhook: typing.Optional[Webhook]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a4/src/vocode/types/agent_params.py` & `vocode_api-0.0.5a5/src/vocode/types/agent_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/agent_update_params.py` & `vocode_api-0.0.5a5/src/vocode/types/agent_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/azure_voice.py` & `vocode_api-0.0.5a5/src/vocode/types/azure_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/azure_voice_params.py` & `vocode_api-0.0.5a5/src/vocode/types/azure_voice_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/azure_voice_update_params.py` & `vocode_api-0.0.5a5/src/vocode/types/azure_voice_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/call.py` & `vocode_api-0.0.5a5/src/vocode/types/call.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .call_agent import CallAgent
+from .agent import Agent
 from .call_status import CallStatus
 
 
 class Call(pydantic.BaseModel):
     id: str
     user_id: str
-    to_number: str
-    from_number: str
-    agent: CallAgent
-    goal: typing.Optional[str]
-    transcript: typing.Optional[str]
-    recording_url: typing.Optional[str]
-    status: CallStatus
+    status: typing.Optional[CallStatus]
     error_message: typing.Optional[str]
     recording_available: typing.Optional[bool]
+    transcript: typing.Optional[str]
+    to_number: str
+    from_number: str
+    agent: Agent
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a4/src/vocode/types/call_status.py` & `vocode_api-0.0.5a5/src/vocode/types/call_status.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/dtmf_action.py` & `vocode_api-0.0.5a5/src/vocode/types/dtmf_action.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/dtmf_action_params.py` & `vocode_api-0.0.5a5/src/vocode/types/dtmf_action_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/dtmf_action_update_params.py` & `vocode_api-0.0.5a5/src/vocode/types/dtmf_action_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/eleven_labs_voice.py` & `vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/eleven_labs_voice_params.py` & `vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/eleven_labs_voice_update_params.py` & `vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/empty_action_config.py` & `vocode_api-0.0.5a5/src/vocode/types/empty_action_config.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/end_conversation_action.py` & `vocode_api-0.0.5a5/src/vocode/types/end_conversation_action.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/end_conversation_action_params.py` & `vocode_api-0.0.5a5/src/vocode/types/end_conversation_action_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/end_conversation_action_update_params.py` & `vocode_api-0.0.5a5/src/vocode/types/end_conversation_action_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/event_type.py` & `vocode_api-0.0.5a5/src/vocode/types/event_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/http_validation_error.py` & `vocode_api-0.0.5a5/src/vocode/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/phone_number.py` & `vocode_api-0.0.5a5/src/vocode/types/rime_voice_update_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .phone_number_inbound_agent import PhoneNumberInboundAgent
+from .rime_voice_update_params_speaker import RimeVoiceUpdateParamsSpeaker
+from .voice_type import VoiceType
 
 
-class PhoneNumber(pydantic.BaseModel):
-    id: str
-    user_id: str
-    number: str
-    active: bool
-    inbound_agent: PhoneNumberInboundAgent
+class RimeVoiceUpdateParams(pydantic.BaseModel):
+    type: VoiceType
+    speaker: typing.Optional[RimeVoiceUpdateParamsSpeaker]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a4/src/vocode/types/plan_type.py` & `vocode_api-0.0.5a5/src/vocode/types/plan_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/rime_voice.py` & `vocode_api-0.0.5a5/src/vocode/types/rime_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/rime_voice_params.py` & `vocode_api-0.0.5a5/src/vocode/types/rime_voice_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/rime_voice_update_params.py` & `vocode_api-0.0.5a5/src/vocode/types/transfer_call_action_update_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .rime_voice_update_params_speaker import RimeVoiceUpdateParamsSpeaker
-from .voice_type import VoiceType
+from .action_type import ActionType
+from .transfer_call_action_update_params_config import TransferCallActionUpdateParamsConfig
 
 
-class RimeVoiceUpdateParams(pydantic.BaseModel):
-    type: VoiceType
-    speaker: typing.Optional[RimeVoiceUpdateParamsSpeaker]
+class TransferCallActionUpdateParams(pydantic.BaseModel):
+    type: ActionType
+    config: typing.Optional[TransferCallActionUpdateParamsConfig]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a4/src/vocode/types/transfer_call_action.py` & `vocode_api-0.0.5a5/src/vocode/types/transfer_call_action.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/transfer_call_action_update_params.py` & `vocode_api-0.0.5a5/src/vocode/types/transfer_call_action_params.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .action_type import ActionType
-from .transfer_call_action_update_params_config import TransferCallActionUpdateParamsConfig
+from .transfer_call_config import TransferCallConfig
 
 
-class TransferCallActionUpdateParams(pydantic.BaseModel):
+class TransferCallActionParams(pydantic.BaseModel):
     type: ActionType
-    config: typing.Optional[TransferCallActionUpdateParamsConfig]
+    config: TransferCallConfig
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a4/src/vocode/types/transfer_call_config.py` & `vocode_api-0.0.5a5/src/vocode/types/transfer_call_config.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/undefined.py` & `vocode_api-0.0.5a5/src/vocode/types/undefined.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/usage.py` & `vocode_api-0.0.5a5/src/vocode/types/usage.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/validation_error.py` & `vocode_api-0.0.5a5/src/vocode/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/voice_type.py` & `vocode_api-0.0.5a5/src/vocode/types/voice_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/webhook.py` & `vocode_api-0.0.5a5/src/vocode/types/webhook.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/webhook_params.py` & `vocode_api-0.0.5a5/src/vocode/types/webhook_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/src/vocode/types/webhook_update_params.py` & `vocode_api-0.0.5a5/src/vocode/types/webhook_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a4/PKG-INFO` & `vocode_api-0.0.5a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocode-api
-Version: 0.0.5a4
+Version: 0.0.5a5
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

