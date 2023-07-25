# Comparing `tmp/pulumi_akamai-6.0.0.tar.gz` & `tmp/pulumi_akamai-6.0.0a1690300875.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_akamai-6.0.0.tar", last modified: Tue Jul 25 17:06:57 2023, max compression
+gzip compressed data, was "pulumi_akamai-6.0.0a1690300875.tar", last modified: Tue Jul 25 16:06:36 2023, max compression
```

## Comparing `pulumi_akamai-6.0.0.tar` & `pulumi_akamai-6.0.0a1690300875.tar`

### file list

```diff
@@ -1,283 +1,283 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:06:57.143410 pulumi_akamai-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-25 17:06:57.143410 pulumi_akamai-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:06:57.139410 pulumi_akamai-6.0.0/pulumi_akamai/
--rw-r--r--   0 runner    (1001) docker     (123)    32809 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  3064992 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    15478 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_advanced_settings_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_advanced_settings_pragma_header.py
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_advanced_settings_prefetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_api_constraints_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_api_request_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_attack_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_by_pass_network_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_configuration_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_custom_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_custom_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_custom_rule_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    17001 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_eval_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_eval_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_eval_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    19890 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_ip_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_ip_geo_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_malware_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_malware_policy_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_malware_policy_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_malware_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_match_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_match_target_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_rate_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_rate_policy_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_rate_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_reputation_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_reputation_profile_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_reputation_profile_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_reputation_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_rule_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_security_policy_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_siem_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_slow_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_slow_post_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_threat_intel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_version_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_waf_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_waf_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/app_sec_wap_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/appsec_advanced_settings_pii_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/appsec_advanced_settings_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_akamai_bot_category_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_bot_analytics_cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_bot_category_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_bot_detection_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_bot_management_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_challenge_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_challenge_interception_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_client_side_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_conditional_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_custom_bot_category.py
--rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_custom_bot_category_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_custom_bot_category_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_custom_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_custom_defined_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_custom_deny_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_javascript_injection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_recategorized_akamai_defined_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_serve_alternate_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_transactional_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/botman_transactional_endpoint_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/cloudlets_application_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/cloudlets_application_load_balancer_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/cloudlets_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/cloudlets_policy_activation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:06:57.139410 pulumi_akamai-6.0.0/pulumi_akamai/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    43352 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/cps_dv_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/cps_dv_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    44892 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/cps_third_party_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    27347 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/cps_upload_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    56350 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/datastream.py
--rw-r--r--   0 runner    (1001) docker     (123)    80130 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/dns_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    21162 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/dns_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    17150 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/edge_host_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/edge_kv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/edge_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/edge_workers_activation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:06:57.139410 pulumi_akamai-6.0.0/pulumi_akamai/edgedns/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/edgedns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/edgedns/get_authorities_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/edgedns/get_dns_record_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/edgekv_group_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_advanced_settings_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_api_request_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_attack_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_bypass_network_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_configuration_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_contracts_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_custom_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_custom_rule_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_custom_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_eval_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_eval_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_eval_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_export_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_failover_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_hostname_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_ip_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_malware_content_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_malware_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_malware_policy_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_match_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_rate_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_rate_policy_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_reputation_profile_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_reputation_profile_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_reputation_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_rule_upgrade_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_security_policy_protections.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_selectable_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_siem_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_siem_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_slow_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_threat_intel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_tuning_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_version_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_waf_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_wap_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_appsec_advanced_settings_pii_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_appsec_advanced_settings_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_authorities_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_akamai_bot_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_akamai_bot_category_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_akamai_defined_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_analytics_cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_analytics_cookie_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_category_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_detection_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_endpoint_coverage_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_management_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_challenge_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_challenge_interception_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_client_side_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_conditional_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_custom_bot_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_custom_bot_category_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_custom_bot_category_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_custom_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_custom_defined_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_custom_deny_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_javascript_injection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_recategorized_akamai_defined_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_response_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_serve_alternate_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_transactional_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_botman_transactional_endpoint_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_application_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_phased_release_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_request_control_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cps_csr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cps_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cps_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cps_enrollments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_cps_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_datastream_activation_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_datastream_dataset_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_datastreams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_dns_record_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_edge_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_edge_worker_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_edge_workers_property_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_edge_workers_resource_tier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_edgekv_group_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_edgekv_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_gtm_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_gtm_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_gtm_default_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_iam_contact_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_iam_countries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_iam_grantable_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_iam_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_iam_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_iam_supported_langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_iam_timeout_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_iam_timezones.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_imaging_policy_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_imaging_policy_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_network_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_properties_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property_include.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property_include_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property_include_parents.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property_include_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property_includes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property_rule_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property_rules_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/get_property_rules_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/gtm_asmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/gtm_cidrmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29745 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/gtm_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44869 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/gtm_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/gtm_geomap.py
--rw-r--r--   0 runner    (1001) docker     (123)    55296 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/gtm_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    26762 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/gtm_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/iam_blocked_user_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/iam_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/iam_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    46760 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/iam_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/imaging_policy_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/imaging_policy_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/imaging_policy_video.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/network_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    16222 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/network_list_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/network_list_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/network_list_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)  2326556 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:06:57.143410 pulumi_akamai-6.0.0/pulumi_akamai/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/properties/get_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/properties/get_cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/properties/get_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/properties/get_property_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/property_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22902 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/property_include.py
--rw-r--r--   0 runner    (1001) docker     (123)    24971 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/property_include_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:06:57.143410 pulumi_akamai-6.0.0/pulumi_akamai/trafficmanagement/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/trafficmanagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:06:57.139410 pulumi_akamai-6.0.0/pulumi_akamai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-25 17:06:57.000000 pulumi_akamai-6.0.0/pulumi_akamai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-07-25 17:06:57.000000 pulumi_akamai-6.0.0/pulumi_akamai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:06:57.000000 pulumi_akamai-6.0.0/pulumi_akamai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:06:57.000000 pulumi_akamai-6.0.0/pulumi_akamai.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 17:06:57.000000 pulumi_akamai-6.0.0/pulumi_akamai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 17:06:57.000000 pulumi_akamai-6.0.0/pulumi_akamai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:06:57.143410 pulumi_akamai-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-25 17:06:56.000000 pulumi_akamai-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:36.432363 pulumi_akamai-6.0.0a1690300875/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-25 16:06:36.432363 pulumi_akamai-6.0.0a1690300875/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:36.428363 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/
+-rw-r--r--   0 runner    (1001) docker     (123)    32809 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  3064992 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15478 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_advanced_settings_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_advanced_settings_pragma_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_advanced_settings_prefetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_api_constraints_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_api_request_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_attack_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_by_pass_network_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_configuration_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_custom_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_custom_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_custom_rule_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17001 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_eval_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_eval_penalty_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_eval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19890 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_ip_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_ip_geo_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_malware_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_malware_policy_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_malware_policy_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_malware_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_match_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_match_target_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_penalty_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rate_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rate_policy_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rate_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_reputation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_reputation_profile_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_reputation_profile_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_reputation_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rule_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_security_policy_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_selected_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_siem_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_slow_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_slow_post_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_threat_intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_version_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_waf_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_waf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_wap_selected_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/appsec_advanced_settings_pii_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/appsec_advanced_settings_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_akamai_bot_category_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_bot_analytics_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_bot_category_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_bot_detection_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_bot_management_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_challenge_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_challenge_interception_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_client_side_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_conditional_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_bot_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_bot_category_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_bot_category_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_defined_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_deny_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_javascript_injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_recategorized_akamai_defined_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_serve_alternate_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_transactional_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_transactional_endpoint_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cloudlets_application_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cloudlets_application_load_balancer_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cloudlets_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cloudlets_policy_activation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:36.432363 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cp_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43352 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cps_dv_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cps_dv_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44892 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cps_third_party_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27347 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cps_upload_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56350 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80130 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/dns_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21162 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/dns_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17150 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edge_host_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edge_kv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edge_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edge_workers_activation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:36.432363 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edgedns/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edgedns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edgedns/get_authorities_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edgedns/get_dns_record_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edgekv_group_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_advanced_settings_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_api_request_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_attack_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_bypass_network_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_configuration_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_contracts_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_custom_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_custom_rule_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_custom_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_eval_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_eval_penalty_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_eval_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_export_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_failover_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_hostname_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_ip_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_malware_content_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_malware_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_malware_policy_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_match_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_penalty_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_rate_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_rate_policy_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_reputation_profile_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_reputation_profile_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_reputation_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_rule_upgrade_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_security_policy_protections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_selectable_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_selected_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_siem_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_siem_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_slow_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_threat_intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_tuning_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_version_notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_waf_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_wap_selected_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_appsec_advanced_settings_pii_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_appsec_advanced_settings_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_authorities_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_akamai_bot_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_akamai_bot_category_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_akamai_defined_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_analytics_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_analytics_cookie_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_category_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_detection_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_endpoint_coverage_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_management_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_challenge_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_challenge_interception_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_client_side_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_conditional_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_bot_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_bot_category_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_bot_category_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_defined_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_deny_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_javascript_injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_recategorized_akamai_defined_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_response_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_serve_alternate_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_transactional_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_transactional_endpoint_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_application_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_phased_release_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_request_control_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cp_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_csr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_datastream_activation_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_datastream_dataset_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_datastreams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_dns_record_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edge_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edge_worker_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edge_workers_property_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edge_workers_resource_tier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edgekv_group_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edgekv_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_gtm_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_gtm_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_gtm_default_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_contact_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_grantable_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_supported_langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_timeout_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_timezones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_imaging_policy_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_imaging_policy_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_network_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_properties_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_include_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_include_parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_include_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_includes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_rule_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_rules_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_rules_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_asmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_cidrmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29745 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44869 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_geomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55296 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26762 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/iam_blocked_user_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/iam_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46760 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/imaging_policy_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/imaging_policy_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/imaging_policy_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/network_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16222 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/network_list_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/network_list_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/network_list_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2326556 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:36.432363 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/get_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/get_cp_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/get_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/get_property_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/property_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22902 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/property_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24971 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/property_include_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:36.432363 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/trafficmanagement/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/trafficmanagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:36.428363 pulumi_akamai-6.0.0a1690300875/pulumi_akamai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-25 16:06:36.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-07-25 16:06:36.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:06:36.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:06:36.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 16:06:36.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 16:06:36.000000 pulumi_akamai-6.0.0a1690300875/pulumi_akamai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 16:06:36.432363 pulumi_akamai-6.0.0a1690300875/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-25 16:06:35.000000 pulumi_akamai-6.0.0a1690300875/setup.py
```

### Comparing `pulumi_akamai-6.0.0/PKG-INFO` & `pulumi_akamai-6.0.0a1690300875/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_akamai
-Version: 6.0.0
+Version: 6.0.0a1690300875
 Summary: A Pulumi package for creating and managing akamai cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-akamai
 Keywords: pulumi akamai
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_akamai-6.0.0/README.md` & `pulumi_akamai-6.0.0a1690300875/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/__init__.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/_inputs.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/_utilities.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_activations.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_activations.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_advanced_settings_logging.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_advanced_settings_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_advanced_settings_pragma_header.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_advanced_settings_pragma_header.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_advanced_settings_prefetch.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_advanced_settings_prefetch.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_api_constraints_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_api_constraints_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_api_request_constraints.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_api_request_constraints.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_attack_group.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_attack_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_by_pass_network_list.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_by_pass_network_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_configuration.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_configuration_rename.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_configuration_rename.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_custom_deny.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_custom_deny.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_custom_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_custom_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_custom_rule_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_custom_rule_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_eval.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_eval.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_eval_group.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_eval_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_eval_penalty_box.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_eval_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_eval_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_eval_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_ip_geo.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_ip_geo.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_ip_geo_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_ip_geo_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_malware_policy.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_malware_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_malware_policy_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_malware_policy_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_malware_policy_actions.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_malware_policy_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_malware_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_malware_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_match_target.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_match_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_match_target_sequence.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_match_target_sequence.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_penalty_box.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_rate_policy.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rate_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_rate_policy_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rate_policy_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_rate_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rate_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_reputation_profile.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_reputation_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_reputation_profile_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_reputation_profile_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_reputation_profile_analysis.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_reputation_profile_analysis.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_reputation_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_reputation_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_rule_upgrade.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rule_upgrade.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_security_policy.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_security_policy_rename.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_security_policy_rename.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_selected_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_siem_settings.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_siem_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_slow_post.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_slow_post.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_slow_post_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_slow_post_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_threat_intel.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_threat_intel.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_version_nodes.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_version_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_waf_mode.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_waf_mode.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_waf_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_waf_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/app_sec_wap_selected_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_wap_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/appsec_advanced_settings_pii_learning.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/appsec_advanced_settings_pii_learning.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/appsec_advanced_settings_request_body.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/appsec_advanced_settings_request_body.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_akamai_bot_category_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_akamai_bot_category_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_bot_analytics_cookie.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_bot_analytics_cookie.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_bot_category_exception.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_bot_category_exception.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_bot_detection_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_bot_detection_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_bot_management_settings.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_bot_management_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_challenge_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_challenge_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_challenge_interception_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_challenge_interception_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_client_side_security.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_client_side_security.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_conditional_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_conditional_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_custom_bot_category.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_bot_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_custom_bot_category_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_bot_category_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_custom_bot_category_sequence.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_bot_category_sequence.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_custom_client.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_custom_defined_bot.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_defined_bot.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_custom_deny_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_deny_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_javascript_injection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_javascript_injection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_recategorized_akamai_defined_bot.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_recategorized_akamai_defined_bot.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_serve_alternate_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_serve_alternate_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_transactional_endpoint.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_transactional_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/botman_transactional_endpoint_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_transactional_endpoint_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/cloudlets_application_load_balancer.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cloudlets_application_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/cloudlets_application_load_balancer_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cloudlets_application_load_balancer_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/cloudlets_policy.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cloudlets_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/cloudlets_policy_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cloudlets_policy_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/config/outputs.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/config/vars.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/cp_code.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cp_code.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/cps_dv_enrollment.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cps_dv_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/cps_dv_validation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cps_dv_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/cps_third_party_enrollment.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cps_third_party_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/cps_upload_certificate.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cps_upload_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/datastream.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/datastream.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/dns_record.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/dns_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/dns_zone.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/dns_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/edge_host_name.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edge_host_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/edge_kv.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edge_kv.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/edge_worker.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edge_worker.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/edge_workers_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edge_workers_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/edgedns/get_authorities_set.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edgedns/get_authorities_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/edgedns/get_dns_record_set.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edgedns/get_dns_record_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/edgekv_group_items.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edgekv_group_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_advanced_settings_logging.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_advanced_settings_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_api_endpoints.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_api_endpoints.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_api_request_constraints.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_api_request_constraints.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_attack_groups.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_attack_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_bypass_network_lists.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_bypass_network_lists.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_configuration.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_configuration_version.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_configuration_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_contracts_groups.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_contracts_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_custom_deny.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_custom_deny.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_custom_rule_actions.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_custom_rule_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_custom_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_custom_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_eval.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_eval.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_eval_groups.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_eval_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_eval_penalty_box.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_eval_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_eval_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_eval_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_export_configuration.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_export_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_failover_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_failover_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_hostname_coverage.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_hostname_coverage.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_ip_geo.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_ip_geo.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_malware_content_types.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_malware_content_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_malware_policies.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_malware_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_malware_policy_actions.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_malware_policy_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_match_targets.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_match_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_penalty_box.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_rate_policies.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_rate_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_rate_policy_actions.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_rate_policy_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_reputation_profile_actions.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_reputation_profile_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_reputation_profile_analysis.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_reputation_profile_analysis.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_reputation_profiles.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_reputation_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_rule_upgrade_details.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_rule_upgrade_details.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_security_policy.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_security_policy_protections.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_security_policy_protections.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_selectable_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_selectable_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_selected_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_siem_definitions.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_siem_definitions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_siem_settings.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_siem_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_slow_post.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_slow_post.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_threat_intel.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_threat_intel.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_tuning_recommendations.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_tuning_recommendations.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_version_notes.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_version_notes.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_waf_mode.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_waf_mode.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_app_sec_wap_selected_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_wap_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_appsec_advanced_settings_pii_learning.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_appsec_advanced_settings_pii_learning.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_appsec_advanced_settings_request_body.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_appsec_advanced_settings_request_body.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_authorities_set.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_authorities_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_akamai_bot_category.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_akamai_bot_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_akamai_bot_category_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_akamai_bot_category_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_akamai_defined_bot.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_akamai_defined_bot.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_analytics_cookie.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_analytics_cookie.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_analytics_cookie_values.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_analytics_cookie_values.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_category_exception.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_category_exception.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_detection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_detection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_detection_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_detection_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_endpoint_coverage_report.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_endpoint_coverage_report.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_bot_management_settings.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_management_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_challenge_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_challenge_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_challenge_interception_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_challenge_interception_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_client_side_security.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_client_side_security.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_conditional_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_conditional_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_custom_bot_category.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_bot_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_custom_bot_category_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_bot_category_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_custom_bot_category_sequence.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_bot_category_sequence.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_custom_client.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_custom_defined_bot.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_defined_bot.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_custom_deny_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_deny_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_javascript_injection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_javascript_injection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_recategorized_akamai_defined_bot.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_recategorized_akamai_defined_bot.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_response_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_response_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_serve_alternate_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_serve_alternate_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_transactional_endpoint.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_transactional_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_botman_transactional_endpoint_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_transactional_endpoint_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_application_load_balancer.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_application_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_phased_release_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_phased_release_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_policy.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_request_control_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_request_control_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_contract.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_contract.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_contracts.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_contracts.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cp_code.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cp_code.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cps_csr.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_csr.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cps_deployments.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_deployments.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cps_enrollment.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cps_enrollments.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_enrollments.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_cps_warnings.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_warnings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_datastream_activation_history.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_datastream_activation_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_datastream_dataset_fields.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_datastream_dataset_fields.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_datastreams.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_datastreams.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_dns_record_set.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_dns_record_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_edge_worker.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edge_worker.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_edge_worker_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edge_worker_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_edge_workers_property_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edge_workers_property_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_edge_workers_resource_tier.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edge_workers_resource_tier.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_edgekv_group_items.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edgekv_group_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_edgekv_groups.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edgekv_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_group.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_groups.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_gtm_datacenter.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_gtm_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_gtm_datacenters.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_gtm_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_gtm_default_datacenter.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_gtm_default_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_iam_contact_types.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_contact_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_iam_countries.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_countries.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_iam_grantable_roles.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_grantable_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_iam_roles.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_iam_states.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_states.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_iam_supported_langs.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_supported_langs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_iam_timeout_policies.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_timeout_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_iam_timezones.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_timezones.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_imaging_policy_image.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_imaging_policy_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_imaging_policy_video.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_imaging_policy_video.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_network_lists.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_network_lists.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_properties.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_properties.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_properties_search.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_properties_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property_include.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_include.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property_include_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_include_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property_include_parents.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_include_parents.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property_include_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_include_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property_includes.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_includes.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property_products.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_products.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property_rule_formats.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_rule_formats.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property_rules_builder.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_rules_builder.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/get_property_rules_template.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_rules_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/gtm_asmap.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_asmap.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/gtm_cidrmap.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_cidrmap.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/gtm_datacenter.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/gtm_domain.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/gtm_geomap.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_geomap.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/gtm_property.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/gtm_resource.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/iam_blocked_user_properties.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/iam_blocked_user_properties.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/iam_group.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/iam_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/iam_role.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/iam_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/iam_user.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/iam_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/imaging_policy_image.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/imaging_policy_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/imaging_policy_set.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/imaging_policy_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/imaging_policy_video.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/imaging_policy_video.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/network_list.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/network_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/network_list_activations.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/network_list_activations.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/network_list_description.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/network_list_description.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/network_list_subscription.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/network_list_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/outputs.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/properties/get_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/get_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/properties/get_cp_code.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/get_cp_code.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/properties/get_property.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/get_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/properties/get_property_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/get_property_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/property.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/property.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/property_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/property_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/property_include.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/property_include.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/property_include_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/property_include_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/provider.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai.egg-info/PKG-INFO` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-akamai
-Version: 6.0.0
+Version: 6.0.0a1690300875
 Summary: A Pulumi package for creating and managing akamai cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-akamai
 Keywords: pulumi akamai
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_akamai-6.0.0/pulumi_akamai.egg-info/SOURCES.txt` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-6.0.0/setup.py` & `pulumi_akamai-6.0.0a1690300875/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.0.0"
-PLUGIN_VERSION = "6.0.0"
+VERSION = "6.0.0a1690300875"
+PLUGIN_VERSION = "6.0.0-alpha.1690300875+c3feb58e"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'akamai', PLUGIN_VERSION])
         except OSError as error:
```

