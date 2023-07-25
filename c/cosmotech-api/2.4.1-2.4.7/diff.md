# Comparing `tmp/cosmotech-api-2.4.1.tar.gz` & `tmp/cosmotech-api-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmotech-api-2.4.1.tar", last modified: Mon May 15 13:16:26 2023, max compression
+gzip compressed data, was "cosmotech-api-2.4.7.tar", last modified: Tue Jul 25 07:44:22 2023, max compression
```

## Comparing `cosmotech-api-2.4.1.tar` & `cosmotech-api-2.4.7.tar`

### file list

```diff
@@ -1,196 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.514235 cosmotech-api-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-15 13:16:26.514235 cosmotech-api-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34808 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.474233 cosmotech-api-2.4.1/cosmotech_api/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.478233 cosmotech-api-2.4.1/cosmotech_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/connector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    54209 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    92967 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/organization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   135369 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/scenario_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    83628 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/scenariorun_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    89628 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/solution_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    85025 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/twingraph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46553 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    48795 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/validator_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   110595 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api/workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37653 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.478233 cosmotech-api-2.4.1/cosmotech_api/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.490234 cosmotech-api-2.4.1/cosmotech_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/component_role_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/connector_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/connector_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/container_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/container_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/dataset_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/dataset_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/dataset_copy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/dataset_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/delete_historical_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/graph_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/organization_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template_handler_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    13435 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/run_template_step_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    19748 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_changed_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_data_download_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_data_download_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_job_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_last_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_container_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_container_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13660 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_status_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/scenario_validation_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/source_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/translated_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_import_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/user_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11574 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/user_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/validator_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model/workspace_web_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    82071 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.490234 cosmotech-api-2.4.1/cosmotech_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/cosmotech_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.474233 cosmotech-api-2.4.1/cosmotech_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-15 13:16:26.000000 cosmotech-api-2.4.1/cosmotech_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-15 13:16:26.000000 cosmotech-api-2.4.1/cosmotech_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:16:26.000000 cosmotech-api-2.4.1/cosmotech_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 13:16:26.000000 cosmotech-api-2.4.1/cosmotech_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 13:16:26.000000 cosmotech-api-2.4.1/cosmotech_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 13:16:26.514235 cosmotech-api-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:16:26.514235 cosmotech-api-2.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_component_role_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_connector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_connector_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_connector_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_container_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_container_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_dataset_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_dataset_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_dataset_copy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_dataset_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_delete_historical_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_graph_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_role.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_security.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_organization_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template_handler_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_run_template_step_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_changed_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_data_download_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_data_download_job.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_job_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_last_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_container.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_container_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_container_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_status_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_security.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenario_validation_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_scenariorun_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_solution_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_source_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_translated_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_twin_graph_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_twin_graph_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_twin_graph_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_twin_graph_import_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_twin_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_twingraph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_user_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_user_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_validator_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_validator_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_role.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_security.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 13:16:15.000000 cosmotech-api-2.4.1/test/test_workspace_web_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:22.879818 cosmotech-api-2.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-25 07:44:22.879818 cosmotech-api-2.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34828 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:22.851817 cosmotech-api-2.4.7/cosmotech_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:22.855818 cosmotech-api-2.4.7/cosmotech_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24323 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/api/connector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54208 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/api/dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92966 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/api/organization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135368 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/api/scenario_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83627 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/api/scenariorun_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89627 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/api/solution_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85054 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/api/twingraph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46562 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48794 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/api/validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110594 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/api/workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37652 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:22.855818 cosmotech-api-2.4.7/cosmotech_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:22.867818 cosmotech-api-2.4.7/cosmotech_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/component_role_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/connector_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/connector_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/container_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/container_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/dataset_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/dataset_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/dataset_copy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/dataset_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/delete_historical_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/graph_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/organization_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/organization_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/organization_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/organization_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22525 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/run_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/run_template_handler_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/run_template_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/run_template_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/run_template_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/run_template_step_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19747 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_changed_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_data_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_data_download_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19509 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14706 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_container_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_container_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_resource_requested.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_status_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/scenario_validation_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/source_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/translated_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/twin_graph_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/twin_graph_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/twin_graph_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/twin_graph_import_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/twin_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/user_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/user_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/validator_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19016 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/workspace_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/workspace_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/workspace_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/workspace_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/workspace_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/workspace_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/workspace_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model/workspace_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82070 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:22.867818 cosmotech-api-2.4.7/cosmotech_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/cosmotech_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:22.851817 cosmotech-api-2.4.7/cosmotech_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-25 07:44:22.000000 cosmotech-api-2.4.7/cosmotech_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-25 07:44:22.000000 cosmotech-api-2.4.7/cosmotech_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:44:22.000000 cosmotech-api-2.4.7/cosmotech_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 07:44:22.000000 cosmotech-api-2.4.7/cosmotech_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 07:44:22.000000 cosmotech-api-2.4.7/cosmotech_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 07:44:22.879818 cosmotech-api-2.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:22.879818 cosmotech-api-2.4.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_component_role_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_connector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_connector_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_connector_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_container_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_container_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_dataset_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_dataset_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_dataset_copy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_dataset_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_delete_historical_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_graph_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_organization_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_organization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_organization_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_organization_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_organization_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_run_template_handler_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_run_template_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_run_template_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_run_template_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_run_template_step_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_changed_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_data_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_data_download_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_run_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_run_container_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_run_container_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_run_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_run_resource_requested.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_run_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_run_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_run_status_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenario_validation_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_scenariorun_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_solution_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_source_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_translated_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_twin_graph_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_twin_graph_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_twin_graph_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_twin_graph_import_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_twin_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_twingraph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_user_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_user_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_validator_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_workspace_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_workspace_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_workspace_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_workspace_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_workspace_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_workspace_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_workspace_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-25 07:44:12.000000 cosmotech-api-2.4.7/test/test_workspace_web_app.py
```

### Comparing `cosmotech-api-2.4.1/LICENSE` & `cosmotech-api-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.1/README.md` & `cosmotech-api-2.4.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # cosmotech-api
 Cosmo Tech Platform API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.4.2-SNAPSHOT
+- API version: 2.4.7-private
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://github.com/Cosmo-Tech/cosmotech-api](https://github.com/Cosmo-Tech/cosmotech-api)
 
 ## Requirements.
 
 Python >=3.6
@@ -176,26 +176,26 @@
 *SolutionApi* | [**remove_all_solution_parameter_groups**](docs/SolutionApi.md#remove_all_solution_parameter_groups) | **DELETE** /organizations/{organization_id}/solutions/{solution_id}/parameterGroups | Remove all Parameter Groups from the Solution specified
 *SolutionApi* | [**remove_all_solution_parameters**](docs/SolutionApi.md#remove_all_solution_parameters) | **DELETE** /organizations/{organization_id}/solutions/{solution_id}/parameters | Remove all Parameters from the Solution specified
 *SolutionApi* | [**update_solution**](docs/SolutionApi.md#update_solution) | **PATCH** /organizations/{organization_id}/solutions/{solution_id} | Update a solution
 *SolutionApi* | [**update_solution_run_template**](docs/SolutionApi.md#update_solution_run_template) | **PATCH** /organizations/{organization_id}/solutions/{solution_id}/runTemplates/{run_template_id} | Update the specified Solution Run Template
 *SolutionApi* | [**upload_run_template_handler**](docs/SolutionApi.md#upload_run_template_handler) | **POST** /organizations/{organization_id}/solutions/{solution_id}/runtemplates/{run_template_id}/handlers/{handler_id}/upload | Upload a Run Template step handler zip file
 *TwingraphApi* | [**batch_query**](docs/TwingraphApi.md#batch_query) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/batch-query | Run a query on a graph instance and return the result as a zip file in async mode
 *TwingraphApi* | [**batch_upload_update**](docs/TwingraphApi.md#batch_upload_update) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/batch | Async batch update by loading a CSV file on a graph instance 
-*TwingraphApi* | [**create_entities**](docs/TwingraphApi.md#create_entities) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | Create new entities in a graph instance
+*TwingraphApi* | [**create_entities**](docs/TwingraphApi.md#create_entities) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/entity/{type} | Create new entities in a graph instance
 *TwingraphApi* | [**create_graph**](docs/TwingraphApi.md#create_graph) | **POST** /organizations/{organization_id}/twingraph/{graph_id} | Create a new graph
-*TwingraphApi* | [**delete**](docs/TwingraphApi.md#delete) | **DELETE** /organizations/{organization_id}/twingraph/{graph_id} | Launch a mass delete job
-*TwingraphApi* | [**delete_entities**](docs/TwingraphApi.md#delete_entities) | **DELETE** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | Delete entities in a graph instance
-*TwingraphApi* | [**download_graph**](docs/TwingraphApi.md#download_graph) | **GET** /organizations/{organization_id}/twingraph/bulk-query/download/{hash} | Download a graph compressed in a zip file
+*TwingraphApi* | [**delete**](docs/TwingraphApi.md#delete) | **DELETE** /organizations/{organization_id}/twingraph/{graph_id} | Delete all versions of a graph and his metadatas
+*TwingraphApi* | [**delete_entities**](docs/TwingraphApi.md#delete_entities) | **DELETE** /organizations/{organization_id}/twingraph/{graph_id}/entity/{type} | Delete entities in a graph instance
+*TwingraphApi* | [**download_graph**](docs/TwingraphApi.md#download_graph) | **GET** /organizations/{organization_id}/twingraph/download/{hash} | Download a graph compressed in a zip file
 *TwingraphApi* | [**find_all_twingraphs**](docs/TwingraphApi.md#find_all_twingraphs) | **GET** /organizations/{organization_id}/twingraphs | Return the list of all graphs stored in the organization
-*TwingraphApi* | [**get_entities**](docs/TwingraphApi.md#get_entities) | **GET** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | Get entities in a graph instance
+*TwingraphApi* | [**get_entities**](docs/TwingraphApi.md#get_entities) | **GET** /organizations/{organization_id}/twingraph/{graph_id}/entity/{type} | Get entities in a graph instance
 *TwingraphApi* | [**get_graph_meta_data**](docs/TwingraphApi.md#get_graph_meta_data) | **GET** /organizations/{organization_id}/twingraph/{graph_id}/metadata | Return the metaData of the specified graph
 *TwingraphApi* | [**import_graph**](docs/TwingraphApi.md#import_graph) | **POST** /organizations/{organization_id}/twingraph/import | Import a new version of a twin graph
 *TwingraphApi* | [**job_status**](docs/TwingraphApi.md#job_status) | **GET** /organizations/{organization_id}/job/{job_id}/status | Get the status of a job
 *TwingraphApi* | [**query**](docs/TwingraphApi.md#query) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/query | Run a query on a graph instance
-*TwingraphApi* | [**update_entities**](docs/TwingraphApi.md#update_entities) | **PATCH** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | Update entities in a graph instance
+*TwingraphApi* | [**update_entities**](docs/TwingraphApi.md#update_entities) | **PATCH** /organizations/{organization_id}/twingraph/{graph_id}/entity/{type} | Update entities in a graph instance
 *TwingraphApi* | [**update_graph_meta_data**](docs/TwingraphApi.md#update_graph_meta_data) | **PATCH** /organizations/{organization_id}/twingraph/{graph_id}/metadata | Update the metaData of the specified graph
 *ValidatorApi* | [**create_validator**](docs/ValidatorApi.md#create_validator) | **POST** /organizations/{organization_id}/datasets/validators | Register a new validator
 *ValidatorApi* | [**create_validator_run**](docs/ValidatorApi.md#create_validator_run) | **POST** /organizations/{organization_id}/datasets/validators/{validator_id}/history | Register a new validator run
 *ValidatorApi* | [**delete_validator**](docs/ValidatorApi.md#delete_validator) | **DELETE** /organizations/{organization_id}/datasets/validators/{validator_id} | Delete a validator
 *ValidatorApi* | [**delete_validator_run**](docs/ValidatorApi.md#delete_validator_run) | **DELETE** /organizations/{organization_id}/datasets/validators/{validator_id}/history/{validatorrun_id} | Delete a validator run
 *ValidatorApi* | [**find_all_validator_runs**](docs/ValidatorApi.md#find_all_validator_runs) | **GET** /organizations/{organization_id}/datasets/validators/{validator_id}/history | List all Validator Runs
 *ValidatorApi* | [**find_all_validators**](docs/ValidatorApi.md#find_all_validators) | **GET** /organizations/{organization_id}/datasets/validators | List all Validators
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/__init__.py` & `cosmotech-api-2.4.7/cosmotech_api/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/api/connector_api.py` & `cosmotech-api-2.4.7/cosmotech_api/api/connector_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/api/dataset_api.py` & `cosmotech-api-2.4.7/cosmotech_api/api/dataset_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/api/organization_api.py` & `cosmotech-api-2.4.7/cosmotech_api/api/organization_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/api/scenario_api.py` & `cosmotech-api-2.4.7/cosmotech_api/api/scenario_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/api/scenariorun_api.py` & `cosmotech-api-2.4.7/cosmotech_api/api/scenariorun_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/api/solution_api.py` & `cosmotech-api-2.4.7/cosmotech_api/api/solution_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/api/twingraph_api.py` & `cosmotech-api-2.4.7/cosmotech_api/api/twingraph_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -174,73 +174,73 @@
                     'application/octet-stream'
                 ]
             },
             api_client=api_client
         )
         self.create_entities_endpoint = _Endpoint(
             settings={
-                'response_type': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),
+                'response_type': (str,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/twingraph/{graph_id}/{modelType}',
+                'endpoint_path': '/organizations/{organization_id}/twingraph/{graph_id}/entity/{type}',
                 'operation_id': 'create_entities',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'graph_id',
-                    'model_type',
+                    'type',
                     'graph_properties',
                 ],
                 'required': [
                     'organization_id',
                     'graph_id',
-                    'model_type',
+                    'type',
                     'graph_properties',
                 ],
                 'nullable': [
                 ],
                 'enum': [
-                    'model_type',
+                    'type',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
-                    ('model_type',): {
+                    ('type',): {
 
                         "NODE": "node",
                         "RELATIONSHIP": "relationship"
                     },
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'graph_id':
                         (str,),
-                    'model_type':
+                    'type':
                         (str,),
                     'graph_properties':
                         ([GraphProperties],),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'graph_id': 'graph_id',
-                    'model_type': 'modelType',
+                    'type': 'type',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'graph_id': 'path',
-                    'model_type': 'path',
+                    'type': 'path',
                     'graph_properties': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -370,70 +370,70 @@
         )
         self.delete_entities_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/twingraph/{graph_id}/{modelType}',
+                'endpoint_path': '/organizations/{organization_id}/twingraph/{graph_id}/entity/{type}',
                 'operation_id': 'delete_entities',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'graph_id',
-                    'model_type',
+                    'type',
                     'ids',
                 ],
                 'required': [
                     'organization_id',
                     'graph_id',
-                    'model_type',
+                    'type',
                     'ids',
                 ],
                 'nullable': [
                 ],
                 'enum': [
-                    'model_type',
+                    'type',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
-                    ('model_type',): {
+                    ('type',): {
 
                         "NODE": "node",
                         "RELATIONSHIP": "relationship"
                     },
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'graph_id':
                         (str,),
-                    'model_type':
+                    'type':
                         (str,),
                     'ids':
                         ([str],),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'graph_id': 'graph_id',
-                    'model_type': 'modelType',
+                    'type': 'type',
                     'ids': 'ids',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'graph_id': 'path',
-                    'model_type': 'path',
+                    'type': 'path',
                     'ids': 'query',
                 },
                 'collection_format_map': {
                     'ids': 'multi',
                 }
             },
             headers_map={
@@ -444,15 +444,15 @@
         )
         self.download_graph_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/twingraph/bulk-query/download/{hash}',
+                'endpoint_path': '/organizations/{organization_id}/twingraph/download/{hash}',
                 'operation_id': 'download_graph',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
@@ -548,74 +548,74 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.get_entities_endpoint = _Endpoint(
             settings={
-                'response_type': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),
+                'response_type': (str,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/twingraph/{graph_id}/{modelType}',
+                'endpoint_path': '/organizations/{organization_id}/twingraph/{graph_id}/entity/{type}',
                 'operation_id': 'get_entities',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'graph_id',
-                    'model_type',
+                    'type',
                     'ids',
                 ],
                 'required': [
                     'organization_id',
                     'graph_id',
-                    'model_type',
+                    'type',
                     'ids',
                 ],
                 'nullable': [
                 ],
                 'enum': [
-                    'model_type',
+                    'type',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
-                    ('model_type',): {
+                    ('type',): {
 
                         "NODE": "node",
                         "RELATIONSHIP": "relationship"
                     },
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'graph_id':
                         (str,),
-                    'model_type':
+                    'type':
                         (str,),
                     'ids':
                         ([str],),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'graph_id': 'graph_id',
-                    'model_type': 'modelType',
+                    'type': 'type',
                     'ids': 'ids',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'graph_id': 'path',
-                    'model_type': 'path',
+                    'type': 'path',
                     'ids': 'query',
                 },
                 'collection_format_map': {
                     'ids': 'multi',
                 }
             },
             headers_map={
@@ -863,73 +863,73 @@
                     'application/yaml'
                 ]
             },
             api_client=api_client
         )
         self.update_entities_endpoint = _Endpoint(
             settings={
-                'response_type': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),
+                'response_type': (str,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/twingraph/{graph_id}/{modelType}',
+                'endpoint_path': '/organizations/{organization_id}/twingraph/{graph_id}/entity/{type}',
                 'operation_id': 'update_entities',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'graph_id',
-                    'model_type',
+                    'type',
                     'graph_properties',
                 ],
                 'required': [
                     'organization_id',
                     'graph_id',
-                    'model_type',
+                    'type',
                     'graph_properties',
                 ],
                 'nullable': [
                 ],
                 'enum': [
-                    'model_type',
+                    'type',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
-                    ('model_type',): {
+                    ('type',): {
 
                         "NODE": "node",
                         "RELATIONSHIP": "relationship"
                     },
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'graph_id':
                         (str,),
-                    'model_type':
+                    'type':
                         (str,),
                     'graph_properties':
                         ([GraphProperties],),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'graph_id': 'graph_id',
-                    'model_type': 'modelType',
+                    'type': 'type',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'graph_id': 'path',
-                    'model_type': 'path',
+                    'type': 'path',
                     'graph_properties': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -1182,31 +1182,31 @@
             body
         return self.batch_upload_update_endpoint.call_with_http_info(**kwargs)
 
     def create_entities(
         self,
         organization_id,
         graph_id,
-        model_type,
+        type,
         graph_properties,
         **kwargs
     ):
         """Create new entities in a graph instance  # noqa: E501
 
         create new entities in a graph instance  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_entities(organization_id, graph_id, model_type, graph_properties, async_req=True)
+        >>> thread = api.create_entities(organization_id, graph_id, type, graph_properties, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             graph_id (str): the Graph Identifier
-            model_type (str): the entity model type
+            type (str): the entity model type
             graph_properties ([GraphProperties]): the entities to create
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -1230,15 +1230,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]
+            str
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1262,29 +1262,29 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['graph_id'] = \
             graph_id
-        kwargs['model_type'] = \
-            model_type
+        kwargs['type'] = \
+            type
         kwargs['graph_properties'] = \
             graph_properties
         return self.create_entities_endpoint.call_with_http_info(**kwargs)
 
     def create_graph(
         self,
         organization_id,
         graph_id,
         **kwargs
     ):
         """Create a new graph  # noqa: E501
 
-        Create a new graph  # noqa: E501
+        To create a new graph from flat files,  you need to create a Zip file. This Zip file must countain two folders named Edges and Nodes.  .zip hierarchy: *main_folder/Nodes *main_folder/Edges  In each folder you can place one or multiple csv files containing your Nodes or Edges data.  Your csv files must follow the following header (column name) requirements:  The Nodes CSVs requires at least one column (the 1st).Column name = 'Id'. It will represent the nodes ID Ids must be populated with string  The Edges CSVs require three columns named, in order, * source * target * Id  those colomns represent * The source of the edge * The target of the edge * The Id of the edge  All following columns content are up to you.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_graph(organization_id, graph_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1357,17 +1357,17 @@
 
     def delete(
         self,
         organization_id,
         graph_id,
         **kwargs
     ):
-        """Launch a mass delete job  # noqa: E501
+        """Delete all versions of a graph and his metadatas  # noqa: E501
 
-        Launch a mass delete job  # noqa: E501
+        Delete all versions of a graph and his metadatas  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete(organization_id, graph_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1437,31 +1437,31 @@
             graph_id
         return self.delete_endpoint.call_with_http_info(**kwargs)
 
     def delete_entities(
         self,
         organization_id,
         graph_id,
-        model_type,
+        type,
         ids,
         **kwargs
     ):
         """Delete entities in a graph instance  # noqa: E501
 
         delete entities in a graph instance  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_entities(organization_id, graph_id, model_type, ids, async_req=True)
+        >>> thread = api.delete_entities(organization_id, graph_id, type, ids, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             graph_id (str): the Graph Identifier
-            model_type (str): the entity model type
+            type (str): the entity model type
             ids ([str]): the entities to delete
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -1517,16 +1517,16 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['graph_id'] = \
             graph_id
-        kwargs['model_type'] = \
-            model_type
+        kwargs['type'] = \
+            type
         kwargs['ids'] = \
             ids
         return self.delete_entities_endpoint.call_with_http_info(**kwargs)
 
     def download_graph(
         self,
         organization_id,
@@ -1687,31 +1687,31 @@
             organization_id
         return self.find_all_twingraphs_endpoint.call_with_http_info(**kwargs)
 
     def get_entities(
         self,
         organization_id,
         graph_id,
-        model_type,
+        type,
         ids,
         **kwargs
     ):
         """Get entities in a graph instance  # noqa: E501
 
         get entities in a graph instance  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_entities(organization_id, graph_id, model_type, ids, async_req=True)
+        >>> thread = api.get_entities(organization_id, graph_id, type, ids, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             graph_id (str): the Graph Identifier
-            model_type (str): the entity model type
+            type (str): the entity model type
             ids ([str]): the entities to get
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -1735,15 +1735,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]
+            str
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1767,16 +1767,16 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['graph_id'] = \
             graph_id
-        kwargs['model_type'] = \
-            model_type
+        kwargs['type'] = \
+            type
         kwargs['ids'] = \
             ids
         return self.get_entities_endpoint.call_with_http_info(**kwargs)
 
     def get_graph_meta_data(
         self,
         organization_id,
@@ -2109,31 +2109,31 @@
             twin_graph_query
         return self.query_endpoint.call_with_http_info(**kwargs)
 
     def update_entities(
         self,
         organization_id,
         graph_id,
-        model_type,
+        type,
         graph_properties,
         **kwargs
     ):
         """Update entities in a graph instance  # noqa: E501
 
         update entities in a graph instance  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_entities(organization_id, graph_id, model_type, graph_properties, async_req=True)
+        >>> thread = api.update_entities(organization_id, graph_id, type, graph_properties, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             graph_id (str): the Graph Identifier
-            model_type (str): the entity model type
+            type (str): the entity model type
             graph_properties ([GraphProperties]): the entities to update
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -2157,15 +2157,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]
+            str
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -2189,16 +2189,16 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['graph_id'] = \
             graph_id
-        kwargs['model_type'] = \
-            model_type
+        kwargs['type'] = \
+            type
         kwargs['graph_properties'] = \
             graph_properties
         return self.update_entities_endpoint.call_with_http_info(**kwargs)
 
     def update_graph_meta_data(
         self,
         organization_id,
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/api/user_api.py` & `cosmotech-api-2.4.7/cosmotech_api/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.8
+    The version of the OpenAPI document: 2.3.15-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/api/validator_api.py` & `cosmotech-api-2.4.7/cosmotech_api/api/validator_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/api/workspace_api.py` & `cosmotech-api-2.4.7/cosmotech_api/api/workspace_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/api_client.py` & `cosmotech-api-2.4.7/cosmotech_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/apis/__init__.py` & `cosmotech-api-2.4.7/cosmotech_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.1/cosmotech_api/configuration.py` & `cosmotech-api-2.4.7/cosmotech_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -384,15 +384,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.4.2-SNAPSHOT\n"\
+               "Version of the API: 2.4.7-private\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/exceptions.py` & `cosmotech-api-2.4.7/cosmotech_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/component_role_permissions.py` & `cosmotech-api-2.4.7/cosmotech_api/model/component_role_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/connector.py` & `cosmotech-api-2.4.7/cosmotech_api/model/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/connector_parameter.py` & `cosmotech-api-2.4.7/cosmotech_api/model/connector_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/connector_parameter_group.py` & `cosmotech-api-2.4.7/cosmotech_api/model/connector_parameter_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/container_resource_size_info.py` & `cosmotech-api-2.4.7/cosmotech_api/model/container_resource_size_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/container_resource_sizing.py` & `cosmotech-api-2.4.7/cosmotech_api/model/container_resource_sizing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/dataset.py` & `cosmotech-api-2.4.7/cosmotech_api/model/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/dataset_compatibility.py` & `cosmotech-api-2.4.7/cosmotech_api/model/dataset_compatibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/dataset_connector.py` & `cosmotech-api-2.4.7/cosmotech_api/model/dataset_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/dataset_copy_parameters.py` & `cosmotech-api-2.4.7/cosmotech_api/model/dataset_copy_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/dataset_search.py` & `cosmotech-api-2.4.7/cosmotech_api/model/dataset_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/delete_historical_data.py` & `cosmotech-api-2.4.7/cosmotech_api/model/delete_historical_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/graph_properties.py` & `cosmotech-api-2.4.7/cosmotech_api/model/graph_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/organization.py` & `cosmotech-api-2.4.7/cosmotech_api/model/organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/organization_access_control.py` & `cosmotech-api-2.4.7/cosmotech_api/model/organization_access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/organization_role.py` & `cosmotech-api-2.4.7/cosmotech_api/model/organization_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/organization_security.py` & `cosmotech-api-2.4.7/cosmotech_api/model/organization_security.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/organization_service.py` & `cosmotech-api-2.4.7/cosmotech_api/model/organization_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/organization_services.py` & `cosmotech-api-2.4.7/cosmotech_api/model/organization_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/organization_user.py` & `cosmotech-api-2.4.7/cosmotech_api/model/organization_user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/resource_size_info.py` & `cosmotech-api-2.4.7/cosmotech_api/model/resource_size_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/run_template.py` & `cosmotech-api-2.4.7/cosmotech_api/model/run_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/run_template_handler_id.py` & `cosmotech-api-2.4.7/cosmotech_api/model/run_template_handler_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/run_template_parameter.py` & `cosmotech-api-2.4.7/cosmotech_api/model/run_template_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/run_template_parameter_group.py` & `cosmotech-api-2.4.7/cosmotech_api/model/run_template_parameter_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/run_template_parameter_value.py` & `cosmotech-api-2.4.7/cosmotech_api/model/run_template_parameter_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/run_template_resource_sizing.py` & `cosmotech-api-2.4.7/cosmotech_api/model/run_template_resource_sizing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/run_template_step_source.py` & `cosmotech-api-2.4.7/cosmotech_api/model/run_template_step_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_access_control.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_changed_parameter_value.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_changed_parameter_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_comparison_result.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_comparison_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_data_download_info.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_data_download_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_data_download_job.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_data_download_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_job_state.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_job_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_last_run.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_last_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_resource_sizing.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_resource_sizing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_role.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_container.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_container_artifact.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_container_artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_container_logs.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_container_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_logs.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_search.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_start_containers.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_start_containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_state.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_status.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_status_node.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_status_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_run_template_parameter_value.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_run_template_parameter_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_security.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_security.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_user.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/scenario_validation_status.py` & `cosmotech-api-2.4.7/cosmotech_api/model/scenario_validation_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/solution.py` & `cosmotech-api-2.4.7/cosmotech_api/model/solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/source_info.py` & `cosmotech-api-2.4.7/cosmotech_api/model/source_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/translated_labels.py` & `cosmotech-api-2.4.7/cosmotech_api/model/translated_labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_batch_result.py` & `cosmotech-api-2.4.7/cosmotech_api/model/twin_graph_batch_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_hash.py` & `cosmotech-api-2.4.7/cosmotech_api/model/twin_graph_hash.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_import.py` & `cosmotech-api-2.4.7/cosmotech_api/model/twin_graph_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_import_info.py` & `cosmotech-api-2.4.7/cosmotech_api/model/twin_graph_import_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/twin_graph_query.py` & `cosmotech-api-2.4.7/cosmotech_api/model/twin_graph_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/user.py` & `cosmotech-api-2.4.7/cosmotech_api/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.8
+    The version of the OpenAPI document: 2.3.15-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/user_organization.py` & `cosmotech-api-2.4.7/cosmotech_api/model/user_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.8
+    The version of the OpenAPI document: 2.3.15-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/user_workspace.py` & `cosmotech-api-2.4.7/cosmotech_api/model/user_workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.8
+    The version of the OpenAPI document: 2.3.15-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/validator.py` & `cosmotech-api-2.4.7/cosmotech_api/model/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/validator_run.py` & `cosmotech-api-2.4.7/cosmotech_api/model/validator_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/workspace.py` & `cosmotech-api-2.4.7/cosmotech_api/model/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/workspace_access_control.py` & `cosmotech-api-2.4.7/cosmotech_api/model/workspace_access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/workspace_file.py` & `cosmotech-api-2.4.7/cosmotech_api/model/workspace_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/workspace_role.py` & `cosmotech-api-2.4.7/cosmotech_api/model/workspace_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/workspace_secret.py` & `cosmotech-api-2.4.7/cosmotech_api/model/workspace_secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/workspace_security.py` & `cosmotech-api-2.4.7/cosmotech_api/model/workspace_security.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/workspace_solution.py` & `cosmotech-api-2.4.7/cosmotech_api/model/workspace_solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/workspace_user.py` & `cosmotech-api-2.4.7/cosmotech_api/model/workspace_user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model/workspace_web_app.py` & `cosmotech-api-2.4.7/cosmotech_api/model/workspace_web_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/model_utils.py` & `cosmotech-api-2.4.7/cosmotech_api/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api/models/__init__.py` & `cosmotech-api-2.4.7/cosmotech_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.1/cosmotech_api/rest.py` & `cosmotech-api-2.4.7/cosmotech_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `cosmotech-api-2.4.1/cosmotech_api.egg-info/SOURCES.txt` & `cosmotech-api-2.4.7/cosmotech_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 cosmotech_api/model/scenario_resource_sizing.py
 cosmotech_api/model/scenario_role.py
 cosmotech_api/model/scenario_run.py
 cosmotech_api/model/scenario_run_container.py
 cosmotech_api/model/scenario_run_container_artifact.py
 cosmotech_api/model/scenario_run_container_logs.py
 cosmotech_api/model/scenario_run_logs.py
+cosmotech_api/model/scenario_run_resource_requested.py
 cosmotech_api/model/scenario_run_search.py
 cosmotech_api/model/scenario_run_start_containers.py
 cosmotech_api/model/scenario_run_state.py
 cosmotech_api/model/scenario_run_status.py
 cosmotech_api/model/scenario_run_status_node.py
 cosmotech_api/model/scenario_run_template_parameter_value.py
 cosmotech_api/model/scenario_security.py
@@ -144,14 +145,15 @@
 test/test_scenario_resource_sizing.py
 test/test_scenario_role.py
 test/test_scenario_run.py
 test/test_scenario_run_container.py
 test/test_scenario_run_container_artifact.py
 test/test_scenario_run_container_logs.py
 test/test_scenario_run_logs.py
+test/test_scenario_run_resource_requested.py
 test/test_scenario_run_search.py
 test/test_scenario_run_start_containers.py
 test/test_scenario_run_state.py
 test/test_scenario_run_status.py
 test/test_scenario_run_status_node.py
 test/test_scenario_run_template_parameter_value.py
 test/test_scenario_security.py
```

### Comparing `cosmotech-api-2.4.1/setup.py` & `cosmotech-api-2.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "cosmotech-api"
-VERSION = "2.4.1"
+VERSION = "2.4.7"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `cosmotech-api-2.4.1/test/test_component_role_permissions.py` & `cosmotech-api-2.4.7/test/test_component_role_permissions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_connector.py` & `cosmotech-api-2.4.7/test/test_connector_parameter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.connector_parameter_group import ConnectorParameterGroup
-globals()['ConnectorParameterGroup'] = ConnectorParameterGroup
-from cosmotech_api.model.connector import Connector
+from cosmotech_api.model.connector_parameter import ConnectorParameter
 
 
-class TestConnector(unittest.TestCase):
-    """Connector unit test stubs"""
+class TestConnectorParameter(unittest.TestCase):
+    """ConnectorParameter unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testConnector(self):
-        """Test Connector"""
+    def testConnectorParameter(self):
+        """Test ConnectorParameter"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Connector()  # noqa: E501
+        # model = ConnectorParameter()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_connector_api.py` & `cosmotech-api-2.4.7/test/test_connector_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_connector_parameter.py` & `cosmotech-api-2.4.7/test/test_dataset_connector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.connector_parameter import ConnectorParameter
+from cosmotech_api.model.dataset_connector import DatasetConnector
 
 
-class TestConnectorParameter(unittest.TestCase):
-    """ConnectorParameter unit test stubs"""
+class TestDatasetConnector(unittest.TestCase):
+    """DatasetConnector unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testConnectorParameter(self):
-        """Test ConnectorParameter"""
+    def testDatasetConnector(self):
+        """Test DatasetConnector"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ConnectorParameter()  # noqa: E501
+        # model = DatasetConnector()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_connector_parameter_group.py` & `cosmotech-api-2.4.7/test/test_connector_parameter_group.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_container_resource_size_info.py` & `cosmotech-api-2.4.7/test/test_container_resource_size_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_container_resource_sizing.py` & `cosmotech-api-2.4.7/test/test_container_resource_sizing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_dataset.py` & `cosmotech-api-2.4.7/test/test_dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_dataset_api.py` & `cosmotech-api-2.4.7/test/test_dataset_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_dataset_compatibility.py` & `cosmotech-api-2.4.7/test/test_dataset_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_dataset_connector.py` & `cosmotech-api-2.4.7/test/test_scenario_validation_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.dataset_connector import DatasetConnector
+from cosmotech_api.model.scenario_validation_status import ScenarioValidationStatus
 
 
-class TestDatasetConnector(unittest.TestCase):
-    """DatasetConnector unit test stubs"""
+class TestScenarioValidationStatus(unittest.TestCase):
+    """ScenarioValidationStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDatasetConnector(self):
-        """Test DatasetConnector"""
+    def testScenarioValidationStatus(self):
+        """Test ScenarioValidationStatus"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DatasetConnector()  # noqa: E501
+        # model = ScenarioValidationStatus()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_dataset_copy_parameters.py` & `cosmotech-api-2.4.7/test/test_dataset_copy_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_dataset_search.py` & `cosmotech-api-2.4.7/test/test_scenario_last_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.dataset_search import DatasetSearch
+from cosmotech_api.model.scenario_last_run import ScenarioLastRun
 
 
-class TestDatasetSearch(unittest.TestCase):
-    """DatasetSearch unit test stubs"""
+class TestScenarioLastRun(unittest.TestCase):
+    """ScenarioLastRun unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDatasetSearch(self):
-        """Test DatasetSearch"""
+    def testScenarioLastRun(self):
+        """Test ScenarioLastRun"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DatasetSearch()  # noqa: E501
+        # model = ScenarioLastRun()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_delete_historical_data.py` & `cosmotech-api-2.4.7/test/test_delete_historical_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_graph_properties.py` & `cosmotech-api-2.4.7/test/test_graph_properties.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_organization.py` & `cosmotech-api-2.4.7/test/test_organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_organization_access_control.py` & `cosmotech-api-2.4.7/test/test_organization_access_control.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_organization_api.py` & `cosmotech-api-2.4.7/test/test_organization_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_organization_role.py` & `cosmotech-api-2.4.7/test/test_organization_role.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_organization_security.py` & `cosmotech-api-2.4.7/test/test_organization_security.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_organization_service.py` & `cosmotech-api-2.4.7/test/test_organization_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_organization_services.py` & `cosmotech-api-2.4.7/test/test_organization_services.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_organization_user.py` & `cosmotech-api-2.4.7/test/test_organization_user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.1/test/test_resource_size_info.py` & `cosmotech-api-2.4.7/test/test_resource_size_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_run_template.py` & `cosmotech-api-2.4.7/test/test_run_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_run_template_handler_id.py` & `cosmotech-api-2.4.7/test/test_run_template_handler_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_run_template_parameter.py` & `cosmotech-api-2.4.7/test/test_run_template_parameter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_run_template_parameter_group.py` & `cosmotech-api-2.4.7/test/test_run_template_parameter_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_run_template_parameter_value.py` & `cosmotech-api-2.4.7/test/test_run_template_parameter_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_run_template_resource_sizing.py` & `cosmotech-api-2.4.7/test/test_run_template_resource_sizing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_run_template_step_source.py` & `cosmotech-api-2.4.7/test/test_run_template_step_source.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario.py` & `cosmotech-api-2.4.7/test/test_scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_access_control.py` & `cosmotech-api-2.4.7/test/test_scenario_access_control.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_api.py` & `cosmotech-api-2.4.7/test/test_scenario_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_changed_parameter_value.py` & `cosmotech-api-2.4.7/test/test_scenario_changed_parameter_value.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_comparison_result.py` & `cosmotech-api-2.4.7/test/test_scenario_comparison_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_data_download_info.py` & `cosmotech-api-2.4.7/test/test_scenario_data_download_info.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_data_download_job.py` & `cosmotech-api-2.4.7/test/test_scenario_data_download_job.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_job_state.py` & `cosmotech-api-2.4.7/test/test_scenario_job_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_last_run.py` & `cosmotech-api-2.4.7/test/test_workspace_role.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.scenario_last_run import ScenarioLastRun
+from cosmotech_api.model.workspace_role import WorkspaceRole
 
 
-class TestScenarioLastRun(unittest.TestCase):
-    """ScenarioLastRun unit test stubs"""
+class TestWorkspaceRole(unittest.TestCase):
+    """WorkspaceRole unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioLastRun(self):
-        """Test ScenarioLastRun"""
+    def testWorkspaceRole(self):
+        """Test WorkspaceRole"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioLastRun()  # noqa: E501
+        # model = WorkspaceRole()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_resource_sizing.py` & `cosmotech-api-2.4.7/test/test_scenario_resource_sizing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_role.py` & `cosmotech-api-2.4.7/test/test_scenario_run_state.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.scenario_role import ScenarioRole
+from cosmotech_api.model.scenario_run_state import ScenarioRunState
 
 
-class TestScenarioRole(unittest.TestCase):
-    """ScenarioRole unit test stubs"""
+class TestScenarioRunState(unittest.TestCase):
+    """ScenarioRunState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioRole(self):
-        """Test ScenarioRole"""
+    def testScenarioRunState(self):
+        """Test ScenarioRunState"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioRole()  # noqa: E501
+        # model = ScenarioRunState()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_run.py` & `cosmotech-api-2.4.7/test/test_scenario_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_run_container.py` & `cosmotech-api-2.4.7/test/test_scenario_run_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_run_container_artifact.py` & `cosmotech-api-2.4.7/test/test_scenario_run_container_artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_run_container_logs.py` & `cosmotech-api-2.4.7/test/test_scenario_run_container_logs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_run_logs.py` & `cosmotech-api-2.4.7/test/test_scenario_run_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_run_search.py` & `cosmotech-api-2.4.7/test/test_scenario_run_search.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_run_start_containers.py` & `cosmotech-api-2.4.7/test/test_scenario_run_start_containers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_run_state.py` & `cosmotech-api-2.4.7/test/test_user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.3.15-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.scenario_run_state import ScenarioRunState
+from cosmotech_api.model.user_organization import UserOrganization
+globals()['UserOrganization'] = UserOrganization
+from cosmotech_api.model.user import User
 
 
-class TestScenarioRunState(unittest.TestCase):
-    """ScenarioRunState unit test stubs"""
+class TestUser(unittest.TestCase):
+    """User unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioRunState(self):
-        """Test ScenarioRunState"""
+    def testUser(self):
+        """Test User"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioRunState()  # noqa: E501
+        # model = User()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_run_status.py` & `cosmotech-api-2.4.7/test/test_scenario_run_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_run_status_node.py` & `cosmotech-api-2.4.7/test/test_scenario_run_status_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_run_template_parameter_value.py` & `cosmotech-api-2.4.7/test/test_scenario_run_template_parameter_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_security.py` & `cosmotech-api-2.4.7/test/test_scenario_security.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_scenario_user.py` & `cosmotech-api-2.4.7/test/test_scenario_user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.4.1/test/test_scenario_validation_status.py` & `cosmotech-api-2.4.7/test/test_validator_run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.scenario_validation_status import ScenarioValidationStatus
+from cosmotech_api.model.validator_run import ValidatorRun
 
 
-class TestScenarioValidationStatus(unittest.TestCase):
-    """ScenarioValidationStatus unit test stubs"""
+class TestValidatorRun(unittest.TestCase):
+    """ValidatorRun unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioValidationStatus(self):
-        """Test ScenarioValidationStatus"""
+    def testValidatorRun(self):
+        """Test ValidatorRun"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioValidationStatus()  # noqa: E501
+        # model = ValidatorRun()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_scenariorun_api.py` & `cosmotech-api-2.4.7/test/test_scenariorun_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_solution.py` & `cosmotech-api-2.4.7/test/test_solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_solution_api.py` & `cosmotech-api-2.4.7/test/test_solution_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_source_info.py` & `cosmotech-api-2.4.7/test/test_source_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_translated_labels.py` & `cosmotech-api-2.4.7/test/test_translated_labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_twin_graph_batch_result.py` & `cosmotech-api-2.4.7/test/test_twin_graph_hash.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.twin_graph_batch_result import TwinGraphBatchResult
+from cosmotech_api.model.twin_graph_hash import TwinGraphHash
 
 
-class TestTwinGraphBatchResult(unittest.TestCase):
-    """TwinGraphBatchResult unit test stubs"""
+class TestTwinGraphHash(unittest.TestCase):
+    """TwinGraphHash unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTwinGraphBatchResult(self):
-        """Test TwinGraphBatchResult"""
+    def testTwinGraphHash(self):
+        """Test TwinGraphHash"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TwinGraphBatchResult()  # noqa: E501
+        # model = TwinGraphHash()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_twin_graph_hash.py` & `cosmotech-api-2.4.7/test/test_twin_graph_import_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.twin_graph_hash import TwinGraphHash
+from cosmotech_api.model.twin_graph_import_info import TwinGraphImportInfo
 
 
-class TestTwinGraphHash(unittest.TestCase):
-    """TwinGraphHash unit test stubs"""
+class TestTwinGraphImportInfo(unittest.TestCase):
+    """TwinGraphImportInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTwinGraphHash(self):
-        """Test TwinGraphHash"""
+    def testTwinGraphImportInfo(self):
+        """Test TwinGraphImportInfo"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TwinGraphHash()  # noqa: E501
+        # model = TwinGraphImportInfo()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_twin_graph_import.py` & `cosmotech-api-2.4.7/test/test_twin_graph_import.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_twin_graph_import_info.py` & `cosmotech-api-2.4.7/test/test_twin_graph_batch_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.twin_graph_import_info import TwinGraphImportInfo
+from cosmotech_api.model.twin_graph_batch_result import TwinGraphBatchResult
 
 
-class TestTwinGraphImportInfo(unittest.TestCase):
-    """TwinGraphImportInfo unit test stubs"""
+class TestTwinGraphBatchResult(unittest.TestCase):
+    """TwinGraphBatchResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTwinGraphImportInfo(self):
-        """Test TwinGraphImportInfo"""
+    def testTwinGraphBatchResult(self):
+        """Test TwinGraphBatchResult"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TwinGraphImportInfo()  # noqa: E501
+        # model = TwinGraphBatchResult()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_twin_graph_query.py` & `cosmotech-api-2.4.7/test/test_twin_graph_query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_twingraph_api.py` & `cosmotech-api-2.4.7/test/test_twingraph_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
@@ -51,15 +51,15 @@
         Create a new graph  # noqa: E501
         """
         pass
 
     def test_delete(self):
         """Test case for delete
 
-        Launch a mass delete job  # noqa: E501
+        Delete all versions of a graph and his metadatas  # noqa: E501
         """
         pass
 
     def test_delete_entities(self):
         """Test case for delete_entities
 
         Delete entities in a graph instance  # noqa: E501
```

### Comparing `cosmotech-api-2.4.1/test/test_user.py` & `cosmotech-api-2.4.7/test/test_dataset_search.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.8
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.user_organization import UserOrganization
-globals()['UserOrganization'] = UserOrganization
-from cosmotech_api.model.user import User
+from cosmotech_api.model.dataset_search import DatasetSearch
 
 
-class TestUser(unittest.TestCase):
-    """User unit test stubs"""
+class TestDatasetSearch(unittest.TestCase):
+    """DatasetSearch unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUser(self):
-        """Test User"""
+    def testDatasetSearch(self):
+        """Test DatasetSearch"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = User()  # noqa: E501
+        # model = DatasetSearch()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_user_api.py` & `cosmotech-api-2.4.7/test/test_user_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.8
+    The version of the OpenAPI document: 2.3.15-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_user_organization.py` & `cosmotech-api-2.4.7/test/test_user_organization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.8
+    The version of the OpenAPI document: 2.3.15-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_user_workspace.py` & `cosmotech-api-2.4.7/test/test_user_workspace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.8
+    The version of the OpenAPI document: 2.3.15-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_validator.py` & `cosmotech-api-2.4.7/test/test_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_validator_api.py` & `cosmotech-api-2.4.7/test/test_validator_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_validator_run.py` & `cosmotech-api-2.4.7/test/test_workspace_user.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Platform API
+    Cosmo Tech Plaform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.3.4-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.validator_run import ValidatorRun
+from cosmotech_api.model.workspace_user import WorkspaceUser
 
 
-class TestValidatorRun(unittest.TestCase):
-    """ValidatorRun unit test stubs"""
+class TestWorkspaceUser(unittest.TestCase):
+    """WorkspaceUser unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testValidatorRun(self):
-        """Test ValidatorRun"""
+    def testWorkspaceUser(self):
+        """Test WorkspaceUser"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ValidatorRun()  # noqa: E501
+        # model = WorkspaceUser()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_workspace.py` & `cosmotech-api-2.4.7/test/test_workspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_workspace_access_control.py` & `cosmotech-api-2.4.7/test/test_workspace_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_workspace_api.py` & `cosmotech-api-2.4.7/test/test_workspace_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_workspace_file.py` & `cosmotech-api-2.4.7/test/test_scenario_role.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.workspace_file import WorkspaceFile
+from cosmotech_api.model.scenario_role import ScenarioRole
 
 
-class TestWorkspaceFile(unittest.TestCase):
-    """WorkspaceFile unit test stubs"""
+class TestScenarioRole(unittest.TestCase):
+    """ScenarioRole unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspaceFile(self):
-        """Test WorkspaceFile"""
+    def testScenarioRole(self):
+        """Test ScenarioRole"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspaceFile()  # noqa: E501
+        # model = ScenarioRole()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_workspace_role.py` & `cosmotech-api-2.4.7/test/test_workspace_secret.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.workspace_role import WorkspaceRole
+from cosmotech_api.model.workspace_secret import WorkspaceSecret
 
 
-class TestWorkspaceRole(unittest.TestCase):
-    """WorkspaceRole unit test stubs"""
+class TestWorkspaceSecret(unittest.TestCase):
+    """WorkspaceSecret unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspaceRole(self):
-        """Test WorkspaceRole"""
+    def testWorkspaceSecret(self):
+        """Test WorkspaceSecret"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspaceRole()  # noqa: E501
+        # model = WorkspaceSecret()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_workspace_security.py` & `cosmotech-api-2.4.7/test/test_workspace_security.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_workspace_solution.py` & `cosmotech-api-2.4.7/test/test_workspace_solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.4.1/test/test_workspace_user.py` & `cosmotech-api-2.4.7/test/test_workspace_file.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.3.4-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.workspace_user import WorkspaceUser
+from cosmotech_api.model.workspace_file import WorkspaceFile
 
 
-class TestWorkspaceUser(unittest.TestCase):
-    """WorkspaceUser unit test stubs"""
+class TestWorkspaceFile(unittest.TestCase):
+    """WorkspaceFile unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspaceUser(self):
-        """Test WorkspaceUser"""
+    def testWorkspaceFile(self):
+        """Test WorkspaceFile"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspaceUser()  # noqa: E501
+        # model = WorkspaceFile()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.4.1/test/test_workspace_web_app.py` & `cosmotech-api-2.4.7/test/test_workspace_web_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.2-SNAPSHOT
+    The version of the OpenAPI document: 2.4.7-private
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

