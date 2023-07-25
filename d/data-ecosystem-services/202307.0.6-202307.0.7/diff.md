# Comparing `tmp/data_ecosystem_services-202307.0.6.tar.gz` & `tmp/data_ecosystem_services-202307.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_services-202307.0.6.tar", max compression
+gzip compressed data, was "data_ecosystem_services-202307.0.7.tar", max compression
```

## Comparing `data_ecosystem_services-202307.0.6.tar` & `data_ecosystem_services-202307.0.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      918 2023-07-24 15:19:54.886852 data_ecosystem_services-202307.0.6/data_ecosystem_services/__main__.py
--rw-r--r--   0        0        0     1264 2023-07-24 15:19:54.886852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/__init__.py
--rw-r--r--   0        0        0     5030 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/column.py
--rw-r--r--   0        0        0    25117 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/customfieldsendpoint.py
--rw-r--r--   0        0        0    13816 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/datasource.py
--rw-r--r--   0        0        0     2037 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/endpoint.py
--rw-r--r--   0        0        0    11758 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/excelmetadata.py
--rw-r--r--   0        0        0      566 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/execution_session.py
--rw-r--r--   0        0        0     7568 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/idfinderendpoint.py
--rw-r--r--   0        0        0    16676 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/manifest.py
--rw-r--r--   0        0        0    10973 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/query.py
--rw-r--r--   0        0        0    55031 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/schema.py
--rw-r--r--   0        0        0     7368 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/table.py
--rw-r--r--   0        0        0     1486 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/tagsendpoint.py
--rw-r--r--   0        0        0    25982 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/tokenendpoint.py
--rw-r--r--   0        0        0     1044 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_client_service/__init__.py
--rw-r--r--   0        0        0       41 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_client_service/az_client.py
--rw-r--r--   0        0        0     4570 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_client_service/azd_client.py
--rw-r--r--   0        0        0     1050 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_key_vault_service/__init__.py
--rw-r--r--   0        0        0     8967 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_key_vault_service/az_key_vault.py
--rw-r--r--   0        0        0     1073 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_storage_service/__init__.py
--rw-r--r--   0        0        0     2665 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_storage_service/az_storage_queue.py
--rw-r--r--   0        0        0     1024 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_admin_service/__init__.py
--rw-r--r--   0        0        0    15940 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_admin_service/environment_logging.py
--rw-r--r--   0        0        0     8398 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_admin_service/environment_tracing.py
--rw-r--r--   0        0        0     1013 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_security_service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_security_service/security_base64.py
--rw-r--r--   0        0        0    21410 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_security_service/security_core.py
--rw-r--r--   0        0        0     1175 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/__init__.py
--rw-r--r--   0        0        0    42751 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/dataset_metadata.py
--rw-r--r--   0        0        0    40188 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/environment_metadata.py
--rw-r--r--   0        0        0    36068 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/job_metadata.py
--rw-r--r--   0        0        0     2254 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/logging_metadata.py
--rw-r--r--   0        0        0    22352 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/pipeline_metadata.py
--rw-r--r--   0        0        0     1727 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/__init__.py
--rw-r--r--   0        0        0    33787 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py
--rw-r--r--   0        0        0     8962 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py
--rw-r--r--   0        0        0    25880 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py
--rw-r--r--   0        0        0     3825 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py
--rw-r--r--   0        0        0     3949 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_core.py
--rw-r--r--   0        0        0    50039 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_file.py
--rw-r--r--   0        0        0     5323 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_http.py
--rw-r--r--   0        0        0     4903 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py
--rw-r--r--   0        0        0     4648 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/job_core.py
--rw-r--r--   0        0        0    17832 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/repo_core.py
--rw-r--r--   0        0        0     8956 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/directory_paths.txt
--rw-r--r--   0        0        0      827 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/github_service/__init__.py
--rw-r--r--   0        0        0     7250 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/github_service/github_secret.py
--rw-r--r--   0        0        0     1707 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/jira_service/__init__.py
--rw-r--r--   0        0        0     6295 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/jira_service/jira_client.py
--rw-r--r--   0        0        0       44 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/output.txt
--rw-r--r--   0        0        0      869 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/posit_service/__init__.py
--rw-r--r--   0        0        0    21086 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/posit_service/posit_connect.py
--rw-r--r--   0        0        0      825 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/python_service/__init__.py
--rw-r--r--   0        0        0       24 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/python_service/python_client.py
--rw-r--r--   0        0        0    15021 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/requirements.txt
--rw-r--r--   0        0        0      832 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/windows_service/__init__.py
--rw-r--r--   0        0        0     2499 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/windows_service/windows_credential.py
--rw-r--r--   0        0        0    11357 2023-07-24 15:19:54.898852 data_ecosystem_services-202307.0.6/license.md
--rw-r--r--   0        0        0     3914 2023-07-24 15:22:32.315117 data_ecosystem_services-202307.0.6/pyproject.toml
--rw-r--r--   0        0        0    52428 2023-07-24 15:19:54.898852 data_ecosystem_services-202307.0.6/readme.md
--rw-r--r--   0        0        0      129 2023-07-24 15:19:54.898852 data_ecosystem_services-202307.0.6/setup.cfg
--rw-r--r--   0        0        0      127 2023-07-24 15:19:54.898852 data_ecosystem_services-202307.0.6/setup.py
--rw-r--r--   0        0        0    55938 1970-01-01 00:00:00.000000 data_ecosystem_services-202307.0.6/PKG-INFO
+-rw-r--r--   0        0        0      918 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/__main__.py
+-rw-r--r--   0        0        0     1264 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/__init__.py
+-rw-r--r--   0        0        0     5030 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/column.py
+-rw-r--r--   0        0        0    25117 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/customfieldsendpoint.py
+-rw-r--r--   0        0        0    13816 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/datasource.py
+-rw-r--r--   0        0        0     2037 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/endpoint.py
+-rw-r--r--   0        0        0    13626 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/excelmetadata.py
+-rw-r--r--   0        0        0      566 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/execution_session.py
+-rw-r--r--   0        0        0     7568 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/idfinderendpoint.py
+-rw-r--r--   0        0        0    16676 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/manifest.py
+-rw-r--r--   0        0        0    10973 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/query.py
+-rw-r--r--   0        0        0    55259 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/schema.py
+-rw-r--r--   0        0        0     7368 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/table.py
+-rw-r--r--   0        0        0     1486 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/tagsendpoint.py
+-rw-r--r--   0        0        0    25982 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/tokenendpoint.py
+-rw-r--r--   0        0        0     1044 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/az_client_service/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/az_client_service/az_client.py
+-rw-r--r--   0        0        0     4570 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/az_client_service/azd_client.py
+-rw-r--r--   0        0        0     1050 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/az_key_vault_service/__init__.py
+-rw-r--r--   0        0        0     8967 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/az_key_vault_service/az_key_vault.py
+-rw-r--r--   0        0        0     1073 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/az_storage_service/__init__.py
+-rw-r--r--   0        0        0     2665 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/az_storage_service/az_storage_queue.py
+-rw-r--r--   0        0        0     1024 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_admin_service/__init__.py
+-rw-r--r--   0        0        0    15940 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_admin_service/environment_logging.py
+-rw-r--r--   0        0        0     8398 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_admin_service/environment_tracing.py
+-rw-r--r--   0        0        0     1013 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_security_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_security_service/security_base64.py
+-rw-r--r--   0        0        0    21410 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_security_service/security_core.py
+-rw-r--r--   0        0        0     1175 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_self_service/__init__.py
+-rw-r--r--   0        0        0    42751 2023-07-25 18:51:15.270629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_self_service/dataset_metadata.py
+-rw-r--r--   0        0        0    40188 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_self_service/environment_metadata.py
+-rw-r--r--   0        0        0    36068 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_self_service/job_metadata.py
+-rw-r--r--   0        0        0     2254 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_self_service/logging_metadata.py
+-rw-r--r--   0        0        0    22352 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_self_service/pipeline_metadata.py
+-rw-r--r--   0        0        0     1727 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/__init__.py
+-rw-r--r--   0        0        0    33787 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py
+-rw-r--r--   0        0        0     8962 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py
+-rw-r--r--   0        0        0    25880 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py
+-rw-r--r--   0        0        0     3825 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py
+-rw-r--r--   0        0        0     3949 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/environment_core.py
+-rw-r--r--   0        0        0    50039 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/environment_file.py
+-rw-r--r--   0        0        0     5323 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/environment_http.py
+-rw-r--r--   0        0        0     4903 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py
+-rw-r--r--   0        0        0     4648 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/job_core.py
+-rw-r--r--   0        0        0    17832 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/repo_core.py
+-rw-r--r--   0        0        0     8956 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/directory_paths.txt
+-rw-r--r--   0        0        0      827 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/github_service/__init__.py
+-rw-r--r--   0        0        0     7250 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/github_service/github_secret.py
+-rw-r--r--   0        0        0     1707 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/jira_service/__init__.py
+-rw-r--r--   0        0        0     6295 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/jira_service/jira_client.py
+-rw-r--r--   0        0        0       44 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/output.txt
+-rw-r--r--   0        0        0      869 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/posit_service/__init__.py
+-rw-r--r--   0        0        0    21050 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/posit_service/posit_connect.py
+-rw-r--r--   0        0        0      825 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/python_service/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/python_service/python_client.py
+-rw-r--r--   0        0        0    15021 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/requirements.txt
+-rw-r--r--   0        0        0      832 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/windows_service/__init__.py
+-rw-r--r--   0        0        0     2499 2023-07-25 18:51:15.274629 data_ecosystem_services-202307.0.7/data_ecosystem_services/windows_service/windows_credential.py
+-rw-r--r--   0        0        0    11357 2023-07-25 18:51:15.278629 data_ecosystem_services-202307.0.7/license.md
+-rw-r--r--   0        0        0     3914 2023-07-25 18:54:10.792473 data_ecosystem_services-202307.0.7/pyproject.toml
+-rw-r--r--   0        0        0    52428 2023-07-25 18:51:15.278629 data_ecosystem_services-202307.0.7/readme.md
+-rw-r--r--   0        0        0      129 2023-07-25 18:51:15.282629 data_ecosystem_services-202307.0.7/setup.cfg
+-rw-r--r--   0        0        0      127 2023-07-25 18:51:15.282629 data_ecosystem_services-202307.0.7/setup.py
+-rw-r--r--   0        0        0    55938 1970-01-01 00:00:00.000000 data_ecosystem_services-202307.0.7/PKG-INFO
```

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/__main__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/__main__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/column.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/column.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/customfieldsendpoint.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/customfieldsendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/datasource.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/datasource.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/endpoint.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/endpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/excelmetadata.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/excelmetadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,42 @@
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
 TIMEOUT_ONE_MIN = 60  # or set to whatever value you want
 
 
 class ExcelMetadata:
+    """
+    This class encapsulates the functionalities to generate Excel file data for a given Alation schema ID and 
+    configuration, and to create an Excel file using the data generated.
+
+    The class includes the following methods:
+    - convert_dict_to_csv: A static method that takes a dictionary as input and converts it to a string 
+      representation in the CSV format.
+    - generate_excel_file_data: A class method that generates data for an Excel file given a Alation schema ID 
+      and configuration. It uses data from Alation and builds DataFrames to represent the schema and table data. 
+      It returns a tuple containing the DataFrame containing the schema data, the DataFrame containing the 
+      table data, and the filename of the generated Excel file.
+    - generate_excel_file_from_data: A class method that generates an Excel file using DataFrame objects and 
+      saves it.
+
+    This class is typically used in scenarios where data from an Alation schema needs to be exported as an Excel file 
+    for further analysis or manipulation. The Excel file created includes two sheets, namely 'Instructions' 
+    and 'Tables', which hold the schema and table data respectively.
+
+    Note:
+    - The generate_excel_file_data method assumes the existence of an `alation_schema` module with a `Schema` class.
+    - This method relies on external logging and tracing modules (`logger_singleton` and `tracer_singleton`) that 
+      are not provided here.
+    - The configuration dictionary (`config`) is expected to contain specific keys such as 'repository_path', 
+      'environment', 'edc_alation_user_id', 'edc_alation_base_url', etc.
+    - The methods make use of the `pd.DataFrame` function from the `pandas` library to create DataFrames.
+    - The generate_excel_file_from_data method uses the xlsxwriter library to create and manipulate the Excel file.
+    - The get_column_letter function is assumed to be imported from the openpyxl.utils module.
+    """
 
     @staticmethod
     def convert_dict_to_csv(dictionary):
 
         return 'UNSUPPORTED LIST'
 
         if isinstance(dictionary, dict):
@@ -73,15 +101,14 @@
         from data_ecosystem_services.alation_service import (
             schema as alation_schema
         )
         schema = alation_schema.Schema()
 
         logger_singleton = pade_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
-        logger = logger_singleton.get_logger()
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         schema_id = alation_schema_id
         schema_name = None
 
@@ -104,34 +131,32 @@
                     f"api_refresh_token_length: {str(len(api_refresh_token))}")
                 assert status_code == 200
 
                 # Get Datasource and Schema Results
                 schema_result, datasource_result = schema.get_schema(
                     edc_alation_api_token, edc_alation_base_url, schema_id)
 
-                alation_data_source_id = schema_result.get("ds_id")
+                schema_result_json = schema_result.json()
+                alation_data_source_id = schema_result_json[0].get("ds_id")
 
-            except Exception as ex:
-                error_msg = "Error: {str(ex)}",
+            except Exception as ex_generic:
+                error_msg = str(ex_generic),
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
             # Pandas Dataframe
             try:
                 # Get Table Results
                 table_result = schema.get_schema_tables(
                     edc_alation_api_token, edc_alation_base_url, alation_data_source_id, alation_schema_id)
 
-                # log results
-                logger.info(f"schema_result length: {len(schema_result)}")
-                logger.info(
-                    f"datasource_result length: {len(datasource_result)}")
+                schema_result_json = schema_result.json()
+                schema_name = schema_result_json[0].get("name")
 
-                schema_name = schema_result.get("name")
                 datasource_title = datasource_result.get("title")
 
                 # Create dictionaries
                 simple_dict = {i: (k, v) for i, (k, v) in enumerate(
                     schema_result.items()) if not isinstance(v, list) and not isinstance(v, dict)}
                 custom_dict = schema_result['custom_fields']
```

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/execution_session.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/execution_session.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/idfinderendpoint.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/idfinderendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/manifest.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/manifest.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/query.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/query.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/schema.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -575,22 +575,25 @@
                     raise ValueError(msg)
 
                 # Get the schema and datasource details
                 schema_result, datasource_result = cls.get_schema(
                     edc_alation_api_token, edc_alation_base_url, schema_id
                 )
 
+                schema_result_json = schema_result.json()
+
                 # Set the schema name, datasource title and datasource_id
-                schema_name = schema_result.get("name")
+                schema_name = schema_result_json[0].get("name")
                 datasource_title = datasource_result.get("title")
                 datasource_id = datasource_result.get("id")
                 alation_data_source_id = datasource_id
 
                 # Log the schema details
-                logger.info(f"schema_result length: {str(len(schema_result))}")
+                logger.info(
+                    f"schema_result length: {str(len(schema_result_json))}")
                 logger.info(
                     f"datasource_result length: {str(len(datasource_result))}")
 
                 # Get the schema manifest
                 msg = f"Loading manifest schema from {schema_file_path}"
                 logger.info(msg)
                 manifest = Manifest(schema_file_path)
@@ -691,15 +694,16 @@
                     raise ValueError(msg)
 
                 # Get the schema and datasource information
                 schema_results, datasource_results = cls.get_schema(
                     edc_alation_api_token, edc_alation_base_url, alation_schema_id
                 )
 
-                schema_name = schema_results.get("name")
+                schema_result_json = schema_results.json()
+                schema_name = schema_result_json[0].get("name")
                 datasource_title = datasource_results.get("title")
                 alation_data_source_id = datasource_results.get("id")
 
                 # Get the manifest file name
                 manifest_json_file = cls.get_manifest_json_file_name(
                     "upload", repository_path, datasource_title, schema_name, environment, alation_user_id)
 
@@ -1084,18 +1088,19 @@
                 NAMESPACE_NAME, SERVICE_NAME)
             logger = logger_singleton.get_logger()
             tracer_singleton = pade_env_tracing.TracerSingleton.instance(
                 NAMESPACE_NAME, SERVICE_NAME)
             tracer = tracer_singleton.get_tracer()
 
             with tracer.start_as_current_span("get_schema_structure"):
-                response_json = None
+                schema_result_json = None
                 try:
-                    response_schema_json = cls.get_schema(
+                    schema_result, datasource_result = cls.get_schema(
                         edc_alation_api_token, edc_alation_base_url, alation_schema_id)
+                    schema_result_json = schema_result.json()
                 except requests.exceptions.RequestException as ex_r:
                     error_msg = "Error in requests: %s", str(ex_r)
                     exc_info = sys.exc_info()
                     logger_singleton.error_with_exception(error_msg, exc_info)
                     raise
                 except Exception as ex_:
                     error_msg = "Error: %s", str(ex_)
@@ -1105,15 +1110,15 @@
 
                 logger.info(f'Info for schema ID: {alation_schema_id}')
                 found_schema = False
                 schema_fields, expected_table_fields, expected_column_fields, required_table_fields = manifest.get_manifest_expected_fields()
                 manifest_dict = {}
                 manifest_dict['tables'] = []
 
-                for schema in response_schema_json:
+                for schema in schema_result_json:
                     logger.info(f"schema_id: {str(schema['id'])}")
                     if schema['id'] == int(alation_schema_id):
                         found_schema = True
 
                         schema_name = schema['name']
                         logger.info(
                             f"Found the desired schema with name: {schema_name}")
@@ -1171,11 +1176,11 @@
                     error_msg = "Could not find the schema ID in the list of schemas for this data source"
                     raise EdcAlationError(error_msg)
 
                 # Create a JSON structure containing the schema, tables, and columns
                 return manifest_dict
 
         except Exception as ex:
-            error_msg = "Error: %s", ex
+            error_msg = str(ex)
             exc_info = sys.exc_info()
             logger_singleton.error_with_exception(error_msg, exc_info)
             raise EdcAlationError(error_msg) from ex
```

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/table.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/table.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/tagsendpoint.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/tagsendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/tokenendpoint.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/alation_service/tokenendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/az_client_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/az_client_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/az_client_service/azd_client.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/az_client_service/azd_client.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/az_key_vault_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/az_key_vault_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/az_key_vault_service/az_key_vault.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/az_key_vault_service/az_key_vault.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/az_storage_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/az_storage_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/az_storage_service/az_storage_queue.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/az_storage_service/az_storage_queue.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_admin_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_admin_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_admin_service/environment_logging.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_admin_service/environment_logging.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_admin_service/environment_tracing.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_admin_service/environment_tracing.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_security_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_security_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_security_service/security_core.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_security_service/security_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_self_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/dataset_metadata.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_self_service/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/environment_metadata.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_self_service/environment_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/job_metadata.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_self_service/job_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/logging_metadata.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_self_service/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/pipeline_metadata.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_self_service/pipeline_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_core.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/environment_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_file.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/environment_file.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_http.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/environment_http.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/job_core.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/job_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/repo_core.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/cdc_tech_environment_service/repo_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/directory_paths.txt` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/directory_paths.txt`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/github_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/github_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/github_service/github_secret.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/github_service/github_secret.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/jira_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/jira_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/jira_service/jira_client.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/jira_service/jira_client.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/posit_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/posit_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/posit_service/posit_connect.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/posit_service/posit_connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         with tracer.start_as_current_span("publish_app"):
 
             if posit_connect_base_url.endswith('/'):
                 posit_connect_base_url = posit_connect_base_url[:-1]
 
             api_url = f"{posit_connect_base_url}/__api__/v1/content"
             headers = {"Authorization": f"Key {api_key}"}
-            data = open(app_manifest_file, "rb", encoding="utf-8").read()
+            data = open(app_manifest_file, "rb").read()
             response = requests.post(api_url, headers=headers, data=data)
 
             # If the request was successful, status_code will be 200
             status_code = response.status_code
 
             # If the request was successful, status_code will be 200
             logger.info(f"response.status_code: {response.status_code}")
@@ -189,15 +189,15 @@
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("generate_manifest"):
 
             # Load the Swagger JSON file
-            with open(swagger_file, "rb", encoding="utf-8") as swagger_file_handle:
+            with open(swagger_file, "rb") as swagger_file_handle:
                 swagger = json.load(swagger_file_handle)
 
             logger.info(f"swagger_length: {len(swagger)}")
 
             # Load the requirements file
             with open(requirements_file, "r", encoding="utf-8") as requirements_file_handle:
                 requirements = [requirements_file_line.strip(
```

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/python_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/python_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/requirements.txt` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/requirements.txt`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/windows_service/__init__.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/windows_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/data_ecosystem_services/windows_service/windows_credential.py` & `data_ecosystem_services-202307.0.7/data_ecosystem_services/windows_service/windows_credential.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/license.md` & `data_ecosystem_services-202307.0.7/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/pyproject.toml` & `data_ecosystem_services-202307.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name="data_ecosystem_services"
-version="202307.0.6"
+version="202307.0.7"
 description="Program Agnostic Data Ecosystem (PADE) - Python Services"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
```

### Comparing `data_ecosystem_services-202307.0.6/readme.md` & `data_ecosystem_services-202307.0.7/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.6/PKG-INFO` & `data_ecosystem_services-202307.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-services
-Version: 202307.0.6
+Version: 202307.0.7
 Summary: Program Agnostic Data Ecosystem (PADE) - Python Services
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

