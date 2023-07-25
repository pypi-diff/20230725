# Comparing `tmp/boxsdk-3.7.3.tar.gz` & `tmp/boxsdk-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jenkins/workspace/Box_SDKs/Python_Release/box-python-sdk-2/pypi-dist/boxsdk-3.7.3.tar", last modified: Fri Jul  7 15:20:33 2023, max compression
+gzip compressed data, was "/home/jenkins/workspace/Box_SDKs/Python_Release/box-python-sdk-3/pypi-dist/boxsdk-3.8.0.tar", last modified: Tue Jul 25 11:00:18 2023, max compression
```

## Comparing `boxsdk-3.7.3.tar` & `boxsdk-3.8.0.tar`

### file list

```diff
@@ -1,295 +1,296 @@
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk/auth/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      759 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/auth/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      637 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/auth/ccg_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1039 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/auth/cooperatively_managed_oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1097 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/auth/developer_token_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12195 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/auth/jwt_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    18876 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/auth/oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      534 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/auth/redis_managed_jwt_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2021 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/auth/redis_managed_oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1135 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/auth/remote_managed_oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8589 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/auth/server_auth.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk/client/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      176 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/client/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    64867 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/client/client.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      468 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/client/developer_token_client.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      297 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/client/development_client.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      315 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/client/logging_client.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk/network/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/network/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10506 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/network/default_network.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3515 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/network/network_interface.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk/object/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      904 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      578 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/api_json_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5956 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/base_api_json_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1480 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/base_endpoint.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6607 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/base_item.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5753 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/base_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1563 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/cloneable.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2334 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/collaboration.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4365 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/collaboration_allowlist.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      543 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/collaboration_allowlist_entry.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      228 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/collaboration_allowlist_exempt_target.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1346 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1357 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/comment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      143 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/device_pinner.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      140 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/email_alias.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1096 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/enterprise.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      140 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/event.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12471 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/events.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    36292 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/file.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2731 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/file_request.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      142 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/file_version.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      171 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/file_version_retention.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    30729 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/folder.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      137 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/folder_lock.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3994 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/group.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      207 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/group_membership.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      123 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/invite.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    17229 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/item.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      316 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/legal_hold.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4327 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/legal_hold_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      186 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/legal_hold_policy_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6999 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/metadata.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1539 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/metadata_cascade_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8933 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/metadata_template.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      189 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/recent_item.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3556 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/retention_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1795 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/retention_policy_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    16861 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/search.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1574 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/sign_request.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2330 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/storage_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      178 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/storage_policy_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2694 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/task.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      377 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/task_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3961 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/terms_of_service.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      777 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/terms_of_service_user_status.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5375 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/trash.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6451 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/upload_session.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8104 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/user.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      175 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/watermark.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4489 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/web_link.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2483 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/object/webhook.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk/pagination/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/pagination/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7071 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/pagination/box_object_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      186 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/pagination/dict_page.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      331 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/pagination/limit_offset_based_dict_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3961 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/pagination/limit_offset_based_object_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      304 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/pagination/marker_based_dict_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4355 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/pagination/marker_based_object_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1864 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/pagination/page.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk/session/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/session/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1050 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/session/box_request.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1357 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/session/box_response.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    22602 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/session/session.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk/util/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3012 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/api_call_decorator.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7541 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/chunked_uploader.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      795 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/datetime_formatter.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       29 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/default_arg_value.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1172 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/deprecation_decorator.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4299 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/enum.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      494 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/json.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3744 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/log.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1314 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/lru_cache.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      585 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/multipart_stream.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      561 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/shared_link.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      214 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/text_enum.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7743 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/util/translator.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      319 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      899 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/config.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3581 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/exception.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/boxsdk/py.typed
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       22 2023-07-07 15:19:41.000000 boxsdk-3.7.3/boxsdk/version.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk.egg-info/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    17404 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk.egg-info/PKG-INFO
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9558 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk.egg-info/SOURCES.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        1 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk.egg-info/dependency_links.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      335 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk.egg-info/requires.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        7 2023-07-07 15:20:33.000000 boxsdk-3.7.3/boxsdk.egg-info/top_level.txt
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/functional/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/functional/mock_box/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/functional/mock_box/behavior/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/behavior/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3889 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/behavior/event_behavior.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5755 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/behavior/file_behavior.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5822 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/behavior/folder_behavior.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      617 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/behavior/item_behavior.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6554 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/behavior/oauth2_behavior.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      945 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/behavior/user_behavior.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/functional/mock_box/db_model/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       87 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/db_model/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      945 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/db_model/application_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      767 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/db_model/collaboration_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1260 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/db_model/event_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1666 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/db_model/file_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1862 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/db_model/folder_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      844 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/db_model/group_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      747 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/db_model/lock_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      804 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/db_model/share_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      738 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/db_model/token_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1214 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/db_model/user_model.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/functional/mock_box/util/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/util/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2696 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/util/chaos_utils.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1085 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/util/db_utils.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3609 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/util/http_utils.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2112 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/util/json_utils.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/functional/mock_box/views/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/views/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      202 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/views/html_response.tpl
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      256 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/views/oauth2.tpl
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       69 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/views/xml_response.tpl
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11636 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/mock_box/box.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3896 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1241 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/test_delete.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7449 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/test_events.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4287 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/test_file_upload_update_download.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3687 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/test_item_info.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1933 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/test_object_clone.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      383 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/test_rate_limits.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3522 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/test_recovery.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      767 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/functional/test_token_refresh.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/integration/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1403 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1019 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration/mock_network.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3909 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration/test_as_user.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1117 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration/test_retry_and_refresh.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4602 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration/test_with_shared_link.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/integration_new/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/integration_new/context_managers/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      652 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/context_managers/box_metadata_template.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1274 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/context_managers/box_retention_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      828 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/context_managers/box_retention_policy_assigment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      504 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/context_managers/box_sign_request.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      785 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/context_managers/box_test_file.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      665 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/context_managers/box_test_folder.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      498 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/context_managers/box_test_group.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      545 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/context_managers/box_test_user.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      740 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/context_managers/box_test_web_link.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      521 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/context_managers/local_large_file.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/integration_new/object/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11058 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/object/file_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8169 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/object/folder_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1445 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/object/legal_hold_policy_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1584 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/object/metadata_template_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2288 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/object/retention_policy_assignement_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1573 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/object/retention_policy_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2346 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/object/sign_request_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2537 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/object/trash_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      192 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/object/user_itest.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/integration_new/resources/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1359 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/resources/image.png
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5558 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/resources/small.pdf
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6235 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/resources/small_v2.pdf
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1703 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/README.md
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2092 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1429 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       37 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/integration_tests.cfg
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      921 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/integration_new/util.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/unit/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/unit/auth/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/auth/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12588 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/auth/test_ccg_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      564 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/auth/test_cooperatively_managed_oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1072 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/auth/test_developer_token_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    26294 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/auth/test_jwt_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    17298 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/auth/test_oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2377 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/auth/test_redis_managed_oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      575 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/auth/test_remote_managed_oauth2.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/unit/client/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/client/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    61032 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/client/test_client.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/unit/network/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/network/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1602 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/network/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11382 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/network/test_network.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/unit/object/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12022 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      477 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_api_json_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2307 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_base_api_json_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6378 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_base_item.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5111 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_base_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    13966 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_chunked_upload.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3250 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_collaboration.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3564 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_collaboration_allowlist.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1143 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_collaboration_allowlist_entry.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1238 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_collaboration_allowlist_exempt_target.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1360 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2262 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_comment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1577 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_device_pin.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1248 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_enterprise.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      430 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_event.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11176 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_events.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    36673 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_file.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3650 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_file_request.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      650 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_file_version_retention.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    27532 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_folder.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9451 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_group.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    19897 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_item.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      895 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_legal_hold.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2091 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_legal_hold_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5705 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_legal_hold_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4628 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_metadata.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2489 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_metadata_cascade_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5421 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_metadata_template.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4579 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_retention_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3503 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_retention_policy_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    14811 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_search.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5195 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_sign_request.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7028 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_storage_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2332 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_storage_policy_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5585 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_task.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3128 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_task_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7926 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_terms_of_service.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2885 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_terms_of_service_user_status.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6814 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_trash.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8088 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_upload_session.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9668 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_user.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4958 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_web_link.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4142 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/object/test_webhook.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/unit/pagination/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/pagination/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4324 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/pagination/box_object_collection_test_base.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5427 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/pagination/test_limit_offset_based_object_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4575 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/pagination/test_marker_based_object_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2966 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/pagination/test_page.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/unit/session/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/session/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    17669 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/session/test_session.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/unit/util/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/util/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3478 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/util/test_api_call_decorator.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2309 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/util/test_datetime_formatter.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4928 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/util/test_enum.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3856 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/util/test_log.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1102 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/util/test_lru_cache.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1098 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/util/test_multipart_stream.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      639 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/util/test_shared_link.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      324 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/util/test_text_enum.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7419 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/util/test_translator.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5085 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1963 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/unit/test_exception.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:20:33.000000 boxsdk-3.7.3/test/util/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/util/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      644 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/util/streamable_mock_open.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8430 2023-07-07 15:08:14.000000 boxsdk-3.7.3/test/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9574 2023-07-07 15:08:14.000000 boxsdk-3.7.3/LICENSE
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       52 2023-07-07 15:08:14.000000 boxsdk-3.7.3/MANIFEST.in
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    15965 2023-07-07 15:08:14.000000 boxsdk-3.7.3/README.md
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      136 2023-07-07 15:20:33.000000 boxsdk-3.7.3/setup.cfg
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3781 2023-07-07 15:08:14.000000 boxsdk-3.7.3/setup.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    17404 2023-07-07 15:20:33.000000 boxsdk-3.7.3/PKG-INFO
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk/auth/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      759 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/auth/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      637 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/auth/ccg_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1039 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/auth/cooperatively_managed_oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1097 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/auth/developer_token_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12195 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/auth/jwt_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18876 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/auth/oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      534 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/auth/redis_managed_jwt_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2021 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/auth/redis_managed_oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1135 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/auth/remote_managed_oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8589 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/auth/server_auth.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk/client/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      176 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/client/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    64867 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/client/client.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      468 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/client/developer_token_client.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      297 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/client/development_client.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      315 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/client/logging_client.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk/network/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/network/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10506 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/network/default_network.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3515 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/network/network_interface.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk/object/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      904 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      578 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/api_json_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5956 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/base_api_json_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1480 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/base_endpoint.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6607 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/base_item.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5749 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/base_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1563 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/cloneable.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2487 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/collaboration.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4365 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/collaboration_allowlist.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      543 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/collaboration_allowlist_entry.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      228 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/collaboration_allowlist_exempt_target.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1346 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1357 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/comment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      143 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/device_pinner.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      140 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/email_alias.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1096 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/enterprise.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      140 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/event.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12471 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/events.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    36292 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/file.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2731 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/file_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      142 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/file_version.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      171 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/file_version_retention.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    30729 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/folder.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      137 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/folder_lock.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3994 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/group.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      207 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/group_membership.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      123 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/invite.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    17229 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/item.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      316 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/legal_hold.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4327 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/legal_hold_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      186 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/legal_hold_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6999 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/metadata.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1539 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/metadata_cascade_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8933 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/metadata_template.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      189 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/recent_item.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3556 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/retention_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1795 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/retention_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    16861 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/search.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1574 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/sign_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2330 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/storage_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      178 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/storage_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2694 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/task.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      377 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/task_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3961 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/terms_of_service.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      777 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/terms_of_service_user_status.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5375 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/trash.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6451 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/upload_session.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8104 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/user.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      175 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/watermark.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4489 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/web_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2483 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/object/webhook.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk/pagination/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/pagination/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7071 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/pagination/box_object_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      186 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/pagination/dict_page.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      331 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/pagination/limit_offset_based_dict_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3961 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/pagination/limit_offset_based_object_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      304 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/pagination/marker_based_dict_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4355 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/pagination/marker_based_object_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1864 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/pagination/page.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk/session/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/session/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1050 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/session/box_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1357 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/session/box_response.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    22602 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/session/session.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk/util/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3012 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/api_call_decorator.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7541 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/chunked_uploader.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      795 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/datetime_formatter.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       29 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/default_arg_value.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1172 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/deprecation_decorator.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4299 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/enum.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      494 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/json.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3744 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/log.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1314 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/lru_cache.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      585 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/multipart_stream.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      561 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/shared_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      214 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/text_enum.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7743 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/util/translator.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      319 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      899 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/config.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3581 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/exception.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/boxsdk/py.typed
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       22 2023-07-25 10:59:03.000000 boxsdk-3.8.0/boxsdk/version.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk.egg-info/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18318 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk.egg-info/PKG-INFO
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9609 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        1 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      335 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk.egg-info/requires.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        7 2023-07-25 11:00:18.000000 boxsdk-3.8.0/boxsdk.egg-info/top_level.txt
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/functional/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/functional/mock_box/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/functional/mock_box/behavior/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/behavior/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3889 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/behavior/event_behavior.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5755 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/behavior/file_behavior.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5822 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/behavior/folder_behavior.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      617 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/behavior/item_behavior.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6554 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/behavior/oauth2_behavior.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      945 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/behavior/user_behavior.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/functional/mock_box/db_model/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       87 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/db_model/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      945 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/db_model/application_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      767 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/db_model/collaboration_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1260 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/db_model/event_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1666 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/db_model/file_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1862 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/db_model/folder_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      844 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/db_model/group_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      747 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/db_model/lock_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      804 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/db_model/share_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      738 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/db_model/token_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1214 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/db_model/user_model.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/functional/mock_box/util/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/util/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2696 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/util/chaos_utils.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1085 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/util/db_utils.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3609 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/util/http_utils.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2112 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/util/json_utils.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/functional/mock_box/views/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/views/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      202 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/views/html_response.tpl
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      256 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/views/oauth2.tpl
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       69 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/views/xml_response.tpl
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11636 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/mock_box/box.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3896 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1241 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/test_delete.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7449 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/test_events.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4287 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/test_file_upload_update_download.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3687 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/test_item_info.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1933 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/test_object_clone.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      383 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/test_rate_limits.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3522 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/test_recovery.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      767 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/functional/test_token_refresh.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/integration/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1403 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1019 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration/mock_network.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3909 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration/test_as_user.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1117 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration/test_retry_and_refresh.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4602 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration/test_with_shared_link.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/integration_new/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/integration_new/context_managers/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      652 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/context_managers/box_metadata_template.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1274 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/context_managers/box_retention_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      828 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/context_managers/box_retention_policy_assigment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      504 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/context_managers/box_sign_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      785 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/context_managers/box_test_file.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      665 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/context_managers/box_test_folder.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      498 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/context_managers/box_test_group.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      545 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/context_managers/box_test_user.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      740 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/context_managers/box_test_web_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      521 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/context_managers/local_large_file.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/integration_new/object/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1502 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/object/collaboration_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11058 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/object/file_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8169 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/object/folder_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1445 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/object/legal_hold_policy_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1584 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/object/metadata_template_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2288 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/object/retention_policy_assignement_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1573 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/object/retention_policy_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2346 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/object/sign_request_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2537 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/object/trash_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      192 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/object/user_itest.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/integration_new/resources/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1359 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/resources/image.png
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5558 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/resources/small.pdf
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6235 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/resources/small_v2.pdf
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1703 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/README.md
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2092 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1429 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       37 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/integration_tests.cfg
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      921 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/integration_new/util.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/unit/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/unit/auth/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/auth/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12588 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/auth/test_ccg_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      564 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/auth/test_cooperatively_managed_oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1072 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/auth/test_developer_token_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    26294 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/auth/test_jwt_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    17298 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/auth/test_oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2377 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/auth/test_redis_managed_oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      575 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/auth/test_remote_managed_oauth2.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/unit/client/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/client/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    61235 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/client/test_client.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/unit/network/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/network/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1602 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/network/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11382 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/network/test_network.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/unit/object/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12022 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      477 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_api_json_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2307 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_base_api_json_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6378 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_base_item.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5111 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_base_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    13966 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_chunked_upload.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4274 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_collaboration.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3564 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_collaboration_allowlist.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1143 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_collaboration_allowlist_entry.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1238 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_collaboration_allowlist_exempt_target.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1360 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2262 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_comment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1577 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_device_pin.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1248 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_enterprise.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      430 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_event.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11176 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_events.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    36673 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_file.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3650 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_file_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      650 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_file_version_retention.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    27532 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_folder.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9451 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_group.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    19897 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_item.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      895 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_legal_hold.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2091 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_legal_hold_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5705 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_legal_hold_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4628 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_metadata.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2489 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_metadata_cascade_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5421 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_metadata_template.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4579 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_retention_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3503 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_retention_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14811 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_search.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5195 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_sign_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7028 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_storage_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2332 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_storage_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5585 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_task.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3128 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_task_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7926 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_terms_of_service.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2885 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_terms_of_service_user_status.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6814 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_trash.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8088 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_upload_session.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9668 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_user.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4958 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_web_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4142 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/object/test_webhook.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/unit/pagination/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/pagination/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4324 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/pagination/box_object_collection_test_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5427 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/pagination/test_limit_offset_based_object_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4575 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/pagination/test_marker_based_object_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2966 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/pagination/test_page.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/unit/session/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/session/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    17669 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/session/test_session.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/unit/util/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/util/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3478 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/util/test_api_call_decorator.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2309 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/util/test_datetime_formatter.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4928 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/util/test_enum.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3856 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/util/test_log.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1102 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/util/test_lru_cache.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1098 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/util/test_multipart_stream.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      639 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/util/test_shared_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      324 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/util/test_text_enum.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7419 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/util/test_translator.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5085 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1963 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/unit/test_exception.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 11:00:18.000000 boxsdk-3.8.0/test/util/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/util/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      644 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/util/streamable_mock_open.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8430 2023-07-25 10:47:43.000000 boxsdk-3.8.0/test/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9574 2023-07-25 10:47:43.000000 boxsdk-3.8.0/LICENSE
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       52 2023-07-25 10:47:43.000000 boxsdk-3.8.0/MANIFEST.in
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    16879 2023-07-25 10:47:43.000000 boxsdk-3.8.0/README.md
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      136 2023-07-25 11:00:18.000000 boxsdk-3.8.0/setup.cfg
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3781 2023-07-25 10:47:43.000000 boxsdk-3.8.0/setup.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18318 2023-07-25 11:00:18.000000 boxsdk-3.8.0/PKG-INFO
```

### Comparing `boxsdk-3.7.3/boxsdk/auth/__init__.py` & `boxsdk-3.8.0/boxsdk/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/auth/ccg_auth.py` & `boxsdk-3.8.0/boxsdk/auth/ccg_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/auth/cooperatively_managed_oauth2.py` & `boxsdk-3.8.0/boxsdk/auth/cooperatively_managed_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/auth/developer_token_auth.py` & `boxsdk-3.8.0/boxsdk/auth/developer_token_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/auth/jwt_auth.py` & `boxsdk-3.8.0/boxsdk/auth/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/auth/oauth2.py` & `boxsdk-3.8.0/boxsdk/auth/oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/auth/redis_managed_jwt_auth.py` & `boxsdk-3.8.0/boxsdk/auth/redis_managed_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/auth/redis_managed_oauth2.py` & `boxsdk-3.8.0/boxsdk/auth/redis_managed_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/auth/remote_managed_oauth2.py` & `boxsdk-3.8.0/boxsdk/auth/remote_managed_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/auth/server_auth.py` & `boxsdk-3.8.0/boxsdk/auth/server_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/client/client.py` & `boxsdk-3.8.0/boxsdk/client/client.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/network/default_network.py` & `boxsdk-3.8.0/boxsdk/network/default_network.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/network/network_interface.py` & `boxsdk-3.8.0/boxsdk/network/network_interface.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/__init__.py` & `boxsdk-3.8.0/boxsdk/object/__init__.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/api_json_object.py` & `boxsdk-3.8.0/boxsdk/object/api_json_object.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/base_api_json_object.py` & `boxsdk-3.8.0/boxsdk/object/base_api_json_object.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/base_endpoint.py` & `boxsdk-3.8.0/boxsdk/object/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/base_item.py` & `boxsdk-3.8.0/boxsdk/object/base_item.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/base_object.py` & `boxsdk-3.8.0/boxsdk/object/base_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         Send a PUT to the object's base endpoint to modify the provided
         attributes.
 
         :param data:
             The updated information about this object.
             Must be JSON serializable.
             Update the object attributes in data.keys(). The semantics of the
-            values depends on the the type and attributes of the object being
+            values depends on the type and attributes of the object being
             updated. For details on particular semantics, refer to the Box
             developer API documentation <https://developer.box.com/>.
         :param params:
             (optional) Query string parameters for the request.
         :param headers:
             (optional) Extra HTTP headers for the request.
         :param kwargs:
```

### Comparing `boxsdk-3.7.3/boxsdk/object/cloneable.py` & `boxsdk-3.8.0/boxsdk/object/cloneable.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/collaboration.py` & `boxsdk-3.8.0/boxsdk/object/collaboration.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,37 +30,40 @@
     """An object that represents a collaboration between a folder and an individual or group"""
     _item_type = 'collaboration'
 
     @api_call
     def update_info(
             self,
             *,
+            data: dict = None,
             role: Optional[CollaborationRole] = None,
             status: Optional[CollaborationStatus] = None,
             **kwargs: Any
     ) -> 'BaseObject':
         """Edit an existing collaboration on Box
-
+        :param data:
+            The updated information about this object.
         :param role:
             The new role for this collaboration or None to leave unchanged
         :param status:
             The new status for this collaboration or None to leave unchanged. A pending collaboration can be set to
             accepted or rejected if permissions allow it.
         :returns:
             Whether or not the edit was successful.
         :raises:
             :class:`BoxAPIException` if current user doesn't have permissions to edit the collaboration.
         """
         # pylint:disable=arguments-differ
-        data = {}
+        if data is None:
+            data = {}
         if role:
             data['role'] = role
         if status:
             data['status'] = status
-        if role == CollaborationRole.OWNER:
+        if data.get('role', None) == CollaborationRole.OWNER:
             return super().update_info(data=data, expect_json_response=False, **kwargs)
 
         return super().update_info(data=data, **kwargs)
 
     @api_call
     def accept(self) -> 'BaseObject':
         """Accepts a pending collaboration"""
```

### Comparing `boxsdk-3.7.3/boxsdk/object/collaboration_allowlist.py` & `boxsdk-3.8.0/boxsdk/object/collaboration_allowlist.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/collaboration_allowlist_entry.py` & `boxsdk-3.8.0/boxsdk/object/collaboration_allowlist_entry.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/collection.py` & `boxsdk-3.8.0/boxsdk/object/collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/comment.py` & `boxsdk-3.8.0/boxsdk/object/comment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/enterprise.py` & `boxsdk-3.8.0/boxsdk/object/enterprise.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/events.py` & `boxsdk-3.8.0/boxsdk/object/events.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/file.py` & `boxsdk-3.8.0/boxsdk/object/file.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/file_request.py` & `boxsdk-3.8.0/boxsdk/object/file_request.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/folder.py` & `boxsdk-3.8.0/boxsdk/object/folder.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/group.py` & `boxsdk-3.8.0/boxsdk/object/group.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/item.py` & `boxsdk-3.8.0/boxsdk/object/item.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/legal_hold_policy.py` & `boxsdk-3.8.0/boxsdk/object/legal_hold_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/metadata.py` & `boxsdk-3.8.0/boxsdk/object/metadata.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/metadata_cascade_policy.py` & `boxsdk-3.8.0/boxsdk/object/metadata_cascade_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/metadata_template.py` & `boxsdk-3.8.0/boxsdk/object/metadata_template.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/retention_policy.py` & `boxsdk-3.8.0/boxsdk/object/retention_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/retention_policy_assignment.py` & `boxsdk-3.8.0/boxsdk/object/retention_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/search.py` & `boxsdk-3.8.0/boxsdk/object/search.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/sign_request.py` & `boxsdk-3.8.0/boxsdk/object/sign_request.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/storage_policy.py` & `boxsdk-3.8.0/boxsdk/object/storage_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/task.py` & `boxsdk-3.8.0/boxsdk/object/task.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/terms_of_service.py` & `boxsdk-3.8.0/boxsdk/object/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/terms_of_service_user_status.py` & `boxsdk-3.8.0/boxsdk/object/terms_of_service_user_status.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/trash.py` & `boxsdk-3.8.0/boxsdk/object/trash.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/upload_session.py` & `boxsdk-3.8.0/boxsdk/object/upload_session.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/user.py` & `boxsdk-3.8.0/boxsdk/object/user.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/web_link.py` & `boxsdk-3.8.0/boxsdk/object/web_link.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/object/webhook.py` & `boxsdk-3.8.0/boxsdk/object/webhook.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/pagination/box_object_collection.py` & `boxsdk-3.8.0/boxsdk/pagination/box_object_collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/pagination/limit_offset_based_object_collection.py` & `boxsdk-3.8.0/boxsdk/pagination/limit_offset_based_object_collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/pagination/marker_based_object_collection.py` & `boxsdk-3.8.0/boxsdk/pagination/marker_based_object_collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/pagination/page.py` & `boxsdk-3.8.0/boxsdk/pagination/page.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/session/box_request.py` & `boxsdk-3.8.0/boxsdk/session/box_request.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/session/box_response.py` & `boxsdk-3.8.0/boxsdk/session/box_response.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/session/session.py` & `boxsdk-3.8.0/boxsdk/session/session.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/util/api_call_decorator.py` & `boxsdk-3.8.0/boxsdk/util/api_call_decorator.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/util/chunked_uploader.py` & `boxsdk-3.8.0/boxsdk/util/chunked_uploader.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/util/datetime_formatter.py` & `boxsdk-3.8.0/boxsdk/util/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/util/deprecation_decorator.py` & `boxsdk-3.8.0/boxsdk/util/deprecation_decorator.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/util/enum.py` & `boxsdk-3.8.0/boxsdk/util/enum.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/util/log.py` & `boxsdk-3.8.0/boxsdk/util/log.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/util/lru_cache.py` & `boxsdk-3.8.0/boxsdk/util/lru_cache.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/util/multipart_stream.py` & `boxsdk-3.8.0/boxsdk/util/multipart_stream.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/util/shared_link.py` & `boxsdk-3.8.0/boxsdk/util/shared_link.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/util/translator.py` & `boxsdk-3.8.0/boxsdk/util/translator.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/config.py` & `boxsdk-3.8.0/boxsdk/config.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk/exception.py` & `boxsdk-3.8.0/boxsdk/exception.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/boxsdk.egg-info/PKG-INFO` & `boxsdk-3.8.0/boxsdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxsdk
-Version: 3.7.3
+Version: 3.8.0
 Summary: Official Box Python SDK
 Home-page: https://github.com/box/box-python-sdk
 Author: Box
 Author-email: oss@box.com
 License: Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Changelog, https://github.com/box/box-python-sdk/blob/main/CHANGELOG.md
 Keywords: box oauth2 sdk
@@ -48,31 +48,32 @@
 [![image](https://coveralls.io/repos/github/box/box-python-sdk/badge.svg?branch=main)](https://coveralls.io/github/box/box-python-sdk?branch=main)
 
 Getting Started Docs: <https://developer.box.com/guides/tooling/sdks/python/>
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
-- [Versions](#versions)
-  - [Supported Version](#supported-version)
-  - [Version schedule](#version-schedule)
 - [Installing](#installing)
 - [Getting Started](#getting-started)
 - [Authorization](#authorization)
   - [Server-to-Server Auth with JWT](#server-to-server-auth-with-jwt)
   - [Traditional 3-legged OAuth2](#traditional-3-legged-oauth2)
   - [Other Auth Options](#other-auth-options)
 - [Usage Documentation](#usage-documentation)
   - [Making API Calls Manually](#making-api-calls-manually)
 - [Other Client Options](#other-client-options)
   - [Logging Client](#logging-client)
   - [Developer Token Client](#developer-token-client)
   - [Development Client](#development-client)
 - [Customization](#customization)
   - [Custom Subclasses](#custom-subclasses)
+- [FIPS 140-2 Compliance](#fips-140-2-compliance)
+- [Versions](#versions)
+  - [Supported Version](#supported-version)
+  - [Version schedule](#version-schedule)
 - [Contributing](#contributing)
   - [Developer Setup](#developer-setup)
   - [Testing](#testing)
 - [Questions, Bugs, and Feature Requests?](#questions-bugs-and-feature-requests)
 - [Copyright and License](#copyright-and-license)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
@@ -420,14 +421,29 @@
 ```
 
 If an object subclass is registered in this way, instances of this
 subclass will be returned from all SDK methods that previously returned
 an instance of the parent. See `BaseAPIJSONObjectMeta` and `Translator`
 to see how the SDK performs dynamic lookups to determine return types.
 
+# FIPS 140-2 Compliance
+
+The Python SDK allows the use of FIPS 140-2 validated SSL libraries, such as OpenSSL 3.0.
+However, some actions are required to enable this functionality.
+
+Currently, the latest distributions of Python default to OpenSSL v1.1.1, which is not FIPS compliant.
+Therefore, if you want to use OpenSSL 3.0 in your network communication,
+you need to ensure that Python uses a custom SSL library.
+One way to achieve this is by creating a custom Python distribution with the ssl module replaced.
+
+If you are using JWT for authentication, it is also necessary to ensure that the cryptography library,
+which is one of the extra dependencies for JWT, uses OpenSSL 3.0.
+To enable FIPS mode for the `cryptography` library, you need to install a FIPS-compliant version of OpenSSL
+during the installation process of cryptography using the `pip` command.
+
 # Versions
 We use a modified version of [Semantic Versioning](https://semver.org/) for all changes. See [version strategy](VERSIONS.md) for details which is effective from 30 July 2022.
 
 ## Supported Version
 
 Only the current MAJOR version of SDK is supported. New features, functionality, bug fixes, and security updates will only be added to the current MAJOR version.
```

### Comparing `boxsdk-3.7.3/boxsdk.egg-info/SOURCES.txt` & `boxsdk-3.8.0/boxsdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -166,14 +166,15 @@
 test/integration_new/context_managers/box_sign_request.py
 test/integration_new/context_managers/box_test_file.py
 test/integration_new/context_managers/box_test_folder.py
 test/integration_new/context_managers/box_test_group.py
 test/integration_new/context_managers/box_test_user.py
 test/integration_new/context_managers/box_test_web_link.py
 test/integration_new/context_managers/local_large_file.py
+test/integration_new/object/collaboration_itest.py
 test/integration_new/object/file_itest.py
 test/integration_new/object/folder_itest.py
 test/integration_new/object/legal_hold_policy_itest.py
 test/integration_new/object/metadata_template_itest.py
 test/integration_new/object/retention_policy_assignement_itest.py
 test/integration_new/object/retention_policy_itest.py
 test/integration_new/object/sign_request_itest.py
```

### Comparing `boxsdk-3.7.3/test/functional/mock_box/behavior/event_behavior.py` & `boxsdk-3.8.0/test/functional/mock_box/behavior/event_behavior.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/behavior/file_behavior.py` & `boxsdk-3.8.0/test/functional/mock_box/behavior/file_behavior.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/behavior/folder_behavior.py` & `boxsdk-3.8.0/test/functional/mock_box/behavior/folder_behavior.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/behavior/item_behavior.py` & `boxsdk-3.8.0/test/functional/mock_box/behavior/item_behavior.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/behavior/oauth2_behavior.py` & `boxsdk-3.8.0/test/functional/mock_box/behavior/oauth2_behavior.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/behavior/user_behavior.py` & `boxsdk-3.8.0/test/functional/mock_box/behavior/user_behavior.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/db_model/application_model.py` & `boxsdk-3.8.0/test/functional/mock_box/db_model/application_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/db_model/collaboration_model.py` & `boxsdk-3.8.0/test/functional/mock_box/db_model/collaboration_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/db_model/event_model.py` & `boxsdk-3.8.0/test/functional/mock_box/db_model/event_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/db_model/file_model.py` & `boxsdk-3.8.0/test/functional/mock_box/db_model/file_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/db_model/folder_model.py` & `boxsdk-3.8.0/test/functional/mock_box/db_model/folder_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/db_model/group_model.py` & `boxsdk-3.8.0/test/functional/mock_box/db_model/group_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/db_model/lock_model.py` & `boxsdk-3.8.0/test/functional/mock_box/db_model/lock_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/db_model/share_model.py` & `boxsdk-3.8.0/test/functional/mock_box/db_model/share_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/db_model/token_model.py` & `boxsdk-3.8.0/test/functional/mock_box/db_model/token_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/db_model/user_model.py` & `boxsdk-3.8.0/test/functional/mock_box/db_model/user_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/util/chaos_utils.py` & `boxsdk-3.8.0/test/functional/mock_box/util/chaos_utils.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/util/db_utils.py` & `boxsdk-3.8.0/test/functional/mock_box/util/db_utils.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/util/http_utils.py` & `boxsdk-3.8.0/test/functional/mock_box/util/http_utils.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/util/json_utils.py` & `boxsdk-3.8.0/test/functional/mock_box/util/json_utils.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/mock_box/box.py` & `boxsdk-3.8.0/test/functional/mock_box/box.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/conftest.py` & `boxsdk-3.8.0/test/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/test_delete.py` & `boxsdk-3.8.0/test/functional/test_delete.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/test_events.py` & `boxsdk-3.8.0/test/functional/test_events.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/test_file_upload_update_download.py` & `boxsdk-3.8.0/test/functional/test_file_upload_update_download.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/test_item_info.py` & `boxsdk-3.8.0/test/functional/test_item_info.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/test_object_clone.py` & `boxsdk-3.8.0/test/functional/test_object_clone.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/test_recovery.py` & `boxsdk-3.8.0/test/functional/test_recovery.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/functional/test_token_refresh.py` & `boxsdk-3.8.0/test/functional/test_token_refresh.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration/conftest.py` & `boxsdk-3.8.0/test/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration/mock_network.py` & `boxsdk-3.8.0/test/integration/mock_network.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration/test_as_user.py` & `boxsdk-3.8.0/test/integration/test_as_user.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration/test_retry_and_refresh.py` & `boxsdk-3.8.0/test/integration/test_retry_and_refresh.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration/test_with_shared_link.py` & `boxsdk-3.8.0/test/integration/test_with_shared_link.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/context_managers/box_metadata_template.py` & `boxsdk-3.8.0/test/integration_new/context_managers/box_metadata_template.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/context_managers/box_retention_policy.py` & `boxsdk-3.8.0/test/integration_new/context_managers/box_retention_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/context_managers/box_retention_policy_assigment.py` & `boxsdk-3.8.0/test/integration_new/context_managers/box_retention_policy_assigment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/context_managers/box_test_file.py` & `boxsdk-3.8.0/test/integration_new/context_managers/box_test_file.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/context_managers/box_test_folder.py` & `boxsdk-3.8.0/test/integration_new/context_managers/box_test_folder.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/context_managers/box_test_user.py` & `boxsdk-3.8.0/test/integration_new/context_managers/box_test_user.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/context_managers/box_test_web_link.py` & `boxsdk-3.8.0/test/integration_new/context_managers/box_test_web_link.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/context_managers/local_large_file.py` & `boxsdk-3.8.0/test/integration_new/context_managers/local_large_file.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/object/file_itest.py` & `boxsdk-3.8.0/test/integration_new/object/file_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/object/folder_itest.py` & `boxsdk-3.8.0/test/integration_new/object/folder_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/object/legal_hold_policy_itest.py` & `boxsdk-3.8.0/test/integration_new/object/legal_hold_policy_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/object/metadata_template_itest.py` & `boxsdk-3.8.0/test/integration_new/object/metadata_template_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/object/retention_policy_assignement_itest.py` & `boxsdk-3.8.0/test/integration_new/object/retention_policy_assignement_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/object/retention_policy_itest.py` & `boxsdk-3.8.0/test/integration_new/object/retention_policy_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/object/sign_request_itest.py` & `boxsdk-3.8.0/test/integration_new/object/sign_request_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/object/trash_itest.py` & `boxsdk-3.8.0/test/integration_new/object/trash_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/resources/image.png` & `boxsdk-3.8.0/test/integration_new/resources/image.png`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/resources/small.pdf` & `boxsdk-3.8.0/test/integration_new/resources/small.pdf`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/resources/small_v2.pdf` & `boxsdk-3.8.0/test/integration_new/resources/small_v2.pdf`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/README.md` & `boxsdk-3.8.0/test/integration_new/README.md`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/__init__.py` & `boxsdk-3.8.0/test/integration_new/__init__.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/conftest.py` & `boxsdk-3.8.0/test/integration_new/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/integration_new/util.py` & `boxsdk-3.8.0/test/integration_new/util.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/auth/test_ccg_auth.py` & `boxsdk-3.8.0/test/unit/auth/test_ccg_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/auth/test_cooperatively_managed_oauth2.py` & `boxsdk-3.8.0/test/unit/auth/test_cooperatively_managed_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/auth/test_developer_token_auth.py` & `boxsdk-3.8.0/test/unit/auth/test_developer_token_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/auth/test_jwt_auth.py` & `boxsdk-3.8.0/test/unit/auth/test_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/auth/test_oauth2.py` & `boxsdk-3.8.0/test/unit/auth/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/auth/test_redis_managed_oauth2.py` & `boxsdk-3.8.0/test/unit/auth/test_redis_managed_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/auth/test_remote_managed_oauth2.py` & `boxsdk-3.8.0/test/unit/auth/test_remote_managed_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/client/test_client.py` & `boxsdk-3.8.0/test/unit/client/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1688,27 +1688,35 @@
     expected_url = f'{API.BASE_API_URL}/sign_requests'
     redirect_url = 'https://www.box.com/accepted'
     declined_redirect_url = 'https://www.box.com/declined'
     source_file = {
         'id': '12345',
         'type': 'file'
     }
-    files = [source_file]
+    source_file2 = {
+        'id': '34567',
+        'type': 'file'
+    }
+    files = [source_file, source_file2]
 
     signer = {
         'email': 'example@gmail.com'
     }
     signers = [signer]
     parent_folder_id = '12345'
 
     data = json.dumps({
         'source_files': [
             {
                 'id': source_file['id'],
                 'type': source_file['type']
+            },
+            {
+                'id': source_file2['id'],
+                'type': source_file2['type']
             }
         ],
         'signers': [
             {
                 'email': signer['email']
             }
         ],
```

### Comparing `boxsdk-3.7.3/test/unit/network/conftest.py` & `boxsdk-3.8.0/test/unit/network/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/network/test_network.py` & `boxsdk-3.8.0/test/unit/network/test_network.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/conftest.py` & `boxsdk-3.8.0/test/unit/object/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_base_api_json_object.py` & `boxsdk-3.8.0/test/unit/object/test_base_api_json_object.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_base_item.py` & `boxsdk-3.8.0/test/unit/object/test_base_item.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_base_object.py` & `boxsdk-3.8.0/test/unit/object/test_base_object.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_chunked_upload.py` & `boxsdk-3.8.0/test/unit/object/test_chunked_upload.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_collaboration.py` & `boxsdk-3.8.0/test/unit/object/test_collaboration.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,22 +28,48 @@
         headers=None,
         params=None,
     )
     assert isinstance(update_response, test_collaboration.__class__)
     assert update_response.object_id == test_collaboration.object_id
 
 
+@pytest.mark.parametrize('data', [
+    {},
+    {'role': CollaborationRole.EDITOR, 'status': CollaborationStatus.REJECTED},
+    {'role': CollaborationRole.EDITOR, 'status': CollaborationStatus.ACCEPTED},
+    {'role': CollaborationRole.EDITOR, 'expires_at': '2025-08-29T23:59:00-07:00'},
+    {'role': CollaborationRole.EDITOR, 'can_view_path': True},
+])
+def test_update_info_returns_the_correct_response_with_data_param(
+        test_collaboration,
+        mock_box_session,
+        mock_collab_response,
+        data):
+    # pylint:disable=protected-access
+    expected_url = test_collaboration.get_url()
+    mock_box_session.put.return_value = mock_collab_response
+    update_response = test_collaboration.update_info(data=data)
+    mock_box_session.put.assert_called_once_with(
+        expected_url,
+        data=json.dumps(data),
+        headers=None,
+        params=None,
+    )
+    assert isinstance(update_response, test_collaboration.__class__)
+    assert update_response.object_id == test_collaboration.object_id
+
+
 def test_update_info_returns_204(
         test_collaboration,
         mock_box_session):
     # pylint:disable=protected-access
     data = {'role': CollaborationRole.OWNER, 'status': CollaborationStatus.ACCEPTED}
     expected_url = test_collaboration.get_url()
     mock_box_session.put.return_value.ok = True
-    is_success = test_collaboration.update_info(**data)
+    is_success = test_collaboration.update_info(data=data)
     mock_box_session.put.assert_called_once_with(
         expected_url,
         data=json.dumps(data),
         expect_json_response=False,
         headers=None,
         params=None,
     )
```

### Comparing `boxsdk-3.7.3/test/unit/object/test_collaboration_allowlist.py` & `boxsdk-3.8.0/test/unit/object/test_collaboration_allowlist.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_collaboration_allowlist_entry.py` & `boxsdk-3.8.0/test/unit/object/test_collaboration_allowlist_entry.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_collaboration_allowlist_exempt_target.py` & `boxsdk-3.8.0/test/unit/object/test_collaboration_allowlist_exempt_target.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_collection.py` & `boxsdk-3.8.0/test/unit/object/test_collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_comment.py` & `boxsdk-3.8.0/test/unit/object/test_comment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_device_pin.py` & `boxsdk-3.8.0/test/unit/object/test_device_pin.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_enterprise.py` & `boxsdk-3.8.0/test/unit/object/test_enterprise.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_events.py` & `boxsdk-3.8.0/test/unit/object/test_events.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_file.py` & `boxsdk-3.8.0/test/unit/object/test_file.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_file_request.py` & `boxsdk-3.8.0/test/unit/object/test_file_request.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_file_version_retention.py` & `boxsdk-3.8.0/test/unit/object/test_file_version_retention.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_folder.py` & `boxsdk-3.8.0/test/unit/object/test_folder.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_group.py` & `boxsdk-3.8.0/test/unit/object/test_group.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_item.py` & `boxsdk-3.8.0/test/unit/object/test_item.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_legal_hold.py` & `boxsdk-3.8.0/test/unit/object/test_legal_hold.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_legal_hold_assignment.py` & `boxsdk-3.8.0/test/unit/object/test_legal_hold_assignment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_legal_hold_policy.py` & `boxsdk-3.8.0/test/unit/object/test_legal_hold_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_metadata.py` & `boxsdk-3.8.0/test/unit/object/test_metadata.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_metadata_cascade_policy.py` & `boxsdk-3.8.0/test/unit/object/test_metadata_cascade_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_metadata_template.py` & `boxsdk-3.8.0/test/unit/object/test_metadata_template.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_retention_policy.py` & `boxsdk-3.8.0/test/unit/object/test_retention_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_retention_policy_assignment.py` & `boxsdk-3.8.0/test/unit/object/test_retention_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_search.py` & `boxsdk-3.8.0/test/unit/object/test_search.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_sign_request.py` & `boxsdk-3.8.0/test/unit/object/test_sign_request.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_storage_policy.py` & `boxsdk-3.8.0/test/unit/object/test_storage_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_storage_policy_assignment.py` & `boxsdk-3.8.0/test/unit/object/test_storage_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_task.py` & `boxsdk-3.8.0/test/unit/object/test_task.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_task_assignment.py` & `boxsdk-3.8.0/test/unit/object/test_task_assignment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_terms_of_service.py` & `boxsdk-3.8.0/test/unit/object/test_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_terms_of_service_user_status.py` & `boxsdk-3.8.0/test/unit/object/test_terms_of_service_user_status.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_trash.py` & `boxsdk-3.8.0/test/unit/object/test_trash.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_upload_session.py` & `boxsdk-3.8.0/test/unit/object/test_upload_session.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_user.py` & `boxsdk-3.8.0/test/unit/object/test_user.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_web_link.py` & `boxsdk-3.8.0/test/unit/object/test_web_link.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/object/test_webhook.py` & `boxsdk-3.8.0/test/unit/object/test_webhook.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/pagination/box_object_collection_test_base.py` & `boxsdk-3.8.0/test/unit/pagination/box_object_collection_test_base.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/pagination/test_limit_offset_based_object_collection.py` & `boxsdk-3.8.0/test/unit/pagination/test_limit_offset_based_object_collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/pagination/test_marker_based_object_collection.py` & `boxsdk-3.8.0/test/unit/pagination/test_marker_based_object_collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/pagination/test_page.py` & `boxsdk-3.8.0/test/unit/pagination/test_page.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/session/test_session.py` & `boxsdk-3.8.0/test/unit/session/test_session.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/util/test_api_call_decorator.py` & `boxsdk-3.8.0/test/unit/util/test_api_call_decorator.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/util/test_datetime_formatter.py` & `boxsdk-3.8.0/test/unit/util/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/util/test_enum.py` & `boxsdk-3.8.0/test/unit/util/test_enum.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/util/test_log.py` & `boxsdk-3.8.0/test/unit/util/test_log.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/util/test_lru_cache.py` & `boxsdk-3.8.0/test/unit/util/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/util/test_multipart_stream.py` & `boxsdk-3.8.0/test/unit/util/test_multipart_stream.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/util/test_shared_link.py` & `boxsdk-3.8.0/test/unit/util/test_shared_link.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/util/test_translator.py` & `boxsdk-3.8.0/test/unit/util/test_translator.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/conftest.py` & `boxsdk-3.8.0/test/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/unit/test_exception.py` & `boxsdk-3.8.0/test/unit/test_exception.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/util/streamable_mock_open.py` & `boxsdk-3.8.0/test/util/streamable_mock_open.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/test/conftest.py` & `boxsdk-3.8.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/LICENSE` & `boxsdk-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/README.md` & `boxsdk-3.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,31 +12,32 @@
 [![image](https://coveralls.io/repos/github/box/box-python-sdk/badge.svg?branch=main)](https://coveralls.io/github/box/box-python-sdk?branch=main)
 
 Getting Started Docs: <https://developer.box.com/guides/tooling/sdks/python/>
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
-- [Versions](#versions)
-  - [Supported Version](#supported-version)
-  - [Version schedule](#version-schedule)
 - [Installing](#installing)
 - [Getting Started](#getting-started)
 - [Authorization](#authorization)
   - [Server-to-Server Auth with JWT](#server-to-server-auth-with-jwt)
   - [Traditional 3-legged OAuth2](#traditional-3-legged-oauth2)
   - [Other Auth Options](#other-auth-options)
 - [Usage Documentation](#usage-documentation)
   - [Making API Calls Manually](#making-api-calls-manually)
 - [Other Client Options](#other-client-options)
   - [Logging Client](#logging-client)
   - [Developer Token Client](#developer-token-client)
   - [Development Client](#development-client)
 - [Customization](#customization)
   - [Custom Subclasses](#custom-subclasses)
+- [FIPS 140-2 Compliance](#fips-140-2-compliance)
+- [Versions](#versions)
+  - [Supported Version](#supported-version)
+  - [Version schedule](#version-schedule)
 - [Contributing](#contributing)
   - [Developer Setup](#developer-setup)
   - [Testing](#testing)
 - [Questions, Bugs, and Feature Requests?](#questions-bugs-and-feature-requests)
 - [Copyright and License](#copyright-and-license)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
@@ -384,14 +385,29 @@
 ```
 
 If an object subclass is registered in this way, instances of this
 subclass will be returned from all SDK methods that previously returned
 an instance of the parent. See `BaseAPIJSONObjectMeta` and `Translator`
 to see how the SDK performs dynamic lookups to determine return types.
 
+# FIPS 140-2 Compliance
+
+The Python SDK allows the use of FIPS 140-2 validated SSL libraries, such as OpenSSL 3.0.
+However, some actions are required to enable this functionality.
+
+Currently, the latest distributions of Python default to OpenSSL v1.1.1, which is not FIPS compliant.
+Therefore, if you want to use OpenSSL 3.0 in your network communication,
+you need to ensure that Python uses a custom SSL library.
+One way to achieve this is by creating a custom Python distribution with the ssl module replaced.
+
+If you are using JWT for authentication, it is also necessary to ensure that the cryptography library,
+which is one of the extra dependencies for JWT, uses OpenSSL 3.0.
+To enable FIPS mode for the `cryptography` library, you need to install a FIPS-compliant version of OpenSSL
+during the installation process of cryptography using the `pip` command.
+
 # Versions
 We use a modified version of [Semantic Versioning](https://semver.org/) for all changes. See [version strategy](VERSIONS.md) for details which is effective from 30 July 2022.
 
 ## Supported Version
 
 Only the current MAJOR version of SDK is supported. New features, functionality, bug fixes, and security updates will only be added to the current MAJOR version.
```

### Comparing `boxsdk-3.7.3/setup.py` & `boxsdk-3.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.7.3/PKG-INFO` & `boxsdk-3.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxsdk
-Version: 3.7.3
+Version: 3.8.0
 Summary: Official Box Python SDK
 Home-page: https://github.com/box/box-python-sdk
 Author: Box
 Author-email: oss@box.com
 License: Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Changelog, https://github.com/box/box-python-sdk/blob/main/CHANGELOG.md
 Keywords: box oauth2 sdk
@@ -48,31 +48,32 @@
 [![image](https://coveralls.io/repos/github/box/box-python-sdk/badge.svg?branch=main)](https://coveralls.io/github/box/box-python-sdk?branch=main)
 
 Getting Started Docs: <https://developer.box.com/guides/tooling/sdks/python/>
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
-- [Versions](#versions)
-  - [Supported Version](#supported-version)
-  - [Version schedule](#version-schedule)
 - [Installing](#installing)
 - [Getting Started](#getting-started)
 - [Authorization](#authorization)
   - [Server-to-Server Auth with JWT](#server-to-server-auth-with-jwt)
   - [Traditional 3-legged OAuth2](#traditional-3-legged-oauth2)
   - [Other Auth Options](#other-auth-options)
 - [Usage Documentation](#usage-documentation)
   - [Making API Calls Manually](#making-api-calls-manually)
 - [Other Client Options](#other-client-options)
   - [Logging Client](#logging-client)
   - [Developer Token Client](#developer-token-client)
   - [Development Client](#development-client)
 - [Customization](#customization)
   - [Custom Subclasses](#custom-subclasses)
+- [FIPS 140-2 Compliance](#fips-140-2-compliance)
+- [Versions](#versions)
+  - [Supported Version](#supported-version)
+  - [Version schedule](#version-schedule)
 - [Contributing](#contributing)
   - [Developer Setup](#developer-setup)
   - [Testing](#testing)
 - [Questions, Bugs, and Feature Requests?](#questions-bugs-and-feature-requests)
 - [Copyright and License](#copyright-and-license)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
@@ -420,14 +421,29 @@
 ```
 
 If an object subclass is registered in this way, instances of this
 subclass will be returned from all SDK methods that previously returned
 an instance of the parent. See `BaseAPIJSONObjectMeta` and `Translator`
 to see how the SDK performs dynamic lookups to determine return types.
 
+# FIPS 140-2 Compliance
+
+The Python SDK allows the use of FIPS 140-2 validated SSL libraries, such as OpenSSL 3.0.
+However, some actions are required to enable this functionality.
+
+Currently, the latest distributions of Python default to OpenSSL v1.1.1, which is not FIPS compliant.
+Therefore, if you want to use OpenSSL 3.0 in your network communication,
+you need to ensure that Python uses a custom SSL library.
+One way to achieve this is by creating a custom Python distribution with the ssl module replaced.
+
+If you are using JWT for authentication, it is also necessary to ensure that the cryptography library,
+which is one of the extra dependencies for JWT, uses OpenSSL 3.0.
+To enable FIPS mode for the `cryptography` library, you need to install a FIPS-compliant version of OpenSSL
+during the installation process of cryptography using the `pip` command.
+
 # Versions
 We use a modified version of [Semantic Versioning](https://semver.org/) for all changes. See [version strategy](VERSIONS.md) for details which is effective from 30 July 2022.
 
 ## Supported Version
 
 Only the current MAJOR version of SDK is supported. New features, functionality, bug fixes, and security updates will only be added to the current MAJOR version.
```

