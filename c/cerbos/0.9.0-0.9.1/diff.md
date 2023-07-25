# Comparing `tmp/cerbos-0.9.0.tar.gz` & `tmp/cerbos-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbos-0.9.0.tar", last modified: Fri Jul 14 10:10:51 2023, max compression
+gzip compressed data, was "cerbos-0.9.1.tar", last modified: Tue Jul 25 07:36:30 2023, max compression
```

## Comparing `cerbos-0.9.0.tar` & `cerbos-0.9.1.tar`

### file list

```diff
@@ -1,75 +1,102 @@
--rw-r--r--   0        0        0    11357 2023-07-14 10:10:11.024972 cerbos-0.9.0/LICENSE
--rw-r--r--   0        0        0     6175 2023-07-14 10:10:11.024972 cerbos-0.9.0/README.md
--rw-r--r--   0        0        0      167 2023-07-14 10:10:11.024972 cerbos-0.9.0/cerbos/__init__.py
--rw-r--r--   0        0        0     5052 2023-07-14 10:10:11.024972 cerbos-0.9.0/cerbos/audit/v1/audit_pb2.py
--rw-r--r--   0        0        0     5463 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/audit/v1/audit_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/audit/v1/audit_pb2_grpc.py
--rw-r--r--   0        0        0     1537 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/effect/v1/effect_pb2.py
--rw-r--r--   0        0        0      541 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/effect/v1/effect_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/effect/v1/effect_pb2_grpc.py
--rw-r--r--   0        0        0    24465 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/engine/v1/engine_pb2.py
--rw-r--r--   0        0        0    18348 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/engine/v1/engine_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/engine/v1/engine_pb2_grpc.py
--rw-r--r--   0        0        0    35452 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/policy/v1/policy_pb2.py
--rw-r--r--   0        0        0    30998 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/policy/v1/policy_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/policy/v1/policy_pb2_grpc.py
--rw-r--r--   0        0        0    40721 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/request/v1/request_pb2.py
--rw-r--r--   0        0        0    14880 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/request/v1/request_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/request/v1/request_pb2_grpc.py
--rw-r--r--   0        0        0    40197 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/response/v1/response_pb2.py
--rw-r--r--   0        0        0    20863 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/response/v1/response_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/response/v1/response_pb2_grpc.py
--rw-r--r--   0        0        0     3055 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/schema/v1/schema_pb2.py
--rw-r--r--   0        0        0     1614 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/schema/v1/schema_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/schema/v1/schema_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/_async/__init__.py
--rw-r--r--   0        0        0    24037 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/_async/_grpc.py
--rw-r--r--   0        0        0    12739 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/_async/_http.py
--rw-r--r--   0        0        0        0 2023-07-14 10:10:47.565674 cerbos-0.9.0/cerbos/sdk/_sync/__init__.py
--rw-r--r--   0        0        0    23695 2023-07-14 10:10:48.865700 cerbos-0.9.0/cerbos/sdk/_sync/_grpc.py
--rw-r--r--   0        0        0    12551 2023-07-14 10:10:47.565674 cerbos-0.9.0/cerbos/sdk/_sync/_http.py
--rw-r--r--   0        0        0      481 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/client.py
--rw-r--r--   0        0        0      881 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/container.py
--rw-r--r--   0        0        0      491 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/grpc/client.py
--rw-r--r--   0        0        0      702 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/grpc/utils.py
--rw-r--r--   0        0        0      106 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/http/client.py
--rw-r--r--   0        0        0     6501 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/model.py
--rw-r--r--   0        0        0    14057 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/svc/v1/svc_pb2.py
--rw-r--r--   0        0        0      449 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/svc/v1/svc_pb2.pyi
--rw-r--r--   0        0        0    38288 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/svc/v1/svc_pb2_grpc.py
--rw-r--r--   0        0        0     9422 2023-07-14 10:10:11.032972 cerbos-0.9.0/cerbos/telemetry/v1/telemetry_pb2.py
--rw-r--r--   0        0        0    10796 2023-07-14 10:10:11.032972 cerbos-0.9.0/cerbos/telemetry/v1/telemetry_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-14 10:10:11.032972 cerbos-0.9.0/cerbos/telemetry/v1/telemetry_pb2_grpc.py
--rw-r--r--   0        0        0     2695 2023-07-14 10:10:51.013743 cerbos-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 10:10:11.032972 cerbos-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     1303 2023-07-14 10:10:11.032972 cerbos-0.9.0/tests/check.py
--rw-r--r--   0        0        0     4868 2023-07-14 10:10:11.032972 cerbos-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0     6496 2023-07-14 10:10:11.032972 cerbos-0.9.0/tests/grpc/test_grpc_admin_client.py
--rw-r--r--   0        0        0    16279 2023-07-14 10:10:11.032972 cerbos-0.9.0/tests/grpc/test_grpc_client.py
--rw-r--r--   0        0        0    20088 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/http/test_http_client.py
--rw-r--r--   0        0        0     2061 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/http/test_http_plan_response.py
--rw-r--r--   0        0        0      758 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/conf.yaml
--rw-r--r--   0        0        0      578 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/_schemas/leave_request.json
--rw-r--r--   0        0        0     1030 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/_schemas/principal.json
--rw-r--r--   0        0        0      402 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/_schemas/purchase_order.json
--rw-r--r--   0        0        0      387 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/_schemas/salary_record.json
--rw-r--r--   0        0        0      451 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/derived_roles/common_roles.yaml
--rw-r--r--   0        0        0      323 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/derived_roles/derived_roles_01.yaml
--rw-r--r--   0        0        0      492 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/derived_roles/derived_roles_02.yaml
--rw-r--r--   0        0        0      599 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/derived_roles/derived_roles_03.yaml
--rw-r--r--   0        0        0      118 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/export_variables/policy_01.yaml
--rw-r--r--   0        0        0      577 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/principal_policies/policy_01.yaml
--rw-r--r--   0        0        0      300 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/principal_policies/policy_02.yaml
--rw-r--r--   0        0        0      226 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/principal_policies/policy_02_acme.hr.yaml
--rw-r--r--   0        0        0      499 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/principal_policies/policy_02_acme.yaml
--rw-r--r--   0        0        0     2090 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_01.yaml
--rw-r--r--   0        0        0      624 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_02.yaml
--rw-r--r--   0        0        0      526 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_03.yaml
--rw-r--r--   0        0        0      710 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_04.yaml
--rw-r--r--   0        0        0      377 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_05.yaml
--rw-r--r--   0        0        0      704 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_05_acme.hr.uk.yaml
--rw-r--r--   0        0        0     1138 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_05_acme.hr.yaml
--rw-r--r--   0        0        0      535 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_05_acme.yaml
--rw-r--r--   0        0        0      450 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/tests/policy_04_test.yaml
--rw-r--r--   0        0        0     6987 1970-01-01 00:00:00.000000 cerbos-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 07:35:40.866376 cerbos-0.9.1/LICENSE
+-rw-r--r--   0        0        0     6175 2023-07-25 07:35:40.866376 cerbos-0.9.1/README.md
+-rw-r--r--   0        0        0      167 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/__init__.py
+-rw-r--r--   0        0        0     5052 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/audit/v1/audit_pb2.py
+-rw-r--r--   0        0        0     5463 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/audit/v1/audit_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/audit/v1/audit_pb2_grpc.py
+-rw-r--r--   0        0        0     1537 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/effect/v1/effect_pb2.py
+-rw-r--r--   0        0        0      541 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/effect/v1/effect_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/effect/v1/effect_pb2_grpc.py
+-rw-r--r--   0        0        0    24465 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/engine/v1/engine_pb2.py
+-rw-r--r--   0        0        0    18348 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/engine/v1/engine_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/engine/v1/engine_pb2_grpc.py
+-rw-r--r--   0        0        0    35452 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/policy/v1/policy_pb2.py
+-rw-r--r--   0        0        0    30998 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/policy/v1/policy_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/policy/v1/policy_pb2_grpc.py
+-rw-r--r--   0        0        0    40721 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/request/v1/request_pb2.py
+-rw-r--r--   0        0        0    14880 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/request/v1/request_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/request/v1/request_pb2_grpc.py
+-rw-r--r--   0        0        0    40197 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/response/v1/response_pb2.py
+-rw-r--r--   0        0        0    20863 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/response/v1/response_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/response/v1/response_pb2_grpc.py
+-rw-r--r--   0        0        0     3055 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/schema/v1/schema_pb2.py
+-rw-r--r--   0        0        0     1614 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/schema/v1/schema_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/schema/v1/schema_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/sdk/_async/__init__.py
+-rw-r--r--   0        0        0    24037 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/sdk/_async/_grpc.py
+-rw-r--r--   0        0        0    12739 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/sdk/_async/_http.py
+-rw-r--r--   0        0        0        0 2023-07-25 07:36:27.574909 cerbos-0.9.1/cerbos/sdk/_sync/__init__.py
+-rw-r--r--   0        0        0    23695 2023-07-25 07:36:28.746922 cerbos-0.9.1/cerbos/sdk/_sync/_grpc.py
+-rw-r--r--   0        0        0    12551 2023-07-25 07:36:27.574909 cerbos-0.9.1/cerbos/sdk/_sync/_http.py
+-rw-r--r--   0        0        0      481 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/sdk/client.py
+-rw-r--r--   0        0        0      881 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/sdk/container.py
+-rw-r--r--   0        0        0      491 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/sdk/grpc/client.py
+-rw-r--r--   0        0        0      702 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/sdk/grpc/utils.py
+-rw-r--r--   0        0        0      106 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/sdk/http/client.py
+-rw-r--r--   0        0        0     6501 2023-07-25 07:35:40.866376 cerbos-0.9.1/cerbos/sdk/model.py
+-rw-r--r--   0        0        0    14057 2023-07-25 07:35:40.870375 cerbos-0.9.1/cerbos/svc/v1/svc_pb2.py
+-rw-r--r--   0        0        0      449 2023-07-25 07:35:40.870375 cerbos-0.9.1/cerbos/svc/v1/svc_pb2.pyi
+-rw-r--r--   0        0        0    38288 2023-07-25 07:35:40.870375 cerbos-0.9.1/cerbos/svc/v1/svc_pb2_grpc.py
+-rw-r--r--   0        0        0     9422 2023-07-25 07:35:40.870375 cerbos-0.9.1/cerbos/telemetry/v1/telemetry_pb2.py
+-rw-r--r--   0        0        0    10796 2023-07-25 07:35:40.870375 cerbos-0.9.1/cerbos/telemetry/v1/telemetry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.870375 cerbos-0.9.1/cerbos/telemetry/v1/telemetry_pb2_grpc.py
+-rw-r--r--   0        0        0     1608 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      310 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     7881 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/expr/v1alpha1/checked_pb2.py
+-rw-r--r--   0        0        0     9298 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/expr/v1alpha1/checked_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/expr/v1alpha1/checked_pb2_grpc.py
+-rw-r--r--   0        0        0     8118 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/expr/v1alpha1/syntax_pb2.py
+-rw-r--r--   0        0        0     9130 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/expr/v1alpha1/syntax_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/expr/v1alpha1/syntax_pb2_grpc.py
+-rw-r--r--   0        0        0     1956 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/field_behavior_pb2.py
+-rw-r--r--   0        0        0     1036 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/field_behavior_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/field_behavior_pb2_grpc.py
+-rw-r--r--   0        0        0     2426 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/http_pb2.py
+-rw-r--r--   0        0        0     2272 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0     3183 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/visibility_pb2.py
+-rw-r--r--   0        0        0     1536 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/visibility_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.870375 cerbos-0.9.1/google/api/visibility_pb2_grpc.py
+-rw-r--r--   0        0        0     2712 2023-07-25 07:35:40.870375 cerbos-0.9.1/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0        0        0      730 2023-07-25 07:35:40.870375 cerbos-0.9.1/protoc_gen_openapiv2/options/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.870375 cerbos-0.9.1/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0    19672 2023-07-25 07:35:40.870375 cerbos-0.9.1/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0        0        0    23802 2023-07-25 07:35:40.870375 cerbos-0.9.1/protoc_gen_openapiv2/options/openapiv2_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.870375 cerbos-0.9.1/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
+-rw-r--r--   0        0        0     2804 2023-07-25 07:36:30.786944 cerbos-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 07:35:40.870375 cerbos-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     1303 2023-07-25 07:35:40.870375 cerbos-0.9.1/tests/check.py
+-rw-r--r--   0        0        0     4868 2023-07-25 07:35:40.870375 cerbos-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0     6496 2023-07-25 07:35:40.870375 cerbos-0.9.1/tests/grpc/test_grpc_admin_client.py
+-rw-r--r--   0        0        0    16279 2023-07-25 07:35:40.870375 cerbos-0.9.1/tests/grpc/test_grpc_client.py
+-rw-r--r--   0        0        0    20088 2023-07-25 07:35:40.870375 cerbos-0.9.1/tests/http/test_http_client.py
+-rw-r--r--   0        0        0     2061 2023-07-25 07:35:40.870375 cerbos-0.9.1/tests/http/test_http_plan_response.py
+-rw-r--r--   0        0        0      758 2023-07-25 07:35:40.870375 cerbos-0.9.1/tests/store/conf.yaml
+-rw-r--r--   0        0        0      578 2023-07-25 07:35:40.870375 cerbos-0.9.1/tests/store/policies/_schemas/leave_request.json
+-rw-r--r--   0        0        0     1030 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/_schemas/principal.json
+-rw-r--r--   0        0        0      402 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/_schemas/purchase_order.json
+-rw-r--r--   0        0        0      387 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/_schemas/salary_record.json
+-rw-r--r--   0        0        0      451 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/derived_roles/common_roles.yaml
+-rw-r--r--   0        0        0      323 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/derived_roles/derived_roles_01.yaml
+-rw-r--r--   0        0        0      492 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/derived_roles/derived_roles_02.yaml
+-rw-r--r--   0        0        0      599 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/derived_roles/derived_roles_03.yaml
+-rw-r--r--   0        0        0      118 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/export_variables/policy_01.yaml
+-rw-r--r--   0        0        0      577 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/principal_policies/policy_01.yaml
+-rw-r--r--   0        0        0      300 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/principal_policies/policy_02.yaml
+-rw-r--r--   0        0        0      226 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/principal_policies/policy_02_acme.hr.yaml
+-rw-r--r--   0        0        0      499 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/principal_policies/policy_02_acme.yaml
+-rw-r--r--   0        0        0     2090 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/resource_policies/policy_01.yaml
+-rw-r--r--   0        0        0      624 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/resource_policies/policy_02.yaml
+-rw-r--r--   0        0        0      526 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/resource_policies/policy_03.yaml
+-rw-r--r--   0        0        0      710 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/resource_policies/policy_04.yaml
+-rw-r--r--   0        0        0      377 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/resource_policies/policy_05.yaml
+-rw-r--r--   0        0        0      704 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/resource_policies/policy_05_acme.hr.uk.yaml
+-rw-r--r--   0        0        0     1138 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/resource_policies/policy_05_acme.hr.yaml
+-rw-r--r--   0        0        0      535 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/resource_policies/policy_05_acme.yaml
+-rw-r--r--   0        0        0      450 2023-07-25 07:35:40.874376 cerbos-0.9.1/tests/store/policies/tests/policy_04_test.yaml
+-rw-r--r--   0        0        0    15874 2023-07-25 07:35:40.874376 cerbos-0.9.1/validate/validate_pb2.py
+-rw-r--r--   0        0        0    23076 2023-07-25 07:35:40.874376 cerbos-0.9.1/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-25 07:35:40.874376 cerbos-0.9.1/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0     6987 1970-01-01 00:00:00.000000 cerbos-0.9.1/PKG-INFO
```

### Comparing `cerbos-0.9.0/LICENSE` & `cerbos-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/README.md` & `cerbos-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/audit/v1/audit_pb2.py` & `cerbos-0.9.1/cerbos/audit/v1/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/audit/v1/audit_pb2.pyi` & `cerbos-0.9.1/cerbos/audit/v1/audit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/effect/v1/effect_pb2.py` & `cerbos-0.9.1/cerbos/effect/v1/effect_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/effect/v1/effect_pb2.pyi` & `cerbos-0.9.1/cerbos/effect/v1/effect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/engine/v1/engine_pb2.py` & `cerbos-0.9.1/cerbos/engine/v1/engine_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/engine/v1/engine_pb2.pyi` & `cerbos-0.9.1/cerbos/engine/v1/engine_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/policy/v1/policy_pb2.py` & `cerbos-0.9.1/cerbos/policy/v1/policy_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/policy/v1/policy_pb2.pyi` & `cerbos-0.9.1/cerbos/policy/v1/policy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/request/v1/request_pb2.py` & `cerbos-0.9.1/cerbos/request/v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/request/v1/request_pb2.pyi` & `cerbos-0.9.1/cerbos/request/v1/request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/response/v1/response_pb2.py` & `cerbos-0.9.1/cerbos/response/v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/response/v1/response_pb2.pyi` & `cerbos-0.9.1/cerbos/response/v1/response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/schema/v1/schema_pb2.py` & `cerbos-0.9.1/cerbos/schema/v1/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/schema/v1/schema_pb2.pyi` & `cerbos-0.9.1/cerbos/schema/v1/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/sdk/_async/_grpc.py` & `cerbos-0.9.1/cerbos/sdk/_async/_grpc.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/sdk/_async/_http.py` & `cerbos-0.9.1/cerbos/sdk/_async/_http.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/sdk/_sync/_grpc.py` & `cerbos-0.9.1/cerbos/sdk/_sync/_grpc.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/sdk/_sync/_http.py` & `cerbos-0.9.1/cerbos/sdk/_sync/_http.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/sdk/container.py` & `cerbos-0.9.1/cerbos/sdk/container.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/sdk/grpc/utils.py` & `cerbos-0.9.1/cerbos/sdk/grpc/utils.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/sdk/model.py` & `cerbos-0.9.1/cerbos/sdk/model.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/svc/v1/svc_pb2.py` & `cerbos-0.9.1/cerbos/svc/v1/svc_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/svc/v1/svc_pb2_grpc.py` & `cerbos-0.9.1/cerbos/svc/v1/svc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/telemetry/v1/telemetry_pb2.py` & `cerbos-0.9.1/cerbos/telemetry/v1/telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/cerbos/telemetry/v1/telemetry_pb2.pyi` & `cerbos-0.9.1/cerbos/telemetry/v1/telemetry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/pyproject.toml` & `cerbos-0.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "httpx[http2]>=0.22.0",
     "anyio>=3.6.1",
     "tenacity>=8.1.0",
     "grpcio-tools>=1.54.2",
 ]
 requires-python = ">=3.8"
 dynamic = []
-version = "0.9.0"
+version = "0.9.1"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Homepage = "https://cerbos.dev"
 
@@ -48,14 +48,22 @@
 tools = [
     "unasync>=0.5.0",
     "setuptools>=63.2.0",
     "commitizen>=3.2.2",
     "ptpython>=3.0.23",
 ]
 
+[tool.pdm.build]
+includes = [
+    "cerbos/",
+    "google/",
+    "protoc_gen_openapiv2/",
+    "validate/",
+]
+
 [tool.pdm.scripts.isort]
 cmd = "isort cerbos/sdk tests"
 
 [tool.pdm.scripts.black]
 cmd = "black cerbos/sdk tests"
 
 [tool.pdm.scripts.format]
```

### Comparing `cerbos-0.9.0/tests/check.py` & `cerbos-0.9.1/tests/check.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/conftest.py` & `cerbos-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/grpc/test_grpc_admin_client.py` & `cerbos-0.9.1/tests/grpc/test_grpc_admin_client.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/grpc/test_grpc_client.py` & `cerbos-0.9.1/tests/grpc/test_grpc_client.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/http/test_http_client.py` & `cerbos-0.9.1/tests/http/test_http_client.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/http/test_http_plan_response.py` & `cerbos-0.9.1/tests/http/test_http_plan_response.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/store/conf.yaml` & `cerbos-0.9.1/tests/store/conf.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/store/policies/_schemas/leave_request.json` & `cerbos-0.9.1/tests/store/policies/_schemas/leave_request.json`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/store/policies/_schemas/principal.json` & `cerbos-0.9.1/tests/store/policies/_schemas/principal.json`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/store/policies/derived_roles/derived_roles_03.yaml` & `cerbos-0.9.1/tests/store/policies/derived_roles/derived_roles_03.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/store/policies/principal_policies/policy_01.yaml` & `cerbos-0.9.1/tests/store/policies/principal_policies/policy_01.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/store/policies/resource_policies/policy_01.yaml` & `cerbos-0.9.1/tests/store/policies/resource_policies/policy_01.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/store/policies/resource_policies/policy_02.yaml` & `cerbos-0.9.1/tests/store/policies/resource_policies/policy_02.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/store/policies/resource_policies/policy_03.yaml` & `cerbos-0.9.1/tests/store/policies/resource_policies/policy_03.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/store/policies/resource_policies/policy_04.yaml` & `cerbos-0.9.1/tests/store/policies/resource_policies/policy_04.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/store/policies/resource_policies/policy_05_acme.hr.uk.yaml` & `cerbos-0.9.1/tests/store/policies/resource_policies/policy_05_acme.hr.uk.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/store/policies/resource_policies/policy_05_acme.hr.yaml` & `cerbos-0.9.1/tests/store/policies/resource_policies/policy_05_acme.hr.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/tests/store/policies/resource_policies/policy_05_acme.yaml` & `cerbos-0.9.1/tests/store/policies/resource_policies/policy_05_acme.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.9.0/PKG-INFO` & `cerbos-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbos
-Version: 0.9.0
+Version: 0.9.1
 Summary: SDK for working with Cerbos: an open core, language-agnostic, scalable authorization solution
 Author-Email: Cerbos Developers <sdk+python@cerbos.dev>
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
```

