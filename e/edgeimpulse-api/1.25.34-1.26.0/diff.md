# Comparing `tmp/edgeimpulse_api-1.25.34.tar.gz` & `tmp/edgeimpulse_api-1.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgeimpulse_api-1.25.34.tar", max compression
+gzip compressed data, was "edgeimpulse_api-1.26.0.tar", max compression
```

## Comparing `edgeimpulse_api-1.25.34.tar` & `edgeimpulse_api-1.26.0.tar`

### file list

```diff
@@ -1,793 +1,811 @@
--rw-r--r--   0        0        0      377 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/README.md
--rw-r--r--   0        0        0    75556 2023-07-23 14:02:37.188862 edgeimpulse_api-1.25.34/edgeimpulse_api/__init__.py
--rw-r--r--   0        0        0     2928 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/__init__.py
--rw-r--r--   0        0        0   263386 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/admin_api.py
--rw-r--r--   0        0        0   303232 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/allows_read_only_api.py
--rw-r--r--   0        0        0    11231 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/auth_api.py
--rw-r--r--   0        0        0     6235 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/cdn_api.py
--rw-r--r--   0        0        0    28575 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/classify_api.py
--rw-r--r--   0        0        0     7426 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/content_disposition_inline_api.py
--rw-r--r--   0        0        0    72480 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/deployment_api.py
--rw-r--r--   0        0        0    38974 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/devices_api.py
--rw-r--r--   0        0        0   131256 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/dsp_api.py
--rw-r--r--   0        0        0     6435 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/export_api.py
--rw-r--r--   0        0        0    11921 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/health_api.py
--rw-r--r--   0        0        0    49621 2023-07-23 14:02:10.629144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/impulse_api.py
--rw-r--r--   0        0        0   239208 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/jobs_api.py
--rw-r--r--   0        0        0   147712 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/learn_api.py
--rw-r--r--   0        0        0     6483 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/login_api.py
--rw-r--r--   0        0        0    12006 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/metrics_api.py
--rw-r--r--   0        0        0    67457 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/optimization_api.py
--rw-r--r--   0        0        0   300920 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_allow_developer_profile_api.py
--rw-r--r--   0        0        0    63140 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_allow_guest_access_api.py
--rw-r--r--   0        0        0   141131 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_blocks_api.py
--rw-r--r--   0        0        0    91908 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_create_project_api.py
--rw-r--r--   0        0        0   255365 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_data_api.py
--rw-r--r--   0        0        0    80882 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_data_campaigns_api.py
--rw-r--r--   0        0        0    58218 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_jobs_api.py
--rw-r--r--   0        0        0    47178 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_pipelines_api.py
--rw-r--r--   0        0        0    45490 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_portals_api.py
--rw-r--r--   0        0        0   266354 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_requires_admin_api.py
--rw-r--r--   0        0        0   176301 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py
--rw-r--r--   0        0        0   300240 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/organizations_api.py
--rw-r--r--   0        0        0    54671 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/performance_calibration_api.py
--rw-r--r--   0        0        0    12662 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/project_requires_admin_api.py
--rw-r--r--   0        0        0   228112 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/projects_api.py
--rw-r--r--   0        0        0   378158 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/raw_data_api.py
--rw-r--r--   0        0        0    24481 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/requires_sudo_api.py
--rw-r--r--   0        0        0     7730 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py
--rw-r--r--   0        0        0    13690 2023-07-23 14:02:10.633144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/supports_range_api.py
--rw-r--r--   0        0        0    35671 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/themes_api.py
--rw-r--r--   0        0        0    43486 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/third_party_auth_api.py
--rw-r--r--   0        0        0    45393 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/upload_portal_api.py
--rw-r--r--   0        0        0   197590 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/user_api.py
--rw-r--r--   0        0        0    42135 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/api/whitelabels_api.py
--rw-r--r--   0        0        0    29331 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/api_client.py
--rw-r--r--   0        0        0    15659 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/configuration.py
--rw-r--r--   0        0        0     5113 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/exceptions.py
--rw-r--r--   0        0        0    72174 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/__init__.py
--rw-r--r--   0        0        0     2897 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
--rw-r--r--   0        0        0     1882 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/activate_user_request.py
--rw-r--r--   0        0        0     2610 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_api_key_request.py
--rw-r--r--   0        0        0     1963 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_collaborator_request.py
--rw-r--r--   0        0        0     2223 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_hmac_key_request.py
--rw-r--r--   0        0        0     2299 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_member_request.py
--rw-r--r--   0        0        0     2418 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_api_key_request.py
--rw-r--r--   0        0        0     2806 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_bucket_request.py
--rw-r--r--   0        0        0     2656 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     2469 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2152 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     4230 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2359 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2042 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
--rw-r--r--   0        0        0     2269 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_deploy_block_response.py
--rw-r--r--   0        0        0     2816 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2248 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_dsp_block_response.py
--rw-r--r--   0        0        0     2054 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_secret_request.py
--rw-r--r--   0        0        0     2266 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_secret_response.py
--rw-r--r--   0        0        0     1949 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_secret_response_all_of.py
--rw-r--r--   0        0        0     4588 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     2339 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
--rw-r--r--   0        0        0     4868 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_transformation_block_request.py
--rw-r--r--   0        0        0     2325 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_transformation_block_response.py
--rw-r--r--   0        0        0     2001 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
--rw-r--r--   0        0        0     1940 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
--rw-r--r--   0        0        0     1961 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
--rw-r--r--   0        0        0     2542 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_add_organization_user_request.py
--rw-r--r--   0        0        0     2246 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
--rw-r--r--   0        0        0     2146 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_add_project_user_request.py
--rw-r--r--   0        0        0     2097 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_add_user_request.py
--rw-r--r--   0        0        0     4696 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_api_organization.py
--rw-r--r--   0        0        0     2396 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_api_organization_all_of.py
--rw-r--r--   0        0        0     3459 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_api_project.py
--rw-r--r--   0        0        0     7268 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_api_user.py
--rw-r--r--   0        0        0     5714 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_api_user_all_of.py
--rw-r--r--   0        0        0     2262 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_create_organization_request.py
--rw-r--r--   0        0        0     2742 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_create_user_trial_request.py
--rw-r--r--   0        0        0     2546 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_data_migration_response.py
--rw-r--r--   0        0        0     2222 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
--rw-r--r--   0        0        0     2735 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_data_migrations_response.py
--rw-r--r--   0        0        0     2428 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
--rw-r--r--   0        0        0     2318 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
--rw-r--r--   0        0        0     2022 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
--rw-r--r--   0        0        0     2217 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_metrics_response.py
--rw-r--r--   0        0        0     1910 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
--rw-r--r--   0        0        0     3046 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_organizations_response.py
--rw-r--r--   0        0        0     2746 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
--rw-r--r--   0        0        0     3409 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
--rw-r--r--   0        0        0     2243 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
--rw-r--r--   0        0        0     1947 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
--rw-r--r--   0        0        0     2914 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_sso_settings_response.py
--rw-r--r--   0        0        0     2614 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
--rw-r--r--   0        0        0     2096 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
--rw-r--r--   0        0        0     2208 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_ids_response.py
--rw-r--r--   0        0        0     1901 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
--rw-r--r--   0        0        0     2245 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_metrics_response.py
--rw-r--r--   0        0        0     1938 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_metrics_response_all_of.py
--rw-r--r--   0        0        0     2452 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_response.py
--rw-r--r--   0        0        0     2128 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_response_all_of.py
--rw-r--r--   0        0        0     2507 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_trial_response.py
--rw-r--r--   0        0        0     2183 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py
--rw-r--r--   0        0        0     2807 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_users_response.py
--rw-r--r--   0        0        0     2500 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_users_response_all_of.py
--rw-r--r--   0        0        0     3087 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
--rw-r--r--   0        0        0     2445 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_list_projects.py
--rw-r--r--   0        0        0     2836 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_list_projects_response.py
--rw-r--r--   0        0        0     7695 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_organization_info_response.py
--rw-r--r--   0        0        0     3752 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_organization_info_response_all_of.py
--rw-r--r--   0        0        0     2158 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_toggle_data_migration_request.py
--rw-r--r--   0        0        0     3269 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_update_organization_request.py
--rw-r--r--   0        0        0     2015 2023-07-23 14:02:10.637144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_update_user_permissions_request.py
--rw-r--r--   0        0        0     2661 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_update_user_request.py
--rw-r--r--   0        0        0     2365 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_update_user_trial_request.py
--rw-r--r--   0        0        0     2525 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/akida_edge_learning_config.py
--rw-r--r--   0        0        0     5499 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_model_metadata.py
--rw-r--r--   0        0        0     5221 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
--rw-r--r--   0        0        0     2151 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
--rw-r--r--   0        0        0     4079 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_response.py
--rw-r--r--   0        0        0     3812 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_response_all_of.py
--rw-r--r--   0        0        0     2044 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_response_all_of_axes.py
--rw-r--r--   0        0        0     3029 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_trained_features_response.py
--rw-r--r--   0        0        0     2729 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2375 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0      506 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/augmentation_policy_image_enum.py
--rw-r--r--   0        0        0     3635 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/augmentation_policy_spectrogram.py
--rw-r--r--   0        0        0     1895 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/autotune_dsp_request.py
--rw-r--r--   0        0        0     2044 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/bounding_box.py
--rw-r--r--   0        0        0     2151 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/bounding_box_with_score.py
--rw-r--r--   0        0        0     2197 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/build_on_device_model_request.py
--rw-r--r--   0        0        0     2433 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/build_organization_on_device_model_request.py
--rw-r--r--   0        0        0     2459 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/calculate_data_quality_metrics_request.py
--rw-r--r--   0        0        0     2041 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/change_password_request.py
--rw-r--r--   0        0        0     3701 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_job_response.py
--rw-r--r--   0        0        0     3394 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_job_response_all_of.py
--rw-r--r--   0        0        0     3769 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
--rw-r--r--   0        0        0     2055 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
--rw-r--r--   0        0        0     3255 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_job_response_page.py
--rw-r--r--   0        0        0     2948 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_job_response_page_all_of.py
--rw-r--r--   0        0        0     3932 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_sample_response.py
--rw-r--r--   0        0        0     3644 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_sample_response_all_of.py
--rw-r--r--   0        0        0     4783 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_sample_response_classification.py
--rw-r--r--   0        0        0     2755 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_sample_response_classification_details.py
--rw-r--r--   0        0        0     3004 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/convert_user_request.py
--rw-r--r--   0        0        0     2183 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/count_samples_response.py
--rw-r--r--   0        0        0     1859 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/count_samples_response_all_of.py
--rw-r--r--   0        0        0     2255 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_block_version_response.py
--rw-r--r--   0        0        0     1938 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_block_version_response_all_of.py
--rw-r--r--   0        0        0     2404 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_developer_profile_response.py
--rw-r--r--   0        0        0     2125 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_developer_profile_response_all_of.py
--rw-r--r--   0        0        0     2387 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_device_request.py
--rw-r--r--   0        0        0     2491 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_evaluation_user_response.py
--rw-r--r--   0        0        0     2185 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
--rw-r--r--   0        0        0     2600 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_organization_portal_request.py
--rw-r--r--   0        0        0     2830 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_organization_portal_response.py
--rw-r--r--   0        0        0     2551 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     1990 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_organization_request.py
--rw-r--r--   0        0        0     2454 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_organization_response.py
--rw-r--r--   0        0        0     2148 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_organization_response_all_of.py
--rw-r--r--   0        0        0     2185 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_pipeline_response.py
--rw-r--r--   0        0        0     2254 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_project_request.py
--rw-r--r--   0        0        0     2378 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_project_response.py
--rw-r--r--   0        0        0     2072 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_project_response_all_of.py
--rw-r--r--   0        0        0     2276 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_signed_upload_link_request.py
--rw-r--r--   0        0        0     2414 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_signed_upload_link_response.py
--rw-r--r--   0        0        0     2135 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
--rw-r--r--   0        0        0     2413 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_third_party_auth_request.py
--rw-r--r--   0        0        0     2450 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_third_party_auth_response.py
--rw-r--r--   0        0        0     2144 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     3835 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_user_request.py
--rw-r--r--   0        0        0     2393 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_user_response.py
--rw-r--r--   0        0        0     2114 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_user_response_all_of.py
--rw-r--r--   0        0        0     2919 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_user_third_party_request.py
--rw-r--r--   0        0        0     2672 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_user_third_party_response.py
--rw-r--r--   0        0        0     2393 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_user_third_party_response_all_of.py
--rw-r--r--   0        0        0     4157 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_whitelabel_request.py
--rw-r--r--   0        0        0     2438 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_whitelabel_response.py
--rw-r--r--   0        0        0     2121 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2051 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/crop_sample_request.py
--rw-r--r--   0        0        0     2248 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/crop_sample_response.py
--rw-r--r--   0        0        0     1943 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/crop_sample_response_all_of.py
--rw-r--r--   0        0        0     4054 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign.py
--rw-r--r--   0        0        0     2851 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign_dashboard.py
--rw-r--r--   0        0        0     2786 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign_graph.py
--rw-r--r--   0        0        0     3352 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
--rw-r--r--   0        0        0     2047 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
--rw-r--r--   0        0        0     1934 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign_link.py
--rw-r--r--   0        0        0     1957 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign_query.py
--rw-r--r--   0        0        0     3292 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_explorer_predictions_response.py
--rw-r--r--   0        0        0     3003 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
--rw-r--r--   0        0        0     2838 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_explorer_settings.py
--rw-r--r--   0        0        0     2149 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dataset_ratio_data.py
--rw-r--r--   0        0        0     2111 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dataset_ratio_data_ratio.py
--rw-r--r--   0        0        0     1898 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/delete_portal_file_request.py
--rw-r--r--   0        0        0     2230 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dependency_data.py
--rw-r--r--   0        0        0     2280 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
--rw-r--r--   0        0        0     2408 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
--rw-r--r--   0        0        0     2155 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
--rw-r--r--   0        0        0     2484 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
--rw-r--r--   0        0        0     2344 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
--rw-r--r--   0        0        0     2780 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
--rw-r--r--   0        0        0     2200 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
--rw-r--r--   0        0        0     4355 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_request.py
--rw-r--r--   0        0        0     2833 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
--rw-r--r--   0        0        0     8503 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
--rw-r--r--   0        0        0     8065 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
--rw-r--r--   0        0        0     5950 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deployment_target.py
--rw-r--r--   0        0        0     1926 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deployment_target_badge.py
--rw-r--r--   0        0        0      679 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deployment_target_engine.py
--rw-r--r--   0        0        0     2702 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deployment_targets_response.py
--rw-r--r--   0        0        0     2395 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     1983 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/development_board.py
--rw-r--r--   0        0        0     2831 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/development_boards_response.py
--rw-r--r--   0        0        0     2531 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/development_boards_response_all_of.py
--rw-r--r--   0        0        0     2030 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/development_keys.py
--rw-r--r--   0        0        0     2400 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/development_keys_response.py
--rw-r--r--   0        0        0     3677 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/device.py
--rw-r--r--   0        0        0     2199 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/device_name_response.py
--rw-r--r--   0        0        0     1920 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/device_name_response_all_of.py
--rw-r--r--   0        0        0     2231 2023-07-23 14:02:10.641144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/device_sensors_inner.py
--rw-r--r--   0        0        0     2094 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/download.py
--rw-r--r--   0        0        0     1912 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/download_portal_file_request.py
--rw-r--r--   0        0        0     2260 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/download_portal_file_response.py
--rw-r--r--   0        0        0     1954 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/download_portal_file_response_all_of.py
--rw-r--r--   0        0        0     2724 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_autotuner_results.py
--rw-r--r--   0        0        0     2417 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
--rw-r--r--   0        0        0     1968 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
--rw-r--r--   0        0        0     2870 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_block.py
--rw-r--r--   0        0        0     1834 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_config_request.py
--rw-r--r--   0        0        0     3092 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_config_response.py
--rw-r--r--   0        0        0     2813 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_config_response_all_of.py
--rw-r--r--   0        0        0     3016 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_feature_importance_response.py
--rw-r--r--   0        0        0     2728 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
--rw-r--r--   0        0        0     2058 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
--rw-r--r--   0        0        0     2572 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
--rw-r--r--   0        0        0     2216 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_feature_labels_response.py
--rw-r--r--   0        0        0     1920 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
--rw-r--r--   0        0        0     2294 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_group.py
--rw-r--r--   0        0        0     3779 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_group_item.py
--rw-r--r--   0        0        0     2190 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
--rw-r--r--   0        0        0     2195 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_group_item_show_if.py
--rw-r--r--   0        0        0     4667 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_info.py
--rw-r--r--   0        0        0     2210 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_info_features.py
--rw-r--r--   0        0        0     1885 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_info_performance.py
--rw-r--r--   0        0        0     5144 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_metadata.py
--rw-r--r--   0        0        0     2025 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
--rw-r--r--   0        0        0     2566 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_metadata_output_config.py
--rw-r--r--   0        0        0     2531 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
--rw-r--r--   0        0        0     5502 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_metadata_response.py
--rw-r--r--   0        0        0     3019 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_performance_all_variants_response.py
--rw-r--r--   0        0        0     2729 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
--rw-r--r--   0        0        0     2278 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
--rw-r--r--   0        0        0     4639 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_graph.py
--rw-r--r--   0        0        0     1899 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
--rw-r--r--   0        0        0     2677 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_request_with_features.py
--rw-r--r--   0        0        0     2151 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_request_without_features.py
--rw-r--r--   0        0        0     2030 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
--rw-r--r--   0        0        0     3513 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_response.py
--rw-r--r--   0        0        0     3234 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_response_all_of.py
--rw-r--r--   0        0        0     1969 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
--rw-r--r--   0        0        0     4142 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_response_with_sample.py
--rw-r--r--   0        0        0     3875 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
--rw-r--r--   0        0        0     3342 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_sample_features_response.py
--rw-r--r--   0        0        0     3042 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
--rw-r--r--   0        0        0     2748 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
--rw-r--r--   0        0        0     2213 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
--rw-r--r--   0        0        0     3353 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_trained_features_response.py
--rw-r--r--   0        0        0     3053 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2773 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0     2205 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
--rw-r--r--   0        0        0     1893 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/edit_sample_label_request.py
--rw-r--r--   0        0        0     3697 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/enterprise_trial.py
--rw-r--r--   0        0        0     2397 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/entitlement_limits.py
--rw-r--r--   0        0        0     2178 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/entity_created_response.py
--rw-r--r--   0        0        0     2656 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/evaluate_job_response.py
--rw-r--r--   0        0        0     2349 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/evaluate_job_response_all_of.py
--rw-r--r--   0        0        0     2099 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/evaluate_result_value.py
--rw-r--r--   0        0        0     2511 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/export_get_url_response.py
--rw-r--r--   0        0        0     2244 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/export_get_url_response_all_of.py
--rw-r--r--   0        0        0     2116 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/export_keras_block_data_request.py
--rw-r--r--   0        0        0     2373 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/export_original_data_request.py
--rw-r--r--   0        0        0     2021 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/export_wav_data_request.py
--rw-r--r--   0        0        0     2206 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_segment_sample_request.py
--rw-r--r--   0        0        0     2804 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_segment_sample_response.py
--rw-r--r--   0        0        0     2497 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_segment_sample_response_all_of.py
--rw-r--r--   0        0        0     2090 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
--rw-r--r--   0        0        0     2665 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_user_response.py
--rw-r--r--   0        0        0     2358 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_user_response_all_of.py
--rw-r--r--   0        0        0     2322 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_user_response_all_of_users.py
--rw-r--r--   0        0        0     2507 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/generate_features_request.py
--rw-r--r--   0        0        0     2083 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/generic_api_response.py
--rw-r--r--   0        0        0     2764 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_imported_from_response.py
--rw-r--r--   0        0        0     2457 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
--rw-r--r--   0        0        0     2156 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
--rw-r--r--   0        0        0     2698 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_third_party_auth_response.py
--rw-r--r--   0        0        0     2391 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     2713 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_whitelabels_response.py
--rw-r--r--   0        0        0     2406 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
--rw-r--r--   0        0        0     3385 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_auto_segmenter_response.py
--rw-r--r--   0        0        0     3108 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_auto_segmenter_response_all_of.py
--rw-r--r--   0        0        0     2610 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_auto_segmenter_response_all_of_clusters.py
--rw-r--r--   0        0        0     1968 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_auto_segmenter_response_all_of_items.py
--rw-r--r--   0        0        0     3400 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_data_explorer_features_response.py
--rw-r--r--   0        0        0     3122 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0     3752 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_data_explorer_settings_response.py
--rw-r--r--   0        0        0     2402 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
--rw-r--r--   0        0        0     2349 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_deployment_response.py
--rw-r--r--   0        0        0     2071 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_deployment_response_all_of.py
--rw-r--r--   0        0        0     2434 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_device_response.py
--rw-r--r--   0        0        0     2137 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_device_response_all_of.py
--rw-r--r--   0        0        0     2752 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_diversity_data_response.py
--rw-r--r--   0        0        0     2455 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_diversity_data_response_all_of.py
--rw-r--r--   0        0        0     4226 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py
--rw-r--r--   0        0        0     2859 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py
--rw-r--r--   0        0        0     3930 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_impulse_blocks_response.py
--rw-r--r--   0        0        0     3630 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
--rw-r--r--   0        0        0     2454 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_impulse_response.py
--rw-r--r--   0        0        0     2157 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_impulse_response_all_of.py
--rw-r--r--   0        0        0     2374 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_job_response.py
--rw-r--r--   0        0        0     2077 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_job_response_all_of.py
--rw-r--r--   0        0        0     2650 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_jwt_request.py
--rw-r--r--   0        0        0     2431 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_jwt_response.py
--rw-r--r--   0        0        0     2152 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_jwt_response_all_of.py
--rw-r--r--   0        0        0     2977 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_last_deployment_build_response.py
--rw-r--r--   0        0        0     2699 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
--rw-r--r--   0        0        0     2869 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
--rw-r--r--   0        0        0     2572 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_notes_response.py
--rw-r--r--   0        0        0     2265 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_notes_response_all_of.py
--rw-r--r--   0        0        0     2701 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2377 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     2890 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
--rw-r--r--   0        0        0     2583 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
--rw-r--r--   0        0        0     3158 2023-07-23 14:02:10.645144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2939 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaigns_response.py
--rw-r--r--   0        0        0     2632 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
--rw-r--r--   0        0        0     2921 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
--rw-r--r--   0        0        0     2561 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_item_response.py
--rw-r--r--   0        0        0     2237 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
--rw-r--r--   0        0        0     3411 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
--rw-r--r--   0        0        0     3111 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
--rw-r--r--   0        0        0     3398 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
--rw-r--r--   0        0        0     2576 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_dataset_response.py
--rw-r--r--   0        0        0     2252 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
--rw-r--r--   0        0        0     2603 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_pipelines_response.py
--rw-r--r--   0        0        0     2279 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     3670 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_portal_response.py
--rw-r--r--   0        0        0     3391 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2323 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_projects_data_count_response.py
--rw-r--r--   0        0        0     2905 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
--rw-r--r--   0        0        0     2598 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
--rw-r--r--   0        0        0     3012 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
--rw-r--r--   0        0        0     2712 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
--rw-r--r--   0        0        0     2722 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
--rw-r--r--   0        0        0     2425 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
--rw-r--r--   0        0        0     2922 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
--rw-r--r--   0        0        0     2615 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
--rw-r--r--   0        0        0     3151 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_status_response.py
--rw-r--r--   0        0        0     2884 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
--rw-r--r--   0        0        0     3761 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_pretrained_model_response.py
--rw-r--r--   0        0        0     3483 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     3861 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
--rw-r--r--   0        0        0     2978 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
--rw-r--r--   0        0        0     3058 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
--rw-r--r--   0        0        0     2397 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_public_metrics_response.py
--rw-r--r--   0        0        0     2073 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_public_metrics_response_all_of.py
--rw-r--r--   0        0        0     2767 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_sample_metadata_response.py
--rw-r--r--   0        0        0     3044 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_sample_response.py
--rw-r--r--   0        0        0     2462 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_syntiant_posterior_response.py
--rw-r--r--   0        0        0     2184 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
--rw-r--r--   0        0        0     2414 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_theme_response.py
--rw-r--r--   0        0        0     2117 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_theme_response_all_of.py
--rw-r--r--   0        0        0     2592 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_themes_response.py
--rw-r--r--   0        0        0     2285 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_themes_response_all_of.py
--rw-r--r--   0        0        0     2495 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_third_party_auth_response.py
--rw-r--r--   0        0        0     2171 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     2703 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_user_need_to_set_password_response.py
--rw-r--r--   0        0        0     2436 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
--rw-r--r--   0        0        0     7717 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_user_response.py
--rw-r--r--   0        0        0     5708 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_user_response_all_of.py
--rw-r--r--   0        0        0     2395 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
--rw-r--r--   0        0        0     2307 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_whitelabel_domain_response.py
--rw-r--r--   0        0        0     2021 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
--rw-r--r--   0        0        0     2514 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_whitelabel_response.py
--rw-r--r--   0        0        0     2217 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2776 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/has_data_explorer_features_response.py
--rw-r--r--   0        0        0     2498 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0      526 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/image_input_scaling.py
--rw-r--r--   0        0        0     3738 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/impulse.py
--rw-r--r--   0        0        0     6723 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/impulse_block_version.py
--rw-r--r--   0        0        0     6814 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/impulse_dsp_block.py
--rw-r--r--   0        0        0     1967 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/impulse_dsp_block_organization.py
--rw-r--r--   0        0        0     8958 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/impulse_input_block.py
--rw-r--r--   0        0        0     5612 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/impulse_learn_block.py
--rw-r--r--   0        0        0     2445 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/input_block.py
--rw-r--r--   0        0        0     2323 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/invite_organization_member_request.py
--rw-r--r--   0        0        0     3668 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job.py
--rw-r--r--   0        0        0     4699 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_details.py
--rw-r--r--   0        0        0     2736 2023-07-23 14:02:10.649144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_details_all_of.py
--rw-r--r--   0        0        0     2613 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_details_response.py
--rw-r--r--   0        0        0     2316 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_details_response_all_of.py
--rw-r--r--   0        0        0     2257 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_failure_details.py
--rw-r--r--   0        0        0     2657 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_logs_response.py
--rw-r--r--   0        0        0     2350 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_logs_response_all_of.py
--rw-r--r--   0        0        0     3297 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_metrics_response.py
--rw-r--r--   0        0        0     3007 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_metrics_response_all_of.py
--rw-r--r--   0        0        0      516 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_parent_type_enum.py
--rw-r--r--   0        0        0     2944 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_state.py
--rw-r--r--   0        0        0     1966 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_state_execution_details.py
--rw-r--r--   0        0        0     2965 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_step.py
--rw-r--r--   0        0        0     2713 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_summary_response.py
--rw-r--r--   0        0        0     2406 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_summary_response_all_of.py
--rw-r--r--   0        0        0     2089 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_summary_response_all_of_summary.py
--rw-r--r--   0        0        0     2510 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_layer.py
--rw-r--r--   0        0        0     2093 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_layer_input.py
--rw-r--r--   0        0        0     2101 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_layer_output.py
--rw-r--r--   0        0        0     5431 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_metadata.py
--rw-r--r--   0        0        0     5164 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_metadata_all_of.py
--rw-r--r--   0        0        0     4792 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_metadata_metrics.py
--rw-r--r--   0        0        0     3228 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
--rw-r--r--   0        0        0     2497 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
--rw-r--r--   0        0        0      562 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_type_enum.py
--rw-r--r--   0        0        0     9842 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_response.py
--rw-r--r--   0        0        0     9575 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_response_all_of.py
--rw-r--r--   0        0        0     3392 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_visual_layer.py
--rw-r--r--   0        0        0     2310 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_visual_layer_type.py
--rw-r--r--   0        0        0     2529 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/last_modification_date_response.py
--rw-r--r--   0        0        0     2239 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/last_modification_date_response_all_of.py
--rw-r--r--   0        0        0     2633 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/latency_device.py
--rw-r--r--   0        0        0     2424 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/learn_block.py
--rw-r--r--   0        0        0      883 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/learn_block_type.py
--rw-r--r--   0        0        0     2788 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_api_keys_response.py
--rw-r--r--   0        0        0     2488 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2682 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2630 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_devices_response.py
--rw-r--r--   0        0        0     2333 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_devices_response_all_of.py
--rw-r--r--   0        0        0     2726 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_email_response.py
--rw-r--r--   0        0        0     2426 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_email_response_all_of.py
--rw-r--r--   0        0        0     2918 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_email_response_all_of_emails.py
--rw-r--r--   0        0        0     2813 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_hmac_keys_response.py
--rw-r--r--   0        0        0     2513 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
--rw-r--r--   0        0        0     2381 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
--rw-r--r--   0        0        0     2745 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_jobs_response.py
--rw-r--r--   0        0        0     2445 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_jobs_response_all_of.py
--rw-r--r--   0        0        0     2200 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_models_response.py
--rw-r--r--   0        0        0     1910 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_models_response_all_of.py
--rw-r--r--   0        0        0     2921 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_api_keys_response.py
--rw-r--r--   0        0        0     2621 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2760 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2857 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_buckets_response.py
--rw-r--r--   0        0        0     2550 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
--rw-r--r--   0        0        0     2995 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py
--rw-r--r--   0        0        0     2902 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_buckets_user_response.py
--rw-r--r--   0        0        0     2595 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
--rw-r--r--   0        0        0     2760 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
--rw-r--r--   0        0        0     3310 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_data_response.py
--rw-r--r--   0        0        0     3031 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_data_response_all_of.py
--rw-r--r--   0        0        0     3430 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
--rw-r--r--   0        0        0     2887 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
--rw-r--r--   0        0        0     2587 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
--rw-r--r--   0        0        0     2824 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
--rw-r--r--   0        0        0     2524 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
--rw-r--r--   0        0        0     3353 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_files_response.py
--rw-r--r--   0        0        0     3074 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_files_response_all_of.py
--rw-r--r--   0        0        0     2792 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_pipelines_response.py
--rw-r--r--   0        0        0     2485 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     2857 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_portals_response.py
--rw-r--r--   0        0        0     2550 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_portals_response_all_of.py
--rw-r--r--   0        0        0     2744 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
--rw-r--r--   0        0        0     3449 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_projects_data_response.py
--rw-r--r--   0        0        0     3142 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
--rw-r--r--   0        0        0     2271 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
--rw-r--r--   0        0        0     2723 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_projects_response.py
--rw-r--r--   0        0        0     2416 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_projects_response_all_of.py
--rw-r--r--   0        0        0     2857 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_secrets_response.py
--rw-r--r--   0        0        0     2550 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
--rw-r--r--   0        0        0     2265 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
--rw-r--r--   0        0        0     3103 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
--rw-r--r--   0        0        0     2803 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
--rw-r--r--   0        0        0     3055 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
--rw-r--r--   0        0        0     2755 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
--rw-r--r--   0        0        0     2786 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organizations_response.py
--rw-r--r--   0        0        0     2486 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organizations_response_all_of.py
--rw-r--r--   0        0        0     1937 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_portal_files_in_folder_request.py
--rw-r--r--   0        0        0     2713 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_portal_files_in_folder_response.py
--rw-r--r--   0        0        0     2416 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
--rw-r--r--   0        0        0     2290 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_projects.py
--rw-r--r--   0        0        0     2681 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_projects_response.py
--rw-r--r--   0        0        0     2553 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_public_projects.py
--rw-r--r--   0        0        0     2944 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_public_projects_response.py
--rw-r--r--   0        0        0     2815 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_public_versions_response.py
--rw-r--r--   0        0        0     2508 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_public_versions_response_all_of.py
--rw-r--r--   0        0        0     2290 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2754 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_samples_response.py
--rw-r--r--   0        0        0     2454 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_samples_response_all_of.py
--rw-r--r--   0        0        0     3933 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_versions_response.py
--rw-r--r--   0        0        0     3633 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_versions_response_all_of.py
--rw-r--r--   0        0        0     2353 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
--rw-r--r--   0        0        0     2053 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
--rw-r--r--   0        0        0     3960 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2900 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/log_stdout_response.py
--rw-r--r--   0        0        0     2600 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/log_stdout_response_all_of.py
--rw-r--r--   0        0        0     2441 2023-07-23 14:02:10.653144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
--rw-r--r--   0        0        0     2191 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/log_website_pageview_request.py
--rw-r--r--   0        0        0     2217 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/login_response.py
--rw-r--r--   0        0        0     1911 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/login_response_all_of.py
--rw-r--r--   0        0        0     2430 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/migration.py
--rw-r--r--   0        0        0     2521 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/model_prediction.py
--rw-r--r--   0        0        0     2895 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/model_result.py
--rw-r--r--   0        0        0     5046 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/model_variant_stats.py
--rw-r--r--   0        0        0     2128 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/move_raw_data_request.py
--rw-r--r--   0        0        0     2687 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/note.py
--rw-r--r--   0        0        0     2221 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_auto_label_request.py
--rw-r--r--   0        0        0     2994 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_auto_label_response.py
--rw-r--r--   0        0        0     2705 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
--rw-r--r--   0        0        0     2275 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
--rw-r--r--   0        0        0     2368 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_label_queue_count_response.py
--rw-r--r--   0        0        0     2051 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
--rw-r--r--   0        0        0     2887 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_label_queue_response.py
--rw-r--r--   0        0        0     2580 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
--rw-r--r--   0        0        0      621 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_last_layer.py
--rw-r--r--   0        0        0     6418 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_config.py
--rw-r--r--   0        0        0     6871 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_config_response.py
--rw-r--r--   0        0        0     1920 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_config_response_all_of.py
--rw-r--r--   0        0        0     2067 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_config_target_device.py
--rw-r--r--   0        0        0     2271 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_dsp_parameters_response.py
--rw-r--r--   0        0        0     1964 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
--rw-r--r--   0        0        0     2756 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_space_response.py
--rw-r--r--   0        0        0     2456 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_space_response_all_of.py
--rw-r--r--   0        0        0     4897 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_state_response.py
--rw-r--r--   0        0        0     4618 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_state_response_all_of.py
--rw-r--r--   0        0        0     3419 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_state_response_all_of_status.py
--rw-r--r--   0        0        0     2366 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
--rw-r--r--   0        0        0     2760 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
--rw-r--r--   0        0        0     2463 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
--rw-r--r--   0        0        0     4717 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
--rw-r--r--   0        0        0     4594 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization.py
--rw-r--r--   0        0        0     2359 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_add_data_folder_request.py
--rw-r--r--   0        0        0     2498 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_add_data_folder_response.py
--rw-r--r--   0        0        0     2209 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
--rw-r--r--   0        0        0     2549 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_add_dataset_request.py
--rw-r--r--   0        0        0     2460 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
--rw-r--r--   0        0        0     8598 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project.py
--rw-r--r--   0        0        0     5422 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_request.py
--rw-r--r--   0        0        0     2543 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_response.py
--rw-r--r--   0        0        0     2237 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_response_all_of.py
--rw-r--r--   0        0        0     2704 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_status_response.py
--rw-r--r--   0        0        0     2407 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
--rw-r--r--   0        0        0     2501 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_transformation_summary.py
--rw-r--r--   0        0        0     9493 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_with_files.py
--rw-r--r--   0        0        0     2744 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
--rw-r--r--   0        0        0     3034 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
--rw-r--r--   0        0        0     2559 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_campaign_diff_request.py
--rw-r--r--   0        0        0     2327 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
--rw-r--r--   0        0        0     3041 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_campaign_diff_response.py
--rw-r--r--   0        0        0     2741 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
--rw-r--r--   0        0        0     2468 2023-07-23 14:02:10.657143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
--rw-r--r--   0        0        0     3476 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_item.py
--rw-r--r--   0        0        0     2303 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_item_files_inner.py
--rw-r--r--   0        0        0     3529 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_dataset.py
--rw-r--r--   0        0        0     2767 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_dataset_bucket.py
--rw-r--r--   0        0        0     4689 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_deploy_block.py
--rw-r--r--   0        0        0     3646 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_dsp_block.py
--rw-r--r--   0        0        0     3037 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_get_create_projects_response.py
--rw-r--r--   0        0        0     2737 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
--rw-r--r--   0        0        0     5707 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
--rw-r--r--   0        0        0     6331 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_info_response.py
--rw-r--r--   0        0        0     6041 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_info_response_all_of.py
--rw-r--r--   0        0        0     3915 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
--rw-r--r--   0        0        0     2267 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
--rw-r--r--   0        0        0     2338 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
--rw-r--r--   0        0        0     2458 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
--rw-r--r--   0        0        0      525 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_member_role.py
--rw-r--r--   0        0        0     2639 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_metrics_response.py
--rw-r--r--   0        0        0     2315 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_metrics_response_all_of.py
--rw-r--r--   0        0        0     3453 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
--rw-r--r--   0        0        0     6132 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline.py
--rw-r--r--   0        0        0     2595 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
--rw-r--r--   0        0        0     2275 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
--rw-r--r--   0        0        0     2314 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline_item_count.py
--rw-r--r--   0        0        0     4109 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline_run.py
--rw-r--r--   0        0        0     5330 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline_run_step.py
--rw-r--r--   0        0        0     4930 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline_step.py
--rw-r--r--   0        0        0     2351 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
--rw-r--r--   0        0        0     2344 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
--rw-r--r--   0        0        0     2037 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_projects_data_batch_request.py
--rw-r--r--   0        0        0     5146 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_transfer_learning_block.py
--rw-r--r--   0        0        0      611 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
--rw-r--r--   0        0        0     6142 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_transformation_block.py
--rw-r--r--   0        0        0     3907 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_update_pipeline_body.py
--rw-r--r--   0        0        0     4225 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_user.py
--rw-r--r--   0        0        0     2294 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_user_all_of.py
--rw-r--r--   0        0        0     2104 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_detection.py
--rw-r--r--   0        0        0     3434 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_false_positive.py
--rw-r--r--   0        0        0     3770 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_ground_truth.py
--rw-r--r--   0        0        0     2477 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
--rw-r--r--   0        0        0     4880 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_parameter_set.py
--rw-r--r--   0        0        0     2255 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
--rw-r--r--   0        0        0     4092 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
--rw-r--r--   0        0        0     3007 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_parameters.py
--rw-r--r--   0        0        0     2585 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_parameters_standard.py
--rw-r--r--   0        0        0     2250 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_raw_detection.py
--rw-r--r--   0        0        0     2366 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
--rw-r--r--   0        0        0     2412 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
--rw-r--r--   0        0        0     2106 2023-07-23 14:02:10.661143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
--rw-r--r--   0        0        0     1629 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/permission.py
--rw-r--r--   0        0        0     2211 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/portal_file.py
--rw-r--r--   0        0        0     2413 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/portal_info_response.py
--rw-r--r--   0        0        0     2666 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/pretrained_model_tensor.py
--rw-r--r--   0        0        0     2955 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_info.py
--rw-r--r--   0        0        0     2640 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_info_memory.py
--rw-r--r--   0        0        0     1918 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_info_memory_eon.py
--rw-r--r--   0        0        0     2065 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_info_memory_tflite.py
--rw-r--r--   0        0        0     4335 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_table.py
--rw-r--r--   0        0        0     2780 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_table_mcu.py
--rw-r--r--   0        0        0     2565 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_table_mcu_memory.py
--rw-r--r--   0        0        0     2250 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_table_mpu.py
--rw-r--r--   0        0        0     2201 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_tf_lite_request.py
--rw-r--r--   0        0        0     3292 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_tf_lite_response.py
--rw-r--r--   0        0        0     6139 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project.py
--rw-r--r--   0        0        0     3888 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_collaborator.py
--rw-r--r--   0        0        0     1895 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_collaborator_all_of.py
--rw-r--r--   0        0        0     2416 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_data_axes_summary_response.py
--rw-r--r--   0        0        0     2116 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
--rw-r--r--   0        0        0     2281 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_data_interval_response.py
--rw-r--r--   0        0        0     1964 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_data_interval_response_all_of.py
--rw-r--r--   0        0        0     2235 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_data_summary.py
--rw-r--r--   0        0        0     6854 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_deployment_target.py
--rw-r--r--   0        0        0     2706 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_deployment_target_all_of.py
--rw-r--r--   0        0        0     2780 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_deployment_targets_response.py
--rw-r--r--   0        0        0     2473 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     2680 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_downloads_response.py
--rw-r--r--   0        0        0     2373 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_downloads_response_all_of.py
--rw-r--r--   0        0        0    13550 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response.py
--rw-r--r--   0        0        0    13283 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of.py
--rw-r--r--   0        0        0     3130 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
--rw-r--r--   0        0        0     2723 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
--rw-r--r--   0        0        0     2997 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
--rw-r--r--   0        0        0     2979 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
--rw-r--r--   0        0        0     2339 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_experiments.py
--rw-r--r--   0        0        0     2285 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_impulse.py
--rw-r--r--   0        0        0     2726 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_performance.py
--rw-r--r--   0        0        0     1977 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_readme.py
--rw-r--r--   0        0        0     2225 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
--rw-r--r--   0        0        0     2735 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_urls.py
--rw-r--r--   0        0        0     2478 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_summary_response.py
--rw-r--r--   0        0        0     2172 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_summary_response_all_of.py
--rw-r--r--   0        0        0     3554 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_private_data.py
--rw-r--r--   0        0        0     4127 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_public_data.py
--rw-r--r--   0        0        0     1928 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_public_data_readme.py
--rw-r--r--   0        0        0     2404 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_sample_metadata.py
--rw-r--r--   0        0        0     2670 2023-07-23 14:02:10.665143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_training_data_summary_response.py
--rw-r--r--   0        0        0     2353 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
--rw-r--r--   0        0        0      606 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_type.py
--rw-r--r--   0        0        0     2316 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_version_request.py
--rw-r--r--   0        0        0     2664 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/raw_sample_data.py
--rw-r--r--   0        0        0     3440 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/raw_sample_payload.py
--rw-r--r--   0        0        0     2537 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/rebalance_dataset_response.py
--rw-r--r--   0        0        0     1984 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/remove_collaborator_request.py
--rw-r--r--   0        0        0     1805 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/remove_member_request.py
--rw-r--r--   0        0        0     1867 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/rename_device_request.py
--rw-r--r--   0        0        0     2081 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/rename_portal_file_request.py
--rw-r--r--   0        0        0     1867 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/rename_sample_request.py
--rw-r--r--   0        0        0     1873 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/request_reset_password_request.py
--rw-r--r--   0        0        0     2031 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/reset_password_request.py
--rw-r--r--   0        0        0     1985 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/restore_project_from_public_request.py
--rw-r--r--   0        0        0     2265 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/restore_project_request.py
--rw-r--r--   0        0        0     2244 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/run_auto_segmenter_request.py
--rw-r--r--   0        0        0     2669 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/run_organization_pipeline_response.py
--rw-r--r--   0        0        0     2352 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
--rw-r--r--   0        0        0     9841 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/sample.py
--rw-r--r--   0        0        0     2443 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/sample_bounding_boxes_request.py
--rw-r--r--   0        0        0     2000 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/sample_metadata.py
--rw-r--r--   0        0        0     2539 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/save_auto_segmenter_clusters_request.py
--rw-r--r--   0        0        0     2085 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/save_auto_segmenter_clusters_request_clusters_inner.py
--rw-r--r--   0        0        0     2355 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/save_auto_segmenter_clusters_response.py
--rw-r--r--   0        0        0     2038 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/save_auto_segmenter_clusters_response_all_of.py
--rw-r--r--   0        0        0     2756 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/save_pretrained_model_request.py
--rw-r--r--   0        0        0     3327 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/score_trial_response.py
--rw-r--r--   0        0        0     3003 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/score_trial_response_all_of.py
--rw-r--r--   0        0        0     2240 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/score_trial_response_all_of_latency.py
--rw-r--r--   0        0        0     1914 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/score_trial_response_all_of_ram.py
--rw-r--r--   0        0        0     2405 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/segment_sample_request.py
--rw-r--r--   0        0        0     2055 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/segment_sample_request_segments_inner.py
--rw-r--r--   0        0        0     3364 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/send_user_feedback_request.py
--rw-r--r--   0        0        0     1981 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/sensor.py
--rw-r--r--   0        0        0     2142 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_anomaly_parameter_request.py
--rw-r--r--   0        0        0     8028 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_keras_parameter_request.py
--rw-r--r--   0        0        0     1893 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_member_datasets_request.py
--rw-r--r--   0        0        0     1905 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_member_role_request.py
--rw-r--r--   0        0        0     2219 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_optimize_space_request.py
--rw-r--r--   0        0        0     2254 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_optimize_space_request_all_of.py
--rw-r--r--   0        0        0     1923 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_organization_data_dataset_request.py
--rw-r--r--   0        0        0     1974 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_project_compute_time_request.py
--rw-r--r--   0        0        0     2011 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_project_dsp_file_size_request.py
--rw-r--r--   0        0        0     1919 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_sample_metadata_request.py
--rw-r--r--   0        0        0     1915 2023-07-23 14:02:10.669144 edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_syntiant_posterior_request.py
--rw-r--r--   0        0        0     2140 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_user_password_request.py
--rw-r--r--   0        0        0     2536 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/socket_token_response.py
--rw-r--r--   0        0        0     2239 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/socket_token_response_all_of.py
--rw-r--r--   0        0        0     2059 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/socket_token_response_all_of_token.py
--rw-r--r--   0        0        0     1971 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/split_sample_in_frames_request.py
--rw-r--r--   0        0        0     2110 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/staff_info.py
--rw-r--r--   0        0        0     2226 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_job_response.py
--rw-r--r--   0        0        0     1909 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_job_response_all_of.py
--rw-r--r--   0        0        0     2883 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_performance_calibration_request.py
--rw-r--r--   0        0        0     2838 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_sampling_request.py
--rw-r--r--   0        0        0     2189 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_sampling_response.py
--rw-r--r--   0        0        0     1892 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_sampling_response_all_of.py
--rw-r--r--   0        0        0     2795 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_training_request_anomaly.py
--rw-r--r--   0        0        0     1967 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/store_segment_length_request.py
--rw-r--r--   0        0        0     3460 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/structured_classify_result.py
--rw-r--r--   0        0        0     2433 2023-07-23 14:02:10.673143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/test_pretrained_model_request.py
--rw-r--r--   0        0        0     3074 2023-07-23 14:02:10.677143 edgeimpulse_api-1.25.34/edgeimpulse_api/models/test_pretrained_model_response.py
--rw-r--r--   0        0        0     2784 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     3251 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/theme.py
--rw-r--r--   0        0        0     2239 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/theme_colors.py
--rw-r--r--   0        0        0     2764 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/theme_favicon.py
--rw-r--r--   0        0        0     2721 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/theme_logos.py
--rw-r--r--   0        0        0     2245 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/third_party_auth.py
--rw-r--r--   0        0        0     1921 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/time_series_data_point.py
--rw-r--r--   0        0        0     2031 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/track_objects_request.py
--rw-r--r--   0        0        0     2736 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/track_objects_response.py
--rw-r--r--   0        0        0     2436 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/track_objects_response_all_of.py
--rw-r--r--   0        0        0     5295 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/transfer_learning_model.py
--rw-r--r--   0        0        0     2012 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/transfer_ownership_organization_request.py
--rw-r--r--   0        0        0     2585 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/transformation_block_additional_mount_point.py
--rw-r--r--   0        0        0      588 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/transformation_job_status_enum.py
--rw-r--r--   0        0        0     2578 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/tuner_create_trial_impulse.py
--rw-r--r--   0        0        0     2570 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/tuner_space_impulse.py
--rw-r--r--   0        0        0     4257 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/tuner_trial.py
--rw-r--r--   0        0        0     2304 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/tuner_trial_blocks_inner.py
--rw-r--r--   0        0        0     1935 2023-07-23 14:02:10.785142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
--rw-r--r--   0        0        0     2028 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_job_request.py
--rw-r--r--   0        0        0     2281 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_add_collaborator_request.py
--rw-r--r--   0        0        0     2882 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_bucket_request.py
--rw-r--r--   0        0        0     2578 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_create_empty_project_request.py
--rw-r--r--   0        0        0     2428 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_create_project_request.py
--rw-r--r--   0        0        0     2764 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     4154 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2158 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_data_item_request.py
--rw-r--r--   0        0        0     2624 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_dataset_request.py
--rw-r--r--   0        0        0     2881 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2724 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_portal_response.py
--rw-r--r--   0        0        0     2445 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2582 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_request.py
--rw-r--r--   0        0        0     4664 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     5010 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_transformation_block_request.py
--rw-r--r--   0        0        0     8081 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_project_request.py
--rw-r--r--   0        0        0     1877 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_project_tags_request.py
--rw-r--r--   0        0        0     2259 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_theme_colors_request.py
--rw-r--r--   0        0        0     2895 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_theme_logos_request.py
--rw-r--r--   0        0        0     2205 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_third_party_auth_request.py
--rw-r--r--   0        0        0     2603 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_user_request.py
--rw-r--r--   0        0        0     1886 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_version_request.py
--rw-r--r--   0        0        0     2393 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
--rw-r--r--   0        0        0     2237 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
--rw-r--r--   0        0        0     2125 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
--rw-r--r--   0        0        0     2059 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_whitelabel_request.py
--rw-r--r--   0        0        0     2168 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/upload_asset_response.py
--rw-r--r--   0        0        0     1882 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/upload_asset_response_all_of.py
--rw-r--r--   0        0        0     2199 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/upload_readme_image_response.py
--rw-r--r--   0        0        0     2185 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/upload_user_photo_response.py
--rw-r--r--   0        0        0     1872 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/upload_user_photo_response_all_of.py
--rw-r--r--   0        0        0     3673 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/user.py
--rw-r--r--   0        0        0     1991 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/user_by_third_party_activation_request.py
--rw-r--r--   0        0        0     2192 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/user_experiment.py
--rw-r--r--   0        0        0     3200 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/user_organization.py
--rw-r--r--   0        0        0     1844 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_dsp_block_url_request.py
--rw-r--r--   0        0        0     2604 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_dsp_block_url_response.py
--rw-r--r--   0        0        0     2307 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
--rw-r--r--   0        0        0     2407 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
--rw-r--r--   0        0        0     2708 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_organization_bucket_request.py
--rw-r--r--   0        0        0     2897 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_organization_bucket_response.py
--rw-r--r--   0        0        0     2597 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
--rw-r--r--   0        0        0     2187 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
--rw-r--r--   0        0        0     1937 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_reset_password_request.py
--rw-r--r--   0        0        0     5887 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/whitelabel.py
--rw-r--r--   0        0        0     2534 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
--rw-r--r--   0        0        0     2120 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
--rw-r--r--   0        0        0     2885 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/window_settings_response.py
--rw-r--r--   0        0        0     2585 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/window_settings_response_all_of.py
--rw-r--r--   0        0        0     2848 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
--rw-r--r--   0        0        0    12674 2023-07-23 14:02:10.789142 edgeimpulse_api-1.25.34/edgeimpulse_api/rest.py
--rw-r--r--   0        0        0      968 2023-07-23 14:02:37.188862 edgeimpulse_api-1.25.34/pyproject.toml
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 edgeimpulse_api-1.25.34/PKG-INFO
+-rw-r--r--   0        0        0      377 2023-07-25 06:13:55.591702 edgeimpulse_api-1.26.0/README.md
+-rw-r--r--   0        0        0    77366 2023-07-25 06:14:22.751816 edgeimpulse_api-1.26.0/edgeimpulse_api/__init__.py
+-rw-r--r--   0        0        0     3004 2023-07-25 06:13:55.591702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/__init__.py
+-rw-r--r--   0        0        0   280031 2023-07-25 06:13:55.591702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/admin_api.py
+-rw-r--r--   0        0        0   303232 2023-07-25 06:13:55.591702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/allows_read_only_api.py
+-rw-r--r--   0        0        0    11231 2023-07-25 06:13:55.591702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/auth_api.py
+-rw-r--r--   0        0        0     6235 2023-07-25 06:13:55.591702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/cdn_api.py
+-rw-r--r--   0        0        0    28575 2023-07-25 06:13:55.591702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/classify_api.py
+-rw-r--r--   0        0        0     7426 2023-07-25 06:13:55.591702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/content_disposition_inline_api.py
+-rw-r--r--   0        0        0    72480 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/deployment_api.py
+-rw-r--r--   0        0        0    38974 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/devices_api.py
+-rw-r--r--   0        0        0   131256 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/dsp_api.py
+-rw-r--r--   0        0        0    19442 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/email_verification_api.py
+-rw-r--r--   0        0        0     6435 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/export_api.py
+-rw-r--r--   0        0        0    11921 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/health_api.py
+-rw-r--r--   0        0        0    49621 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/impulse_api.py
+-rw-r--r--   0        0        0   239208 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/jobs_api.py
+-rw-r--r--   0        0        0   147712 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/learn_api.py
+-rw-r--r--   0        0        0     6483 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/login_api.py
+-rw-r--r--   0        0        0    12006 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/metrics_api.py
+-rw-r--r--   0        0        0    67457 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/optimization_api.py
+-rw-r--r--   0        0        0   300920 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_allow_developer_profile_api.py
+-rw-r--r--   0        0        0    63140 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_allow_guest_access_api.py
+-rw-r--r--   0        0        0   141131 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_blocks_api.py
+-rw-r--r--   0        0        0    91908 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_create_project_api.py
+-rw-r--r--   0        0        0   255365 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_data_api.py
+-rw-r--r--   0        0        0    80882 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_data_campaigns_api.py
+-rw-r--r--   0        0        0    58218 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_jobs_api.py
+-rw-r--r--   0        0        0    47178 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_pipelines_api.py
+-rw-r--r--   0        0        0    45490 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_portals_api.py
+-rw-r--r--   0        0        0   266354 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_requires_admin_api.py
+-rw-r--r--   0        0        0   176301 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py
+-rw-r--r--   0        0        0   307148 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/organizations_api.py
+-rw-r--r--   0        0        0    54671 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/performance_calibration_api.py
+-rw-r--r--   0        0        0    12662 2023-07-25 06:13:55.595702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/project_requires_admin_api.py
+-rw-r--r--   0        0        0   228112 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/projects_api.py
+-rw-r--r--   0        0        0   378158 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/raw_data_api.py
+-rw-r--r--   0        0        0    24481 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/requires_sudo_api.py
+-rw-r--r--   0        0        0     7730 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py
+-rw-r--r--   0        0        0    13690 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/supports_range_api.py
+-rw-r--r--   0        0        0    35671 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/themes_api.py
+-rw-r--r--   0        0        0    43486 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/third_party_auth_api.py
+-rw-r--r--   0        0        0    45393 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/upload_portal_api.py
+-rw-r--r--   0        0        0   223338 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/user_api.py
+-rw-r--r--   0        0        0    42135 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/api/whitelabels_api.py
+-rw-r--r--   0        0        0    29331 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/api_client.py
+-rw-r--r--   0        0        0    15659 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/configuration.py
+-rw-r--r--   0        0        0     5113 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/exceptions.py
+-rw-r--r--   0        0        0    73909 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/__init__.py
+-rw-r--r--   0        0        0     2897 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
+-rw-r--r--   0        0        0     1982 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/activate_user_or_verify_email_request.py
+-rw-r--r--   0        0        0     2610 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_api_key_request.py
+-rw-r--r--   0        0        0     1963 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_collaborator_request.py
+-rw-r--r--   0        0        0     2223 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_hmac_key_request.py
+-rw-r--r--   0        0        0     2299 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_member_request.py
+-rw-r--r--   0        0        0     2418 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_api_key_request.py
+-rw-r--r--   0        0        0     2806 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_bucket_request.py
+-rw-r--r--   0        0        0     2656 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     2469 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2152 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     4230 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2359 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2042 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
+-rw-r--r--   0        0        0     2269 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_deploy_block_response.py
+-rw-r--r--   0        0        0     2816 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2248 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_dsp_block_response.py
+-rw-r--r--   0        0        0     2054 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_secret_request.py
+-rw-r--r--   0        0        0     2266 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_secret_response.py
+-rw-r--r--   0        0        0     1949 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_secret_response_all_of.py
+-rw-r--r--   0        0        0     4588 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     2339 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
+-rw-r--r--   0        0        0     4868 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_transformation_block_request.py
+-rw-r--r--   0        0        0     2325 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_transformation_block_response.py
+-rw-r--r--   0        0        0     2001 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
+-rw-r--r--   0        0        0     1940 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
+-rw-r--r--   0        0        0     1961 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
+-rw-r--r--   0        0        0     2542 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_add_organization_user_request.py
+-rw-r--r--   0        0        0     2246 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
+-rw-r--r--   0        0        0     2146 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_add_project_user_request.py
+-rw-r--r--   0        0        0     2097 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_add_user_request.py
+-rw-r--r--   0        0        0     4696 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_api_organization.py
+-rw-r--r--   0        0        0     2396 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_api_organization_all_of.py
+-rw-r--r--   0        0        0     3459 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_api_project.py
+-rw-r--r--   0        0        0     7260 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_api_user.py
+-rw-r--r--   0        0        0     5706 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_api_user_all_of.py
+-rw-r--r--   0        0        0     2262 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_create_organization_request.py
+-rw-r--r--   0        0        0     1905 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_enable_feature_request.py
+-rw-r--r--   0        0        0     2546 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_data_migration_response.py
+-rw-r--r--   0        0        0     2222 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
+-rw-r--r--   0        0        0     2735 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_data_migrations_response.py
+-rw-r--r--   0        0        0     2428 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
+-rw-r--r--   0        0        0     2318 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
+-rw-r--r--   0        0        0     2022 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
+-rw-r--r--   0        0        0     2844 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_feature_flags_response.py
+-rw-r--r--   0        0        0     2544 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_feature_flags_response_all_of.py
+-rw-r--r--   0        0        0     2153 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_feature_flags_response_all_of_flags.py
+-rw-r--r--   0        0        0     2217 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_metrics_response.py
+-rw-r--r--   0        0        0     1910 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3046 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_organizations_response.py
+-rw-r--r--   0        0        0     2746 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
+-rw-r--r--   0        0        0     3409 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
+-rw-r--r--   0        0        0     2243 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
+-rw-r--r--   0        0        0     1947 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
+-rw-r--r--   0        0        0     2914 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_sso_settings_response.py
+-rw-r--r--   0        0        0     2614 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
+-rw-r--r--   0        0        0     2096 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
+-rw-r--r--   0        0        0     2208 2023-07-25 06:13:55.599702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_ids_response.py
+-rw-r--r--   0        0        0     1901 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
+-rw-r--r--   0        0        0     2245 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_metrics_response.py
+-rw-r--r--   0        0        0     2452 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_response.py
+-rw-r--r--   0        0        0     2128 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_response_all_of.py
+-rw-r--r--   0        0        0     2507 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_trial_response.py
+-rw-r--r--   0        0        0     2183 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py
+-rw-r--r--   0        0        0     2807 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_users_response.py
+-rw-r--r--   0        0        0     2500 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_users_response_all_of.py
+-rw-r--r--   0        0        0     3087 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
+-rw-r--r--   0        0        0     2445 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_list_projects.py
+-rw-r--r--   0        0        0     2836 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_list_projects_response.py
+-rw-r--r--   0        0        0     7695 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_organization_info_response.py
+-rw-r--r--   0        0        0     3752 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_organization_info_response_all_of.py
+-rw-r--r--   0        0        0     2158 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_toggle_data_migration_request.py
+-rw-r--r--   0        0        0     3269 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_update_organization_request.py
+-rw-r--r--   0        0        0     2015 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_update_user_permissions_request.py
+-rw-r--r--   0        0        0     2661 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_update_user_request.py
+-rw-r--r--   0        0        0     2532 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_update_user_trial_request.py
+-rw-r--r--   0        0        0     2525 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/akida_edge_learning_config.py
+-rw-r--r--   0        0        0     5499 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_model_metadata.py
+-rw-r--r--   0        0        0     5221 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
+-rw-r--r--   0        0        0     2151 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
+-rw-r--r--   0        0        0     4079 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_response.py
+-rw-r--r--   0        0        0     3812 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_response_all_of.py
+-rw-r--r--   0        0        0     2044 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_response_all_of_axes.py
+-rw-r--r--   0        0        0     3029 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_trained_features_response.py
+-rw-r--r--   0        0        0     2729 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2375 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0      506 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/augmentation_policy_image_enum.py
+-rw-r--r--   0        0        0     3635 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/augmentation_policy_spectrogram.py
+-rw-r--r--   0        0        0     1895 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/autotune_dsp_request.py
+-rw-r--r--   0        0        0     2044 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/bounding_box.py
+-rw-r--r--   0        0        0     2151 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/bounding_box_with_score.py
+-rw-r--r--   0        0        0     2197 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/build_on_device_model_request.py
+-rw-r--r--   0        0        0     2433 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/build_organization_on_device_model_request.py
+-rw-r--r--   0        0        0     2459 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/calculate_data_quality_metrics_request.py
+-rw-r--r--   0        0        0     2041 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/change_password_request.py
+-rw-r--r--   0        0        0     3701 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_job_response.py
+-rw-r--r--   0        0        0     3394 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_job_response_all_of.py
+-rw-r--r--   0        0        0     3769 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
+-rw-r--r--   0        0        0     2055 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
+-rw-r--r--   0        0        0     3255 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_job_response_page.py
+-rw-r--r--   0        0        0     2948 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_job_response_page_all_of.py
+-rw-r--r--   0        0        0     3932 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_sample_response.py
+-rw-r--r--   0        0        0     3644 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_sample_response_all_of.py
+-rw-r--r--   0        0        0     4783 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_sample_response_classification.py
+-rw-r--r--   0        0        0     2755 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_sample_response_classification_details.py
+-rw-r--r--   0        0        0     3004 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/convert_user_request.py
+-rw-r--r--   0        0        0     2183 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/count_samples_response.py
+-rw-r--r--   0        0        0     1859 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/count_samples_response_all_of.py
+-rw-r--r--   0        0        0     2255 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_block_version_response.py
+-rw-r--r--   0        0        0     1938 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_block_version_response_all_of.py
+-rw-r--r--   0        0        0     2404 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_developer_profile_response.py
+-rw-r--r--   0        0        0     2125 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_developer_profile_response_all_of.py
+-rw-r--r--   0        0        0     2387 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_device_request.py
+-rw-r--r--   0        0        0     2850 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_enterprise_trial_response.py
+-rw-r--r--   0        0        0     2319 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py
+-rw-r--r--   0        0        0     5405 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_enterprise_trial_user_request.py
+-rw-r--r--   0        0        0     3321 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py
+-rw-r--r--   0        0        0     2491 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_evaluation_user_response.py
+-rw-r--r--   0        0        0     2185 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
+-rw-r--r--   0        0        0     2600 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_organization_portal_request.py
+-rw-r--r--   0        0        0     2830 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_organization_portal_response.py
+-rw-r--r--   0        0        0     2551 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     1990 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_organization_request.py
+-rw-r--r--   0        0        0     2454 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_organization_response.py
+-rw-r--r--   0        0        0     2148 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_organization_response_all_of.py
+-rw-r--r--   0        0        0     2185 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_pipeline_response.py
+-rw-r--r--   0        0        0     2254 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_project_request.py
+-rw-r--r--   0        0        0     2378 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_project_response.py
+-rw-r--r--   0        0        0     2072 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_project_response_all_of.py
+-rw-r--r--   0        0        0     2276 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_signed_upload_link_request.py
+-rw-r--r--   0        0        0     2414 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_signed_upload_link_response.py
+-rw-r--r--   0        0        0     2135 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
+-rw-r--r--   0        0        0     2413 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_third_party_auth_request.py
+-rw-r--r--   0        0        0     2450 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_third_party_auth_response.py
+-rw-r--r--   0        0        0     2144 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     4000 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_user_request.py
+-rw-r--r--   0        0        0     2393 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_user_response.py
+-rw-r--r--   0        0        0     2114 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_user_response_all_of.py
+-rw-r--r--   0        0        0     2919 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_user_third_party_request.py
+-rw-r--r--   0        0        0     2672 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_user_third_party_response.py
+-rw-r--r--   0        0        0     2393 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_user_third_party_response_all_of.py
+-rw-r--r--   0        0        0     4157 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_whitelabel_request.py
+-rw-r--r--   0        0        0     2438 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_whitelabel_response.py
+-rw-r--r--   0        0        0     2121 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2051 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/crop_sample_request.py
+-rw-r--r--   0        0        0     2248 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/crop_sample_response.py
+-rw-r--r--   0        0        0     1943 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/crop_sample_response_all_of.py
+-rw-r--r--   0        0        0     4054 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign.py
+-rw-r--r--   0        0        0     2851 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign_dashboard.py
+-rw-r--r--   0        0        0     2786 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign_graph.py
+-rw-r--r--   0        0        0     3352 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
+-rw-r--r--   0        0        0     2047 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
+-rw-r--r--   0        0        0     1934 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign_link.py
+-rw-r--r--   0        0        0     1957 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign_query.py
+-rw-r--r--   0        0        0     3292 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_explorer_predictions_response.py
+-rw-r--r--   0        0        0     3003 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
+-rw-r--r--   0        0        0     2838 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_explorer_settings.py
+-rw-r--r--   0        0        0     2149 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dataset_ratio_data.py
+-rw-r--r--   0        0        0     2111 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dataset_ratio_data_ratio.py
+-rw-r--r--   0        0        0     1898 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/delete_portal_file_request.py
+-rw-r--r--   0        0        0     2230 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dependency_data.py
+-rw-r--r--   0        0        0     2280 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
+-rw-r--r--   0        0        0     2408 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
+-rw-r--r--   0        0        0     2155 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
+-rw-r--r--   0        0        0     2484 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
+-rw-r--r--   0        0        0     2344 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
+-rw-r--r--   0        0        0     2780 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
+-rw-r--r--   0        0        0     2200 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
+-rw-r--r--   0        0        0     4355 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_request.py
+-rw-r--r--   0        0        0     2833 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
+-rw-r--r--   0        0        0     8503 2023-07-25 06:13:55.603702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
+-rw-r--r--   0        0        0     8065 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
+-rw-r--r--   0        0        0     5950 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deployment_target.py
+-rw-r--r--   0        0        0     1926 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deployment_target_badge.py
+-rw-r--r--   0        0        0      679 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deployment_target_engine.py
+-rw-r--r--   0        0        0     2702 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deployment_targets_response.py
+-rw-r--r--   0        0        0     2395 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     1983 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/development_board.py
+-rw-r--r--   0        0        0     2831 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/development_boards_response.py
+-rw-r--r--   0        0        0     2531 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/development_boards_response_all_of.py
+-rw-r--r--   0        0        0     2030 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/development_keys.py
+-rw-r--r--   0        0        0     2400 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/development_keys_response.py
+-rw-r--r--   0        0        0     3677 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/device.py
+-rw-r--r--   0        0        0     2199 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/device_name_response.py
+-rw-r--r--   0        0        0     1920 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/device_name_response_all_of.py
+-rw-r--r--   0        0        0     2231 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/device_sensors_inner.py
+-rw-r--r--   0        0        0     2094 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/download.py
+-rw-r--r--   0        0        0     1912 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/download_portal_file_request.py
+-rw-r--r--   0        0        0     2260 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/download_portal_file_response.py
+-rw-r--r--   0        0        0     1954 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/download_portal_file_response_all_of.py
+-rw-r--r--   0        0        0     2724 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_autotuner_results.py
+-rw-r--r--   0        0        0     2417 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
+-rw-r--r--   0        0        0     1968 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
+-rw-r--r--   0        0        0     2870 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_block.py
+-rw-r--r--   0        0        0     1834 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_config_request.py
+-rw-r--r--   0        0        0     3092 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_config_response.py
+-rw-r--r--   0        0        0     2813 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_config_response_all_of.py
+-rw-r--r--   0        0        0     3016 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_feature_importance_response.py
+-rw-r--r--   0        0        0     2728 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
+-rw-r--r--   0        0        0     2058 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
+-rw-r--r--   0        0        0     2572 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
+-rw-r--r--   0        0        0     2216 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_feature_labels_response.py
+-rw-r--r--   0        0        0     1920 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
+-rw-r--r--   0        0        0     2294 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_group.py
+-rw-r--r--   0        0        0     3779 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_group_item.py
+-rw-r--r--   0        0        0     2190 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
+-rw-r--r--   0        0        0     2195 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_group_item_show_if.py
+-rw-r--r--   0        0        0     4667 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_info.py
+-rw-r--r--   0        0        0     2210 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_info_features.py
+-rw-r--r--   0        0        0     1885 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_info_performance.py
+-rw-r--r--   0        0        0     5144 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_metadata.py
+-rw-r--r--   0        0        0     2025 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
+-rw-r--r--   0        0        0     2566 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_metadata_output_config.py
+-rw-r--r--   0        0        0     2531 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
+-rw-r--r--   0        0        0     5502 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_metadata_response.py
+-rw-r--r--   0        0        0     3019 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_performance_all_variants_response.py
+-rw-r--r--   0        0        0     2729 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
+-rw-r--r--   0        0        0     2278 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
+-rw-r--r--   0        0        0     4639 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_graph.py
+-rw-r--r--   0        0        0     1899 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
+-rw-r--r--   0        0        0     2677 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_request_with_features.py
+-rw-r--r--   0        0        0     2151 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_request_without_features.py
+-rw-r--r--   0        0        0     2030 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
+-rw-r--r--   0        0        0     3513 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_response.py
+-rw-r--r--   0        0        0     3234 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_response_all_of.py
+-rw-r--r--   0        0        0     1969 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
+-rw-r--r--   0        0        0     4142 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_response_with_sample.py
+-rw-r--r--   0        0        0     3875 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
+-rw-r--r--   0        0        0     3342 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_sample_features_response.py
+-rw-r--r--   0        0        0     3042 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
+-rw-r--r--   0        0        0     2748 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2213 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     3353 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_trained_features_response.py
+-rw-r--r--   0        0        0     3053 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2773 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2205 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     1893 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/edit_sample_label_request.py
+-rw-r--r--   0        0        0     3886 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/enterprise_trial.py
+-rw-r--r--   0        0        0     2741 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py
+-rw-r--r--   0        0        0     2397 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/entitlement_limits.py
+-rw-r--r--   0        0        0     2367 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/entity_created_response.py
+-rw-r--r--   0        0        0     2077 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/entity_created_response_all_of.py
+-rw-r--r--   0        0        0     2656 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/evaluate_job_response.py
+-rw-r--r--   0        0        0     2349 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/evaluate_job_response_all_of.py
+-rw-r--r--   0        0        0     2099 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/evaluate_result_value.py
+-rw-r--r--   0        0        0     2511 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/export_get_url_response.py
+-rw-r--r--   0        0        0     2244 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/export_get_url_response_all_of.py
+-rw-r--r--   0        0        0     2116 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/export_keras_block_data_request.py
+-rw-r--r--   0        0        0     2373 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/export_original_data_request.py
+-rw-r--r--   0        0        0     2021 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/export_wav_data_request.py
+-rw-r--r--   0        0        0      490 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/feature.py
+-rw-r--r--   0        0        0     2206 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_segment_sample_request.py
+-rw-r--r--   0        0        0     2804 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_segment_sample_response.py
+-rw-r--r--   0        0        0     2497 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_segment_sample_response_all_of.py
+-rw-r--r--   0        0        0     2090 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
+-rw-r--r--   0        0        0     2665 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_user_response.py
+-rw-r--r--   0        0        0     2358 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_user_response_all_of.py
+-rw-r--r--   0        0        0     2322 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_user_response_all_of_users.py
+-rw-r--r--   0        0        0     2507 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/generate_features_request.py
+-rw-r--r--   0        0        0     2083 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/generic_api_response.py
+-rw-r--r--   0        0        0     2764 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_imported_from_response.py
+-rw-r--r--   0        0        0     2457 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
+-rw-r--r--   0        0        0     2156 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
+-rw-r--r--   0        0        0     2698 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_third_party_auth_response.py
+-rw-r--r--   0        0        0     2391 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     2713 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_whitelabels_response.py
+-rw-r--r--   0        0        0     2406 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
+-rw-r--r--   0        0        0     3385 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_auto_segmenter_response.py
+-rw-r--r--   0        0        0     3108 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_auto_segmenter_response_all_of.py
+-rw-r--r--   0        0        0     2610 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_auto_segmenter_response_all_of_clusters.py
+-rw-r--r--   0        0        0     1968 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_auto_segmenter_response_all_of_items.py
+-rw-r--r--   0        0        0     3400 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_data_explorer_features_response.py
+-rw-r--r--   0        0        0     3122 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0     3752 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_data_explorer_settings_response.py
+-rw-r--r--   0        0        0     2402 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
+-rw-r--r--   0        0        0     2349 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_deployment_response.py
+-rw-r--r--   0        0        0     2071 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_deployment_response_all_of.py
+-rw-r--r--   0        0        0     2434 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_device_response.py
+-rw-r--r--   0        0        0     2137 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_device_response_all_of.py
+-rw-r--r--   0        0        0     2752 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_diversity_data_response.py
+-rw-r--r--   0        0        0     2455 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_diversity_data_response_all_of.py
+-rw-r--r--   0        0        0     4226 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py
+-rw-r--r--   0        0        0     2859 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2350 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_email_verification_status_response.py
+-rw-r--r--   0        0        0     2045 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_email_verification_status_response_all_of.py
+-rw-r--r--   0        0        0     3930 2023-07-25 06:13:55.607702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_impulse_blocks_response.py
+-rw-r--r--   0        0        0     3630 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2454 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_impulse_response.py
+-rw-r--r--   0        0        0     2157 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_impulse_response_all_of.py
+-rw-r--r--   0        0        0     2374 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_job_response.py
+-rw-r--r--   0        0        0     2077 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_job_response_all_of.py
+-rw-r--r--   0        0        0     2650 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_jwt_request.py
+-rw-r--r--   0        0        0     2431 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_jwt_response.py
+-rw-r--r--   0        0        0     2152 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_jwt_response_all_of.py
+-rw-r--r--   0        0        0     2977 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_last_deployment_build_response.py
+-rw-r--r--   0        0        0     2699 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
+-rw-r--r--   0        0        0     2869 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
+-rw-r--r--   0        0        0     2572 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_notes_response.py
+-rw-r--r--   0        0        0     2265 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_notes_response_all_of.py
+-rw-r--r--   0        0        0     2701 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2377 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     2890 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
+-rw-r--r--   0        0        0     2583 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
+-rw-r--r--   0        0        0     3158 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2939 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaigns_response.py
+-rw-r--r--   0        0        0     2632 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
+-rw-r--r--   0        0        0     2921 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
+-rw-r--r--   0        0        0     2561 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_item_response.py
+-rw-r--r--   0        0        0     2237 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
+-rw-r--r--   0        0        0     3411 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
+-rw-r--r--   0        0        0     3111 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
+-rw-r--r--   0        0        0     3398 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
+-rw-r--r--   0        0        0     2576 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_dataset_response.py
+-rw-r--r--   0        0        0     2252 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
+-rw-r--r--   0        0        0     2603 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2279 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     3670 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_portal_response.py
+-rw-r--r--   0        0        0     3391 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2323 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_projects_data_count_response.py
+-rw-r--r--   0        0        0     2905 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
+-rw-r--r--   0        0        0     2598 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
+-rw-r--r--   0        0        0     3012 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
+-rw-r--r--   0        0        0     2712 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
+-rw-r--r--   0        0        0     2722 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
+-rw-r--r--   0        0        0     2425 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2922 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
+-rw-r--r--   0        0        0     2615 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
+-rw-r--r--   0        0        0     3151 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_status_response.py
+-rw-r--r--   0        0        0     2884 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
+-rw-r--r--   0        0        0     3761 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_pretrained_model_response.py
+-rw-r--r--   0        0        0     3483 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     3861 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
+-rw-r--r--   0        0        0     2978 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
+-rw-r--r--   0        0        0     3058 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
+-rw-r--r--   0        0        0     2397 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_public_metrics_response.py
+-rw-r--r--   0        0        0     2073 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_public_metrics_response_all_of.py
+-rw-r--r--   0        0        0     2767 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_sample_metadata_response.py
+-rw-r--r--   0        0        0     3044 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_sample_response.py
+-rw-r--r--   0        0        0     2462 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_syntiant_posterior_response.py
+-rw-r--r--   0        0        0     2184 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
+-rw-r--r--   0        0        0     2414 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_theme_response.py
+-rw-r--r--   0        0        0     2117 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_theme_response_all_of.py
+-rw-r--r--   0        0        0     2592 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_themes_response.py
+-rw-r--r--   0        0        0     2285 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_themes_response_all_of.py
+-rw-r--r--   0        0        0     2495 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_third_party_auth_response.py
+-rw-r--r--   0        0        0     2171 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     3543 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_user_need_to_set_password_response.py
+-rw-r--r--   0        0        0     3276 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
+-rw-r--r--   0        0        0     7717 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_user_response.py
+-rw-r--r--   0        0        0     5708 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_user_response_all_of.py
+-rw-r--r--   0        0        0     2395 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
+-rw-r--r--   0        0        0     2307 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_whitelabel_domain_response.py
+-rw-r--r--   0        0        0     2021 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
+-rw-r--r--   0        0        0     2514 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_whitelabel_response.py
+-rw-r--r--   0        0        0     2217 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2776 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/has_data_explorer_features_response.py
+-rw-r--r--   0        0        0     2498 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0      526 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/image_input_scaling.py
+-rw-r--r--   0        0        0     3738 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/impulse.py
+-rw-r--r--   0        0        0     6723 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/impulse_block_version.py
+-rw-r--r--   0        0        0     6814 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/impulse_dsp_block.py
+-rw-r--r--   0        0        0     1967 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/impulse_dsp_block_organization.py
+-rw-r--r--   0        0        0     8958 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/impulse_input_block.py
+-rw-r--r--   0        0        0     5612 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/impulse_learn_block.py
+-rw-r--r--   0        0        0     2445 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/input_block.py
+-rw-r--r--   0        0        0     2323 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/invite_organization_member_request.py
+-rw-r--r--   0        0        0     3668 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job.py
+-rw-r--r--   0        0        0     4699 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_details.py
+-rw-r--r--   0        0        0     2736 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_details_all_of.py
+-rw-r--r--   0        0        0     2613 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_details_response.py
+-rw-r--r--   0        0        0     2316 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_details_response_all_of.py
+-rw-r--r--   0        0        0     2257 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_failure_details.py
+-rw-r--r--   0        0        0     2657 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_logs_response.py
+-rw-r--r--   0        0        0     2350 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_logs_response_all_of.py
+-rw-r--r--   0        0        0     3297 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_metrics_response.py
+-rw-r--r--   0        0        0     3007 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_metrics_response_all_of.py
+-rw-r--r--   0        0        0      516 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_parent_type_enum.py
+-rw-r--r--   0        0        0     2944 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_state.py
+-rw-r--r--   0        0        0     1966 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_state_execution_details.py
+-rw-r--r--   0        0        0     2965 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_step.py
+-rw-r--r--   0        0        0     2713 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_summary_response.py
+-rw-r--r--   0        0        0     2406 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_summary_response_all_of.py
+-rw-r--r--   0        0        0     2089 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_summary_response_all_of_summary.py
+-rw-r--r--   0        0        0     2510 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_layer.py
+-rw-r--r--   0        0        0     2093 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_layer_input.py
+-rw-r--r--   0        0        0     2101 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_layer_output.py
+-rw-r--r--   0        0        0     5431 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_metadata.py
+-rw-r--r--   0        0        0     5164 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_metadata_all_of.py
+-rw-r--r--   0        0        0     4792 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_metadata_metrics.py
+-rw-r--r--   0        0        0     3228 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
+-rw-r--r--   0        0        0     2497 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
+-rw-r--r--   0        0        0      562 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_type_enum.py
+-rw-r--r--   0        0        0     9842 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_response.py
+-rw-r--r--   0        0        0     9575 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_response_all_of.py
+-rw-r--r--   0        0        0     3392 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_visual_layer.py
+-rw-r--r--   0        0        0     2310 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_visual_layer_type.py
+-rw-r--r--   0        0        0     2529 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/last_modification_date_response.py
+-rw-r--r--   0        0        0     2239 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/last_modification_date_response_all_of.py
+-rw-r--r--   0        0        0     2633 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/latency_device.py
+-rw-r--r--   0        0        0     2424 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/learn_block.py
+-rw-r--r--   0        0        0      883 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/learn_block_type.py
+-rw-r--r--   0        0        0     2788 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_api_keys_response.py
+-rw-r--r--   0        0        0     2488 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2682 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2630 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_devices_response.py
+-rw-r--r--   0        0        0     2333 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_devices_response_all_of.py
+-rw-r--r--   0        0        0     2726 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_email_response.py
+-rw-r--r--   0        0        0     2426 2023-07-25 06:13:55.611702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_email_response_all_of.py
+-rw-r--r--   0        0        0     2918 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_email_response_all_of_emails.py
+-rw-r--r--   0        0        0     2767 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_enterprise_trials_response.py
+-rw-r--r--   0        0        0     2467 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py
+-rw-r--r--   0        0        0     2813 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_hmac_keys_response.py
+-rw-r--r--   0        0        0     2513 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
+-rw-r--r--   0        0        0     2381 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
+-rw-r--r--   0        0        0     2745 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_jobs_response.py
+-rw-r--r--   0        0        0     2445 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_jobs_response_all_of.py
+-rw-r--r--   0        0        0     2200 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_models_response.py
+-rw-r--r--   0        0        0     1910 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_models_response_all_of.py
+-rw-r--r--   0        0        0     2921 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_api_keys_response.py
+-rw-r--r--   0        0        0     2621 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2760 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2857 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_buckets_response.py
+-rw-r--r--   0        0        0     2550 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
+-rw-r--r--   0        0        0     2995 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py
+-rw-r--r--   0        0        0     2902 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_buckets_user_response.py
+-rw-r--r--   0        0        0     2595 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
+-rw-r--r--   0        0        0     2760 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
+-rw-r--r--   0        0        0     3310 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_data_response.py
+-rw-r--r--   0        0        0     3031 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_data_response_all_of.py
+-rw-r--r--   0        0        0     3430 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2887 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
+-rw-r--r--   0        0        0     2587 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2824 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
+-rw-r--r--   0        0        0     2524 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3353 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_files_response.py
+-rw-r--r--   0        0        0     3074 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_files_response_all_of.py
+-rw-r--r--   0        0        0     2792 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2485 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     2857 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_portals_response.py
+-rw-r--r--   0        0        0     2550 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_portals_response_all_of.py
+-rw-r--r--   0        0        0     2744 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
+-rw-r--r--   0        0        0     3449 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_projects_data_response.py
+-rw-r--r--   0        0        0     3142 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
+-rw-r--r--   0        0        0     2271 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
+-rw-r--r--   0        0        0     2723 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_projects_response.py
+-rw-r--r--   0        0        0     2416 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_projects_response_all_of.py
+-rw-r--r--   0        0        0     2857 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_secrets_response.py
+-rw-r--r--   0        0        0     2550 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
+-rw-r--r--   0        0        0     2265 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
+-rw-r--r--   0        0        0     3103 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
+-rw-r--r--   0        0        0     2803 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3055 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
+-rw-r--r--   0        0        0     2755 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2786 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organizations_response.py
+-rw-r--r--   0        0        0     2486 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organizations_response_all_of.py
+-rw-r--r--   0        0        0     1937 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_portal_files_in_folder_request.py
+-rw-r--r--   0        0        0     2713 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_portal_files_in_folder_response.py
+-rw-r--r--   0        0        0     2416 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
+-rw-r--r--   0        0        0     2290 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_projects.py
+-rw-r--r--   0        0        0     2681 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_projects_response.py
+-rw-r--r--   0        0        0     2553 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_public_projects.py
+-rw-r--r--   0        0        0     2944 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_public_projects_response.py
+-rw-r--r--   0        0        0     2815 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_public_versions_response.py
+-rw-r--r--   0        0        0     2508 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_public_versions_response_all_of.py
+-rw-r--r--   0        0        0     2290 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2754 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_samples_response.py
+-rw-r--r--   0        0        0     2454 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_samples_response_all_of.py
+-rw-r--r--   0        0        0     3933 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_versions_response.py
+-rw-r--r--   0        0        0     3633 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_versions_response_all_of.py
+-rw-r--r--   0        0        0     2353 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
+-rw-r--r--   0        0        0     2053 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
+-rw-r--r--   0        0        0     3960 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2900 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/log_stdout_response.py
+-rw-r--r--   0        0        0     2600 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/log_stdout_response_all_of.py
+-rw-r--r--   0        0        0     2441 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
+-rw-r--r--   0        0        0     2191 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/log_website_pageview_request.py
+-rw-r--r--   0        0        0     2217 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/login_response.py
+-rw-r--r--   0        0        0     1911 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/login_response_all_of.py
+-rw-r--r--   0        0        0     2430 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/migration.py
+-rw-r--r--   0        0        0     2521 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/model_prediction.py
+-rw-r--r--   0        0        0     2895 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/model_result.py
+-rw-r--r--   0        0        0     5046 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/model_variant_stats.py
+-rw-r--r--   0        0        0     2128 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/move_raw_data_request.py
+-rw-r--r--   0        0        0     2687 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/note.py
+-rw-r--r--   0        0        0     2221 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_auto_label_request.py
+-rw-r--r--   0        0        0     2994 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_auto_label_response.py
+-rw-r--r--   0        0        0     2705 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
+-rw-r--r--   0        0        0     2275 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
+-rw-r--r--   0        0        0     2368 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_label_queue_count_response.py
+-rw-r--r--   0        0        0     2051 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
+-rw-r--r--   0        0        0     2887 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_label_queue_response.py
+-rw-r--r--   0        0        0     2580 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
+-rw-r--r--   0        0        0      621 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_last_layer.py
+-rw-r--r--   0        0        0     6418 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_config.py
+-rw-r--r--   0        0        0     6871 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_config_response.py
+-rw-r--r--   0        0        0     1920 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_config_response_all_of.py
+-rw-r--r--   0        0        0     2067 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_config_target_device.py
+-rw-r--r--   0        0        0     2271 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_dsp_parameters_response.py
+-rw-r--r--   0        0        0     1964 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_space_response.py
+-rw-r--r--   0        0        0     2456 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_space_response_all_of.py
+-rw-r--r--   0        0        0     4897 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_state_response.py
+-rw-r--r--   0        0        0     4618 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_state_response_all_of.py
+-rw-r--r--   0        0        0     3419 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_state_response_all_of_status.py
+-rw-r--r--   0        0        0     2366 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
+-rw-r--r--   0        0        0     2760 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
+-rw-r--r--   0        0        0     2463 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
+-rw-r--r--   0        0        0     4717 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
+-rw-r--r--   0        0        0     4594 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization.py
+-rw-r--r--   0        0        0     2359 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_add_data_folder_request.py
+-rw-r--r--   0        0        0     2498 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_add_data_folder_response.py
+-rw-r--r--   0        0        0     2209 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
+-rw-r--r--   0        0        0     2549 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_add_dataset_request.py
+-rw-r--r--   0        0        0     2460 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
+-rw-r--r--   0        0        0     8598 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project.py
+-rw-r--r--   0        0        0     5422 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_request.py
+-rw-r--r--   0        0        0     2543 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_response.py
+-rw-r--r--   0        0        0     2237 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_response_all_of.py
+-rw-r--r--   0        0        0     2704 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_status_response.py
+-rw-r--r--   0        0        0     2407 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
+-rw-r--r--   0        0        0     2501 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_transformation_summary.py
+-rw-r--r--   0        0        0     9493 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_with_files.py
+-rw-r--r--   0        0        0     2744 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
+-rw-r--r--   0        0        0     3034 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
+-rw-r--r--   0        0        0     2559 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_campaign_diff_request.py
+-rw-r--r--   0        0        0     2327 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
+-rw-r--r--   0        0        0     3041 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_campaign_diff_response.py
+-rw-r--r--   0        0        0     2741 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
+-rw-r--r--   0        0        0     2468 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
+-rw-r--r--   0        0        0     3476 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_item.py
+-rw-r--r--   0        0        0     2303 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_item_files_inner.py
+-rw-r--r--   0        0        0     3529 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_dataset.py
+-rw-r--r--   0        0        0     2767 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_dataset_bucket.py
+-rw-r--r--   0        0        0     4689 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_deploy_block.py
+-rw-r--r--   0        0        0     3646 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_dsp_block.py
+-rw-r--r--   0        0        0     3037 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_get_create_projects_response.py
+-rw-r--r--   0        0        0     2737 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
+-rw-r--r--   0        0        0     5707 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
+-rw-r--r--   0        0        0     6331 2023-07-25 06:13:55.615702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_info_response.py
+-rw-r--r--   0        0        0     6041 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_info_response_all_of.py
+-rw-r--r--   0        0        0     3915 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
+-rw-r--r--   0        0        0     2267 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
+-rw-r--r--   0        0        0     2338 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
+-rw-r--r--   0        0        0     2458 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
+-rw-r--r--   0        0        0      525 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_member_role.py
+-rw-r--r--   0        0        0     2639 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_metrics_response.py
+-rw-r--r--   0        0        0     2315 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3453 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
+-rw-r--r--   0        0        0     6132 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline.py
+-rw-r--r--   0        0        0     2595 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
+-rw-r--r--   0        0        0     2275 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
+-rw-r--r--   0        0        0     2314 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline_item_count.py
+-rw-r--r--   0        0        0     4109 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline_run.py
+-rw-r--r--   0        0        0     5330 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline_run_step.py
+-rw-r--r--   0        0        0     4930 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline_step.py
+-rw-r--r--   0        0        0     2351 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
+-rw-r--r--   0        0        0     2344 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
+-rw-r--r--   0        0        0     2037 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_projects_data_batch_request.py
+-rw-r--r--   0        0        0     5146 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_transfer_learning_block.py
+-rw-r--r--   0        0        0      611 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
+-rw-r--r--   0        0        0     6142 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_transformation_block.py
+-rw-r--r--   0        0        0     3907 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_update_pipeline_body.py
+-rw-r--r--   0        0        0     4225 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_user.py
+-rw-r--r--   0        0        0     2294 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_user_all_of.py
+-rw-r--r--   0        0        0     2104 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_detection.py
+-rw-r--r--   0        0        0     3434 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_false_positive.py
+-rw-r--r--   0        0        0     3770 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_ground_truth.py
+-rw-r--r--   0        0        0     2477 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
+-rw-r--r--   0        0        0     4880 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_parameter_set.py
+-rw-r--r--   0        0        0     2255 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
+-rw-r--r--   0        0        0     4092 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
+-rw-r--r--   0        0        0     3007 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_parameters.py
+-rw-r--r--   0        0        0     2585 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_parameters_standard.py
+-rw-r--r--   0        0        0     2250 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_raw_detection.py
+-rw-r--r--   0        0        0     2366 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
+-rw-r--r--   0        0        0     2412 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
+-rw-r--r--   0        0        0     2106 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
+-rw-r--r--   0        0        0     1763 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/permission.py
+-rw-r--r--   0        0        0     2211 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/portal_file.py
+-rw-r--r--   0        0        0     2413 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/portal_info_response.py
+-rw-r--r--   0        0        0     2666 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/pretrained_model_tensor.py
+-rw-r--r--   0        0        0     2955 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_info.py
+-rw-r--r--   0        0        0     2640 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_info_memory.py
+-rw-r--r--   0        0        0     1918 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_info_memory_eon.py
+-rw-r--r--   0        0        0     2065 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_info_memory_tflite.py
+-rw-r--r--   0        0        0     4335 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_table.py
+-rw-r--r--   0        0        0     2780 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_table_mcu.py
+-rw-r--r--   0        0        0     2565 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_table_mcu_memory.py
+-rw-r--r--   0        0        0     2250 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_table_mpu.py
+-rw-r--r--   0        0        0     2201 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_tf_lite_request.py
+-rw-r--r--   0        0        0     3292 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_tf_lite_response.py
+-rw-r--r--   0        0        0     6139 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project.py
+-rw-r--r--   0        0        0     3888 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_collaborator.py
+-rw-r--r--   0        0        0     1895 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_collaborator_all_of.py
+-rw-r--r--   0        0        0     2416 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_data_axes_summary_response.py
+-rw-r--r--   0        0        0     2116 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
+-rw-r--r--   0        0        0     2281 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_data_interval_response.py
+-rw-r--r--   0        0        0     1964 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_data_interval_response_all_of.py
+-rw-r--r--   0        0        0     2235 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_data_summary.py
+-rw-r--r--   0        0        0     6854 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_deployment_target.py
+-rw-r--r--   0        0        0     2706 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_deployment_target_all_of.py
+-rw-r--r--   0        0        0     2780 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_deployment_targets_response.py
+-rw-r--r--   0        0        0     2473 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     2680 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_downloads_response.py
+-rw-r--r--   0        0        0     2373 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_downloads_response_all_of.py
+-rw-r--r--   0        0        0    13550 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response.py
+-rw-r--r--   0        0        0    13283 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of.py
+-rw-r--r--   0        0        0     3130 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
+-rw-r--r--   0        0        0     2723 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
+-rw-r--r--   0        0        0     2997 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
+-rw-r--r--   0        0        0     2979 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
+-rw-r--r--   0        0        0     2339 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_experiments.py
+-rw-r--r--   0        0        0     2285 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_impulse.py
+-rw-r--r--   0        0        0     2726 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_performance.py
+-rw-r--r--   0        0        0     1977 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_readme.py
+-rw-r--r--   0        0        0     2225 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
+-rw-r--r--   0        0        0     2735 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_urls.py
+-rw-r--r--   0        0        0     2478 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_summary_response.py
+-rw-r--r--   0        0        0     2172 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_summary_response_all_of.py
+-rw-r--r--   0        0        0     3554 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_private_data.py
+-rw-r--r--   0        0        0     4127 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_public_data.py
+-rw-r--r--   0        0        0     1928 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_public_data_readme.py
+-rw-r--r--   0        0        0     2404 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_sample_metadata.py
+-rw-r--r--   0        0        0     2670 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_training_data_summary_response.py
+-rw-r--r--   0        0        0     2353 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
+-rw-r--r--   0        0        0      606 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_type.py
+-rw-r--r--   0        0        0     2316 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_version_request.py
+-rw-r--r--   0        0        0     2664 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/raw_sample_data.py
+-rw-r--r--   0        0        0     3440 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/raw_sample_payload.py
+-rw-r--r--   0        0        0     2537 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/rebalance_dataset_response.py
+-rw-r--r--   0        0        0     1984 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/remove_collaborator_request.py
+-rw-r--r--   0        0        0     1805 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/remove_member_request.py
+-rw-r--r--   0        0        0     1867 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/rename_device_request.py
+-rw-r--r--   0        0        0     2081 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/rename_portal_file_request.py
+-rw-r--r--   0        0        0     1867 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/rename_sample_request.py
+-rw-r--r--   0        0        0     2028 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/request_email_verification_request.py
+-rw-r--r--   0        0        0     1873 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/request_reset_password_request.py
+-rw-r--r--   0        0        0     2031 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/reset_password_request.py
+-rw-r--r--   0        0        0     1985 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/restore_project_from_public_request.py
+-rw-r--r--   0        0        0     2265 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/restore_project_request.py
+-rw-r--r--   0        0        0     2244 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/run_auto_segmenter_request.py
+-rw-r--r--   0        0        0     2669 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/run_organization_pipeline_response.py
+-rw-r--r--   0        0        0     2352 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
+-rw-r--r--   0        0        0     9841 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/sample.py
+-rw-r--r--   0        0        0     2443 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/sample_bounding_boxes_request.py
+-rw-r--r--   0        0        0     2000 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/sample_metadata.py
+-rw-r--r--   0        0        0     2539 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/save_auto_segmenter_clusters_request.py
+-rw-r--r--   0        0        0     2085 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/save_auto_segmenter_clusters_request_clusters_inner.py
+-rw-r--r--   0        0        0     2355 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/save_auto_segmenter_clusters_response.py
+-rw-r--r--   0        0        0     2038 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/save_auto_segmenter_clusters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/save_pretrained_model_request.py
+-rw-r--r--   0        0        0     3327 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/score_trial_response.py
+-rw-r--r--   0        0        0     3003 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/score_trial_response_all_of.py
+-rw-r--r--   0        0        0     2240 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/score_trial_response_all_of_latency.py
+-rw-r--r--   0        0        0     1914 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/score_trial_response_all_of_ram.py
+-rw-r--r--   0        0        0     2405 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/segment_sample_request.py
+-rw-r--r--   0        0        0     2055 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/segment_sample_request_segments_inner.py
+-rw-r--r--   0        0        0     3364 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/send_user_feedback_request.py
+-rw-r--r--   0        0        0     1981 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/sensor.py
+-rw-r--r--   0        0        0     2142 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_anomaly_parameter_request.py
+-rw-r--r--   0        0        0     8028 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_keras_parameter_request.py
+-rw-r--r--   0        0        0     1893 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_member_datasets_request.py
+-rw-r--r--   0        0        0     1905 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_member_role_request.py
+-rw-r--r--   0        0        0     2219 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_optimize_space_request.py
+-rw-r--r--   0        0        0     2254 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_optimize_space_request_all_of.py
+-rw-r--r--   0        0        0     1923 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_organization_data_dataset_request.py
+-rw-r--r--   0        0        0     1974 2023-07-25 06:13:55.619702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_project_compute_time_request.py
+-rw-r--r--   0        0        0     2011 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_project_dsp_file_size_request.py
+-rw-r--r--   0        0        0     1919 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_sample_metadata_request.py
+-rw-r--r--   0        0        0     1915 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_syntiant_posterior_request.py
+-rw-r--r--   0        0        0     2140 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_user_password_request.py
+-rw-r--r--   0        0        0     2536 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/socket_token_response.py
+-rw-r--r--   0        0        0     2239 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/socket_token_response_all_of.py
+-rw-r--r--   0        0        0     2059 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/socket_token_response_all_of_token.py
+-rw-r--r--   0        0        0     1971 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/split_sample_in_frames_request.py
+-rw-r--r--   0        0        0     2110 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/staff_info.py
+-rw-r--r--   0        0        0     4421 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_enterprise_trial_request.py
+-rw-r--r--   0        0        0     2226 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_job_response.py
+-rw-r--r--   0        0        0     1909 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_job_response_all_of.py
+-rw-r--r--   0        0        0     2883 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_performance_calibration_request.py
+-rw-r--r--   0        0        0     2838 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_sampling_request.py
+-rw-r--r--   0        0        0     2189 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_sampling_response.py
+-rw-r--r--   0        0        0     1892 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_sampling_response_all_of.py
+-rw-r--r--   0        0        0     2795 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_training_request_anomaly.py
+-rw-r--r--   0        0        0     1967 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/store_segment_length_request.py
+-rw-r--r--   0        0        0     3460 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/structured_classify_result.py
+-rw-r--r--   0        0        0     2433 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/test_pretrained_model_request.py
+-rw-r--r--   0        0        0     3074 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/test_pretrained_model_response.py
+-rw-r--r--   0        0        0     2784 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     3251 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/theme.py
+-rw-r--r--   0        0        0     2239 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/theme_colors.py
+-rw-r--r--   0        0        0     2764 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/theme_favicon.py
+-rw-r--r--   0        0        0     2721 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/theme_logos.py
+-rw-r--r--   0        0        0     2245 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/third_party_auth.py
+-rw-r--r--   0        0        0     1921 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/time_series_data_point.py
+-rw-r--r--   0        0        0     2031 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/track_objects_request.py
+-rw-r--r--   0        0        0     2736 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/track_objects_response.py
+-rw-r--r--   0        0        0     2436 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/track_objects_response_all_of.py
+-rw-r--r--   0        0        0     5295 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/transfer_learning_model.py
+-rw-r--r--   0        0        0     2012 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/transfer_ownership_organization_request.py
+-rw-r--r--   0        0        0     2585 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/transformation_block_additional_mount_point.py
+-rw-r--r--   0        0        0      588 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/transformation_job_status_enum.py
+-rw-r--r--   0        0        0     2578 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/tuner_create_trial_impulse.py
+-rw-r--r--   0        0        0     2570 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/tuner_space_impulse.py
+-rw-r--r--   0        0        0     4257 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/tuner_trial.py
+-rw-r--r--   0        0        0     2304 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/tuner_trial_blocks_inner.py
+-rw-r--r--   0        0        0     1935 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
+-rw-r--r--   0        0        0     2028 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_job_request.py
+-rw-r--r--   0        0        0     2281 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_add_collaborator_request.py
+-rw-r--r--   0        0        0     2882 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_bucket_request.py
+-rw-r--r--   0        0        0     2578 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_create_empty_project_request.py
+-rw-r--r--   0        0        0     2428 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_create_project_request.py
+-rw-r--r--   0        0        0     2764 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     4154 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2158 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_data_item_request.py
+-rw-r--r--   0        0        0     2624 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_dataset_request.py
+-rw-r--r--   0        0        0     2881 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2724 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_portal_response.py
+-rw-r--r--   0        0        0     2445 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2582 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_request.py
+-rw-r--r--   0        0        0     4664 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     5010 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_transformation_block_request.py
+-rw-r--r--   0        0        0     8081 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_project_request.py
+-rw-r--r--   0        0        0     1877 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_project_tags_request.py
+-rw-r--r--   0        0        0     2259 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_theme_colors_request.py
+-rw-r--r--   0        0        0     2895 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_theme_logos_request.py
+-rw-r--r--   0        0        0     2205 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_third_party_auth_request.py
+-rw-r--r--   0        0        0     2603 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_user_request.py
+-rw-r--r--   0        0        0     1886 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_version_request.py
+-rw-r--r--   0        0        0     2393 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
+-rw-r--r--   0        0        0     2237 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
+-rw-r--r--   0        0        0     2125 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
+-rw-r--r--   0        0        0     2059 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_whitelabel_request.py
+-rw-r--r--   0        0        0     2168 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/upload_asset_response.py
+-rw-r--r--   0        0        0     1882 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/upload_asset_response_all_of.py
+-rw-r--r--   0        0        0     2199 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/upload_readme_image_response.py
+-rw-r--r--   0        0        0     2185 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/upload_user_photo_response.py
+-rw-r--r--   0        0        0     1872 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/upload_user_photo_response_all_of.py
+-rw-r--r--   0        0        0     3673 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/user.py
+-rw-r--r--   0        0        0     1991 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/user_by_third_party_activation_request.py
+-rw-r--r--   0        0        0     2192 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/user_experiment.py
+-rw-r--r--   0        0        0     3200 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/user_organization.py
+-rw-r--r--   0        0        0     1844 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_dsp_block_url_request.py
+-rw-r--r--   0        0        0     2604 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_dsp_block_url_response.py
+-rw-r--r--   0        0        0     2307 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
+-rw-r--r--   0        0        0     2407 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
+-rw-r--r--   0        0        0     2633 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_email_response.py
+-rw-r--r--   0        0        0     2354 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_email_response_all_of.py
+-rw-r--r--   0        0        0     2708 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_organization_bucket_request.py
+-rw-r--r--   0        0        0     2897 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_organization_bucket_response.py
+-rw-r--r--   0        0        0     2597 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
+-rw-r--r--   0        0        0     2187 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
+-rw-r--r--   0        0        0     1937 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_reset_password_request.py
+-rw-r--r--   0        0        0     5887 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/whitelabel.py
+-rw-r--r--   0        0        0     2534 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
+-rw-r--r--   0        0        0     2120 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
+-rw-r--r--   0        0        0     2885 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/window_settings_response.py
+-rw-r--r--   0        0        0     2585 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/window_settings_response_all_of.py
+-rw-r--r--   0        0        0     2848 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
+-rw-r--r--   0        0        0    12674 2023-07-25 06:13:55.623702 edgeimpulse_api-1.26.0/edgeimpulse_api/rest.py
+-rw-r--r--   0        0        0      967 2023-07-25 06:14:22.751816 edgeimpulse_api-1.26.0/pyproject.toml
+-rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 edgeimpulse_api-1.26.0/PKG-INFO
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/__init__.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,27 @@
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.25.34" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+__version__ = "1.26.0" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 
 # import apis into sdk package
 from edgeimpulse_api.api.admin_api import AdminApi
 from edgeimpulse_api.api.allows_read_only_api import AllowsReadOnlyApi
 from edgeimpulse_api.api.auth_api import AuthApi
 from edgeimpulse_api.api.cdn_api import CDNApi
 from edgeimpulse_api.api.classify_api import ClassifyApi
 from edgeimpulse_api.api.content_disposition_inline_api import ContentDispositionInlineApi
 from edgeimpulse_api.api.dsp_api import DSPApi
 from edgeimpulse_api.api.deployment_api import DeploymentApi
 from edgeimpulse_api.api.devices_api import DevicesApi
+from edgeimpulse_api.api.email_verification_api import EmailVerificationApi
 from edgeimpulse_api.api.export_api import ExportApi
 from edgeimpulse_api.api.health_api import HealthApi
 from edgeimpulse_api.api.impulse_api import ImpulseApi
 from edgeimpulse_api.api.jobs_api import JobsApi
 from edgeimpulse_api.api.learn_api import LearnApi
 from edgeimpulse_api.api.login_api import LoginApi
 from edgeimpulse_api.api.metrics_api import MetricsApi
@@ -66,15 +67,15 @@
 from edgeimpulse_api.exceptions import ApiTypeError
 from edgeimpulse_api.exceptions import ApiValueError
 from edgeimpulse_api.exceptions import ApiKeyError
 from edgeimpulse_api.exceptions import ApiAttributeError
 from edgeimpulse_api.exceptions import ApiException
 # import models into sdk package
 from edgeimpulse_api.models.activate_user_by_third_party_activation_code_request import ActivateUserByThirdPartyActivationCodeRequest
-from edgeimpulse_api.models.activate_user_request import ActivateUserRequest
+from edgeimpulse_api.models.activate_user_or_verify_email_request import ActivateUserOrVerifyEmailRequest
 from edgeimpulse_api.models.add_api_key_request import AddApiKeyRequest
 from edgeimpulse_api.models.add_collaborator_request import AddCollaboratorRequest
 from edgeimpulse_api.models.add_hmac_key_request import AddHmacKeyRequest
 from edgeimpulse_api.models.add_member_request import AddMemberRequest
 from edgeimpulse_api.models.add_organization_api_key_request import AddOrganizationApiKeyRequest
 from edgeimpulse_api.models.add_organization_bucket_request import AddOrganizationBucketRequest
 from edgeimpulse_api.models.add_organization_data_campaign_dashboard_request import AddOrganizationDataCampaignDashboardRequest
@@ -102,35 +103,37 @@
 from edgeimpulse_api.models.admin_add_user_request import AdminAddUserRequest
 from edgeimpulse_api.models.admin_api_organization import AdminApiOrganization
 from edgeimpulse_api.models.admin_api_organization_all_of import AdminApiOrganizationAllOf
 from edgeimpulse_api.models.admin_api_project import AdminApiProject
 from edgeimpulse_api.models.admin_api_user import AdminApiUser
 from edgeimpulse_api.models.admin_api_user_all_of import AdminApiUserAllOf
 from edgeimpulse_api.models.admin_create_organization_request import AdminCreateOrganizationRequest
-from edgeimpulse_api.models.admin_create_user_trial_request import AdminCreateUserTrialRequest
+from edgeimpulse_api.models.admin_enable_feature_request import AdminEnableFeatureRequest
 from edgeimpulse_api.models.admin_get_data_migration_response import AdminGetDataMigrationResponse
 from edgeimpulse_api.models.admin_get_data_migration_response_all_of import AdminGetDataMigrationResponseAllOf
 from edgeimpulse_api.models.admin_get_data_migrations_response import AdminGetDataMigrationsResponse
 from edgeimpulse_api.models.admin_get_data_migrations_response_all_of import AdminGetDataMigrationsResponseAllOf
 from edgeimpulse_api.models.admin_get_disallowed_email_domains_response import AdminGetDisallowedEmailDomainsResponse
 from edgeimpulse_api.models.admin_get_disallowed_email_domains_response_all_of import AdminGetDisallowedEmailDomainsResponseAllOf
+from edgeimpulse_api.models.admin_get_feature_flags_response import AdminGetFeatureFlagsResponse
+from edgeimpulse_api.models.admin_get_feature_flags_response_all_of import AdminGetFeatureFlagsResponseAllOf
+from edgeimpulse_api.models.admin_get_feature_flags_response_all_of_flags import AdminGetFeatureFlagsResponseAllOfFlags
 from edgeimpulse_api.models.admin_get_metrics_response import AdminGetMetricsResponse
 from edgeimpulse_api.models.admin_get_metrics_response_all_of import AdminGetMetricsResponseAllOf
 from edgeimpulse_api.models.admin_get_organizations_response import AdminGetOrganizationsResponse
 from edgeimpulse_api.models.admin_get_organizations_response_all_of import AdminGetOrganizationsResponseAllOf
 from edgeimpulse_api.models.admin_get_organizations_response_all_of_organizations import AdminGetOrganizationsResponseAllOfOrganizations
 from edgeimpulse_api.models.admin_get_sso_domain_id_ps_response import AdminGetSSODomainIdPsResponse
 from edgeimpulse_api.models.admin_get_sso_domain_id_ps_response_all_of import AdminGetSSODomainIdPsResponseAllOf
 from edgeimpulse_api.models.admin_get_sso_settings_response import AdminGetSSOSettingsResponse
 from edgeimpulse_api.models.admin_get_sso_settings_response_all_of import AdminGetSSOSettingsResponseAllOf
 from edgeimpulse_api.models.admin_get_sso_settings_response_all_of_sso_whitelist import AdminGetSSOSettingsResponseAllOfSsoWhitelist
 from edgeimpulse_api.models.admin_get_user_ids_response import AdminGetUserIdsResponse
 from edgeimpulse_api.models.admin_get_user_ids_response_all_of import AdminGetUserIdsResponseAllOf
 from edgeimpulse_api.models.admin_get_user_metrics_response import AdminGetUserMetricsResponse
-from edgeimpulse_api.models.admin_get_user_metrics_response_all_of import AdminGetUserMetricsResponseAllOf
 from edgeimpulse_api.models.admin_get_user_response import AdminGetUserResponse
 from edgeimpulse_api.models.admin_get_user_response_all_of import AdminGetUserResponseAllOf
 from edgeimpulse_api.models.admin_get_user_trial_response import AdminGetUserTrialResponse
 from edgeimpulse_api.models.admin_get_user_trial_response_all_of import AdminGetUserTrialResponseAllOf
 from edgeimpulse_api.models.admin_get_users_response import AdminGetUsersResponse
 from edgeimpulse_api.models.admin_get_users_response_all_of import AdminGetUsersResponseAllOf
 from edgeimpulse_api.models.admin_get_users_response_all_of_users import AdminGetUsersResponseAllOfUsers
@@ -176,14 +179,18 @@
 from edgeimpulse_api.models.count_samples_response import CountSamplesResponse
 from edgeimpulse_api.models.count_samples_response_all_of import CountSamplesResponseAllOf
 from edgeimpulse_api.models.create_block_version_response import CreateBlockVersionResponse
 from edgeimpulse_api.models.create_block_version_response_all_of import CreateBlockVersionResponseAllOf
 from edgeimpulse_api.models.create_developer_profile_response import CreateDeveloperProfileResponse
 from edgeimpulse_api.models.create_developer_profile_response_all_of import CreateDeveloperProfileResponseAllOf
 from edgeimpulse_api.models.create_device_request import CreateDeviceRequest
+from edgeimpulse_api.models.create_enterprise_trial_response import CreateEnterpriseTrialResponse
+from edgeimpulse_api.models.create_enterprise_trial_response_all_of import CreateEnterpriseTrialResponseAllOf
+from edgeimpulse_api.models.create_enterprise_trial_user_request import CreateEnterpriseTrialUserRequest
+from edgeimpulse_api.models.create_enterprise_trial_user_request_all_of import CreateEnterpriseTrialUserRequestAllOf
 from edgeimpulse_api.models.create_evaluation_user_response import CreateEvaluationUserResponse
 from edgeimpulse_api.models.create_evaluation_user_response_all_of import CreateEvaluationUserResponseAllOf
 from edgeimpulse_api.models.create_organization_portal_request import CreateOrganizationPortalRequest
 from edgeimpulse_api.models.create_organization_portal_response import CreateOrganizationPortalResponse
 from edgeimpulse_api.models.create_organization_portal_response_all_of import CreateOrganizationPortalResponseAllOf
 from edgeimpulse_api.models.create_organization_request import CreateOrganizationRequest
 from edgeimpulse_api.models.create_organization_response import CreateOrganizationResponse
@@ -297,24 +304,27 @@
 from edgeimpulse_api.models.dsp_sample_features_response_all_of_sample import DspSampleFeaturesResponseAllOfSample
 from edgeimpulse_api.models.dsp_trained_features_response import DspTrainedFeaturesResponse
 from edgeimpulse_api.models.dsp_trained_features_response_all_of import DspTrainedFeaturesResponseAllOf
 from edgeimpulse_api.models.dsp_trained_features_response_all_of_data import DspTrainedFeaturesResponseAllOfData
 from edgeimpulse_api.models.dsp_trained_features_response_all_of_sample import DspTrainedFeaturesResponseAllOfSample
 from edgeimpulse_api.models.edit_sample_label_request import EditSampleLabelRequest
 from edgeimpulse_api.models.enterprise_trial import EnterpriseTrial
+from edgeimpulse_api.models.enterprise_upgrade_or_trial_extension_request import EnterpriseUpgradeOrTrialExtensionRequest
 from edgeimpulse_api.models.entitlement_limits import EntitlementLimits
 from edgeimpulse_api.models.entity_created_response import EntityCreatedResponse
+from edgeimpulse_api.models.entity_created_response_all_of import EntityCreatedResponseAllOf
 from edgeimpulse_api.models.evaluate_job_response import EvaluateJobResponse
 from edgeimpulse_api.models.evaluate_job_response_all_of import EvaluateJobResponseAllOf
 from edgeimpulse_api.models.evaluate_result_value import EvaluateResultValue
 from edgeimpulse_api.models.export_get_url_response import ExportGetUrlResponse
 from edgeimpulse_api.models.export_get_url_response_all_of import ExportGetUrlResponseAllOf
 from edgeimpulse_api.models.export_keras_block_data_request import ExportKerasBlockDataRequest
 from edgeimpulse_api.models.export_original_data_request import ExportOriginalDataRequest
 from edgeimpulse_api.models.export_wav_data_request import ExportWavDataRequest
+from edgeimpulse_api.models.feature import Feature
 from edgeimpulse_api.models.find_segment_sample_request import FindSegmentSampleRequest
 from edgeimpulse_api.models.find_segment_sample_response import FindSegmentSampleResponse
 from edgeimpulse_api.models.find_segment_sample_response_all_of import FindSegmentSampleResponseAllOf
 from edgeimpulse_api.models.find_segment_sample_response_all_of_segments import FindSegmentSampleResponseAllOfSegments
 from edgeimpulse_api.models.find_user_response import FindUserResponse
 from edgeimpulse_api.models.find_user_response_all_of import FindUserResponseAllOf
 from edgeimpulse_api.models.find_user_response_all_of_users import FindUserResponseAllOfUsers
@@ -339,14 +349,16 @@
 from edgeimpulse_api.models.get_deployment_response_all_of import GetDeploymentResponseAllOf
 from edgeimpulse_api.models.get_device_response import GetDeviceResponse
 from edgeimpulse_api.models.get_device_response_all_of import GetDeviceResponseAllOf
 from edgeimpulse_api.models.get_diversity_data_response import GetDiversityDataResponse
 from edgeimpulse_api.models.get_diversity_data_response_all_of import GetDiversityDataResponseAllOf
 from edgeimpulse_api.models.get_diversity_data_response_all_of_cluster_infos import GetDiversityDataResponseAllOfClusterInfos
 from edgeimpulse_api.models.get_diversity_data_response_all_of_data import GetDiversityDataResponseAllOfData
+from edgeimpulse_api.models.get_email_verification_status_response import GetEmailVerificationStatusResponse
+from edgeimpulse_api.models.get_email_verification_status_response_all_of import GetEmailVerificationStatusResponseAllOf
 from edgeimpulse_api.models.get_impulse_blocks_response import GetImpulseBlocksResponse
 from edgeimpulse_api.models.get_impulse_blocks_response_all_of import GetImpulseBlocksResponseAllOf
 from edgeimpulse_api.models.get_impulse_response import GetImpulseResponse
 from edgeimpulse_api.models.get_impulse_response_all_of import GetImpulseResponseAllOf
 from edgeimpulse_api.models.get_jwt_request import GetJWTRequest
 from edgeimpulse_api.models.get_jwt_response import GetJWTResponse
 from edgeimpulse_api.models.get_jwt_response_all_of import GetJWTResponseAllOf
@@ -463,14 +475,16 @@
 from edgeimpulse_api.models.list_api_keys_response_all_of import ListApiKeysResponseAllOf
 from edgeimpulse_api.models.list_api_keys_response_all_of_api_keys import ListApiKeysResponseAllOfApiKeys
 from edgeimpulse_api.models.list_devices_response import ListDevicesResponse
 from edgeimpulse_api.models.list_devices_response_all_of import ListDevicesResponseAllOf
 from edgeimpulse_api.models.list_email_response import ListEmailResponse
 from edgeimpulse_api.models.list_email_response_all_of import ListEmailResponseAllOf
 from edgeimpulse_api.models.list_email_response_all_of_emails import ListEmailResponseAllOfEmails
+from edgeimpulse_api.models.list_enterprise_trials_response import ListEnterpriseTrialsResponse
+from edgeimpulse_api.models.list_enterprise_trials_response_all_of import ListEnterpriseTrialsResponseAllOf
 from edgeimpulse_api.models.list_hmac_keys_response import ListHmacKeysResponse
 from edgeimpulse_api.models.list_hmac_keys_response_all_of import ListHmacKeysResponseAllOf
 from edgeimpulse_api.models.list_hmac_keys_response_all_of_hmac_keys import ListHmacKeysResponseAllOfHmacKeys
 from edgeimpulse_api.models.list_jobs_response import ListJobsResponse
 from edgeimpulse_api.models.list_jobs_response_all_of import ListJobsResponseAllOf
 from edgeimpulse_api.models.list_models_response import ListModelsResponse
 from edgeimpulse_api.models.list_models_response_all_of import ListModelsResponseAllOf
@@ -687,14 +701,15 @@
 from edgeimpulse_api.models.raw_sample_payload import RawSamplePayload
 from edgeimpulse_api.models.rebalance_dataset_response import RebalanceDatasetResponse
 from edgeimpulse_api.models.remove_collaborator_request import RemoveCollaboratorRequest
 from edgeimpulse_api.models.remove_member_request import RemoveMemberRequest
 from edgeimpulse_api.models.rename_device_request import RenameDeviceRequest
 from edgeimpulse_api.models.rename_portal_file_request import RenamePortalFileRequest
 from edgeimpulse_api.models.rename_sample_request import RenameSampleRequest
+from edgeimpulse_api.models.request_email_verification_request import RequestEmailVerificationRequest
 from edgeimpulse_api.models.request_reset_password_request import RequestResetPasswordRequest
 from edgeimpulse_api.models.reset_password_request import ResetPasswordRequest
 from edgeimpulse_api.models.restore_project_from_public_request import RestoreProjectFromPublicRequest
 from edgeimpulse_api.models.restore_project_request import RestoreProjectRequest
 from edgeimpulse_api.models.run_auto_segmenter_request import RunAutoSegmenterRequest
 from edgeimpulse_api.models.run_organization_pipeline_response import RunOrganizationPipelineResponse
 from edgeimpulse_api.models.run_organization_pipeline_response_all_of import RunOrganizationPipelineResponseAllOf
@@ -727,14 +742,15 @@
 from edgeimpulse_api.models.set_syntiant_posterior_request import SetSyntiantPosteriorRequest
 from edgeimpulse_api.models.set_user_password_request import SetUserPasswordRequest
 from edgeimpulse_api.models.socket_token_response import SocketTokenResponse
 from edgeimpulse_api.models.socket_token_response_all_of import SocketTokenResponseAllOf
 from edgeimpulse_api.models.socket_token_response_all_of_token import SocketTokenResponseAllOfToken
 from edgeimpulse_api.models.split_sample_in_frames_request import SplitSampleInFramesRequest
 from edgeimpulse_api.models.staff_info import StaffInfo
+from edgeimpulse_api.models.start_enterprise_trial_request import StartEnterpriseTrialRequest
 from edgeimpulse_api.models.start_job_response import StartJobResponse
 from edgeimpulse_api.models.start_job_response_all_of import StartJobResponseAllOf
 from edgeimpulse_api.models.start_performance_calibration_request import StartPerformanceCalibrationRequest
 from edgeimpulse_api.models.start_sampling_request import StartSamplingRequest
 from edgeimpulse_api.models.start_sampling_response import StartSamplingResponse
 from edgeimpulse_api.models.start_sampling_response_all_of import StartSamplingResponseAllOf
 from edgeimpulse_api.models.start_training_request_anomaly import StartTrainingRequestAnomaly
@@ -796,14 +812,16 @@
 from edgeimpulse_api.models.user_by_third_party_activation_request import UserByThirdPartyActivationRequest
 from edgeimpulse_api.models.user_experiment import UserExperiment
 from edgeimpulse_api.models.user_organization import UserOrganization
 from edgeimpulse_api.models.verify_dsp_block_url_request import VerifyDspBlockUrlRequest
 from edgeimpulse_api.models.verify_dsp_block_url_response import VerifyDspBlockUrlResponse
 from edgeimpulse_api.models.verify_dsp_block_url_response_all_of import VerifyDspBlockUrlResponseAllOf
 from edgeimpulse_api.models.verify_dsp_block_url_response_all_of_block import VerifyDspBlockUrlResponseAllOfBlock
+from edgeimpulse_api.models.verify_email_response import VerifyEmailResponse
+from edgeimpulse_api.models.verify_email_response_all_of import VerifyEmailResponseAllOf
 from edgeimpulse_api.models.verify_organization_bucket_request import VerifyOrganizationBucketRequest
 from edgeimpulse_api.models.verify_organization_bucket_response import VerifyOrganizationBucketResponse
 from edgeimpulse_api.models.verify_organization_bucket_response_all_of import VerifyOrganizationBucketResponseAllOf
 from edgeimpulse_api.models.verify_organization_bucket_response_all_of_files import VerifyOrganizationBucketResponseAllOfFiles
 from edgeimpulse_api.models.verify_reset_password_request import VerifyResetPasswordRequest
 from edgeimpulse_api.models.whitelabel import Whitelabel
 from edgeimpulse_api.models.whitelabel_admin_create_organization_request import WhitelabelAdminCreateOrganizationRequest
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/__init__.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from edgeimpulse_api.api.auth_api import AuthApi
 from edgeimpulse_api.api.cdn_api import CDNApi
 from edgeimpulse_api.api.classify_api import ClassifyApi
 from edgeimpulse_api.api.content_disposition_inline_api import ContentDispositionInlineApi
 from edgeimpulse_api.api.dsp_api import DSPApi
 from edgeimpulse_api.api.deployment_api import DeploymentApi
 from edgeimpulse_api.api.devices_api import DevicesApi
+from edgeimpulse_api.api.email_verification_api import EmailVerificationApi
 from edgeimpulse_api.api.export_api import ExportApi
 from edgeimpulse_api.api.health_api import HealthApi
 from edgeimpulse_api.api.impulse_api import ImpulseApi
 from edgeimpulse_api.api.jobs_api import JobsApi
 from edgeimpulse_api.api.learn_api import LearnApi
 from edgeimpulse_api.api.login_api import LoginApi
 from edgeimpulse_api.api.metrics_api import MetricsApi
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/admin_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/admin_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 from typing import Optional
 
 from edgeimpulse_api.models.admin_add_disallowed_email_domain_request import AdminAddDisallowedEmailDomainRequest
 from edgeimpulse_api.models.admin_add_or_update_sso_domain_id_ps_request import AdminAddOrUpdateSSODomainIdPsRequest
 from edgeimpulse_api.models.admin_add_organization_user_request import AdminAddOrganizationUserRequest
 from edgeimpulse_api.models.admin_add_project_user_request import AdminAddProjectUserRequest
 from edgeimpulse_api.models.admin_create_organization_request import AdminCreateOrganizationRequest
-from edgeimpulse_api.models.admin_create_user_trial_request import AdminCreateUserTrialRequest
 from edgeimpulse_api.models.admin_get_data_migration_response import AdminGetDataMigrationResponse
 from edgeimpulse_api.models.admin_get_data_migrations_response import AdminGetDataMigrationsResponse
 from edgeimpulse_api.models.admin_get_disallowed_email_domains_response import AdminGetDisallowedEmailDomainsResponse
+from edgeimpulse_api.models.admin_get_feature_flags_response import AdminGetFeatureFlagsResponse
 from edgeimpulse_api.models.admin_get_metrics_response import AdminGetMetricsResponse
 from edgeimpulse_api.models.admin_get_organizations_response import AdminGetOrganizationsResponse
 from edgeimpulse_api.models.admin_get_sso_domain_id_ps_response import AdminGetSSODomainIdPsResponse
 from edgeimpulse_api.models.admin_get_sso_settings_response import AdminGetSSOSettingsResponse
 from edgeimpulse_api.models.admin_get_user_ids_response import AdminGetUserIdsResponse
 from edgeimpulse_api.models.admin_get_user_metrics_response import AdminGetUserMetricsResponse
 from edgeimpulse_api.models.admin_get_user_response import AdminGetUserResponse
@@ -44,21 +44,23 @@
 from edgeimpulse_api.models.admin_toggle_data_migration_request import AdminToggleDataMigrationRequest
 from edgeimpulse_api.models.admin_update_organization_request import AdminUpdateOrganizationRequest
 from edgeimpulse_api.models.admin_update_user_permissions_request import AdminUpdateUserPermissionsRequest
 from edgeimpulse_api.models.admin_update_user_request import AdminUpdateUserRequest
 from edgeimpulse_api.models.admin_update_user_trial_request import AdminUpdateUserTrialRequest
 from edgeimpulse_api.models.create_organization_response import CreateOrganizationResponse
 from edgeimpulse_api.models.entity_created_response import EntityCreatedResponse
+from edgeimpulse_api.models.feature import Feature
 from edgeimpulse_api.models.find_user_response import FindUserResponse
 from edgeimpulse_api.models.generic_api_response import GenericApiResponse
 from edgeimpulse_api.models.job_details_response import JobDetailsResponse
 from edgeimpulse_api.models.job_logs_response import JobLogsResponse
 from edgeimpulse_api.models.job_metrics_response import JobMetricsResponse
 from edgeimpulse_api.models.job_parent_type_enum import JobParentTypeEnum
 from edgeimpulse_api.models.project_info_response import ProjectInfoResponse
+from edgeimpulse_api.models.start_enterprise_trial_request import StartEnterpriseTrialRequest
 from edgeimpulse_api.models.update_project_request import UpdateProjectRequest
 
 from edgeimpulse_api.api_client import ApiClient
 from edgeimpulse_api.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -921,23 +923,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_create_user_trial(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], admin_create_user_trial_request : AdminCreateUserTrialRequest, **kwargs) -> EntityCreatedResponse:  # noqa: E501
+    def admin_create_user_trial(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], start_enterprise_trial_request : StartEnterpriseTrialRequest, **kwargs) -> EntityCreatedResponse:  # noqa: E501
         """Create user enterprise trial
 
         Admin-only API to create an enterprise trial for a user.
 
         :param user_id: User ID (required)
         :type user_id: int
-        :param admin_create_user_trial_request: (required)
-        :type admin_create_user_trial_request: AdminCreateUserTrialRequest
+        :param start_enterprise_trial_request: (required)
+        :type start_enterprise_trial_request: StartEnterpriseTrialRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -946,26 +948,26 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: EntityCreatedResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._admin_create_user_trial_with_http_info(user_id, admin_create_user_trial_request, **kwargs)  # noqa: E501
+        return self._admin_create_user_trial_with_http_info(user_id, start_enterprise_trial_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_create_user_trial_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], admin_create_user_trial_request : AdminCreateUserTrialRequest, **kwargs):  # noqa: E501
+    def _admin_create_user_trial_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], start_enterprise_trial_request : StartEnterpriseTrialRequest, **kwargs):  # noqa: E501
         """Create user enterprise trial 
 
         Admin-only API to create an enterprise trial for a user.
 
         :param user_id: User ID (required)
         :type user_id: int
-        :param admin_create_user_trial_request: (required)
-        :type admin_create_user_trial_request: AdminCreateUserTrialRequest
+        :param start_enterprise_trial_request: (required)
+        :type start_enterprise_trial_request: StartEnterpriseTrialRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -986,15 +988,15 @@
         :rtype: tuple(EntityCreatedResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'user_id',
-            'admin_create_user_trial_request'
+            'start_enterprise_trial_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1029,16 +1031,16 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['admin_create_user_trial_request']:
-            _body_params = _params['admin_create_user_trial_request']
+        if _params['start_enterprise_trial_request']:
+            _body_params = _params['start_enterprise_trial_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -1887,14 +1889,280 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def admin_disable_feature(self, feature_id : Annotated[Feature, Field(..., description="Feature ID.")], **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Set a feature flag OFF
+
+        Admin-only API to delete a feature flag. Deleting a feature flag essentially disables the feature for all users.
+
+        :param feature_id: Feature ID. (required)
+        :type feature_id: Feature
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenericApiResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._admin_disable_feature_with_http_info(feature_id, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _admin_disable_feature_with_http_info(self, feature_id : Annotated[Feature, Field(..., description="Feature ID.")], **kwargs):  # noqa: E501
+        """Set a feature flag OFF 
+
+        Admin-only API to delete a feature flag. Deleting a feature flag essentially disables the feature for all users.
+
+        :param feature_id: Feature ID. (required)
+        :type feature_id: Feature
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'feature_id'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method admin_disable_feature" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['feature_id']:
+            _path_params['featureId'] = _params['feature_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GenericApiResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/admin/infra/featureFlags/{featureId}', 'DELETE',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def admin_enable_feature(self, feature_id : Annotated[Feature, Field(..., description="Feature ID.")], **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Set a feature flag ON
+
+        Admin-only API to set a feature flag ON. Setting a feature flag ON essentially enables the feature for all users.
+
+        :param feature_id: Feature ID. (required)
+        :type feature_id: Feature
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenericApiResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._admin_enable_feature_with_http_info(feature_id, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _admin_enable_feature_with_http_info(self, feature_id : Annotated[Feature, Field(..., description="Feature ID.")], **kwargs):  # noqa: E501
+        """Set a feature flag ON 
+
+        Admin-only API to set a feature flag ON. Setting a feature flag ON essentially enables the feature for all users.
+
+        :param feature_id: Feature ID. (required)
+        :type feature_id: Feature
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'feature_id'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method admin_enable_feature" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['feature_id']:
+            _path_params['featureId'] = _params['feature_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GenericApiResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/admin/infra/featureFlags/{featureId}', 'PUT',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def admin_find_user(self, query : Annotated[StrictStr, Field(..., description="Part of e-mail address or username")], **kwargs) -> FindUserResponse:  # noqa: E501
         """Find a user
 
         DEPRECATED. Admin-only API to find a user by username or email address.
 
         :param query: Part of e-mail address or username (required)
         :type query: str
@@ -2648,14 +2916,140 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def admin_get_feature_flags(self, **kwargs) -> AdminGetFeatureFlagsResponse:  # noqa: E501
+        """Get all feature flags
+
+        Admin-only API to get all feature flags.
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: AdminGetFeatureFlagsResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._admin_get_feature_flags_with_http_info(**kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _admin_get_feature_flags_with_http_info(self, **kwargs):  # noqa: E501
+        """Get all feature flags 
+
+        Admin-only API to get all feature flags.
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(AdminGetFeatureFlagsResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method admin_get_feature_flags" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "AdminGetFeatureFlagsResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/admin/infra/featureFlags', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/allows_read_only_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/allows_read_only_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/auth_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/cdn_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/cdn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/classify_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/classify_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/content_disposition_inline_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/content_disposition_inline_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/deployment_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/deployment_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/devices_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/devices_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/dsp_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/dsp_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/export_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/export_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/health_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/health_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/impulse_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/impulse_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/jobs_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/learn_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/learn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/login_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/login_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/metrics_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/optimization_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/optimization_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_allow_developer_profile_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_allow_developer_profile_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_allow_guest_access_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_allow_guest_access_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_blocks_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_blocks_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_create_project_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_create_project_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_data_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_data_campaigns_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_data_campaigns_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_jobs_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_pipelines_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_pipelines_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_portals_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_portals_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_requires_admin_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_requires_admin_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/organizations_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/organizations_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from edgeimpulse_api.models.admin_get_users_response import AdminGetUsersResponse
 from edgeimpulse_api.models.admin_list_projects_response import AdminListProjectsResponse
 from edgeimpulse_api.models.admin_organization_info_response import AdminOrganizationInfoResponse
 from edgeimpulse_api.models.admin_update_organization_request import AdminUpdateOrganizationRequest
 from edgeimpulse_api.models.admin_update_user_request import AdminUpdateUserRequest
 from edgeimpulse_api.models.create_organization_request import CreateOrganizationRequest
 from edgeimpulse_api.models.create_organization_response import CreateOrganizationResponse
+from edgeimpulse_api.models.enterprise_upgrade_or_trial_extension_request import EnterpriseUpgradeOrTrialExtensionRequest
 from edgeimpulse_api.models.generic_api_response import GenericApiResponse
 from edgeimpulse_api.models.get_whitelabel_response import GetWhitelabelResponse
 from edgeimpulse_api.models.invite_organization_member_request import InviteOrganizationMemberRequest
 from edgeimpulse_api.models.list_organization_api_keys_response import ListOrganizationApiKeysResponse
 from edgeimpulse_api.models.list_organization_projects_response import ListOrganizationProjectsResponse
 from edgeimpulse_api.models.list_organizations_response import ListOrganizationsResponse
 from edgeimpulse_api.models.organization_info_response import OrganizationInfoResponse
@@ -1579,14 +1580,161 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def request_enterprise_trial_extension(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], enterprise_upgrade_or_trial_extension_request : EnterpriseUpgradeOrTrialExtensionRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Request trial extension
+
+        Request an extension for an enterprise trial.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param enterprise_upgrade_or_trial_extension_request: (required)
+        :type enterprise_upgrade_or_trial_extension_request: EnterpriseUpgradeOrTrialExtensionRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenericApiResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._request_enterprise_trial_extension_with_http_info(organization_id, enterprise_upgrade_or_trial_extension_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _request_enterprise_trial_extension_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], enterprise_upgrade_or_trial_extension_request : EnterpriseUpgradeOrTrialExtensionRequest, **kwargs):  # noqa: E501
+        """Request trial extension 
+
+        Request an extension for an enterprise trial.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param enterprise_upgrade_or_trial_extension_request: (required)
+        :type enterprise_upgrade_or_trial_extension_request: EnterpriseUpgradeOrTrialExtensionRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'organization_id',
+            'enterprise_upgrade_or_trial_extension_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method request_enterprise_trial_extension" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['organization_id']:
+            _path_params['organizationId'] = _params['organization_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['enterprise_upgrade_or_trial_extension_request']:
+            _body_params = _params['enterprise_upgrade_or_trial_extension_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GenericApiResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/organizations/{organizationId}/trial/request-extension', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/performance_calibration_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/performance_calibration_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/project_requires_admin_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/project_requires_admin_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/projects_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/raw_data_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/raw_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/requires_sudo_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/requires_sudo_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/supports_range_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/supports_range_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/themes_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/themes_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/third_party_auth_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/third_party_auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/upload_portal_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/upload_portal_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/user_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/user_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,32 +16,37 @@
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr
 
 from edgeimpulse_api.models.activate_user_by_third_party_activation_code_request import ActivateUserByThirdPartyActivationCodeRequest
-from edgeimpulse_api.models.activate_user_request import ActivateUserRequest
+from edgeimpulse_api.models.activate_user_or_verify_email_request import ActivateUserOrVerifyEmailRequest
 from edgeimpulse_api.models.change_password_request import ChangePasswordRequest
 from edgeimpulse_api.models.convert_user_request import ConvertUserRequest
 from edgeimpulse_api.models.create_developer_profile_response import CreateDeveloperProfileResponse
+from edgeimpulse_api.models.create_enterprise_trial_response import CreateEnterpriseTrialResponse
+from edgeimpulse_api.models.create_enterprise_trial_user_request import CreateEnterpriseTrialUserRequest
 from edgeimpulse_api.models.create_evaluation_user_response import CreateEvaluationUserResponse
 from edgeimpulse_api.models.create_user_request import CreateUserRequest
 from edgeimpulse_api.models.create_user_response import CreateUserResponse
+from edgeimpulse_api.models.enterprise_upgrade_or_trial_extension_request import EnterpriseUpgradeOrTrialExtensionRequest
 from edgeimpulse_api.models.generic_api_response import GenericApiResponse
 from edgeimpulse_api.models.get_jwt_response import GetJWTResponse
 from edgeimpulse_api.models.get_user_need_to_set_password_response import GetUserNeedToSetPasswordResponse
 from edgeimpulse_api.models.get_user_response import GetUserResponse
 from edgeimpulse_api.models.list_email_response import ListEmailResponse
+from edgeimpulse_api.models.list_enterprise_trials_response import ListEnterpriseTrialsResponse
 from edgeimpulse_api.models.list_organization_buckets_user_response import ListOrganizationBucketsUserResponse
 from edgeimpulse_api.models.list_organizations_response import ListOrganizationsResponse
 from edgeimpulse_api.models.request_reset_password_request import RequestResetPasswordRequest
 from edgeimpulse_api.models.reset_password_request import ResetPasswordRequest
 from edgeimpulse_api.models.send_user_feedback_request import SendUserFeedbackRequest
 from edgeimpulse_api.models.set_user_password_request import SetUserPasswordRequest
+from edgeimpulse_api.models.start_enterprise_trial_request import StartEnterpriseTrialRequest
 from edgeimpulse_api.models.update_user_request import UpdateUserRequest
 from edgeimpulse_api.models.upload_user_photo_response import UploadUserPhotoResponse
 from edgeimpulse_api.models.user_by_third_party_activation_request import UserByThirdPartyActivationRequest
 from edgeimpulse_api.models.verify_reset_password_request import VerifyResetPasswordRequest
 
 from edgeimpulse_api.api_client import ApiClient
 from edgeimpulse_api.exceptions import (  # noqa: F401
@@ -179,21 +184,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def activate_current_user(self, activate_user_request : ActivateUserRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+    def activate_current_user(self, activate_user_or_verify_email_request : ActivateUserOrVerifyEmailRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
         """Activate current user
 
         Activate the current user account (requires an activation code). This function is only available through a JWT token.
 
-        :param activate_user_request: (required)
-        :type activate_user_request: ActivateUserRequest
+        :param activate_user_or_verify_email_request: (required)
+        :type activate_user_or_verify_email_request: ActivateUserOrVerifyEmailRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -202,24 +207,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._activate_current_user_with_http_info(activate_user_request, **kwargs)  # noqa: E501
+        return self._activate_current_user_with_http_info(activate_user_or_verify_email_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _activate_current_user_with_http_info(self, activate_user_request : ActivateUserRequest, **kwargs):  # noqa: E501
+    def _activate_current_user_with_http_info(self, activate_user_or_verify_email_request : ActivateUserOrVerifyEmailRequest, **kwargs):  # noqa: E501
         """Activate current user 
 
         Activate the current user account (requires an activation code). This function is only available through a JWT token.
 
-        :param activate_user_request: (required)
-        :type activate_user_request: ActivateUserRequest
+        :param activate_user_or_verify_email_request: (required)
+        :type activate_user_or_verify_email_request: ActivateUserOrVerifyEmailRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -239,15 +244,15 @@
                  returns the request thread.
         :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'activate_user_request'
+            'activate_user_or_verify_email_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -280,16 +285,16 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['activate_user_request']:
-            _body_params = _params['activate_user_request']
+        if _params['activate_user_or_verify_email_request']:
+            _body_params = _params['activate_user_or_verify_email_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -319,23 +324,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def activate_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], activate_user_request : ActivateUserRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+    def activate_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], activate_user_or_verify_email_request : ActivateUserOrVerifyEmailRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
         """Activate user
 
         Activate a user account (requires an activation code). This function is only available through a JWT token.
 
         :param user_id: User ID (required)
         :type user_id: int
-        :param activate_user_request: (required)
-        :type activate_user_request: ActivateUserRequest
+        :param activate_user_or_verify_email_request: (required)
+        :type activate_user_or_verify_email_request: ActivateUserOrVerifyEmailRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -344,26 +349,26 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._activate_user_with_http_info(user_id, activate_user_request, **kwargs)  # noqa: E501
+        return self._activate_user_with_http_info(user_id, activate_user_or_verify_email_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _activate_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], activate_user_request : ActivateUserRequest, **kwargs):  # noqa: E501
+    def _activate_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], activate_user_or_verify_email_request : ActivateUserOrVerifyEmailRequest, **kwargs):  # noqa: E501
         """Activate user 
 
         Activate a user account (requires an activation code). This function is only available through a JWT token.
 
         :param user_id: User ID (required)
         :type user_id: int
-        :param activate_user_request: (required)
-        :type activate_user_request: ActivateUserRequest
+        :param activate_user_or_verify_email_request: (required)
+        :type activate_user_or_verify_email_request: ActivateUserOrVerifyEmailRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -384,15 +389,15 @@
         :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'user_id',
-            'activate_user_request'
+            'activate_user_or_verify_email_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -427,16 +432,16 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['activate_user_request']:
-            _body_params = _params['activate_user_request']
+        if _params['activate_user_or_verify_email_request']:
+            _body_params = _params['activate_user_or_verify_email_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -1159,14 +1164,154 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def create_enterprise_trial_user(self, create_enterprise_trial_user_request : Annotated[CreateEnterpriseTrialUserRequest, Field(..., description="Trial request")], **kwargs) -> CreateEnterpriseTrialResponse:  # noqa: E501
+        """Create enterprise trial user
+
+        Creates an enterprise trial user and a new trial organization, and redirects the user to the new organization.
+
+        :param create_enterprise_trial_user_request: Trial request (required)
+        :type create_enterprise_trial_user_request: CreateEnterpriseTrialUserRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: CreateEnterpriseTrialResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._create_enterprise_trial_user_with_http_info(create_enterprise_trial_user_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _create_enterprise_trial_user_with_http_info(self, create_enterprise_trial_user_request : Annotated[CreateEnterpriseTrialUserRequest, Field(..., description="Trial request")], **kwargs):  # noqa: E501
+        """Create enterprise trial user 
+
+        Creates an enterprise trial user and a new trial organization, and redirects the user to the new organization.
+
+        :param create_enterprise_trial_user_request: Trial request (required)
+        :type create_enterprise_trial_user_request: CreateEnterpriseTrialUserRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(CreateEnterpriseTrialResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'create_enterprise_trial_user_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_enterprise_trial_user" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['create_enterprise_trial_user_request']:
+            _body_params = _params['create_enterprise_trial_user_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = []  # noqa: E501
+
+        _response_types_map = {
+            '200': "CreateEnterpriseTrialResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api-user-create-enterprise-trial', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def create_evaluation_user(self, **kwargs) -> CreateEvaluationUserResponse:  # noqa: E501
         """Create evaluation user
 
         Creates an evaluation user and a new project, and redirects the user to the new project.
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -2210,17 +2355,17 @@
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def get_user_need_to_set_password(self, username_or_email : Annotated[StrictStr, Field(..., description="Username or email")], **kwargs) -> GetUserNeedToSetPasswordResponse:  # noqa: E501
-        """Get user password state
+        """Get user registration state
 
-        Tells whether the user needs to set its password.
+        Tells whether a user is registered and whether it needs to set its password.
 
         :param username_or_email: Username or email (required)
         :type username_or_email: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -2236,17 +2381,17 @@
         :rtype: GetUserNeedToSetPasswordResponse
         """
         kwargs['_return_http_data_only'] = True
         return self._get_user_need_to_set_password_with_http_info(username_or_email, **kwargs)  # noqa: E501
 
     @validate_arguments
     def _get_user_need_to_set_password_with_http_info(self, username_or_email : Annotated[StrictStr, Field(..., description="Username or email")], **kwargs):  # noqa: E501
-        """Get user password state 
+        """Get user registration state 
 
-        Tells whether the user needs to set its password.
+        Tells whether a user is registered and whether it needs to set its password.
 
         :param username_or_email: Username or email (required)
         :type username_or_email: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
@@ -2601,14 +2746,147 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def list_enterprise_trials_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs) -> ListEnterpriseTrialsResponse:  # noqa: E501
+        """Get enterprise trials
+
+        Get a list of all enterprise trials for a user. This function is only available through a JWT token.
+
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ListEnterpriseTrialsResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._list_enterprise_trials_user_with_http_info(user_id, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _list_enterprise_trials_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs):  # noqa: E501
+        """Get enterprise trials 
+
+        Get a list of all enterprise trials for a user. This function is only available through a JWT token.
+
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(ListEnterpriseTrialsResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'user_id'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method list_enterprise_trials_user" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['user_id']:
+            _path_params['userId'] = _params['user_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "ListEnterpriseTrialsResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/users/{userId}/trials', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def list_organization_buckets_current_user(self, **kwargs) -> ListOrganizationBucketsUserResponse:  # noqa: E501
         """Get buckets current user
 
         List all organizational storage buckets that the current user has access to. This function is only available through a JWT token.
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -3805,14 +4083,161 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def send_user_upgrade_request(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_upgrade_or_trial_extension_request : EnterpriseUpgradeOrTrialExtensionRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Send upgrade request
+
+        Send an upgrade to Enterprise request to Edge Impulse.
+
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param enterprise_upgrade_or_trial_extension_request: (required)
+        :type enterprise_upgrade_or_trial_extension_request: EnterpriseUpgradeOrTrialExtensionRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenericApiResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._send_user_upgrade_request_with_http_info(user_id, enterprise_upgrade_or_trial_extension_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _send_user_upgrade_request_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_upgrade_or_trial_extension_request : EnterpriseUpgradeOrTrialExtensionRequest, **kwargs):  # noqa: E501
+        """Send upgrade request 
+
+        Send an upgrade to Enterprise request to Edge Impulse.
+
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param enterprise_upgrade_or_trial_extension_request: (required)
+        :type enterprise_upgrade_or_trial_extension_request: EnterpriseUpgradeOrTrialExtensionRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'user_id',
+            'enterprise_upgrade_or_trial_extension_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method send_user_upgrade_request" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['user_id']:
+            _path_params['userId'] = _params['user_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['enterprise_upgrade_or_trial_extension_request']:
+            _body_params = _params['enterprise_upgrade_or_trial_extension_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GenericApiResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/users/{userId}/upgrade', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def set_user_password(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], set_user_password_request : SetUserPasswordRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
         """Set password for SSO user
 
         Set the password for a new SSO user. This function is only available through an SSO access token.
 
         :param user_id: User ID (required)
         :type user_id: int
@@ -3943,14 +4368,154 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def start_enterprise_trial(self, start_enterprise_trial_request : StartEnterpriseTrialRequest, **kwargs) -> CreateEnterpriseTrialResponse:  # noqa: E501
+        """Start enterprise trial
+
+        Create an enterprise trial for the current user. Users can only go through a trial once.
+
+        :param start_enterprise_trial_request: (required)
+        :type start_enterprise_trial_request: StartEnterpriseTrialRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: CreateEnterpriseTrialResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._start_enterprise_trial_with_http_info(start_enterprise_trial_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _start_enterprise_trial_with_http_info(self, start_enterprise_trial_request : StartEnterpriseTrialRequest, **kwargs):  # noqa: E501
+        """Start enterprise trial 
+
+        Create an enterprise trial for the current user. Users can only go through a trial once.
+
+        :param start_enterprise_trial_request: (required)
+        :type start_enterprise_trial_request: StartEnterpriseTrialRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(CreateEnterpriseTrialResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'start_enterprise_trial_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method start_enterprise_trial" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['start_enterprise_trial_request']:
+            _body_params = _params['start_enterprise_trial_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "CreateEnterpriseTrialResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/user/trial', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api/whitelabels_api.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api/whitelabels_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/api_client.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/api_client.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/configuration.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/configuration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/exceptions.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/__init__.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from edgeimpulse_api.models.activate_user_by_third_party_activation_code_request import ActivateUserByThirdPartyActivationCodeRequest
-from edgeimpulse_api.models.activate_user_request import ActivateUserRequest
+from edgeimpulse_api.models.activate_user_or_verify_email_request import ActivateUserOrVerifyEmailRequest
 from edgeimpulse_api.models.add_api_key_request import AddApiKeyRequest
 from edgeimpulse_api.models.add_collaborator_request import AddCollaboratorRequest
 from edgeimpulse_api.models.add_hmac_key_request import AddHmacKeyRequest
 from edgeimpulse_api.models.add_member_request import AddMemberRequest
 from edgeimpulse_api.models.add_organization_api_key_request import AddOrganizationApiKeyRequest
 from edgeimpulse_api.models.add_organization_bucket_request import AddOrganizationBucketRequest
 from edgeimpulse_api.models.add_organization_data_campaign_dashboard_request import AddOrganizationDataCampaignDashboardRequest
@@ -47,35 +47,37 @@
 from edgeimpulse_api.models.admin_add_user_request import AdminAddUserRequest
 from edgeimpulse_api.models.admin_api_organization import AdminApiOrganization
 from edgeimpulse_api.models.admin_api_organization_all_of import AdminApiOrganizationAllOf
 from edgeimpulse_api.models.admin_api_project import AdminApiProject
 from edgeimpulse_api.models.admin_api_user import AdminApiUser
 from edgeimpulse_api.models.admin_api_user_all_of import AdminApiUserAllOf
 from edgeimpulse_api.models.admin_create_organization_request import AdminCreateOrganizationRequest
-from edgeimpulse_api.models.admin_create_user_trial_request import AdminCreateUserTrialRequest
+from edgeimpulse_api.models.admin_enable_feature_request import AdminEnableFeatureRequest
 from edgeimpulse_api.models.admin_get_data_migration_response import AdminGetDataMigrationResponse
 from edgeimpulse_api.models.admin_get_data_migration_response_all_of import AdminGetDataMigrationResponseAllOf
 from edgeimpulse_api.models.admin_get_data_migrations_response import AdminGetDataMigrationsResponse
 from edgeimpulse_api.models.admin_get_data_migrations_response_all_of import AdminGetDataMigrationsResponseAllOf
 from edgeimpulse_api.models.admin_get_disallowed_email_domains_response import AdminGetDisallowedEmailDomainsResponse
 from edgeimpulse_api.models.admin_get_disallowed_email_domains_response_all_of import AdminGetDisallowedEmailDomainsResponseAllOf
+from edgeimpulse_api.models.admin_get_feature_flags_response import AdminGetFeatureFlagsResponse
+from edgeimpulse_api.models.admin_get_feature_flags_response_all_of import AdminGetFeatureFlagsResponseAllOf
+from edgeimpulse_api.models.admin_get_feature_flags_response_all_of_flags import AdminGetFeatureFlagsResponseAllOfFlags
 from edgeimpulse_api.models.admin_get_metrics_response import AdminGetMetricsResponse
 from edgeimpulse_api.models.admin_get_metrics_response_all_of import AdminGetMetricsResponseAllOf
 from edgeimpulse_api.models.admin_get_organizations_response import AdminGetOrganizationsResponse
 from edgeimpulse_api.models.admin_get_organizations_response_all_of import AdminGetOrganizationsResponseAllOf
 from edgeimpulse_api.models.admin_get_organizations_response_all_of_organizations import AdminGetOrganizationsResponseAllOfOrganizations
 from edgeimpulse_api.models.admin_get_sso_domain_id_ps_response import AdminGetSSODomainIdPsResponse
 from edgeimpulse_api.models.admin_get_sso_domain_id_ps_response_all_of import AdminGetSSODomainIdPsResponseAllOf
 from edgeimpulse_api.models.admin_get_sso_settings_response import AdminGetSSOSettingsResponse
 from edgeimpulse_api.models.admin_get_sso_settings_response_all_of import AdminGetSSOSettingsResponseAllOf
 from edgeimpulse_api.models.admin_get_sso_settings_response_all_of_sso_whitelist import AdminGetSSOSettingsResponseAllOfSsoWhitelist
 from edgeimpulse_api.models.admin_get_user_ids_response import AdminGetUserIdsResponse
 from edgeimpulse_api.models.admin_get_user_ids_response_all_of import AdminGetUserIdsResponseAllOf
 from edgeimpulse_api.models.admin_get_user_metrics_response import AdminGetUserMetricsResponse
-from edgeimpulse_api.models.admin_get_user_metrics_response_all_of import AdminGetUserMetricsResponseAllOf
 from edgeimpulse_api.models.admin_get_user_response import AdminGetUserResponse
 from edgeimpulse_api.models.admin_get_user_response_all_of import AdminGetUserResponseAllOf
 from edgeimpulse_api.models.admin_get_user_trial_response import AdminGetUserTrialResponse
 from edgeimpulse_api.models.admin_get_user_trial_response_all_of import AdminGetUserTrialResponseAllOf
 from edgeimpulse_api.models.admin_get_users_response import AdminGetUsersResponse
 from edgeimpulse_api.models.admin_get_users_response_all_of import AdminGetUsersResponseAllOf
 from edgeimpulse_api.models.admin_get_users_response_all_of_users import AdminGetUsersResponseAllOfUsers
@@ -121,14 +123,18 @@
 from edgeimpulse_api.models.count_samples_response import CountSamplesResponse
 from edgeimpulse_api.models.count_samples_response_all_of import CountSamplesResponseAllOf
 from edgeimpulse_api.models.create_block_version_response import CreateBlockVersionResponse
 from edgeimpulse_api.models.create_block_version_response_all_of import CreateBlockVersionResponseAllOf
 from edgeimpulse_api.models.create_developer_profile_response import CreateDeveloperProfileResponse
 from edgeimpulse_api.models.create_developer_profile_response_all_of import CreateDeveloperProfileResponseAllOf
 from edgeimpulse_api.models.create_device_request import CreateDeviceRequest
+from edgeimpulse_api.models.create_enterprise_trial_response import CreateEnterpriseTrialResponse
+from edgeimpulse_api.models.create_enterprise_trial_response_all_of import CreateEnterpriseTrialResponseAllOf
+from edgeimpulse_api.models.create_enterprise_trial_user_request import CreateEnterpriseTrialUserRequest
+from edgeimpulse_api.models.create_enterprise_trial_user_request_all_of import CreateEnterpriseTrialUserRequestAllOf
 from edgeimpulse_api.models.create_evaluation_user_response import CreateEvaluationUserResponse
 from edgeimpulse_api.models.create_evaluation_user_response_all_of import CreateEvaluationUserResponseAllOf
 from edgeimpulse_api.models.create_organization_portal_request import CreateOrganizationPortalRequest
 from edgeimpulse_api.models.create_organization_portal_response import CreateOrganizationPortalResponse
 from edgeimpulse_api.models.create_organization_portal_response_all_of import CreateOrganizationPortalResponseAllOf
 from edgeimpulse_api.models.create_organization_request import CreateOrganizationRequest
 from edgeimpulse_api.models.create_organization_response import CreateOrganizationResponse
@@ -242,24 +248,27 @@
 from edgeimpulse_api.models.dsp_sample_features_response_all_of_sample import DspSampleFeaturesResponseAllOfSample
 from edgeimpulse_api.models.dsp_trained_features_response import DspTrainedFeaturesResponse
 from edgeimpulse_api.models.dsp_trained_features_response_all_of import DspTrainedFeaturesResponseAllOf
 from edgeimpulse_api.models.dsp_trained_features_response_all_of_data import DspTrainedFeaturesResponseAllOfData
 from edgeimpulse_api.models.dsp_trained_features_response_all_of_sample import DspTrainedFeaturesResponseAllOfSample
 from edgeimpulse_api.models.edit_sample_label_request import EditSampleLabelRequest
 from edgeimpulse_api.models.enterprise_trial import EnterpriseTrial
+from edgeimpulse_api.models.enterprise_upgrade_or_trial_extension_request import EnterpriseUpgradeOrTrialExtensionRequest
 from edgeimpulse_api.models.entitlement_limits import EntitlementLimits
 from edgeimpulse_api.models.entity_created_response import EntityCreatedResponse
+from edgeimpulse_api.models.entity_created_response_all_of import EntityCreatedResponseAllOf
 from edgeimpulse_api.models.evaluate_job_response import EvaluateJobResponse
 from edgeimpulse_api.models.evaluate_job_response_all_of import EvaluateJobResponseAllOf
 from edgeimpulse_api.models.evaluate_result_value import EvaluateResultValue
 from edgeimpulse_api.models.export_get_url_response import ExportGetUrlResponse
 from edgeimpulse_api.models.export_get_url_response_all_of import ExportGetUrlResponseAllOf
 from edgeimpulse_api.models.export_keras_block_data_request import ExportKerasBlockDataRequest
 from edgeimpulse_api.models.export_original_data_request import ExportOriginalDataRequest
 from edgeimpulse_api.models.export_wav_data_request import ExportWavDataRequest
+from edgeimpulse_api.models.feature import Feature
 from edgeimpulse_api.models.find_segment_sample_request import FindSegmentSampleRequest
 from edgeimpulse_api.models.find_segment_sample_response import FindSegmentSampleResponse
 from edgeimpulse_api.models.find_segment_sample_response_all_of import FindSegmentSampleResponseAllOf
 from edgeimpulse_api.models.find_segment_sample_response_all_of_segments import FindSegmentSampleResponseAllOfSegments
 from edgeimpulse_api.models.find_user_response import FindUserResponse
 from edgeimpulse_api.models.find_user_response_all_of import FindUserResponseAllOf
 from edgeimpulse_api.models.find_user_response_all_of_users import FindUserResponseAllOfUsers
@@ -284,14 +293,16 @@
 from edgeimpulse_api.models.get_deployment_response_all_of import GetDeploymentResponseAllOf
 from edgeimpulse_api.models.get_device_response import GetDeviceResponse
 from edgeimpulse_api.models.get_device_response_all_of import GetDeviceResponseAllOf
 from edgeimpulse_api.models.get_diversity_data_response import GetDiversityDataResponse
 from edgeimpulse_api.models.get_diversity_data_response_all_of import GetDiversityDataResponseAllOf
 from edgeimpulse_api.models.get_diversity_data_response_all_of_cluster_infos import GetDiversityDataResponseAllOfClusterInfos
 from edgeimpulse_api.models.get_diversity_data_response_all_of_data import GetDiversityDataResponseAllOfData
+from edgeimpulse_api.models.get_email_verification_status_response import GetEmailVerificationStatusResponse
+from edgeimpulse_api.models.get_email_verification_status_response_all_of import GetEmailVerificationStatusResponseAllOf
 from edgeimpulse_api.models.get_impulse_blocks_response import GetImpulseBlocksResponse
 from edgeimpulse_api.models.get_impulse_blocks_response_all_of import GetImpulseBlocksResponseAllOf
 from edgeimpulse_api.models.get_impulse_response import GetImpulseResponse
 from edgeimpulse_api.models.get_impulse_response_all_of import GetImpulseResponseAllOf
 from edgeimpulse_api.models.get_jwt_request import GetJWTRequest
 from edgeimpulse_api.models.get_jwt_response import GetJWTResponse
 from edgeimpulse_api.models.get_jwt_response_all_of import GetJWTResponseAllOf
@@ -408,14 +419,16 @@
 from edgeimpulse_api.models.list_api_keys_response_all_of import ListApiKeysResponseAllOf
 from edgeimpulse_api.models.list_api_keys_response_all_of_api_keys import ListApiKeysResponseAllOfApiKeys
 from edgeimpulse_api.models.list_devices_response import ListDevicesResponse
 from edgeimpulse_api.models.list_devices_response_all_of import ListDevicesResponseAllOf
 from edgeimpulse_api.models.list_email_response import ListEmailResponse
 from edgeimpulse_api.models.list_email_response_all_of import ListEmailResponseAllOf
 from edgeimpulse_api.models.list_email_response_all_of_emails import ListEmailResponseAllOfEmails
+from edgeimpulse_api.models.list_enterprise_trials_response import ListEnterpriseTrialsResponse
+from edgeimpulse_api.models.list_enterprise_trials_response_all_of import ListEnterpriseTrialsResponseAllOf
 from edgeimpulse_api.models.list_hmac_keys_response import ListHmacKeysResponse
 from edgeimpulse_api.models.list_hmac_keys_response_all_of import ListHmacKeysResponseAllOf
 from edgeimpulse_api.models.list_hmac_keys_response_all_of_hmac_keys import ListHmacKeysResponseAllOfHmacKeys
 from edgeimpulse_api.models.list_jobs_response import ListJobsResponse
 from edgeimpulse_api.models.list_jobs_response_all_of import ListJobsResponseAllOf
 from edgeimpulse_api.models.list_models_response import ListModelsResponse
 from edgeimpulse_api.models.list_models_response_all_of import ListModelsResponseAllOf
@@ -632,14 +645,15 @@
 from edgeimpulse_api.models.raw_sample_payload import RawSamplePayload
 from edgeimpulse_api.models.rebalance_dataset_response import RebalanceDatasetResponse
 from edgeimpulse_api.models.remove_collaborator_request import RemoveCollaboratorRequest
 from edgeimpulse_api.models.remove_member_request import RemoveMemberRequest
 from edgeimpulse_api.models.rename_device_request import RenameDeviceRequest
 from edgeimpulse_api.models.rename_portal_file_request import RenamePortalFileRequest
 from edgeimpulse_api.models.rename_sample_request import RenameSampleRequest
+from edgeimpulse_api.models.request_email_verification_request import RequestEmailVerificationRequest
 from edgeimpulse_api.models.request_reset_password_request import RequestResetPasswordRequest
 from edgeimpulse_api.models.reset_password_request import ResetPasswordRequest
 from edgeimpulse_api.models.restore_project_from_public_request import RestoreProjectFromPublicRequest
 from edgeimpulse_api.models.restore_project_request import RestoreProjectRequest
 from edgeimpulse_api.models.run_auto_segmenter_request import RunAutoSegmenterRequest
 from edgeimpulse_api.models.run_organization_pipeline_response import RunOrganizationPipelineResponse
 from edgeimpulse_api.models.run_organization_pipeline_response_all_of import RunOrganizationPipelineResponseAllOf
@@ -672,14 +686,15 @@
 from edgeimpulse_api.models.set_syntiant_posterior_request import SetSyntiantPosteriorRequest
 from edgeimpulse_api.models.set_user_password_request import SetUserPasswordRequest
 from edgeimpulse_api.models.socket_token_response import SocketTokenResponse
 from edgeimpulse_api.models.socket_token_response_all_of import SocketTokenResponseAllOf
 from edgeimpulse_api.models.socket_token_response_all_of_token import SocketTokenResponseAllOfToken
 from edgeimpulse_api.models.split_sample_in_frames_request import SplitSampleInFramesRequest
 from edgeimpulse_api.models.staff_info import StaffInfo
+from edgeimpulse_api.models.start_enterprise_trial_request import StartEnterpriseTrialRequest
 from edgeimpulse_api.models.start_job_response import StartJobResponse
 from edgeimpulse_api.models.start_job_response_all_of import StartJobResponseAllOf
 from edgeimpulse_api.models.start_performance_calibration_request import StartPerformanceCalibrationRequest
 from edgeimpulse_api.models.start_sampling_request import StartSamplingRequest
 from edgeimpulse_api.models.start_sampling_response import StartSamplingResponse
 from edgeimpulse_api.models.start_sampling_response_all_of import StartSamplingResponseAllOf
 from edgeimpulse_api.models.start_training_request_anomaly import StartTrainingRequestAnomaly
@@ -741,14 +756,16 @@
 from edgeimpulse_api.models.user_by_third_party_activation_request import UserByThirdPartyActivationRequest
 from edgeimpulse_api.models.user_experiment import UserExperiment
 from edgeimpulse_api.models.user_organization import UserOrganization
 from edgeimpulse_api.models.verify_dsp_block_url_request import VerifyDspBlockUrlRequest
 from edgeimpulse_api.models.verify_dsp_block_url_response import VerifyDspBlockUrlResponse
 from edgeimpulse_api.models.verify_dsp_block_url_response_all_of import VerifyDspBlockUrlResponseAllOf
 from edgeimpulse_api.models.verify_dsp_block_url_response_all_of_block import VerifyDspBlockUrlResponseAllOfBlock
+from edgeimpulse_api.models.verify_email_response import VerifyEmailResponse
+from edgeimpulse_api.models.verify_email_response_all_of import VerifyEmailResponseAllOf
 from edgeimpulse_api.models.verify_organization_bucket_request import VerifyOrganizationBucketRequest
 from edgeimpulse_api.models.verify_organization_bucket_response import VerifyOrganizationBucketResponse
 from edgeimpulse_api.models.verify_organization_bucket_response_all_of import VerifyOrganizationBucketResponseAllOf
 from edgeimpulse_api.models.verify_organization_bucket_response_all_of_files import VerifyOrganizationBucketResponseAllOfFiles
 from edgeimpulse_api.models.verify_reset_password_request import VerifyResetPasswordRequest
 from edgeimpulse_api.models.whitelabel import Whitelabel
 from edgeimpulse_api.models.whitelabel_admin_create_organization_request import WhitelabelAdminCreateOrganizationRequest
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/activate_user_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/activate_user_or_verify_email_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import re  # noqa: F401
 import json
 
 
 
 from pydantic import BaseModel, Field, StrictStr
 
-class ActivateUserRequest(BaseModel):
-    code: StrictStr = Field(..., description="Activation code (sent through an email)")
+class ActivateUserOrVerifyEmailRequest(BaseModel):
+    code: StrictStr = Field(..., description="Activation or verification code (sent via email)")
     __properties = ["code"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
@@ -33,33 +33,33 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ActivateUserRequest:
-        """Create an instance of ActivateUserRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> ActivateUserOrVerifyEmailRequest:
+        """Create an instance of ActivateUserOrVerifyEmailRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ActivateUserRequest:
-        """Create an instance of ActivateUserRequest from a dict"""
+    def from_dict(cls, obj: dict) -> ActivateUserOrVerifyEmailRequest:
+        """Create an instance of ActivateUserOrVerifyEmailRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ActivateUserRequest.construct(**obj)
+            return ActivateUserOrVerifyEmailRequest.construct(**obj)
 
-        _obj = ActivateUserRequest.construct(**{
+        _obj = ActivateUserOrVerifyEmailRequest.construct(**{
             "code": obj.get("code")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_api_key_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_collaborator_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_hmac_key_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_hmac_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_member_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_api_key_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_bucket_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_data_campaign_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_data_campaign_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_deploy_block_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_deploy_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_dsp_block_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_dsp_block_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_dsp_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_secret_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_secret_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_secret_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_secret_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_secret_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_secret_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_transformation_block_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_transformation_block_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_transformation_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_add_organization_user_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_add_organization_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_add_project_user_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_add_project_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_add_user_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_add_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_api_organization.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_api_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_api_organization_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_api_organization_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_api_project.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_api_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_api_user.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_api_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     projects: List[Project] = ...
     experiments: List[UserExperiment] = Field(..., description="Experiments the user has access to. Enabling experiments can only be done through a JWT token.")
     evaluation: Optional[StrictBool] = Field(None, description="Whether this is an ephemeral evaluation account.")
     ambassador: Optional[StrictBool] = Field(None, description="Whether this user is an ambassador.")
     show_imagine2022: StrictBool = Field(..., alias="showImagine2022", description="Whether to show the Imagine 2022 banner.")
     tier: StrictStr = Field(..., description="The user account tier.")
     suspended: StrictBool = Field(..., description="Whether the user is suspended.")
-    trials: List[EnterpriseTrial] = Field(..., description="Current, past or future enterprise trials.")
+    trials: List[EnterpriseTrial] = Field(..., description="Current or past enterprise trials.")
     __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "organizations", "projects", "experiments", "evaluation", "ambassador", "showImagine2022", "tier", "suspended", "trials"]
 
     @validator('tier')
     def tier_validate_enum(cls, v):
         if v not in ('free', 'pro'):
             raise ValueError("must validate the enum values ('free', 'pro')")
         return v
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_api_user_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_api_user_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     experiments: List[UserExperiment] = Field(..., description="Experiments the user has access to. Enabling experiments can only be done through a JWT token.")
     evaluation: Optional[StrictBool] = Field(None, description="Whether this is an ephemeral evaluation account.")
     ambassador: Optional[StrictBool] = Field(None, description="Whether this user is an ambassador.")
     show_imagine2022: StrictBool = Field(..., alias="showImagine2022", description="Whether to show the Imagine 2022 banner.")
     tier: StrictStr = Field(..., description="The user account tier.")
     last_seen: Optional[datetime] = Field(None, alias="lastSeen")
     suspended: StrictBool = Field(..., description="Whether the user is suspended.")
-    trials: List[EnterpriseTrial] = Field(..., description="Current, past or future enterprise trials.")
+    trials: List[EnterpriseTrial] = Field(..., description="Current or past enterprise trials.")
     __properties = ["email", "activated", "organizations", "projects", "experiments", "evaluation", "ambassador", "showImagine2022", "tier", "lastSeen", "suspended", "trials"]
 
     @validator('tier')
     def tier_validate_enum(cls, v):
         if v not in ('free', 'pro'):
             raise ValueError("must validate the enum values ('free', 'pro')")
         return v
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_create_organization_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_create_user_trial_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/user_organization.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,56 +14,74 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 
-class AdminCreateUserTrialRequest(BaseModel):
-    organization_name: Optional[StrictStr] = Field(None, alias="organizationName", description="Name of the trial organization. All enterprise features are tied to an organization. This organization will be deleted after the trial ends. If no organization name is provided, the user's name will be used.")
-    expiration_date: datetime = Field(..., alias="expirationDate", description="Expiration date of the trial. The trial will be set as expired after this date. There will be a grace period of 30 days after a trial expires before fully deleting the trial organization.")
-    notes: Optional[StrictStr] = Field(None, description="Notes about the trial. Free form text.")
-    __properties = ["organizationName", "expirationDate", "notes"]
+class UserOrganization(BaseModel):
+    id: StrictInt = ...
+    name: StrictStr = ...
+    logo: Optional[StrictStr] = None
+    is_developer_profile: StrictBool = Field(..., alias="isDeveloperProfile")
+    whitelabel_id: Optional[StrictInt] = Field(..., alias="whitelabelId", description="Unique identifier of the white label this project belongs to, if any.")
+    is_admin: StrictBool = Field(..., alias="isAdmin", description="Whether the user is admin of this organization or not.")
+    created: datetime = Field(..., description="When the organization was created.")
+    trial_id: Optional[float] = Field(..., alias="trialId", description="Unique identifier of the trial this organization belongs to, if any.")
+    __properties = ["id", "name", "logo", "isDeveloperProfile", "whitelabelId", "isAdmin", "created", "trialId"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AdminCreateUserTrialRequest:
-        """Create an instance of AdminCreateUserTrialRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> UserOrganization:
+        """Create an instance of UserOrganization from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # set to None if whitelabel_id (nullable) is None
+        if self.whitelabel_id is None:
+            _dict['whitelabelId'] = None
+
+        # set to None if trial_id (nullable) is None
+        if self.trial_id is None:
+            _dict['trialId'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AdminCreateUserTrialRequest:
-        """Create an instance of AdminCreateUserTrialRequest from a dict"""
+    def from_dict(cls, obj: dict) -> UserOrganization:
+        """Create an instance of UserOrganization from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AdminCreateUserTrialRequest.construct(**obj)
+            return UserOrganization.construct(**obj)
 
-        _obj = AdminCreateUserTrialRequest.construct(**{
-            "organization_name": obj.get("organizationName"),
-            "expiration_date": obj.get("expirationDate"),
-            "notes": obj.get("notes")
+        _obj = UserOrganization.construct(**{
+            "id": obj.get("id"),
+            "name": obj.get("name"),
+            "logo": obj.get("logo"),
+            "is_developer_profile": obj.get("isDeveloperProfile"),
+            "whitelabel_id": obj.get("whitelabelId"),
+            "is_admin": obj.get("isAdmin"),
+            "created": obj.get("created"),
+            "trial_id": obj.get("trialId")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_data_migration_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_data_migration_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_data_migrations_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_data_migrations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_metrics_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_metrics_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_organizations_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_organizations_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_sso_settings_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_sso_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_ids_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_ids_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_metrics_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_metrics_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_models_response_all_of.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,53 +13,53 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict
-from pydantic import BaseModel
+from typing import Optional
+from pydantic import BaseModel, Field, StrictInt
 
-class AdminGetUserMetricsResponseAllOf(BaseModel):
-    metrics: Dict[str, Any] = ...
-    __properties = ["metrics"]
+class ListModelsResponseAllOf(BaseModel):
+    id: Optional[StrictInt] = Field(None, description="projectId")
+    __properties = ["id"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AdminGetUserMetricsResponseAllOf:
-        """Create an instance of AdminGetUserMetricsResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> ListModelsResponseAllOf:
+        """Create an instance of ListModelsResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AdminGetUserMetricsResponseAllOf:
-        """Create an instance of AdminGetUserMetricsResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> ListModelsResponseAllOf:
+        """Create an instance of ListModelsResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AdminGetUserMetricsResponseAllOf.construct(**obj)
+            return ListModelsResponseAllOf.construct(**obj)
 
-        _obj = AdminGetUserMetricsResponseAllOf.construct(**{
-            "metrics": obj.get("metrics")
+        _obj = ListModelsResponseAllOf.construct(**{
+            "id": obj.get("id")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_trial_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_users_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_users_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_users_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_users_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_get_users_response_all_of_users.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_get_users_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_list_projects.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_list_projects_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_organization_info_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_organization_info_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_toggle_data_migration_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_toggle_data_migration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_update_organization_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_update_user_permissions_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_update_user_permissions_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_update_user_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/admin_update_user_trial_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/admin_update_user_trial_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
 class AdminUpdateUserTrialRequest(BaseModel):
-    expiration_date: Optional[datetime] = Field(None, alias="expirationDate", description="Expiration date of the trial. The trial will be set as expired after this date. There will be a grace period of 30 days after a trial expires before fully deleting the trial organization.")
-    notes: Optional[StrictStr] = Field(None, description="Notes about the trial. Free form text.")
+    expiration_date: Optional[datetime] = Field(None, alias="expirationDate", description="Expiration date of the trial. The trial will be set as expired after this date. There will be a grace period of 30 days after a trial expires before fully deleting the trial organization. This field is ignored if the trial is requested by a non-admin user, defaulting to 14 days trial.")
+    notes: Optional[StrictStr] = Field(None, description="Notes about the trial. Free form text. This field is ignored if the trial is requested by a non-admin user.")
     __properties = ["expirationDate", "notes"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/akida_edge_learning_config.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/akida_edge_learning_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_model_metadata.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_model_metadata_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_model_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_response_all_of_axes.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_response_all_of_axes.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_trained_features_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/augmentation_policy_spectrogram.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/augmentation_policy_spectrogram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/autotune_dsp_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/autotune_dsp_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/bounding_box.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/bounding_box.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/bounding_box_with_score.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/bounding_box_with_score.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/build_on_device_model_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/build_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/build_organization_on_device_model_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/build_organization_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/calculate_data_quality_metrics_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/calculate_data_quality_metrics_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/change_password_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/change_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_job_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_job_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_job_response_page.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_job_response_page.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_job_response_page_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_job_response_page_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_sample_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_sample_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_sample_response_classification.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_sample_response_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/classify_sample_response_classification_details.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/classify_sample_response_classification_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/convert_user_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/convert_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/count_samples_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/count_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/count_samples_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/count_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_block_version_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_block_version_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_block_version_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_block_version_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_developer_profile_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_developer_profile_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_developer_profile_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_developer_profile_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_device_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_evaluation_user_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_evaluation_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_evaluation_user_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_evaluation_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_organization_portal_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_organization_portal_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_organization_portal_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_organization_portal_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_organization_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_organization_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_organization_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_organization_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_organization_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_pipeline_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_project_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_project_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_project_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_signed_upload_link_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_signed_upload_link_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_signed_upload_link_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_signed_upload_link_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_third_party_auth_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_third_party_auth_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_user_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_user_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     password: Optional[StrictStr] = Field(None, description="Password, minimum length 8 characters.")
     project_name: Optional[StrictStr] = Field(None, alias="projectName", description="A project will automatically be created. Sets the name of the first project. If not set, this will be derived from the username.")
     privacy_policy: StrictBool = Field(..., alias="privacyPolicy", description="Whether the user accepted the privacy policy")
     activation_token: Optional[StrictStr] = Field(None, alias="activationToken", description="Activation token for users created via SSO")
     identity_provider: Optional[StrictStr] = Field(None, alias="identityProvider", description="Unique identifier of the identity provider asserting the identity of this user")
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle", description="Job title of the user. Optional field")
     session_id: Optional[StrictStr] = Field(None, alias="sessionId", description="Session ID. Optional field")
-    __properties = ["name", "username", "email", "password", "projectName", "privacyPolicy", "activationToken", "identityProvider", "jobTitle", "sessionId"]
+    company_name: Optional[StrictStr] = Field(None, alias="companyName", description="ACME Inc.")
+    __properties = ["name", "username", "email", "password", "projectName", "privacyPolicy", "activationToken", "identityProvider", "jobTitle", "sessionId", "companyName"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -73,11 +74,12 @@
             "email": obj.get("email"),
             "password": obj.get("password"),
             "project_name": obj.get("projectName"),
             "privacy_policy": obj.get("privacyPolicy"),
             "activation_token": obj.get("activationToken"),
             "identity_provider": obj.get("identityProvider"),
             "job_title": obj.get("jobTitle"),
-            "session_id": obj.get("sessionId")
+            "session_id": obj.get("sessionId"),
+            "company_name": obj.get("companyName")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_user_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_user_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_user_third_party_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_user_third_party_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_user_third_party_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_user_third_party_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_user_third_party_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_user_third_party_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_whitelabel_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_whitelabel_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/create_whitelabel_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/crop_sample_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/crop_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/crop_sample_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/crop_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/crop_sample_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/crop_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign_dashboard.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign_dashboard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign_graph.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign_link.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign_link.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_campaign_query.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_campaign_query.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_explorer_predictions_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_explorer_predictions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/data_explorer_settings.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/data_explorer_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dataset_ratio_data.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dataset_ratio_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dataset_ratio_data_ratio.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dataset_ratio_data_ratio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/delete_portal_file_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/delete_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dependency_data.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dependency_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_input_image.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_input_image.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_input_other.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_input_other.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deployment_target.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deployment_target_badge.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deployment_target_badge.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deployment_target_engine.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deployment_target_engine.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deployment_targets_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/deployment_targets_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/development_board.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/development_board.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/development_boards_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/development_boards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/development_boards_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/development_boards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/development_keys.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/development_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/development_keys_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/development_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/device.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/device_name_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/device_name_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/device_name_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/device_name_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/device_sensors_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/device_sensors_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/download.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/download.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/download_portal_file_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/download_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/download_portal_file_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/download_portal_file_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/download_portal_file_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/download_portal_file_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_autotuner_results.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_autotuner_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_autotuner_results_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_autotuner_results_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_block.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_config_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_config_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_config_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_config_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_feature_importance_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_feature_importance_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_feature_labels_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_feature_labels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_group.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_group.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_group_item.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_group_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_group_item_select_options_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_group_item_select_options_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_group_item_show_if.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_group_item_show_if.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_info.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_info_features.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_info_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_info_performance.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_info_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_metadata.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_metadata_output_config.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_metadata_output_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_metadata_output_config_shape.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_metadata_output_config_shape.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_metadata_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_performance_all_variants_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_performance_all_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_graph.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_graph_axis_labels.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_graph_axis_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_request_with_features.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_request_with_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_request_without_features.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_request_without_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_response_all_of_performance.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_response_with_sample.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_response_with_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_sample_features_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_sample_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_sample_features_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_sample_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_trained_features_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_trained_features_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/edit_sample_label_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/edit_sample_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/enterprise_trial.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/enterprise_trial.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
 class EnterpriseTrial(BaseModel):
     id: StrictInt = Field(..., description="Unique identifier of the trial.")
-    user_id: StrictInt = Field(..., alias="userId", description="ID of the user who created the trial.")
-    organization_id: StrictInt = Field(..., alias="organizationId", description="ID of the organization created for the trial.")
+    user_id: Optional[StrictInt] = Field(None, alias="userId", description="ID of the user who created the trial.")
+    organization_id: Optional[StrictInt] = Field(None, alias="organizationId", description="ID of the organization created for the trial.")
     created: datetime = Field(..., description="Date when the trial was created. Trials start immediately on creation.")
-    expiration_date: datetime = Field(..., alias="expirationDate", description="Expiration date of the trial. The trial will be set as expired after this date. There will be a grace period of 30 days after a trial expires before fully deleting the trial organization.")
-    notes: Optional[StrictStr] = Field(None, description="Notes about the trial. Free form text.")
+    expiration_date: datetime = Field(..., alias="expirationDate", description="Expiration date of the trial. The trial will be set as expired after this date. There will be a grace period of 30 days after a trial expires before fully deleting the trial organization. This field is ignored if the trial is requested by a non-admin user, defaulting to 14 days trial.")
+    notes: Optional[StrictStr] = Field(None, description="Notes about the trial. Free form text. This field is ignored if the trial is requested by a non-admin user.")
     expired_date: Optional[datetime] = Field(..., alias="expiredDate", description="Date when the trial actually expired. This is set when the trial is expired by the system.")
     deleted_date: Optional[datetime] = Field(..., alias="deletedDate", description="Date when the trial was deleted. This is set when the trial is fully  deleted by the system.")
     __properties = ["id", "userId", "organizationId", "created", "expirationDate", "notes", "expiredDate", "deletedDate"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/entitlement_limits.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/entitlement_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/entity_created_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/generic_api_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,56 +14,54 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class EntityCreatedResponse(BaseModel):
+class GenericApiResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    id: StrictInt = ...
-    __properties = ["success", "error", "id"]
+    __properties = ["success", "error"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> EntityCreatedResponse:
-        """Create an instance of EntityCreatedResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> GenericApiResponse:
+        """Create an instance of GenericApiResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> EntityCreatedResponse:
-        """Create an instance of EntityCreatedResponse from a dict"""
+    def from_dict(cls, obj: dict) -> GenericApiResponse:
+        """Create an instance of GenericApiResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return EntityCreatedResponse.construct(**obj)
+            return GenericApiResponse.construct(**obj)
 
-        _obj = EntityCreatedResponse.construct(**{
+        _obj = GenericApiResponse.construct(**{
             "success": obj.get("success"),
-            "error": obj.get("error"),
-            "id": obj.get("id")
+            "error": obj.get("error")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/evaluate_job_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/evaluate_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/evaluate_job_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/evaluate_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/evaluate_result_value.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/evaluate_result_value.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/export_get_url_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/export_get_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/export_get_url_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/export_get_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/export_keras_block_data_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/export_keras_block_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/export_original_data_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/export_original_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/export_wav_data_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/export_wav_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_segment_sample_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_segment_sample_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_segment_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_segment_sample_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_segment_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_user_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_user_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/find_user_response_all_of_users.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/find_user_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/generate_features_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/generate_features_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/generic_api_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_email_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,52 +16,58 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class GenericApiResponse(BaseModel):
+class VerifyEmailResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    __properties = ["success", "error"]
+    email: Optional[StrictStr] = Field(None, description="Email address that was verified.")
+    user_id: Optional[float] = Field(None, alias="userId", description="ID of the user associated with the verified email address, if any.")
+    redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="URL to redirect the user to after email verification.")
+    __properties = ["success", "error", "email", "userId", "redirectUrl"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GenericApiResponse:
-        """Create an instance of GenericApiResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyEmailResponse:
+        """Create an instance of VerifyEmailResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GenericApiResponse:
-        """Create an instance of GenericApiResponse from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyEmailResponse:
+        """Create an instance of VerifyEmailResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return GenericApiResponse.construct(**obj)
+            return VerifyEmailResponse.construct(**obj)
 
-        _obj = GenericApiResponse.construct(**{
+        _obj = VerifyEmailResponse.construct(**{
             "success": obj.get("success"),
-            "error": obj.get("error")
+            "error": obj.get("error"),
+            "email": obj.get("email"),
+            "user_id": obj.get("userId"),
+            "redirect_url": obj.get("redirectUrl")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_imported_from_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_imported_from_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_imported_from_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_imported_from_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_third_party_auth_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_whitelabels_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_whitelabels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_auto_segmenter_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_auto_segmenter_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_auto_segmenter_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_auto_segmenter_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_auto_segmenter_response_all_of_clusters.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_auto_segmenter_response_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_auto_segmenter_response_all_of_items.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_auto_segmenter_response_all_of_items.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_data_explorer_features_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_data_explorer_settings_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_data_explorer_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_deployment_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_deployment_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_deployment_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_deployment_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_device_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_device_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_device_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_device_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_diversity_data_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_diversity_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_diversity_data_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_diversity_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_impulse_blocks_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_impulse_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_impulse_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_impulse_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_impulse_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_impulse_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_job_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_job_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_jwt_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_jwt_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_jwt_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_jwt_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_jwt_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_jwt_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_last_deployment_build_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_last_deployment_build_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_notes_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_notes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_notes_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_notes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaign_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaigns_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaigns_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_item_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_item_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_item_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_dataset_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_dataset_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_dataset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_pipelines_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_portal_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_portal_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_organization_projects_data_count_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_organization_projects_data_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_parameters_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_status_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_pretrained_model_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_public_metrics_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_public_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_public_metrics_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_public_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_sample_metadata_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_sample_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_sample_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_syntiant_posterior_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_syntiant_posterior_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_theme_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_theme_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_theme_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_theme_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_themes_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_themes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_themes_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_themes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_third_party_auth_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_user_need_to_set_password_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/upload_asset_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,61 +13,57 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class GetUserNeedToSetPasswordResponse(BaseModel):
+class UploadAssetResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    email: Optional[StrictStr] = Field(None, description="User email")
-    need_password: Optional[StrictBool] = Field(None, alias="needPassword", description="Whether the user needs to set its password or not")
-    whitelabels: Optional[List[StrictStr]] = Field(None, description="White label domains the user belongs to, if any")
-    __properties = ["success", "error", "email", "needPassword", "whitelabels"]
+    url: Optional[StrictStr] = None
+    __properties = ["success", "error", "url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GetUserNeedToSetPasswordResponse:
-        """Create an instance of GetUserNeedToSetPasswordResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> UploadAssetResponse:
+        """Create an instance of UploadAssetResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetUserNeedToSetPasswordResponse:
-        """Create an instance of GetUserNeedToSetPasswordResponse from a dict"""
+    def from_dict(cls, obj: dict) -> UploadAssetResponse:
+        """Create an instance of UploadAssetResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return GetUserNeedToSetPasswordResponse.construct(**obj)
+            return UploadAssetResponse.construct(**obj)
 
-        _obj = GetUserNeedToSetPasswordResponse.construct(**{
+        _obj = UploadAssetResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
-            "email": obj.get("email"),
-            "need_password": obj.get("needPassword"),
-            "whitelabels": obj.get("whitelabels")
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/upload_asset_response_all_of.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,57 +13,53 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from typing import Optional
+from pydantic import BaseModel, StrictStr
 
-class GetUserNeedToSetPasswordResponseAllOf(BaseModel):
-    email: Optional[StrictStr] = Field(None, description="User email")
-    need_password: Optional[StrictBool] = Field(None, alias="needPassword", description="Whether the user needs to set its password or not")
-    whitelabels: Optional[List[StrictStr]] = Field(None, description="White label domains the user belongs to, if any")
-    __properties = ["email", "needPassword", "whitelabels"]
+class UploadAssetResponseAllOf(BaseModel):
+    url: Optional[StrictStr] = None
+    __properties = ["url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GetUserNeedToSetPasswordResponseAllOf:
-        """Create an instance of GetUserNeedToSetPasswordResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> UploadAssetResponseAllOf:
+        """Create an instance of UploadAssetResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetUserNeedToSetPasswordResponseAllOf:
-        """Create an instance of GetUserNeedToSetPasswordResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> UploadAssetResponseAllOf:
+        """Create an instance of UploadAssetResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return GetUserNeedToSetPasswordResponseAllOf.construct(**obj)
+            return UploadAssetResponseAllOf.construct(**obj)
 
-        _obj = GetUserNeedToSetPasswordResponseAllOf.construct(**{
-            "email": obj.get("email"),
-            "need_password": obj.get("needPassword"),
-            "whitelabels": obj.get("whitelabels")
+        _obj = UploadAssetResponseAllOf.construct(**{
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_user_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_user_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_whitelabel_domain_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_whitelabel_domain_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_whitelabel_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/get_whitelabel_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/get_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/has_data_explorer_features_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/has_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/image_input_scaling.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/image_input_scaling.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/impulse.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/impulse_block_version.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/impulse_block_version.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/impulse_dsp_block.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/impulse_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/impulse_dsp_block_organization.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/impulse_dsp_block_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/impulse_input_block.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/impulse_input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/impulse_learn_block.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/impulse_learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/input_block.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/invite_organization_member_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/invite_organization_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_details.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_details_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_details_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_details_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_details_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_details_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_details_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_failure_details.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_failure_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_logs_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_logs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_logs_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_logs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_metrics_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_metrics_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_parent_type_enum.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_parent_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_state.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_state.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_state_execution_details.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_state_execution_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_step.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_summary_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_summary_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/job_summary_response_all_of_summary.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/job_summary_response_all_of_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_layer.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_layer_input.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_layer_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_layer_output.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_layer_output.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_metadata.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_metadata_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_metadata_metrics.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_metadata_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_model_type_enum.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_model_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_visual_layer.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_visual_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/keras_visual_layer_type.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/keras_visual_layer_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/last_modification_date_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/last_modification_date_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/last_modification_date_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/last_modification_date_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/latency_device.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/latency_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/learn_block.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/learn_block_type.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/learn_block_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_api_keys_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_api_keys_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_devices_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_devices_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_devices_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_devices_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_email_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_email_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_email_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_email_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_email_response_all_of_emails.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_email_response_all_of_emails.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_hmac_keys_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_hmac_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_hmac_keys_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_hmac_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_jobs_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_jobs_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_models_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_models_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/entity_created_response_all_of.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt
 
-class ListModelsResponseAllOf(BaseModel):
-    id: Optional[StrictInt] = Field(None, description="projectId")
+class EntityCreatedResponseAllOf(BaseModel):
+    id: Optional[StrictInt] = Field(None, description="Unique identifier of the created entity, if any.")
     __properties = ["id"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
@@ -33,33 +33,37 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ListModelsResponseAllOf:
-        """Create an instance of ListModelsResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> EntityCreatedResponseAllOf:
+        """Create an instance of EntityCreatedResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # set to None if id (nullable) is None
+        if self.id is None:
+            _dict['id'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ListModelsResponseAllOf:
-        """Create an instance of ListModelsResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> EntityCreatedResponseAllOf:
+        """Create an instance of EntityCreatedResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ListModelsResponseAllOf.construct(**obj)
+            return EntityCreatedResponseAllOf.construct(**obj)
 
-        _obj = ListModelsResponseAllOf.construct(**{
+        _obj = EntityCreatedResponseAllOf.construct(**{
             "id": obj.get("id")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_api_keys_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_buckets_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_buckets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_buckets_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_buckets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_buckets_user_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_buckets_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_data_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_data_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_data_response_all_of_data.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_deploy_blocks_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_deploy_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_dsp_blocks_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_dsp_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_files_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_files_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_files_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_files_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_pipelines_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_portals_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_portals_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_portals_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_portals_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_projects_data_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_projects_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_projects_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_projects_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_projects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_secrets_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_secrets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_secrets_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_secrets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_transformation_blocks_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_transformation_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organizations_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_organizations_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_portal_files_in_folder_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_portal_files_in_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_portal_files_in_folder_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_portal_files_in_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_projects.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_projects_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_public_projects.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_public_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_public_projects_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_public_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_public_versions_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_public_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_public_versions_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_public_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_samples_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_samples_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_versions_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_versions_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_versions_response_all_of_bucket.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_versions_response_all_of_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/list_versions_response_all_of_versions.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/log_stdout_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/log_stdout_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/log_stdout_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/log_stdout_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/log_website_pageview_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/log_website_pageview_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/login_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/login_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/login_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/login_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/migration.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/migration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/model_prediction.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/model_prediction.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/model_result.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/model_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/model_variant_stats.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/model_variant_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/move_raw_data_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/move_raw_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/note.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/note.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_auto_label_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_auto_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_auto_label_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_auto_label_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_label_queue_count_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_label_queue_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_label_queue_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_label_queue_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/object_detection_last_layer.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/object_detection_last_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_config.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_config_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_config_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_config_target_device.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_config_target_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_dsp_parameters_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_dsp_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_space_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_space_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_space_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_space_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_state_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_state_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_state_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_state_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_state_response_all_of_status.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_state_response_all_of_status.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_state_response_all_of_workers.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_state_response_all_of_workers.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_transfer_learning_models_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_transfer_learning_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_add_data_folder_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_add_data_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_add_data_folder_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_add_data_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_add_dataset_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_add_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_add_dataset_request_bucket.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_add_dataset_request_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_status_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_status_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_transformation_summary.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_transformation_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_with_files.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_with_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_with_files_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_with_files_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_campaign_diff_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_campaign_diff_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_campaign_diff_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_campaign_diff_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_item.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_data_item_files_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_data_item_files_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_dataset.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_dataset_bucket.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_dataset_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_deploy_block.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_deploy_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_dsp_block.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_get_create_projects_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_get_create_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_info_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_info_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_member_role.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_member_role.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_metrics_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_metrics_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline_item_count.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline_item_count.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline_run.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline_run.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline_run_step.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline_run_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_pipeline_step.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_projects_data_batch_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_projects_data_batch_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_transfer_learning_block.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_transfer_learning_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_transfer_learning_operates_on.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_transfer_learning_operates_on.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_transformation_block.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_transformation_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_update_pipeline_body.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_update_pipeline_body.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_user.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/organization_user_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/organization_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_detection.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_false_positive.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_false_positive.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_ground_truth.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_ground_truth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_parameter_set.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_parameter_set.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_parameters.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_parameters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_parameters_standard.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_parameters_standard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_raw_detection.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_raw_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/permission.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/permission.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 class Permission(str, Enum):
     """
     allowed enum values
     """
 
     ADMININFRADISALLOWED_EMAIL_DOMAINSWRITE = 'admin:infra:disallowedEmailDomains:write'
+    ADMININFRAFEATURE_FLAGSREAD = 'admin:infra:featureFlags:read'
+    ADMININFRAFEATURE_FLAGSWRITE = 'admin:infra:featureFlags:write'
     ADMININFRAMIGRATIONSREAD = 'admin:infra:migrations:read'
     ADMININFRAMIGRATIONSWRITE = 'admin:infra:migrations:write'
     ADMINMETRICSREAD = 'admin:metrics:read'
     ADMINORGANIZATIONSREAD = 'admin:organizations:read'
     ADMINORGANIZATIONSWRITE = 'admin:organizations:write'
     ADMINORGANIZATIONSMEMBERSWRITE = 'admin:organizations:members:write'
     ADMINPROJECTSMEMBERSWRITE = 'admin:projects:members:write'
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/portal_file.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/portal_file.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/portal_info_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/portal_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/pretrained_model_tensor.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/pretrained_model_tensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_info.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_info_memory.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_info_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_info_memory_eon.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_info_memory_eon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_info_memory_tflite.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_info_memory_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_table.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_table.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_table_mcu.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_table_mcu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_table_mcu_memory.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_table_mcu_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_model_table_mpu.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_model_table_mpu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_tf_lite_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_tf_lite_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/profile_tf_lite_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/profile_tf_lite_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_collaborator.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_collaborator.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_collaborator_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_collaborator_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_data_axes_summary_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_data_axes_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_data_interval_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_data_interval_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_data_interval_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_data_interval_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_data_summary.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_data_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_deployment_target.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_deployment_target_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_deployment_target_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_deployment_targets_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_deployment_targets_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_downloads_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_downloads_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_downloads_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_downloads_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_compute_time.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_compute_time.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_experiments.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_experiments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_impulse.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_performance.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_readme.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_response_all_of_urls.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_response_all_of_urls.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_summary_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_info_summary_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_info_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_private_data.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_private_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_public_data.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_public_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_public_data_readme.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_public_data_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_sample_metadata.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_training_data_summary_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_training_data_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_training_data_summary_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_training_data_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_type.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/project_version_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/project_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/raw_sample_data.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/raw_sample_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/raw_sample_payload.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/raw_sample_payload.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/rebalance_dataset_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/rebalance_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/remove_collaborator_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/remove_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/remove_member_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/remove_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/rename_device_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/rename_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/rename_portal_file_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/rename_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/rename_sample_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/rename_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/request_reset_password_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/request_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/reset_password_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/restore_project_from_public_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/restore_project_from_public_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/restore_project_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/restore_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/run_auto_segmenter_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/run_auto_segmenter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/run_organization_pipeline_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/run_organization_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/sample.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/sample_bounding_boxes_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/sample_bounding_boxes_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/sample_metadata.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/save_auto_segmenter_clusters_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/save_auto_segmenter_clusters_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/save_auto_segmenter_clusters_request_clusters_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/save_auto_segmenter_clusters_request_clusters_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/save_auto_segmenter_clusters_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/save_auto_segmenter_clusters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/save_auto_segmenter_clusters_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/save_auto_segmenter_clusters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/save_pretrained_model_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/save_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/score_trial_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/score_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/score_trial_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/score_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/score_trial_response_all_of_latency.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/score_trial_response_all_of_latency.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/score_trial_response_all_of_ram.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/score_trial_response_all_of_ram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/segment_sample_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/segment_sample_request_segments_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/segment_sample_request_segments_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/send_user_feedback_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/send_user_feedback_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/sensor.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/sensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_anomaly_parameter_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_anomaly_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_keras_parameter_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_keras_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_member_datasets_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_member_datasets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_member_role_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_member_role_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_optimize_space_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_optimize_space_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_optimize_space_request_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_optimize_space_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_organization_data_dataset_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_organization_data_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_project_compute_time_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_project_compute_time_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_project_dsp_file_size_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_project_dsp_file_size_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_sample_metadata_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_sample_metadata_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_syntiant_posterior_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_syntiant_posterior_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/set_user_password_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/set_user_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/socket_token_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/socket_token_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/socket_token_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/socket_token_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/socket_token_response_all_of_token.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/socket_token_response_all_of_token.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/split_sample_in_frames_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/split_sample_in_frames_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/staff_info.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/staff_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_job_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_job_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_performance_calibration_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_performance_calibration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_sampling_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_sampling_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_sampling_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_sampling_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_sampling_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_sampling_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/start_training_request_anomaly.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/start_training_request_anomaly.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/store_segment_length_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/store_segment_length_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/structured_classify_result.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/structured_classify_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/test_pretrained_model_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/test_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/test_pretrained_model_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/test_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/test_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/test_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/theme.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/theme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/theme_colors.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/theme_colors.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/theme_favicon.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/theme_favicon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/theme_logos.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/theme_logos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/third_party_auth.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/third_party_auth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/time_series_data_point.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/time_series_data_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/track_objects_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/track_objects_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/track_objects_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/track_objects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/track_objects_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/track_objects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/transfer_learning_model.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/transfer_ownership_organization_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/transfer_ownership_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/transformation_block_additional_mount_point.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/transformation_block_additional_mount_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/transformation_job_status_enum.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/transformation_job_status_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/tuner_create_trial_impulse.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/tuner_create_trial_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/tuner_space_impulse.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/tuner_space_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/tuner_trial.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/tuner_trial.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/tuner_trial_blocks_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/tuner_trial_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/tuner_trial_dsp_job_id.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/tuner_trial_dsp_job_id.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_job_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_job_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_add_collaborator_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_bucket_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_create_empty_project_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_create_empty_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_create_project_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_data_campaign_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_data_item_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_data_item_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_dataset_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_dsp_block_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_portal_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_portal_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_organization_transformation_block_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_project_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_project_tags_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_project_tags_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_theme_colors_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_theme_colors_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_theme_logos_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_theme_logos_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_third_party_auth_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_user_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_version_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/update_whitelabel_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/update_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/upload_asset_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/upload_user_photo_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class UploadAssetResponse(BaseModel):
+class UploadUserPhotoResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    url: Optional[StrictStr] = None
+    url: StrictStr = ...
     __properties = ["success", "error", "url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
@@ -35,35 +35,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UploadAssetResponse:
-        """Create an instance of UploadAssetResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> UploadUserPhotoResponse:
+        """Create an instance of UploadUserPhotoResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UploadAssetResponse:
-        """Create an instance of UploadAssetResponse from a dict"""
+    def from_dict(cls, obj: dict) -> UploadUserPhotoResponse:
+        """Create an instance of UploadUserPhotoResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UploadAssetResponse.construct(**obj)
+            return UploadUserPhotoResponse.construct(**obj)
 
-        _obj = UploadAssetResponse.construct(**{
+        _obj = UploadUserPhotoResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
             "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/upload_asset_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,52 +14,56 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel
+from edgeimpulse_api.models.verify_dsp_block_url_response_all_of_block import VerifyDspBlockUrlResponseAllOfBlock
 
-class UploadAssetResponseAllOf(BaseModel):
-    url: Optional[StrictStr] = None
-    __properties = ["url"]
+class VerifyDspBlockUrlResponseAllOf(BaseModel):
+    block: Optional[VerifyDspBlockUrlResponseAllOfBlock] = None
+    __properties = ["block"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UploadAssetResponseAllOf:
-        """Create an instance of UploadAssetResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyDspBlockUrlResponseAllOf:
+        """Create an instance of VerifyDspBlockUrlResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of block
+        if self.block:
+            _dict['block'] = self.block.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UploadAssetResponseAllOf:
-        """Create an instance of UploadAssetResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyDspBlockUrlResponseAllOf:
+        """Create an instance of VerifyDspBlockUrlResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UploadAssetResponseAllOf.construct(**obj)
+            return VerifyDspBlockUrlResponseAllOf.construct(**obj)
 
-        _obj = UploadAssetResponseAllOf.construct(**{
-            "url": obj.get("url")
+        _obj = VerifyDspBlockUrlResponseAllOf.construct(**{
+            "block": VerifyDspBlockUrlResponseAllOfBlock.from_dict(obj.get("block")) if obj.get("block") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/upload_readme_image_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/upload_readme_image_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/upload_user_photo_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_email_response_all_of.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,56 +14,56 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
-class UploadUserPhotoResponse(BaseModel):
-    success: StrictBool = Field(..., description="Whether the operation succeeded")
-    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    url: StrictStr = ...
-    __properties = ["success", "error", "url"]
+class VerifyEmailResponseAllOf(BaseModel):
+    email: Optional[StrictStr] = Field(None, description="Email address that was verified.")
+    user_id: Optional[float] = Field(None, alias="userId", description="ID of the user associated with the verified email address, if any.")
+    redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="URL to redirect the user to after email verification.")
+    __properties = ["email", "userId", "redirectUrl"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UploadUserPhotoResponse:
-        """Create an instance of UploadUserPhotoResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyEmailResponseAllOf:
+        """Create an instance of VerifyEmailResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UploadUserPhotoResponse:
-        """Create an instance of UploadUserPhotoResponse from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyEmailResponseAllOf:
+        """Create an instance of VerifyEmailResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UploadUserPhotoResponse.construct(**obj)
+            return VerifyEmailResponseAllOf.construct(**obj)
 
-        _obj = UploadUserPhotoResponse.construct(**{
-            "success": obj.get("success"),
-            "error": obj.get("error"),
-            "url": obj.get("url")
+        _obj = VerifyEmailResponseAllOf.construct(**{
+            "email": obj.get("email"),
+            "user_id": obj.get("userId"),
+            "redirect_url": obj.get("redirectUrl")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/upload_user_photo_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/upload_user_photo_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/user.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/user_by_third_party_activation_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/user_by_third_party_activation_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/user_experiment.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/user_experiment.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/user_organization.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/create_enterprise_trial_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,76 +12,66 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
+
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 
-class UserOrganization(BaseModel):
-    id: StrictInt = ...
-    name: StrictStr = ...
-    logo: Optional[StrictStr] = None
-    is_developer_profile: StrictBool = Field(..., alias="isDeveloperProfile")
-    whitelabel_id: Optional[StrictInt] = Field(..., alias="whitelabelId", description="Unique identifier of the white label this project belongs to, if any.")
-    is_admin: StrictBool = Field(..., alias="isAdmin", description="Whether the user is admin of this organization or not.")
-    created: datetime = Field(..., description="When the organization was created.")
-    trial_id: Optional[float] = Field(..., alias="trialId", description="Unique identifier of the trial this organization belongs to, if any.")
-    __properties = ["id", "name", "logo", "isDeveloperProfile", "whitelabelId", "isAdmin", "created", "trialId"]
+class CreateEnterpriseTrialResponse(BaseModel):
+    success: StrictBool = Field(..., description="Whether the operation succeeded")
+    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+    id: Optional[StrictInt] = Field(None, description="Unique identifier of the created entity, if any.")
+    user_id: Optional[StrictInt] = Field(None, alias="userId", description="ID of the user created for the trial, if the user did not already exist.")
+    redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="URL to redirect the user to in order to access the enterprise trial.")
+    __properties = ["success", "error", "id", "userId", "redirectUrl"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UserOrganization:
-        """Create an instance of UserOrganization from a JSON string"""
+    def from_json(cls, json_str: str) -> CreateEnterpriseTrialResponse:
+        """Create an instance of CreateEnterpriseTrialResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if whitelabel_id (nullable) is None
-        if self.whitelabel_id is None:
-            _dict['whitelabelId'] = None
-
-        # set to None if trial_id (nullable) is None
-        if self.trial_id is None:
-            _dict['trialId'] = None
+        # set to None if id (nullable) is None
+        if self.id is None:
+            _dict['id'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UserOrganization:
-        """Create an instance of UserOrganization from a dict"""
+    def from_dict(cls, obj: dict) -> CreateEnterpriseTrialResponse:
+        """Create an instance of CreateEnterpriseTrialResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UserOrganization.construct(**obj)
+            return CreateEnterpriseTrialResponse.construct(**obj)
 
-        _obj = UserOrganization.construct(**{
+        _obj = CreateEnterpriseTrialResponse.construct(**{
+            "success": obj.get("success"),
+            "error": obj.get("error"),
             "id": obj.get("id"),
-            "name": obj.get("name"),
-            "logo": obj.get("logo"),
-            "is_developer_profile": obj.get("isDeveloperProfile"),
-            "whitelabel_id": obj.get("whitelabelId"),
-            "is_admin": obj.get("isAdmin"),
-            "created": obj.get("created"),
-            "trial_id": obj.get("trialId")
+            "user_id": obj.get("userId"),
+            "redirect_url": obj.get("redirectUrl")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_dsp_block_url_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_dsp_block_url_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_dsp_block_url_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_dsp_block_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,57 +13,61 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel
-from edgeimpulse_api.models.verify_dsp_block_url_response_all_of_block import VerifyDspBlockUrlResponseAllOfBlock
-
-class VerifyDspBlockUrlResponseAllOf(BaseModel):
-    block: Optional[VerifyDspBlockUrlResponseAllOfBlock] = None
-    __properties = ["block"]
+from typing import List
+from pydantic import BaseModel, Field
+from edgeimpulse_api.models.verify_organization_bucket_response_all_of_files import VerifyOrganizationBucketResponseAllOfFiles
+
+class VerifyOrganizationBucketResponseAllOf(BaseModel):
+    files: List[VerifyOrganizationBucketResponseAllOfFiles] = Field(..., description="20 random files from the bucket.")
+    __properties = ["files"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyDspBlockUrlResponseAllOf:
-        """Create an instance of VerifyDspBlockUrlResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyOrganizationBucketResponseAllOf:
+        """Create an instance of VerifyOrganizationBucketResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of block
-        if self.block:
-            _dict['block'] = self.block.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in files (list)
+        _items = []
+        if self.files:
+            for _item in self.files:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['files'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyDspBlockUrlResponseAllOf:
-        """Create an instance of VerifyDspBlockUrlResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketResponseAllOf:
+        """Create an instance of VerifyOrganizationBucketResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyDspBlockUrlResponseAllOf.construct(**obj)
+            return VerifyOrganizationBucketResponseAllOf.construct(**obj)
 
-        _obj = VerifyDspBlockUrlResponseAllOf.construct(**{
-            "block": VerifyDspBlockUrlResponseAllOfBlock.from_dict(obj.get("block")) if obj.get("block") is not None else None
+        _obj = VerifyOrganizationBucketResponseAllOf.construct(**{
+            "files": [VerifyOrganizationBucketResponseAllOfFiles.from_dict(_item) for _item in obj.get("files")] if obj.get("files") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_organization_bucket_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_organization_bucket_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_organization_bucket_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,59 +15,59 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
 from pydantic import BaseModel, Field
-from edgeimpulse_api.models.verify_organization_bucket_response_all_of_files import VerifyOrganizationBucketResponseAllOfFiles
+from edgeimpulse_api.models.enterprise_trial import EnterpriseTrial
 
-class VerifyOrganizationBucketResponseAllOf(BaseModel):
-    files: List[VerifyOrganizationBucketResponseAllOfFiles] = Field(..., description="20 random files from the bucket.")
-    __properties = ["files"]
+class ListEnterpriseTrialsResponseAllOf(BaseModel):
+    trials: List[EnterpriseTrial] = Field(..., description="Current or past enterprise trials.")
+    __properties = ["trials"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyOrganizationBucketResponseAllOf:
-        """Create an instance of VerifyOrganizationBucketResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> ListEnterpriseTrialsResponseAllOf:
+        """Create an instance of ListEnterpriseTrialsResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in files (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in trials (list)
         _items = []
-        if self.files:
-            for _item in self.files:
+        if self.trials:
+            for _item in self.trials:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['files'] = _items
+            _dict['trials'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketResponseAllOf:
-        """Create an instance of VerifyOrganizationBucketResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> ListEnterpriseTrialsResponseAllOf:
+        """Create an instance of ListEnterpriseTrialsResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyOrganizationBucketResponseAllOf.construct(**obj)
+            return ListEnterpriseTrialsResponseAllOf.construct(**obj)
 
-        _obj = VerifyOrganizationBucketResponseAllOf.construct(**{
-            "files": [VerifyOrganizationBucketResponseAllOfFiles.from_dict(_item) for _item in obj.get("files")] if obj.get("files") is not None else None
+        _obj = ListEnterpriseTrialsResponseAllOf.construct(**{
+            "trials": [EnterpriseTrial.from_dict(_item) for _item in obj.get("trials")] if obj.get("trials") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/verify_reset_password_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/verify_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/whitelabel.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/whitelabel.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/window_settings_response.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/window_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/window_settings_response_all_of.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/window_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/edgeimpulse_api/rest.py` & `edgeimpulse_api-1.26.0/edgeimpulse_api/rest.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.34/pyproject.toml` & `edgeimpulse_api-1.26.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgeimpulse-api"
-version = "1.25.34" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+version = "1.26.0" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 description = "Python bindings for the Edge Impulse API."
 authors = ["EdgeImpulse Inc. <hello@edgeimpulse.com>"]
 license = "Apache-2.0"
 homepage = "https://edgeimpulse.com"
 documentation = "https://docs.edgeimpulse.com/reference/edge-impulse-api/edge-impulse-api"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `edgeimpulse_api-1.25.34/PKG-INFO` & `edgeimpulse_api-1.26.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgeimpulse-api
-Version: 1.25.34
+Version: 1.26.0
 Summary: Python bindings for the Edge Impulse API.
 Home-page: https://edgeimpulse.com
 License: Apache-2.0
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

