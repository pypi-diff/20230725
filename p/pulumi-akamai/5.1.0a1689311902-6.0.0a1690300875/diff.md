# Comparing `tmp/pulumi_akamai-5.1.0a1689311902.tar.gz` & `tmp/pulumi_akamai-6.0.0a1690300875.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_akamai-5.1.0a1689311902.tar", last modified: Fri Jul 14 05:23:27 2023, max compression
+gzip compressed data, was "pulumi_akamai-6.0.0a1690300875.tar", last modified: Tue Jul 25 16:06:36 2023, max compression
```

## Comparing `pulumi_akamai-5.1.0a1689311902.tar` & `pulumi_akamai-6.0.0a1690300875.tar`

### file list

```diff
@@ -1,276 +1,283 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:23:27.175077 pulumi_akamai-5.1.0a1689311902/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-14 05:23:27.175077 pulumi_akamai-5.1.0a1689311902/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:23:27.171076 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/
--rw-r--r--   0 runner    (1001) docker     (123)    31717 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1564777 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_advanced_settings_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_advanced_settings_pragma_header.py
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_advanced_settings_prefetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_api_constraints_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_api_request_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_attack_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_by_pass_network_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_configuration_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_custom_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_custom_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_custom_rule_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    17001 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_eval_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_eval_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_eval_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_ip_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_ip_geo_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_malware_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_malware_policy_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_malware_policy_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_malware_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_match_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_match_target_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_rate_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_rate_policy_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_rate_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_reputation_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_reputation_profile_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_reputation_profile_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_reputation_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_rule_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_security_policy_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_siem_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_slow_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_slow_post_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_threat_intel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_version_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_waf_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_waf_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_wap_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/appsec_advanced_settings_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_akamai_bot_category_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_bot_analytics_cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_bot_category_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_bot_detection_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_bot_management_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_challenge_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_challenge_interception_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_client_side_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_conditional_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_custom_bot_category.py
--rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_custom_bot_category_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_custom_bot_category_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_custom_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_custom_defined_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_custom_deny_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_javascript_injection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_recategorized_akamai_defined_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_serve_alternate_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_transactional_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_transactional_endpoint_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cloudlets_application_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cloudlets_application_load_balancer_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cloudlets_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cloudlets_policy_activation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:23:27.175077 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    47610 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cps_dv_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cps_dv_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    44892 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cps_third_party_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    27347 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cps_upload_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    58490 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/datastream.py
--rw-r--r--   0 runner    (1001) docker     (123)    78637 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/dns_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    21162 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/dns_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edge_host_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edge_kv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edge_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edge_workers_activation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:23:27.175077 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edgedns/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edgedns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edgedns/get_authorities_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edgedns/get_dns_record_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edgekv_group_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_advanced_settings_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_api_request_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_attack_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_bypass_network_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_configuration_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_contracts_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_custom_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_custom_rule_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_custom_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_eval_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_eval_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_eval_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_export_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_failover_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_hostname_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_ip_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_malware_content_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_malware_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_malware_policy_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_match_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_rate_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_rate_policy_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_reputation_profile_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_reputation_profile_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_reputation_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_rule_upgrade_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_security_policy_protections.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_selectable_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_siem_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_siem_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_slow_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_threat_intel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_tuning_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_version_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_waf_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_wap_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_appsec_advanced_settings_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_authorities_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_akamai_bot_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_akamai_bot_category_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_akamai_defined_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_analytics_cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_analytics_cookie_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_category_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_detection_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_endpoint_coverage_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_management_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_challenge_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_challenge_interception_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_client_side_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_conditional_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_custom_bot_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_custom_bot_category_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_custom_bot_category_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_custom_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_custom_defined_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_custom_deny_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_javascript_injection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_recategorized_akamai_defined_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_response_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_serve_alternate_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_transactional_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_transactional_endpoint_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_application_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_phased_release_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_request_control_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cps_csr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cps_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cps_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cps_enrollments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cps_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_datastream_activation_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_datastream_dataset_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_datastreams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_dns_record_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_edge_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_edge_worker_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_edge_workers_property_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_edge_workers_resource_tier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_edgekv_group_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_edgekv_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_gtm_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_gtm_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_gtm_default_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_contact_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_countries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_grantable_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_supported_langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_timeout_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_timezones.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_network_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_properties_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_include.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_include_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_include_parents.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_include_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_includes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_rule_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_rules_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_rules_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_asmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_cidrmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29745 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44869 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_geomap.py
--rw-r--r--   0 runner    (1001) docker     (123)    55296 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    26762 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/iam_blocked_user_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/iam_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/iam_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    48609 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/iam_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/network_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/network_list_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/network_list_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/network_list_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)  1231072 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:23:27.175077 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/properties/get_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/properties/get_cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/properties/get_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/properties/get_property_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    47346 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/property_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22902 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/property_include.py
--rw-r--r--   0 runner    (1001) docker     (123)    24971 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/property_include_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25793 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:23:27.175077 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/trafficmanagement/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/trafficmanagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:23:27.175077 pulumi_akamai-5.1.0a1689311902/pulumi_akamai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-14 05:23:27.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-14 05:23:27.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:23:27.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:23:27.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 05:23:27.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 05:23:27.000000 pulumi_akamai-5.1.0a1689311902/pulumi_akamai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:23:27.175077 pulumi_akamai-5.1.0a1689311902/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-14 05:23:26.000000 pulumi_akamai-5.1.0a1689311902/setup.py
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

### Comparing `pulumi_akamai-5.1.0a1689311902/PKG-INFO` & `pulumi_akamai-6.0.0a1690300875/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_akamai
-Version: 5.1.0a1689311902
+Version: 6.0.0a1690300875
 Summary: A Pulumi package for creating and managing akamai cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-akamai
 Keywords: pulumi akamai
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -34,15 +34,15 @@
 
     $ pip install pulumi_akamai
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-akamai/sdk/v5
+    $ go get github.com/pulumi/pulumi-akamai/sdk/v6
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Akamai
```

### Comparing `pulumi_akamai-5.1.0a1689311902/README.md` & `pulumi_akamai-6.0.0a1690300875/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     $ pip install pulumi_akamai
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-akamai/sdk/v5
+    $ go get github.com/pulumi/pulumi-akamai/sdk/v6
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Akamai
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/__init__.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 from .app_sec_slow_post_protection import *
 from .app_sec_threat_intel import *
 from .app_sec_version_nodes import *
 from .app_sec_waf_mode import *
 from .app_sec_waf_protection import *
 from .app_sec_wap_selected_hostnames import *
 from .appsec_advanced_settings_attack_payload_logging import *
+from .appsec_advanced_settings_pii_learning import *
 from .appsec_advanced_settings_request_body import *
 from .botman_akamai_bot_category_action import *
 from .botman_bot_analytics_cookie import *
 from .botman_bot_category_exception import *
 from .botman_bot_detection_action import *
 from .botman_bot_management_settings import *
 from .botman_challenge_action import *
@@ -136,14 +137,15 @@
 from .get_app_sec_slow_post import *
 from .get_app_sec_threat_intel import *
 from .get_app_sec_tuning_recommendations import *
 from .get_app_sec_version_notes import *
 from .get_app_sec_waf_mode import *
 from .get_app_sec_wap_selected_hostnames import *
 from .get_appsec_advanced_settings_attack_payload_logging import *
+from .get_appsec_advanced_settings_pii_learning import *
 from .get_appsec_advanced_settings_request_body import *
 from .get_authorities_set import *
 from .get_botman_akamai_bot_category import *
 from .get_botman_akamai_bot_category_action import *
 from .get_botman_akamai_defined_bot import *
 from .get_botman_bot_analytics_cookie import *
 from .get_botman_bot_analytics_cookie_values import *
@@ -205,14 +207,16 @@
 from .get_iam_countries import *
 from .get_iam_grantable_roles import *
 from .get_iam_roles import *
 from .get_iam_states import *
 from .get_iam_supported_langs import *
 from .get_iam_timeout_policies import *
 from .get_iam_timezones import *
+from .get_imaging_policy_image import *
+from .get_imaging_policy_video import *
 from .get_network_lists import *
 from .get_properties import *
 from .get_properties_search import *
 from .get_property import *
 from .get_property_activation import *
 from .get_property_hostnames import *
 from .get_property_include import *
@@ -232,14 +236,17 @@
 from .gtm_geomap import *
 from .gtm_property import *
 from .gtm_resource import *
 from .iam_blocked_user_properties import *
 from .iam_group import *
 from .iam_role import *
 from .iam_user import *
+from .imaging_policy_image import *
+from .imaging_policy_set import *
+from .imaging_policy_video import *
 from .network_list import *
 from .network_list_activations import *
 from .network_list_description import *
 from .network_list_subscription import *
 from .property import *
 from .property_activation import *
 from .property_include import *
@@ -649,14 +656,22 @@
   "fqn": "pulumi_akamai",
   "classes": {
    "akamai:index/appsecAdvancedSettingsAttackPayloadLogging:AppsecAdvancedSettingsAttackPayloadLogging": "AppsecAdvancedSettingsAttackPayloadLogging"
   }
  },
  {
   "pkg": "akamai",
+  "mod": "index/appsecAdvancedSettingsPiiLearning",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/appsecAdvancedSettingsPiiLearning:AppsecAdvancedSettingsPiiLearning": "AppsecAdvancedSettingsPiiLearning"
+  }
+ },
+ {
+  "pkg": "akamai",
   "mod": "index/appsecAdvancedSettingsRequestBody",
   "fqn": "pulumi_akamai",
   "classes": {
    "akamai:index/appsecAdvancedSettingsRequestBody:AppsecAdvancedSettingsRequestBody": "AppsecAdvancedSettingsRequestBody"
   }
  },
  {
@@ -1041,14 +1056,38 @@
   "fqn": "pulumi_akamai",
   "classes": {
    "akamai:index/iamUser:IamUser": "IamUser"
   }
  },
  {
   "pkg": "akamai",
+  "mod": "index/imagingPolicyImage",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/imagingPolicyImage:ImagingPolicyImage": "ImagingPolicyImage"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/imagingPolicySet",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/imagingPolicySet:ImagingPolicySet": "ImagingPolicySet"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/imagingPolicyVideo",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/imagingPolicyVideo:ImagingPolicyVideo": "ImagingPolicyVideo"
+  }
+ },
+ {
+  "pkg": "akamai",
   "mod": "index/networkList",
   "fqn": "pulumi_akamai",
   "classes": {
    "akamai:index/networkList:NetworkList": "NetworkList"
   }
  },
  {
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/_utilities.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_activations.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/property_include_activation.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,489 +4,552 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = ['AppSecActivationsArgs', 'AppSecActivations']
+__all__ = ['PropertyIncludeActivationArgs', 'PropertyIncludeActivation']
 
 @pulumi.input_type
-class AppSecActivationsArgs:
+class PropertyIncludeActivationArgs:
     def __init__(__self__, *,
-                 config_id: pulumi.Input[int],
-                 notification_emails: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 contract_id: pulumi.Input[str],
+                 group_id: pulumi.Input[str],
+                 include_id: pulumi.Input[str],
+                 network: pulumi.Input[str],
+                 notify_emails: pulumi.Input[Sequence[pulumi.Input[str]]],
                  version: pulumi.Input[int],
-                 activate: Optional[pulumi.Input[bool]] = None,
-                 network: Optional[pulumi.Input[str]] = None,
-                 note: Optional[pulumi.Input[str]] = None,
-                 notes: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a AppSecActivations resource.
-        :param pulumi.Input[int] config_id: Unique identifier of the security configuration to be activated
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_emails: List of email addresses to be notified with the results of the activation
-        :param pulumi.Input[int] version: Version of the security configuration to be activated
-        :param pulumi.Input[bool] activate: Whether to activate or deactivate the specified security configuration and version
-        :param pulumi.Input[str] network: Network on which to activate the configuration version (STAGING or PRODUCTION)
-        :param pulumi.Input[str] note: Note describing the activation. Will use timestamp if omitted.
-        :param pulumi.Input[str] notes: Note describing the activation
-        """
-        pulumi.set(__self__, "config_id", config_id)
-        pulumi.set(__self__, "notification_emails", notification_emails)
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordArgs']] = None,
+                 note: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a PropertyIncludeActivation resource.
+        :param pulumi.Input[str] contract_id: The contract under which the include is activated
+        :param pulumi.Input[str] group_id: The group under which the include is activated
+        :param pulumi.Input[str] include_id: The unique identifier of the include
+        :param pulumi.Input[str] network: The network for which the activation will be performed
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notify_emails: The list of email addresses to notify about an activation status
+        :param pulumi.Input[int] version: The unique identifier of the include
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: Automatically acknowledge all rule warnings for activation and continue
+        :param pulumi.Input['PropertyIncludeActivationComplianceRecordArgs'] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] note: The note to assign to a log message of the activation request
+        """
+        pulumi.set(__self__, "contract_id", contract_id)
+        pulumi.set(__self__, "group_id", group_id)
+        pulumi.set(__self__, "include_id", include_id)
+        pulumi.set(__self__, "network", network)
+        pulumi.set(__self__, "notify_emails", notify_emails)
         pulumi.set(__self__, "version", version)
-        if activate is not None:
-            warnings.warn("""The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""", DeprecationWarning)
-            pulumi.log.warn("""activate is deprecated: The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""")
-        if activate is not None:
-            pulumi.set(__self__, "activate", activate)
-        if network is not None:
-            pulumi.set(__self__, "network", network)
+        if auto_acknowledge_rule_warnings is not None:
+            pulumi.set(__self__, "auto_acknowledge_rule_warnings", auto_acknowledge_rule_warnings)
+        if compliance_record is not None:
+            pulumi.set(__self__, "compliance_record", compliance_record)
         if note is not None:
             pulumi.set(__self__, "note", note)
-        if notes is not None:
-            warnings.warn("""The setting notes has been deprecated. Use \"note\" instead.""", DeprecationWarning)
-            pulumi.log.warn("""notes is deprecated: The setting notes has been deprecated. Use \"note\" instead.""")
-        if notes is not None:
-            pulumi.set(__self__, "notes", notes)
 
     @property
-    @pulumi.getter(name="configId")
-    def config_id(self) -> pulumi.Input[int]:
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> pulumi.Input[str]:
+        """
+        The contract under which the include is activated
+        """
+        return pulumi.get(self, "contract_id")
+
+    @contract_id.setter
+    def contract_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "contract_id", value)
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> pulumi.Input[str]:
         """
-        Unique identifier of the security configuration to be activated
+        The group under which the include is activated
         """
-        return pulumi.get(self, "config_id")
+        return pulumi.get(self, "group_id")
 
-    @config_id.setter
-    def config_id(self, value: pulumi.Input[int]):
-        pulumi.set(self, "config_id", value)
+    @group_id.setter
+    def group_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "group_id", value)
 
     @property
-    @pulumi.getter(name="notificationEmails")
-    def notification_emails(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+    @pulumi.getter(name="includeId")
+    def include_id(self) -> pulumi.Input[str]:
         """
-        List of email addresses to be notified with the results of the activation
+        The unique identifier of the include
         """
-        return pulumi.get(self, "notification_emails")
+        return pulumi.get(self, "include_id")
 
-    @notification_emails.setter
-    def notification_emails(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "notification_emails", value)
+    @include_id.setter
+    def include_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "include_id", value)
+
+    @property
+    @pulumi.getter
+    def network(self) -> pulumi.Input[str]:
+        """
+        The network for which the activation will be performed
+        """
+        return pulumi.get(self, "network")
+
+    @network.setter
+    def network(self, value: pulumi.Input[str]):
+        pulumi.set(self, "network", value)
+
+    @property
+    @pulumi.getter(name="notifyEmails")
+    def notify_emails(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        """
+        The list of email addresses to notify about an activation status
+        """
+        return pulumi.get(self, "notify_emails")
+
+    @notify_emails.setter
+    def notify_emails(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "notify_emails", value)
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Input[int]:
         """
-        Version of the security configuration to be activated
+        The unique identifier of the include
         """
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: pulumi.Input[int]):
         pulumi.set(self, "version", value)
 
     @property
-    @pulumi.getter
-    def activate(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
+    def auto_acknowledge_rule_warnings(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether to activate or deactivate the specified security configuration and version
+        Automatically acknowledge all rule warnings for activation and continue
         """
-        warnings.warn("""The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""", DeprecationWarning)
-        pulumi.log.warn("""activate is deprecated: The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""")
-
-        return pulumi.get(self, "activate")
+        return pulumi.get(self, "auto_acknowledge_rule_warnings")
 
-    @activate.setter
-    def activate(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "activate", value)
+    @auto_acknowledge_rule_warnings.setter
+    def auto_acknowledge_rule_warnings(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "auto_acknowledge_rule_warnings", value)
 
     @property
-    @pulumi.getter
-    def network(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="complianceRecord")
+    def compliance_record(self) -> Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordArgs']]:
         """
-        Network on which to activate the configuration version (STAGING or PRODUCTION)
+        Provides an audit record when activating on a production network
         """
-        return pulumi.get(self, "network")
+        return pulumi.get(self, "compliance_record")
 
-    @network.setter
-    def network(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "network", value)
+    @compliance_record.setter
+    def compliance_record(self, value: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordArgs']]):
+        pulumi.set(self, "compliance_record", value)
 
     @property
     @pulumi.getter
     def note(self) -> Optional[pulumi.Input[str]]:
         """
-        Note describing the activation. Will use timestamp if omitted.
+        The note to assign to a log message of the activation request
         """
         return pulumi.get(self, "note")
 
     @note.setter
     def note(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "note", value)
 
-    @property
-    @pulumi.getter
-    def notes(self) -> Optional[pulumi.Input[str]]:
-        """
-        Note describing the activation
-        """
-        warnings.warn("""The setting notes has been deprecated. Use \"note\" instead.""", DeprecationWarning)
-        pulumi.log.warn("""notes is deprecated: The setting notes has been deprecated. Use \"note\" instead.""")
-
-        return pulumi.get(self, "notes")
-
-    @notes.setter
-    def notes(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "notes", value)
-
 
 @pulumi.input_type
-class _AppSecActivationsState:
+class _PropertyIncludeActivationState:
     def __init__(__self__, *,
-                 activate: Optional[pulumi.Input[bool]] = None,
-                 config_id: Optional[pulumi.Input[int]] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordArgs']] = None,
+                 contract_id: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[str]] = None,
+                 include_id: Optional[pulumi.Input[str]] = None,
                  network: Optional[pulumi.Input[str]] = None,
                  note: Optional[pulumi.Input[str]] = None,
-                 notes: Optional[pulumi.Input[str]] = None,
-                 notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 status: Optional[pulumi.Input[str]] = None,
+                 notify_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 validations: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[int]] = None):
         """
-        Input properties used for looking up and filtering AppSecActivations resources.
-        :param pulumi.Input[bool] activate: Whether to activate or deactivate the specified security configuration and version
-        :param pulumi.Input[int] config_id: Unique identifier of the security configuration to be activated
-        :param pulumi.Input[str] network: Network on which to activate the configuration version (STAGING or PRODUCTION)
-        :param pulumi.Input[str] note: Note describing the activation. Will use timestamp if omitted.
-        :param pulumi.Input[str] notes: Note describing the activation
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_emails: List of email addresses to be notified with the results of the activation
-        :param pulumi.Input[str] status: The results of the activation
-        :param pulumi.Input[int] version: Version of the security configuration to be activated
-        """
-        if activate is not None:
-            warnings.warn("""The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""", DeprecationWarning)
-            pulumi.log.warn("""activate is deprecated: The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""")
-        if activate is not None:
-            pulumi.set(__self__, "activate", activate)
-        if config_id is not None:
-            pulumi.set(__self__, "config_id", config_id)
+        Input properties used for looking up and filtering PropertyIncludeActivation resources.
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: Automatically acknowledge all rule warnings for activation and continue
+        :param pulumi.Input['PropertyIncludeActivationComplianceRecordArgs'] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] contract_id: The contract under which the include is activated
+        :param pulumi.Input[str] group_id: The group under which the include is activated
+        :param pulumi.Input[str] include_id: The unique identifier of the include
+        :param pulumi.Input[str] network: The network for which the activation will be performed
+        :param pulumi.Input[str] note: The note to assign to a log message of the activation request
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notify_emails: The list of email addresses to notify about an activation status
+        :param pulumi.Input[str] validations: The validation information in JSON format
+        :param pulumi.Input[int] version: The unique identifier of the include
+        """
+        if auto_acknowledge_rule_warnings is not None:
+            pulumi.set(__self__, "auto_acknowledge_rule_warnings", auto_acknowledge_rule_warnings)
+        if compliance_record is not None:
+            pulumi.set(__self__, "compliance_record", compliance_record)
+        if contract_id is not None:
+            pulumi.set(__self__, "contract_id", contract_id)
+        if group_id is not None:
+            pulumi.set(__self__, "group_id", group_id)
+        if include_id is not None:
+            pulumi.set(__self__, "include_id", include_id)
         if network is not None:
             pulumi.set(__self__, "network", network)
         if note is not None:
             pulumi.set(__self__, "note", note)
-        if notes is not None:
-            warnings.warn("""The setting notes has been deprecated. Use \"note\" instead.""", DeprecationWarning)
-            pulumi.log.warn("""notes is deprecated: The setting notes has been deprecated. Use \"note\" instead.""")
-        if notes is not None:
-            pulumi.set(__self__, "notes", notes)
-        if notification_emails is not None:
-            pulumi.set(__self__, "notification_emails", notification_emails)
-        if status is not None:
-            pulumi.set(__self__, "status", status)
+        if notify_emails is not None:
+            pulumi.set(__self__, "notify_emails", notify_emails)
+        if validations is not None:
+            pulumi.set(__self__, "validations", validations)
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
-    @pulumi.getter
-    def activate(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
+    def auto_acknowledge_rule_warnings(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Automatically acknowledge all rule warnings for activation and continue
+        """
+        return pulumi.get(self, "auto_acknowledge_rule_warnings")
+
+    @auto_acknowledge_rule_warnings.setter
+    def auto_acknowledge_rule_warnings(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "auto_acknowledge_rule_warnings", value)
+
+    @property
+    @pulumi.getter(name="complianceRecord")
+    def compliance_record(self) -> Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordArgs']]:
+        """
+        Provides an audit record when activating on a production network
+        """
+        return pulumi.get(self, "compliance_record")
+
+    @compliance_record.setter
+    def compliance_record(self, value: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordArgs']]):
+        pulumi.set(self, "compliance_record", value)
+
+    @property
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Whether to activate or deactivate the specified security configuration and version
+        The contract under which the include is activated
         """
-        warnings.warn("""The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""", DeprecationWarning)
-        pulumi.log.warn("""activate is deprecated: The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""")
+        return pulumi.get(self, "contract_id")
+
+    @contract_id.setter
+    def contract_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "contract_id", value)
 
-        return pulumi.get(self, "activate")
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The group under which the include is activated
+        """
+        return pulumi.get(self, "group_id")
 
-    @activate.setter
-    def activate(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "activate", value)
+    @group_id.setter
+    def group_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "group_id", value)
 
     @property
-    @pulumi.getter(name="configId")
-    def config_id(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="includeId")
+    def include_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Unique identifier of the security configuration to be activated
+        The unique identifier of the include
         """
-        return pulumi.get(self, "config_id")
+        return pulumi.get(self, "include_id")
 
-    @config_id.setter
-    def config_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "config_id", value)
+    @include_id.setter
+    def include_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "include_id", value)
 
     @property
     @pulumi.getter
     def network(self) -> Optional[pulumi.Input[str]]:
         """
-        Network on which to activate the configuration version (STAGING or PRODUCTION)
+        The network for which the activation will be performed
         """
         return pulumi.get(self, "network")
 
     @network.setter
     def network(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network", value)
 
     @property
     @pulumi.getter
     def note(self) -> Optional[pulumi.Input[str]]:
         """
-        Note describing the activation. Will use timestamp if omitted.
+        The note to assign to a log message of the activation request
         """
         return pulumi.get(self, "note")
 
     @note.setter
     def note(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "note", value)
 
     @property
-    @pulumi.getter
-    def notes(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="notifyEmails")
+    def notify_emails(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Note describing the activation
+        The list of email addresses to notify about an activation status
         """
-        warnings.warn("""The setting notes has been deprecated. Use \"note\" instead.""", DeprecationWarning)
-        pulumi.log.warn("""notes is deprecated: The setting notes has been deprecated. Use \"note\" instead.""")
-
-        return pulumi.get(self, "notes")
+        return pulumi.get(self, "notify_emails")
 
-    @notes.setter
-    def notes(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "notes", value)
-
-    @property
-    @pulumi.getter(name="notificationEmails")
-    def notification_emails(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        List of email addresses to be notified with the results of the activation
-        """
-        return pulumi.get(self, "notification_emails")
-
-    @notification_emails.setter
-    def notification_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "notification_emails", value)
+    @notify_emails.setter
+    def notify_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "notify_emails", value)
 
     @property
     @pulumi.getter
-    def status(self) -> Optional[pulumi.Input[str]]:
+    def validations(self) -> Optional[pulumi.Input[str]]:
         """
-        The results of the activation
+        The validation information in JSON format
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "validations")
 
-    @status.setter
-    def status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "status", value)
+    @validations.setter
+    def validations(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "validations", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[int]]:
         """
-        Version of the security configuration to be activated
+        The unique identifier of the include
         """
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "version", value)
 
 
-class AppSecActivations(pulumi.CustomResource):
+class PropertyIncludeActivation(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 activate: Optional[pulumi.Input[bool]] = None,
-                 config_id: Optional[pulumi.Input[int]] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyIncludeActivationComplianceRecordArgs']]] = None,
+                 contract_id: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[str]] = None,
+                 include_id: Optional[pulumi.Input[str]] = None,
                  network: Optional[pulumi.Input[str]] = None,
                  note: Optional[pulumi.Input[str]] = None,
-                 notes: Optional[pulumi.Input[str]] = None,
-                 notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 notify_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  version: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Create a AppSecActivations resource with the given unique name, props, and options.
+        Create a PropertyIncludeActivation resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] activate: Whether to activate or deactivate the specified security configuration and version
-        :param pulumi.Input[int] config_id: Unique identifier of the security configuration to be activated
-        :param pulumi.Input[str] network: Network on which to activate the configuration version (STAGING or PRODUCTION)
-        :param pulumi.Input[str] note: Note describing the activation. Will use timestamp if omitted.
-        :param pulumi.Input[str] notes: Note describing the activation
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_emails: List of email addresses to be notified with the results of the activation
-        :param pulumi.Input[int] version: Version of the security configuration to be activated
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: Automatically acknowledge all rule warnings for activation and continue
+        :param pulumi.Input[pulumi.InputType['PropertyIncludeActivationComplianceRecordArgs']] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] contract_id: The contract under which the include is activated
+        :param pulumi.Input[str] group_id: The group under which the include is activated
+        :param pulumi.Input[str] include_id: The unique identifier of the include
+        :param pulumi.Input[str] network: The network for which the activation will be performed
+        :param pulumi.Input[str] note: The note to assign to a log message of the activation request
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notify_emails: The list of email addresses to notify about an activation status
+        :param pulumi.Input[int] version: The unique identifier of the include
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: AppSecActivationsArgs,
+                 args: PropertyIncludeActivationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a AppSecActivations resource with the given unique name, props, and options.
+        Create a PropertyIncludeActivation resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param AppSecActivationsArgs args: The arguments to use to populate this resource's properties.
+        :param PropertyIncludeActivationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(AppSecActivationsArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(PropertyIncludeActivationArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 activate: Optional[pulumi.Input[bool]] = None,
-                 config_id: Optional[pulumi.Input[int]] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyIncludeActivationComplianceRecordArgs']]] = None,
+                 contract_id: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[str]] = None,
+                 include_id: Optional[pulumi.Input[str]] = None,
                  network: Optional[pulumi.Input[str]] = None,
                  note: Optional[pulumi.Input[str]] = None,
-                 notes: Optional[pulumi.Input[str]] = None,
-                 notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 notify_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  version: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = AppSecActivationsArgs.__new__(AppSecActivationsArgs)
+            __props__ = PropertyIncludeActivationArgs.__new__(PropertyIncludeActivationArgs)
 
-            if activate is not None and not opts.urn:
-                warnings.warn("""The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""", DeprecationWarning)
-                pulumi.log.warn("""activate is deprecated: The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""")
-            __props__.__dict__["activate"] = activate
-            if config_id is None and not opts.urn:
-                raise TypeError("Missing required property 'config_id'")
-            __props__.__dict__["config_id"] = config_id
+            __props__.__dict__["auto_acknowledge_rule_warnings"] = auto_acknowledge_rule_warnings
+            __props__.__dict__["compliance_record"] = compliance_record
+            if contract_id is None and not opts.urn:
+                raise TypeError("Missing required property 'contract_id'")
+            __props__.__dict__["contract_id"] = contract_id
+            if group_id is None and not opts.urn:
+                raise TypeError("Missing required property 'group_id'")
+            __props__.__dict__["group_id"] = group_id
+            if include_id is None and not opts.urn:
+                raise TypeError("Missing required property 'include_id'")
+            __props__.__dict__["include_id"] = include_id
+            if network is None and not opts.urn:
+                raise TypeError("Missing required property 'network'")
             __props__.__dict__["network"] = network
             __props__.__dict__["note"] = note
-            if notes is not None and not opts.urn:
-                warnings.warn("""The setting notes has been deprecated. Use \"note\" instead.""", DeprecationWarning)
-                pulumi.log.warn("""notes is deprecated: The setting notes has been deprecated. Use \"note\" instead.""")
-            __props__.__dict__["notes"] = notes
-            if notification_emails is None and not opts.urn:
-                raise TypeError("Missing required property 'notification_emails'")
-            __props__.__dict__["notification_emails"] = notification_emails
+            if notify_emails is None and not opts.urn:
+                raise TypeError("Missing required property 'notify_emails'")
+            __props__.__dict__["notify_emails"] = notify_emails
             if version is None and not opts.urn:
                 raise TypeError("Missing required property 'version'")
             __props__.__dict__["version"] = version
-            __props__.__dict__["status"] = None
-        super(AppSecActivations, __self__).__init__(
-            'akamai:index/appSecActivations:AppSecActivations',
+            __props__.__dict__["validations"] = None
+        super(PropertyIncludeActivation, __self__).__init__(
+            'akamai:index/propertyIncludeActivation:PropertyIncludeActivation',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            activate: Optional[pulumi.Input[bool]] = None,
-            config_id: Optional[pulumi.Input[int]] = None,
+            auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+            compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyIncludeActivationComplianceRecordArgs']]] = None,
+            contract_id: Optional[pulumi.Input[str]] = None,
+            group_id: Optional[pulumi.Input[str]] = None,
+            include_id: Optional[pulumi.Input[str]] = None,
             network: Optional[pulumi.Input[str]] = None,
             note: Optional[pulumi.Input[str]] = None,
-            notes: Optional[pulumi.Input[str]] = None,
-            notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            status: Optional[pulumi.Input[str]] = None,
-            version: Optional[pulumi.Input[int]] = None) -> 'AppSecActivations':
+            notify_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            validations: Optional[pulumi.Input[str]] = None,
+            version: Optional[pulumi.Input[int]] = None) -> 'PropertyIncludeActivation':
         """
-        Get an existing AppSecActivations resource's state with the given name, id, and optional extra
+        Get an existing PropertyIncludeActivation resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] activate: Whether to activate or deactivate the specified security configuration and version
-        :param pulumi.Input[int] config_id: Unique identifier of the security configuration to be activated
-        :param pulumi.Input[str] network: Network on which to activate the configuration version (STAGING or PRODUCTION)
-        :param pulumi.Input[str] note: Note describing the activation. Will use timestamp if omitted.
-        :param pulumi.Input[str] notes: Note describing the activation
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_emails: List of email addresses to be notified with the results of the activation
-        :param pulumi.Input[str] status: The results of the activation
-        :param pulumi.Input[int] version: Version of the security configuration to be activated
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: Automatically acknowledge all rule warnings for activation and continue
+        :param pulumi.Input[pulumi.InputType['PropertyIncludeActivationComplianceRecordArgs']] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] contract_id: The contract under which the include is activated
+        :param pulumi.Input[str] group_id: The group under which the include is activated
+        :param pulumi.Input[str] include_id: The unique identifier of the include
+        :param pulumi.Input[str] network: The network for which the activation will be performed
+        :param pulumi.Input[str] note: The note to assign to a log message of the activation request
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notify_emails: The list of email addresses to notify about an activation status
+        :param pulumi.Input[str] validations: The validation information in JSON format
+        :param pulumi.Input[int] version: The unique identifier of the include
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _AppSecActivationsState.__new__(_AppSecActivationsState)
+        __props__ = _PropertyIncludeActivationState.__new__(_PropertyIncludeActivationState)
 
-        __props__.__dict__["activate"] = activate
-        __props__.__dict__["config_id"] = config_id
+        __props__.__dict__["auto_acknowledge_rule_warnings"] = auto_acknowledge_rule_warnings
+        __props__.__dict__["compliance_record"] = compliance_record
+        __props__.__dict__["contract_id"] = contract_id
+        __props__.__dict__["group_id"] = group_id
+        __props__.__dict__["include_id"] = include_id
         __props__.__dict__["network"] = network
         __props__.__dict__["note"] = note
-        __props__.__dict__["notes"] = notes
-        __props__.__dict__["notification_emails"] = notification_emails
-        __props__.__dict__["status"] = status
+        __props__.__dict__["notify_emails"] = notify_emails
+        __props__.__dict__["validations"] = validations
         __props__.__dict__["version"] = version
-        return AppSecActivations(resource_name, opts=opts, __props__=__props__)
+        return PropertyIncludeActivation(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def activate(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
+    def auto_acknowledge_rule_warnings(self) -> pulumi.Output[Optional[bool]]:
         """
-        Whether to activate or deactivate the specified security configuration and version
+        Automatically acknowledge all rule warnings for activation and continue
         """
-        warnings.warn("""The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""", DeprecationWarning)
-        pulumi.log.warn("""activate is deprecated: The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""")
+        return pulumi.get(self, "auto_acknowledge_rule_warnings")
 
-        return pulumi.get(self, "activate")
+    @property
+    @pulumi.getter(name="complianceRecord")
+    def compliance_record(self) -> pulumi.Output[Optional['outputs.PropertyIncludeActivationComplianceRecord']]:
+        """
+        Provides an audit record when activating on a production network
+        """
+        return pulumi.get(self, "compliance_record")
 
     @property
-    @pulumi.getter(name="configId")
-    def config_id(self) -> pulumi.Output[int]:
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> pulumi.Output[str]:
         """
-        Unique identifier of the security configuration to be activated
+        The contract under which the include is activated
         """
-        return pulumi.get(self, "config_id")
+        return pulumi.get(self, "contract_id")
 
     @property
-    @pulumi.getter
-    def network(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> pulumi.Output[str]:
         """
-        Network on which to activate the configuration version (STAGING or PRODUCTION)
+        The group under which the include is activated
         """
-        return pulumi.get(self, "network")
+        return pulumi.get(self, "group_id")
 
     @property
-    @pulumi.getter
-    def note(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="includeId")
+    def include_id(self) -> pulumi.Output[str]:
         """
-        Note describing the activation. Will use timestamp if omitted.
+        The unique identifier of the include
         """
-        return pulumi.get(self, "note")
+        return pulumi.get(self, "include_id")
 
     @property
     @pulumi.getter
-    def notes(self) -> pulumi.Output[Optional[str]]:
+    def network(self) -> pulumi.Output[str]:
         """
-        Note describing the activation
+        The network for which the activation will be performed
         """
-        warnings.warn("""The setting notes has been deprecated. Use \"note\" instead.""", DeprecationWarning)
-        pulumi.log.warn("""notes is deprecated: The setting notes has been deprecated. Use \"note\" instead.""")
+        return pulumi.get(self, "network")
 
-        return pulumi.get(self, "notes")
+    @property
+    @pulumi.getter
+    def note(self) -> pulumi.Output[Optional[str]]:
+        """
+        The note to assign to a log message of the activation request
+        """
+        return pulumi.get(self, "note")
 
     @property
-    @pulumi.getter(name="notificationEmails")
-    def notification_emails(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter(name="notifyEmails")
+    def notify_emails(self) -> pulumi.Output[Sequence[str]]:
         """
-        List of email addresses to be notified with the results of the activation
+        The list of email addresses to notify about an activation status
         """
-        return pulumi.get(self, "notification_emails")
+        return pulumi.get(self, "notify_emails")
 
     @property
     @pulumi.getter
-    def status(self) -> pulumi.Output[str]:
+    def validations(self) -> pulumi.Output[str]:
         """
-        The results of the activation
+        The validation information in JSON format
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "validations")
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Output[int]:
         """
-        Version of the security configuration to be activated
+        The unique identifier of the include
         """
         return pulumi.get(self, "version")
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_advanced_settings_logging.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_advanced_settings_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_advanced_settings_pragma_header.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_advanced_settings_pragma_header.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_advanced_settings_prefetch.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_advanced_settings_prefetch.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_api_constraints_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_api_constraints_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_api_request_constraints.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_api_request_constraints.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_attack_group.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_attack_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_by_pass_network_list.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_by_pass_network_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_configuration.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_configuration_rename.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_configuration_rename.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_custom_deny.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_custom_deny.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_custom_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_custom_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_custom_rule_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_custom_rule_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_eval.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_eval.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_eval_group.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_eval_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_eval_penalty_box.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_eval_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_eval_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_eval_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_ip_geo.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_ip_geo.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,33 +15,37 @@
 class AppSecIPGeoArgs:
     def __init__(__self__, *,
                  config_id: pulumi.Input[int],
                  mode: pulumi.Input[str],
                  security_policy_id: pulumi.Input[str],
                  exception_ip_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  geo_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 ip_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+                 ip_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 ukraine_geo_control_action: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a AppSecIPGeo resource.
         :param pulumi.Input[int] config_id: Unique identifier of the security configuration
         :param pulumi.Input[str] mode: Protection mode (block or allow)
         :param pulumi.Input[str] security_policy_id: Unique identifier of the security policy
         :param pulumi.Input[Sequence[pulumi.Input[str]]] exception_ip_network_lists: List of IDs of network list that are always allowed
         :param pulumi.Input[Sequence[pulumi.Input[str]]] geo_network_lists: List of IDs of geographic network list to be blocked
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_network_lists: List of IDs of IP network list to be blocked
+        :param pulumi.Input[str] ukraine_geo_control_action: Action set for Ukraine geo control
         """
         pulumi.set(__self__, "config_id", config_id)
         pulumi.set(__self__, "mode", mode)
         pulumi.set(__self__, "security_policy_id", security_policy_id)
         if exception_ip_network_lists is not None:
             pulumi.set(__self__, "exception_ip_network_lists", exception_ip_network_lists)
         if geo_network_lists is not None:
             pulumi.set(__self__, "geo_network_lists", geo_network_lists)
         if ip_network_lists is not None:
             pulumi.set(__self__, "ip_network_lists", ip_network_lists)
+        if ukraine_geo_control_action is not None:
+            pulumi.set(__self__, "ukraine_geo_control_action", ukraine_geo_control_action)
 
     @property
     @pulumi.getter(name="configId")
     def config_id(self) -> pulumi.Input[int]:
         """
         Unique identifier of the security configuration
         """
@@ -107,45 +111,61 @@
         """
         return pulumi.get(self, "ip_network_lists")
 
     @ip_network_lists.setter
     def ip_network_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "ip_network_lists", value)
 
+    @property
+    @pulumi.getter(name="ukraineGeoControlAction")
+    def ukraine_geo_control_action(self) -> Optional[pulumi.Input[str]]:
+        """
+        Action set for Ukraine geo control
+        """
+        return pulumi.get(self, "ukraine_geo_control_action")
+
+    @ukraine_geo_control_action.setter
+    def ukraine_geo_control_action(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ukraine_geo_control_action", value)
+
 
 @pulumi.input_type
 class _AppSecIPGeoState:
     def __init__(__self__, *,
                  config_id: Optional[pulumi.Input[int]] = None,
                  exception_ip_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  geo_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ip_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  mode: Optional[pulumi.Input[str]] = None,
-                 security_policy_id: Optional[pulumi.Input[str]] = None):
+                 security_policy_id: Optional[pulumi.Input[str]] = None,
+                 ukraine_geo_control_action: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering AppSecIPGeo resources.
         :param pulumi.Input[int] config_id: Unique identifier of the security configuration
         :param pulumi.Input[Sequence[pulumi.Input[str]]] exception_ip_network_lists: List of IDs of network list that are always allowed
         :param pulumi.Input[Sequence[pulumi.Input[str]]] geo_network_lists: List of IDs of geographic network list to be blocked
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_network_lists: List of IDs of IP network list to be blocked
         :param pulumi.Input[str] mode: Protection mode (block or allow)
         :param pulumi.Input[str] security_policy_id: Unique identifier of the security policy
+        :param pulumi.Input[str] ukraine_geo_control_action: Action set for Ukraine geo control
         """
         if config_id is not None:
             pulumi.set(__self__, "config_id", config_id)
         if exception_ip_network_lists is not None:
             pulumi.set(__self__, "exception_ip_network_lists", exception_ip_network_lists)
         if geo_network_lists is not None:
             pulumi.set(__self__, "geo_network_lists", geo_network_lists)
         if ip_network_lists is not None:
             pulumi.set(__self__, "ip_network_lists", ip_network_lists)
         if mode is not None:
             pulumi.set(__self__, "mode", mode)
         if security_policy_id is not None:
             pulumi.set(__self__, "security_policy_id", security_policy_id)
+        if ukraine_geo_control_action is not None:
+            pulumi.set(__self__, "ukraine_geo_control_action", ukraine_geo_control_action)
 
     @property
     @pulumi.getter(name="configId")
     def config_id(self) -> Optional[pulumi.Input[int]]:
         """
         Unique identifier of the security configuration
         """
@@ -211,37 +231,51 @@
         """
         return pulumi.get(self, "security_policy_id")
 
     @security_policy_id.setter
     def security_policy_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_policy_id", value)
 
+    @property
+    @pulumi.getter(name="ukraineGeoControlAction")
+    def ukraine_geo_control_action(self) -> Optional[pulumi.Input[str]]:
+        """
+        Action set for Ukraine geo control
+        """
+        return pulumi.get(self, "ukraine_geo_control_action")
+
+    @ukraine_geo_control_action.setter
+    def ukraine_geo_control_action(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ukraine_geo_control_action", value)
+
 
 class AppSecIPGeo(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  config_id: Optional[pulumi.Input[int]] = None,
                  exception_ip_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  geo_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ip_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  mode: Optional[pulumi.Input[str]] = None,
                  security_policy_id: Optional[pulumi.Input[str]] = None,
+                 ukraine_geo_control_action: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a AppSecIPGeo resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] config_id: Unique identifier of the security configuration
         :param pulumi.Input[Sequence[pulumi.Input[str]]] exception_ip_network_lists: List of IDs of network list that are always allowed
         :param pulumi.Input[Sequence[pulumi.Input[str]]] geo_network_lists: List of IDs of geographic network list to be blocked
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_network_lists: List of IDs of IP network list to be blocked
         :param pulumi.Input[str] mode: Protection mode (block or allow)
         :param pulumi.Input[str] security_policy_id: Unique identifier of the security policy
+        :param pulumi.Input[str] ukraine_geo_control_action: Action set for Ukraine geo control
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: AppSecIPGeoArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -264,14 +298,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  config_id: Optional[pulumi.Input[int]] = None,
                  exception_ip_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  geo_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ip_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  mode: Optional[pulumi.Input[str]] = None,
                  security_policy_id: Optional[pulumi.Input[str]] = None,
+                 ukraine_geo_control_action: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -285,14 +320,15 @@
             __props__.__dict__["ip_network_lists"] = ip_network_lists
             if mode is None and not opts.urn:
                 raise TypeError("Missing required property 'mode'")
             __props__.__dict__["mode"] = mode
             if security_policy_id is None and not opts.urn:
                 raise TypeError("Missing required property 'security_policy_id'")
             __props__.__dict__["security_policy_id"] = security_policy_id
+            __props__.__dict__["ukraine_geo_control_action"] = ukraine_geo_control_action
         super(AppSecIPGeo, __self__).__init__(
             'akamai:index/appSecIPGeo:AppSecIPGeo',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -300,39 +336,42 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             config_id: Optional[pulumi.Input[int]] = None,
             exception_ip_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             geo_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             ip_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             mode: Optional[pulumi.Input[str]] = None,
-            security_policy_id: Optional[pulumi.Input[str]] = None) -> 'AppSecIPGeo':
+            security_policy_id: Optional[pulumi.Input[str]] = None,
+            ukraine_geo_control_action: Optional[pulumi.Input[str]] = None) -> 'AppSecIPGeo':
         """
         Get an existing AppSecIPGeo resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] config_id: Unique identifier of the security configuration
         :param pulumi.Input[Sequence[pulumi.Input[str]]] exception_ip_network_lists: List of IDs of network list that are always allowed
         :param pulumi.Input[Sequence[pulumi.Input[str]]] geo_network_lists: List of IDs of geographic network list to be blocked
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_network_lists: List of IDs of IP network list to be blocked
         :param pulumi.Input[str] mode: Protection mode (block or allow)
         :param pulumi.Input[str] security_policy_id: Unique identifier of the security policy
+        :param pulumi.Input[str] ukraine_geo_control_action: Action set for Ukraine geo control
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _AppSecIPGeoState.__new__(_AppSecIPGeoState)
 
         __props__.__dict__["config_id"] = config_id
         __props__.__dict__["exception_ip_network_lists"] = exception_ip_network_lists
         __props__.__dict__["geo_network_lists"] = geo_network_lists
         __props__.__dict__["ip_network_lists"] = ip_network_lists
         __props__.__dict__["mode"] = mode
         __props__.__dict__["security_policy_id"] = security_policy_id
+        __props__.__dict__["ukraine_geo_control_action"] = ukraine_geo_control_action
         return AppSecIPGeo(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="configId")
     def config_id(self) -> pulumi.Output[int]:
         """
         Unique identifier of the security configuration
@@ -375,7 +414,15 @@
     @pulumi.getter(name="securityPolicyId")
     def security_policy_id(self) -> pulumi.Output[str]:
         """
         Unique identifier of the security policy
         """
         return pulumi.get(self, "security_policy_id")
 
+    @property
+    @pulumi.getter(name="ukraineGeoControlAction")
+    def ukraine_geo_control_action(self) -> pulumi.Output[Optional[str]]:
+        """
+        Action set for Ukraine geo control
+        """
+        return pulumi.get(self, "ukraine_geo_control_action")
+
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_ip_geo_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_ip_geo_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_malware_policy.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_malware_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_malware_policy_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_malware_policy_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_malware_policy_actions.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_malware_policy_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_malware_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_malware_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_match_target.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_match_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_match_target_sequence.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_match_target_sequence.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_penalty_box.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_rate_policy.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rate_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_rate_policy_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rate_policy_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_rate_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rate_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_reputation_profile.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_reputation_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_reputation_profile_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_reputation_profile_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_reputation_profile_analysis.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_reputation_profile_analysis.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_reputation_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_reputation_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_rule_upgrade.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_rule_upgrade.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_security_policy.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_security_policy_rename.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_security_policy_rename.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_selected_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_siem_settings.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_siem_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_slow_post.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_slow_post.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_slow_post_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_slow_post_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_threat_intel.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_threat_intel.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_version_nodes.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_version_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_waf_mode.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_waf_mode.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_waf_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_waf_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/app_sec_wap_selected_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/app_sec_wap_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/appsec_advanced_settings_request_body.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/appsec_advanced_settings_request_body.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_akamai_bot_category_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_akamai_bot_category_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_bot_analytics_cookie.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_bot_analytics_cookie.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_bot_category_exception.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_bot_category_exception.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_bot_detection_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_bot_detection_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_bot_management_settings.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_bot_management_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_challenge_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_challenge_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_challenge_interception_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_challenge_interception_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_client_side_security.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_client_side_security.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_conditional_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_conditional_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_custom_bot_category.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_bot_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_custom_bot_category_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_bot_category_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_custom_bot_category_sequence.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_bot_category_sequence.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_custom_client.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_custom_defined_bot.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_defined_bot.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_custom_deny_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_custom_deny_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_javascript_injection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_javascript_injection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_recategorized_akamai_defined_bot.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_recategorized_akamai_defined_bot.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_serve_alternate_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_serve_alternate_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_transactional_endpoint.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_transactional_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/botman_transactional_endpoint_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/botman_transactional_endpoint_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cloudlets_application_load_balancer.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cloudlets_application_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cloudlets_application_load_balancer_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cloudlets_application_load_balancer_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cloudlets_policy.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cloudlets_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cloudlets_policy_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cloudlets_policy_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cp_code.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/property_include.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,386 +5,565 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['CpCodeArgs', 'CpCode']
+__all__ = ['PropertyIncludeArgs', 'PropertyInclude']
 
 @pulumi.input_type
-class CpCodeArgs:
+class PropertyIncludeArgs:
     def __init__(__self__, *,
-                 contract: Optional[pulumi.Input[str]] = None,
-                 contract_id: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 group_id: Optional[pulumi.Input[str]] = None,
+                 contract_id: pulumi.Input[str],
+                 group_id: pulumi.Input[str],
+                 rule_format: pulumi.Input[str],
+                 type: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
-                 product: Optional[pulumi.Input[str]] = None,
-                 product_id: Optional[pulumi.Input[str]] = None):
+                 product_id: Optional[pulumi.Input[str]] = None,
+                 rules: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a CpCode resource.
+        The set of arguments for constructing a PropertyInclude resource.
+        :param pulumi.Input[str] contract_id: Identifies the contract to which the include is assigned
+        :param pulumi.Input[str] group_id: Identifies the group to which the include is assigned
+        :param pulumi.Input[str] rule_format: Indicates the versioned set of features and criteria
+        :param pulumi.Input[str] type: Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
+        :param pulumi.Input[str] name: A descriptive name for the include
+        :param pulumi.Input[str] product_id: The product assigned to the include
+        :param pulumi.Input[str] rules: Property Rules as JSON
         """
-        if contract is not None:
-            warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-        if contract is not None:
-            pulumi.set(__self__, "contract", contract)
-        if contract_id is not None:
-            pulumi.set(__self__, "contract_id", contract_id)
-        if group is not None:
-            warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-        if group is not None:
-            pulumi.set(__self__, "group", group)
-        if group_id is not None:
-            pulumi.set(__self__, "group_id", group_id)
+        pulumi.set(__self__, "contract_id", contract_id)
+        pulumi.set(__self__, "group_id", group_id)
+        pulumi.set(__self__, "rule_format", rule_format)
+        pulumi.set(__self__, "type", type)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if product is not None:
-            warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
-        if product is not None:
-            pulumi.set(__self__, "product", product)
         if product_id is not None:
             pulumi.set(__self__, "product_id", product_id)
-
-    @property
-    @pulumi.getter
-    def contract(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-
-        return pulumi.get(self, "contract")
-
-    @contract.setter
-    def contract(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "contract", value)
+        if rules is not None:
+            pulumi.set(__self__, "rules", rules)
 
     @property
     @pulumi.getter(name="contractId")
-    def contract_id(self) -> Optional[pulumi.Input[str]]:
+    def contract_id(self) -> pulumi.Input[str]:
+        """
+        Identifies the contract to which the include is assigned
+        """
         return pulumi.get(self, "contract_id")
 
     @contract_id.setter
-    def contract_id(self, value: Optional[pulumi.Input[str]]):
+    def contract_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "contract_id", value)
 
     @property
-    @pulumi.getter
-    def group(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-
-        return pulumi.get(self, "group")
-
-    @group.setter
-    def group(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group", value)
-
-    @property
     @pulumi.getter(name="groupId")
-    def group_id(self) -> Optional[pulumi.Input[str]]:
+    def group_id(self) -> pulumi.Input[str]:
+        """
+        Identifies the group to which the include is assigned
+        """
         return pulumi.get(self, "group_id")
 
     @group_id.setter
-    def group_id(self, value: Optional[pulumi.Input[str]]):
+    def group_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "group_id", value)
 
     @property
+    @pulumi.getter(name="ruleFormat")
+    def rule_format(self) -> pulumi.Input[str]:
+        """
+        Indicates the versioned set of features and criteria
+        """
+        return pulumi.get(self, "rule_format")
+
+    @rule_format.setter
+    def rule_format(self, value: pulumi.Input[str]):
+        pulumi.set(self, "rule_format", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> pulumi.Input[str]:
+        """
+        Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "type", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        A descriptive name for the include
+        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def product(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
-
-        return pulumi.get(self, "product")
-
-    @product.setter
-    def product(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "product", value)
-
-    @property
     @pulumi.getter(name="productId")
     def product_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The product assigned to the include
+        """
         return pulumi.get(self, "product_id")
 
     @product_id.setter
     def product_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "product_id", value)
 
+    @property
+    @pulumi.getter
+    def rules(self) -> Optional[pulumi.Input[str]]:
+        """
+        Property Rules as JSON
+        """
+        return pulumi.get(self, "rules")
+
+    @rules.setter
+    def rules(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rules", value)
+
 
 @pulumi.input_type
-class _CpCodeState:
+class _PropertyIncludeState:
     def __init__(__self__, *,
-                 contract: Optional[pulumi.Input[str]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
+                 latest_version: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 product: Optional[pulumi.Input[str]] = None,
-                 product_id: Optional[pulumi.Input[str]] = None):
+                 product_id: Optional[pulumi.Input[str]] = None,
+                 production_version: Optional[pulumi.Input[str]] = None,
+                 rule_errors: Optional[pulumi.Input[str]] = None,
+                 rule_format: Optional[pulumi.Input[str]] = None,
+                 rule_warnings: Optional[pulumi.Input[str]] = None,
+                 rules: Optional[pulumi.Input[str]] = None,
+                 staging_version: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering CpCode resources.
+        Input properties used for looking up and filtering PropertyInclude resources.
+        :param pulumi.Input[str] contract_id: Identifies the contract to which the include is assigned
+        :param pulumi.Input[str] group_id: Identifies the group to which the include is assigned
+        :param pulumi.Input[int] latest_version: Specifies the most recent version of the include
+        :param pulumi.Input[str] name: A descriptive name for the include
+        :param pulumi.Input[str] product_id: The product assigned to the include
+        :param pulumi.Input[str] production_version: The most recent version to be activated to the production network
+        :param pulumi.Input[str] rule_errors: Rule validation errors
+        :param pulumi.Input[str] rule_format: Indicates the versioned set of features and criteria
+        :param pulumi.Input[str] rule_warnings: Rule validation warnings
+        :param pulumi.Input[str] rules: Property Rules as JSON
+        :param pulumi.Input[str] staging_version: The most recent version to be activated to the staging network
+        :param pulumi.Input[str] type: Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
         """
-        if contract is not None:
-            warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-        if contract is not None:
-            pulumi.set(__self__, "contract", contract)
         if contract_id is not None:
             pulumi.set(__self__, "contract_id", contract_id)
-        if group is not None:
-            warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-        if group is not None:
-            pulumi.set(__self__, "group", group)
         if group_id is not None:
             pulumi.set(__self__, "group_id", group_id)
+        if latest_version is not None:
+            pulumi.set(__self__, "latest_version", latest_version)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if product is not None:
-            warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
-        if product is not None:
-            pulumi.set(__self__, "product", product)
         if product_id is not None:
             pulumi.set(__self__, "product_id", product_id)
-
-    @property
-    @pulumi.getter
-    def contract(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-
-        return pulumi.get(self, "contract")
-
-    @contract.setter
-    def contract(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "contract", value)
+        if production_version is not None:
+            pulumi.set(__self__, "production_version", production_version)
+        if rule_errors is not None:
+            pulumi.set(__self__, "rule_errors", rule_errors)
+        if rule_format is not None:
+            pulumi.set(__self__, "rule_format", rule_format)
+        if rule_warnings is not None:
+            pulumi.set(__self__, "rule_warnings", rule_warnings)
+        if rules is not None:
+            pulumi.set(__self__, "rules", rules)
+        if staging_version is not None:
+            pulumi.set(__self__, "staging_version", staging_version)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Identifies the contract to which the include is assigned
+        """
         return pulumi.get(self, "contract_id")
 
     @contract_id.setter
     def contract_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract_id", value)
 
     @property
-    @pulumi.getter
-    def group(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-
-        return pulumi.get(self, "group")
-
-    @group.setter
-    def group(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group", value)
-
-    @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Identifies the group to which the include is assigned
+        """
         return pulumi.get(self, "group_id")
 
     @group_id.setter
     def group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group_id", value)
 
     @property
+    @pulumi.getter(name="latestVersion")
+    def latest_version(self) -> Optional[pulumi.Input[int]]:
+        """
+        Specifies the most recent version of the include
+        """
+        return pulumi.get(self, "latest_version")
+
+    @latest_version.setter
+    def latest_version(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "latest_version", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        A descriptive name for the include
+        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def product(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
-
-        return pulumi.get(self, "product")
-
-    @product.setter
-    def product(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "product", value)
-
-    @property
     @pulumi.getter(name="productId")
     def product_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The product assigned to the include
+        """
         return pulumi.get(self, "product_id")
 
     @product_id.setter
     def product_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "product_id", value)
 
+    @property
+    @pulumi.getter(name="productionVersion")
+    def production_version(self) -> Optional[pulumi.Input[str]]:
+        """
+        The most recent version to be activated to the production network
+        """
+        return pulumi.get(self, "production_version")
+
+    @production_version.setter
+    def production_version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "production_version", value)
 
-class CpCode(pulumi.CustomResource):
+    @property
+    @pulumi.getter(name="ruleErrors")
+    def rule_errors(self) -> Optional[pulumi.Input[str]]:
+        """
+        Rule validation errors
+        """
+        return pulumi.get(self, "rule_errors")
+
+    @rule_errors.setter
+    def rule_errors(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rule_errors", value)
+
+    @property
+    @pulumi.getter(name="ruleFormat")
+    def rule_format(self) -> Optional[pulumi.Input[str]]:
+        """
+        Indicates the versioned set of features and criteria
+        """
+        return pulumi.get(self, "rule_format")
+
+    @rule_format.setter
+    def rule_format(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rule_format", value)
+
+    @property
+    @pulumi.getter(name="ruleWarnings")
+    def rule_warnings(self) -> Optional[pulumi.Input[str]]:
+        """
+        Rule validation warnings
+        """
+        return pulumi.get(self, "rule_warnings")
+
+    @rule_warnings.setter
+    def rule_warnings(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rule_warnings", value)
+
+    @property
+    @pulumi.getter
+    def rules(self) -> Optional[pulumi.Input[str]]:
+        """
+        Property Rules as JSON
+        """
+        return pulumi.get(self, "rules")
+
+    @rules.setter
+    def rules(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rules", value)
+
+    @property
+    @pulumi.getter(name="stagingVersion")
+    def staging_version(self) -> Optional[pulumi.Input[str]]:
+        """
+        The most recent version to be activated to the staging network
+        """
+        return pulumi.get(self, "staging_version")
+
+    @staging_version.setter
+    def staging_version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "staging_version", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
+
+
+class PropertyInclude(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 product: Optional[pulumi.Input[str]] = None,
                  product_id: Optional[pulumi.Input[str]] = None,
+                 rule_format: Optional[pulumi.Input[str]] = None,
+                 rules: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a CpCode resource with the given unique name, props, and options.
+        Create a PropertyInclude resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] contract_id: Identifies the contract to which the include is assigned
+        :param pulumi.Input[str] group_id: Identifies the group to which the include is assigned
+        :param pulumi.Input[str] name: A descriptive name for the include
+        :param pulumi.Input[str] product_id: The product assigned to the include
+        :param pulumi.Input[str] rule_format: Indicates the versioned set of features and criteria
+        :param pulumi.Input[str] rules: Property Rules as JSON
+        :param pulumi.Input[str] type: Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[CpCodeArgs] = None,
+                 args: PropertyIncludeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a CpCode resource with the given unique name, props, and options.
+        Create a PropertyInclude resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param CpCodeArgs args: The arguments to use to populate this resource's properties.
+        :param PropertyIncludeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CpCodeArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(PropertyIncludeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 product: Optional[pulumi.Input[str]] = None,
                  product_id: Optional[pulumi.Input[str]] = None,
+                 rule_format: Optional[pulumi.Input[str]] = None,
+                 rules: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CpCodeArgs.__new__(CpCodeArgs)
+            __props__ = PropertyIncludeArgs.__new__(PropertyIncludeArgs)
 
-            if contract is not None and not opts.urn:
-                warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-                pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-            __props__.__dict__["contract"] = contract
+            if contract_id is None and not opts.urn:
+                raise TypeError("Missing required property 'contract_id'")
             __props__.__dict__["contract_id"] = contract_id
-            if group is not None and not opts.urn:
-                warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-                pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-            __props__.__dict__["group"] = group
+            if group_id is None and not opts.urn:
+                raise TypeError("Missing required property 'group_id'")
             __props__.__dict__["group_id"] = group_id
             __props__.__dict__["name"] = name
-            if product is not None and not opts.urn:
-                warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-                pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
-            __props__.__dict__["product"] = product
             __props__.__dict__["product_id"] = product_id
-        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="akamai:properties/cpCode:CpCode")])
-        opts = pulumi.ResourceOptions.merge(opts, alias_opts)
-        super(CpCode, __self__).__init__(
-            'akamai:index/cpCode:CpCode',
+            if rule_format is None and not opts.urn:
+                raise TypeError("Missing required property 'rule_format'")
+            __props__.__dict__["rule_format"] = rule_format
+            __props__.__dict__["rules"] = rules
+            if type is None and not opts.urn:
+                raise TypeError("Missing required property 'type'")
+            __props__.__dict__["type"] = type
+            __props__.__dict__["latest_version"] = None
+            __props__.__dict__["production_version"] = None
+            __props__.__dict__["rule_errors"] = None
+            __props__.__dict__["rule_warnings"] = None
+            __props__.__dict__["staging_version"] = None
+        super(PropertyInclude, __self__).__init__(
+            'akamai:index/propertyInclude:PropertyInclude',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            contract: Optional[pulumi.Input[str]] = None,
             contract_id: Optional[pulumi.Input[str]] = None,
-            group: Optional[pulumi.Input[str]] = None,
             group_id: Optional[pulumi.Input[str]] = None,
+            latest_version: Optional[pulumi.Input[int]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            product: Optional[pulumi.Input[str]] = None,
-            product_id: Optional[pulumi.Input[str]] = None) -> 'CpCode':
+            product_id: Optional[pulumi.Input[str]] = None,
+            production_version: Optional[pulumi.Input[str]] = None,
+            rule_errors: Optional[pulumi.Input[str]] = None,
+            rule_format: Optional[pulumi.Input[str]] = None,
+            rule_warnings: Optional[pulumi.Input[str]] = None,
+            rules: Optional[pulumi.Input[str]] = None,
+            staging_version: Optional[pulumi.Input[str]] = None,
+            type: Optional[pulumi.Input[str]] = None) -> 'PropertyInclude':
         """
-        Get an existing CpCode resource's state with the given name, id, and optional extra
+        Get an existing PropertyInclude resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] contract_id: Identifies the contract to which the include is assigned
+        :param pulumi.Input[str] group_id: Identifies the group to which the include is assigned
+        :param pulumi.Input[int] latest_version: Specifies the most recent version of the include
+        :param pulumi.Input[str] name: A descriptive name for the include
+        :param pulumi.Input[str] product_id: The product assigned to the include
+        :param pulumi.Input[str] production_version: The most recent version to be activated to the production network
+        :param pulumi.Input[str] rule_errors: Rule validation errors
+        :param pulumi.Input[str] rule_format: Indicates the versioned set of features and criteria
+        :param pulumi.Input[str] rule_warnings: Rule validation warnings
+        :param pulumi.Input[str] rules: Property Rules as JSON
+        :param pulumi.Input[str] staging_version: The most recent version to be activated to the staging network
+        :param pulumi.Input[str] type: Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _CpCodeState.__new__(_CpCodeState)
+        __props__ = _PropertyIncludeState.__new__(_PropertyIncludeState)
 
-        __props__.__dict__["contract"] = contract
         __props__.__dict__["contract_id"] = contract_id
-        __props__.__dict__["group"] = group
         __props__.__dict__["group_id"] = group_id
+        __props__.__dict__["latest_version"] = latest_version
         __props__.__dict__["name"] = name
-        __props__.__dict__["product"] = product
         __props__.__dict__["product_id"] = product_id
-        return CpCode(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter
-    def contract(self) -> pulumi.Output[str]:
-        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-
-        return pulumi.get(self, "contract")
+        __props__.__dict__["production_version"] = production_version
+        __props__.__dict__["rule_errors"] = rule_errors
+        __props__.__dict__["rule_format"] = rule_format
+        __props__.__dict__["rule_warnings"] = rule_warnings
+        __props__.__dict__["rules"] = rules
+        __props__.__dict__["staging_version"] = staging_version
+        __props__.__dict__["type"] = type
+        return PropertyInclude(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> pulumi.Output[str]:
+        """
+        Identifies the contract to which the include is assigned
+        """
         return pulumi.get(self, "contract_id")
 
     @property
-    @pulumi.getter
-    def group(self) -> pulumi.Output[str]:
-        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-
-        return pulumi.get(self, "group")
-
-    @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> pulumi.Output[str]:
+        """
+        Identifies the group to which the include is assigned
+        """
         return pulumi.get(self, "group_id")
 
     @property
+    @pulumi.getter(name="latestVersion")
+    def latest_version(self) -> pulumi.Output[int]:
+        """
+        Specifies the most recent version of the include
+        """
+        return pulumi.get(self, "latest_version")
+
+    @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
+        """
+        A descriptive name for the include
+        """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="productId")
+    def product_id(self) -> pulumi.Output[Optional[str]]:
+        """
+        The product assigned to the include
+        """
+        return pulumi.get(self, "product_id")
+
+    @property
+    @pulumi.getter(name="productionVersion")
+    def production_version(self) -> pulumi.Output[str]:
+        """
+        The most recent version to be activated to the production network
+        """
+        return pulumi.get(self, "production_version")
+
+    @property
+    @pulumi.getter(name="ruleErrors")
+    def rule_errors(self) -> pulumi.Output[str]:
+        """
+        Rule validation errors
+        """
+        return pulumi.get(self, "rule_errors")
+
+    @property
+    @pulumi.getter(name="ruleFormat")
+    def rule_format(self) -> pulumi.Output[str]:
+        """
+        Indicates the versioned set of features and criteria
+        """
+        return pulumi.get(self, "rule_format")
+
+    @property
+    @pulumi.getter(name="ruleWarnings")
+    def rule_warnings(self) -> pulumi.Output[str]:
+        """
+        Rule validation warnings
+        """
+        return pulumi.get(self, "rule_warnings")
+
+    @property
     @pulumi.getter
-    def product(self) -> pulumi.Output[str]:
-        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
+    def rules(self) -> pulumi.Output[str]:
+        """
+        Property Rules as JSON
+        """
+        return pulumi.get(self, "rules")
 
-        return pulumi.get(self, "product")
+    @property
+    @pulumi.getter(name="stagingVersion")
+    def staging_version(self) -> pulumi.Output[str]:
+        """
+        The most recent version to be activated to the staging network
+        """
+        return pulumi.get(self, "staging_version")
 
     @property
-    @pulumi.getter(name="productId")
-    def product_id(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "product_id")
+    @pulumi.getter
+    def type(self) -> pulumi.Output[str]:
+        """
+        Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
+        """
+        return pulumi.get(self, "type")
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cps_dv_enrollment.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cps_third_party_enrollment.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,86 +7,92 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['CpsDvEnrollmentArgs', 'CpsDvEnrollment']
+__all__ = ['CpsThirdPartyEnrollmentArgs', 'CpsThirdPartyEnrollment']
 
 @pulumi.input_type
-class CpsDvEnrollmentArgs:
+class CpsThirdPartyEnrollmentArgs:
     def __init__(__self__, *,
-                 admin_contact: pulumi.Input['CpsDvEnrollmentAdminContactArgs'],
+                 admin_contact: pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs'],
                  common_name: pulumi.Input[str],
                  contract_id: pulumi.Input[str],
-                 csr: pulumi.Input['CpsDvEnrollmentCsrArgs'],
-                 network_configuration: pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs'],
-                 organization: pulumi.Input['CpsDvEnrollmentOrganizationArgs'],
+                 csr: pulumi.Input['CpsThirdPartyEnrollmentCsrArgs'],
+                 network_configuration: pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs'],
+                 organization: pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs'],
                  secure_network: pulumi.Input[str],
-                 signature_algorithm: pulumi.Input[str],
                  sni_only: pulumi.Input[bool],
-                 tech_contact: pulumi.Input['CpsDvEnrollmentTechContactArgs'],
+                 tech_contact: pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs'],
                  acknowledge_pre_verification_warnings: Optional[pulumi.Input[bool]] = None,
                  allow_duplicate_common_name: Optional[pulumi.Input[bool]] = None,
+                 auto_approve_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  certificate_chain_type: Optional[pulumi.Input[str]] = None,
-                 enable_multi_stacked_certificates: Optional[pulumi.Input[bool]] = None,
-                 sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+                 change_management: Optional[pulumi.Input[bool]] = None,
+                 exclude_sans: Optional[pulumi.Input[bool]] = None,
+                 sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 signature_algorithm: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a CpsDvEnrollment resource.
-        :param pulumi.Input['CpsDvEnrollmentAdminContactArgs'] admin_contact: Contact information for the certificate administrator to use at organization
+        The set of arguments for constructing a CpsThirdPartyEnrollment resource.
+        :param pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs'] admin_contact: Contact information for the certificate administrator to use at organization
         :param pulumi.Input[str] common_name: Common name used for enrollment
         :param pulumi.Input[str] contract_id: Contract ID for which enrollment is retrieved
-        :param pulumi.Input['CpsDvEnrollmentCsrArgs'] csr: Certificate signing request generated during enrollment creation
-        :param pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs'] network_configuration: Settings containing network information and TLS Metadata used by CPS
-        :param pulumi.Input['CpsDvEnrollmentOrganizationArgs'] organization: Organization information
+        :param pulumi.Input['CpsThirdPartyEnrollmentCsrArgs'] csr: Data used for generation of Certificate Signing Request
+        :param pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs'] network_configuration: Settings containing network information and TLS metadata used by CPS
+        :param pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs'] organization: Organization information
         :param pulumi.Input[str] secure_network: Type of TLS deployment network
-        :param pulumi.Input[str] signature_algorithm: SHA algorithm type
         :param pulumi.Input[bool] sni_only: Whether Server Name Indication is used for enrollment
-        :param pulumi.Input['CpsDvEnrollmentTechContactArgs'] tech_contact: Contact information for an administrator at Akamai
+        :param pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs'] tech_contact: Contact information for an administrator at Akamai
         :param pulumi.Input[bool] acknowledge_pre_verification_warnings: Whether acknowledge warnings before certificate verification
         :param pulumi.Input[bool] allow_duplicate_common_name: Allow to duplicate common name
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] auto_approve_warnings: List of warnings to be automatically approved
         :param pulumi.Input[str] certificate_chain_type: Certificate trust chain type
-        :param pulumi.Input[bool] enable_multi_stacked_certificates: Enable Dual-Stacked certificate deployment for enrollment
+        :param pulumi.Input[bool] change_management: When set to false, the certificate will be deployed to both staging and production networks
+        :param pulumi.Input[bool] exclude_sans: When true, SANs are excluded from the CSR
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sans: List of SANs
+        :param pulumi.Input[str] signature_algorithm: The SHA function. Changing this value may require running terraform destroy, terraform apply
         """
         pulumi.set(__self__, "admin_contact", admin_contact)
         pulumi.set(__self__, "common_name", common_name)
         pulumi.set(__self__, "contract_id", contract_id)
         pulumi.set(__self__, "csr", csr)
         pulumi.set(__self__, "network_configuration", network_configuration)
         pulumi.set(__self__, "organization", organization)
         pulumi.set(__self__, "secure_network", secure_network)
-        pulumi.set(__self__, "signature_algorithm", signature_algorithm)
         pulumi.set(__self__, "sni_only", sni_only)
         pulumi.set(__self__, "tech_contact", tech_contact)
         if acknowledge_pre_verification_warnings is not None:
             pulumi.set(__self__, "acknowledge_pre_verification_warnings", acknowledge_pre_verification_warnings)
         if allow_duplicate_common_name is not None:
             pulumi.set(__self__, "allow_duplicate_common_name", allow_duplicate_common_name)
+        if auto_approve_warnings is not None:
+            pulumi.set(__self__, "auto_approve_warnings", auto_approve_warnings)
         if certificate_chain_type is not None:
             pulumi.set(__self__, "certificate_chain_type", certificate_chain_type)
-        if enable_multi_stacked_certificates is not None:
-            warnings.warn("""Deprecated, don't use; always false""", DeprecationWarning)
-            pulumi.log.warn("""enable_multi_stacked_certificates is deprecated: Deprecated, don't use; always false""")
-        if enable_multi_stacked_certificates is not None:
-            pulumi.set(__self__, "enable_multi_stacked_certificates", enable_multi_stacked_certificates)
+        if change_management is not None:
+            pulumi.set(__self__, "change_management", change_management)
+        if exclude_sans is not None:
+            pulumi.set(__self__, "exclude_sans", exclude_sans)
         if sans is not None:
             pulumi.set(__self__, "sans", sans)
+        if signature_algorithm is not None:
+            pulumi.set(__self__, "signature_algorithm", signature_algorithm)
 
     @property
     @pulumi.getter(name="adminContact")
-    def admin_contact(self) -> pulumi.Input['CpsDvEnrollmentAdminContactArgs']:
+    def admin_contact(self) -> pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs']:
         """
         Contact information for the certificate administrator to use at organization
         """
         return pulumi.get(self, "admin_contact")
 
     @admin_contact.setter
-    def admin_contact(self, value: pulumi.Input['CpsDvEnrollmentAdminContactArgs']):
+    def admin_contact(self, value: pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs']):
         pulumi.set(self, "admin_contact", value)
 
     @property
     @pulumi.getter(name="commonName")
     def common_name(self) -> pulumi.Input[str]:
         """
         Common name used for enrollment
@@ -107,46 +113,46 @@
 
     @contract_id.setter
     def contract_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "contract_id", value)
 
     @property
     @pulumi.getter
-    def csr(self) -> pulumi.Input['CpsDvEnrollmentCsrArgs']:
+    def csr(self) -> pulumi.Input['CpsThirdPartyEnrollmentCsrArgs']:
         """
-        Certificate signing request generated during enrollment creation
+        Data used for generation of Certificate Signing Request
         """
         return pulumi.get(self, "csr")
 
     @csr.setter
-    def csr(self, value: pulumi.Input['CpsDvEnrollmentCsrArgs']):
+    def csr(self, value: pulumi.Input['CpsThirdPartyEnrollmentCsrArgs']):
         pulumi.set(self, "csr", value)
 
     @property
     @pulumi.getter(name="networkConfiguration")
-    def network_configuration(self) -> pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs']:
+    def network_configuration(self) -> pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs']:
         """
-        Settings containing network information and TLS Metadata used by CPS
+        Settings containing network information and TLS metadata used by CPS
         """
         return pulumi.get(self, "network_configuration")
 
     @network_configuration.setter
-    def network_configuration(self, value: pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs']):
+    def network_configuration(self, value: pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs']):
         pulumi.set(self, "network_configuration", value)
 
     @property
     @pulumi.getter
-    def organization(self) -> pulumi.Input['CpsDvEnrollmentOrganizationArgs']:
+    def organization(self) -> pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs']:
         """
         Organization information
         """
         return pulumi.get(self, "organization")
 
     @organization.setter
-    def organization(self, value: pulumi.Input['CpsDvEnrollmentOrganizationArgs']):
+    def organization(self, value: pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs']):
         pulumi.set(self, "organization", value)
 
     @property
     @pulumi.getter(name="secureNetwork")
     def secure_network(self) -> pulumi.Input[str]:
         """
         Type of TLS deployment network
@@ -154,47 +160,35 @@
         return pulumi.get(self, "secure_network")
 
     @secure_network.setter
     def secure_network(self, value: pulumi.Input[str]):
         pulumi.set(self, "secure_network", value)
 
     @property
-    @pulumi.getter(name="signatureAlgorithm")
-    def signature_algorithm(self) -> pulumi.Input[str]:
-        """
-        SHA algorithm type
-        """
-        return pulumi.get(self, "signature_algorithm")
-
-    @signature_algorithm.setter
-    def signature_algorithm(self, value: pulumi.Input[str]):
-        pulumi.set(self, "signature_algorithm", value)
-
-    @property
     @pulumi.getter(name="sniOnly")
     def sni_only(self) -> pulumi.Input[bool]:
         """
         Whether Server Name Indication is used for enrollment
         """
         return pulumi.get(self, "sni_only")
 
     @sni_only.setter
     def sni_only(self, value: pulumi.Input[bool]):
         pulumi.set(self, "sni_only", value)
 
     @property
     @pulumi.getter(name="techContact")
-    def tech_contact(self) -> pulumi.Input['CpsDvEnrollmentTechContactArgs']:
+    def tech_contact(self) -> pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs']:
         """
         Contact information for an administrator at Akamai
         """
         return pulumi.get(self, "tech_contact")
 
     @tech_contact.setter
-    def tech_contact(self, value: pulumi.Input['CpsDvEnrollmentTechContactArgs']):
+    def tech_contact(self, value: pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs']):
         pulumi.set(self, "tech_contact", value)
 
     @property
     @pulumi.getter(name="acknowledgePreVerificationWarnings")
     def acknowledge_pre_verification_warnings(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether acknowledge warnings before certificate verification
@@ -214,142 +208,160 @@
         return pulumi.get(self, "allow_duplicate_common_name")
 
     @allow_duplicate_common_name.setter
     def allow_duplicate_common_name(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_duplicate_common_name", value)
 
     @property
+    @pulumi.getter(name="autoApproveWarnings")
+    def auto_approve_warnings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of warnings to be automatically approved
+        """
+        return pulumi.get(self, "auto_approve_warnings")
+
+    @auto_approve_warnings.setter
+    def auto_approve_warnings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "auto_approve_warnings", value)
+
+    @property
     @pulumi.getter(name="certificateChainType")
     def certificate_chain_type(self) -> Optional[pulumi.Input[str]]:
         """
         Certificate trust chain type
         """
         return pulumi.get(self, "certificate_chain_type")
 
     @certificate_chain_type.setter
     def certificate_chain_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "certificate_chain_type", value)
 
     @property
-    @pulumi.getter(name="enableMultiStackedCertificates")
-    def enable_multi_stacked_certificates(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="changeManagement")
+    def change_management(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable Dual-Stacked certificate deployment for enrollment
+        When set to false, the certificate will be deployed to both staging and production networks
         """
-        warnings.warn("""Deprecated, don't use; always false""", DeprecationWarning)
-        pulumi.log.warn("""enable_multi_stacked_certificates is deprecated: Deprecated, don't use; always false""")
+        return pulumi.get(self, "change_management")
+
+    @change_management.setter
+    def change_management(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "change_management", value)
 
-        return pulumi.get(self, "enable_multi_stacked_certificates")
+    @property
+    @pulumi.getter(name="excludeSans")
+    def exclude_sans(self) -> Optional[pulumi.Input[bool]]:
+        """
+        When true, SANs are excluded from the CSR
+        """
+        return pulumi.get(self, "exclude_sans")
 
-    @enable_multi_stacked_certificates.setter
-    def enable_multi_stacked_certificates(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enable_multi_stacked_certificates", value)
+    @exclude_sans.setter
+    def exclude_sans(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "exclude_sans", value)
 
     @property
     @pulumi.getter
     def sans(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of SANs
         """
         return pulumi.get(self, "sans")
 
     @sans.setter
     def sans(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "sans", value)
 
+    @property
+    @pulumi.getter(name="signatureAlgorithm")
+    def signature_algorithm(self) -> Optional[pulumi.Input[str]]:
+        """
+        The SHA function. Changing this value may require running terraform destroy, terraform apply
+        """
+        return pulumi.get(self, "signature_algorithm")
+
+    @signature_algorithm.setter
+    def signature_algorithm(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "signature_algorithm", value)
+
 
 @pulumi.input_type
-class _CpsDvEnrollmentState:
+class _CpsThirdPartyEnrollmentState:
     def __init__(__self__, *,
                  acknowledge_pre_verification_warnings: Optional[pulumi.Input[bool]] = None,
-                 admin_contact: Optional[pulumi.Input['CpsDvEnrollmentAdminContactArgs']] = None,
+                 admin_contact: Optional[pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs']] = None,
                  allow_duplicate_common_name: Optional[pulumi.Input[bool]] = None,
+                 auto_approve_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  certificate_chain_type: Optional[pulumi.Input[str]] = None,
-                 certificate_type: Optional[pulumi.Input[str]] = None,
+                 change_management: Optional[pulumi.Input[bool]] = None,
                  common_name: Optional[pulumi.Input[str]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
-                 csr: Optional[pulumi.Input['CpsDvEnrollmentCsrArgs']] = None,
-                 dns_challenges: Optional[pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentDnsChallengeArgs']]]] = None,
-                 enable_multi_stacked_certificates: Optional[pulumi.Input[bool]] = None,
-                 http_challenges: Optional[pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentHttpChallengeArgs']]]] = None,
-                 network_configuration: Optional[pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs']] = None,
-                 organization: Optional[pulumi.Input['CpsDvEnrollmentOrganizationArgs']] = None,
-                 registration_authority: Optional[pulumi.Input[str]] = None,
+                 csr: Optional[pulumi.Input['CpsThirdPartyEnrollmentCsrArgs']] = None,
+                 exclude_sans: Optional[pulumi.Input[bool]] = None,
+                 network_configuration: Optional[pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs']] = None,
+                 organization: Optional[pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs']] = None,
                  sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  secure_network: Optional[pulumi.Input[str]] = None,
                  signature_algorithm: Optional[pulumi.Input[str]] = None,
                  sni_only: Optional[pulumi.Input[bool]] = None,
-                 tech_contact: Optional[pulumi.Input['CpsDvEnrollmentTechContactArgs']] = None,
-                 validation_type: Optional[pulumi.Input[str]] = None):
+                 tech_contact: Optional[pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs']] = None):
         """
-        Input properties used for looking up and filtering CpsDvEnrollment resources.
+        Input properties used for looking up and filtering CpsThirdPartyEnrollment resources.
         :param pulumi.Input[bool] acknowledge_pre_verification_warnings: Whether acknowledge warnings before certificate verification
-        :param pulumi.Input['CpsDvEnrollmentAdminContactArgs'] admin_contact: Contact information for the certificate administrator to use at organization
+        :param pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs'] admin_contact: Contact information for the certificate administrator to use at organization
         :param pulumi.Input[bool] allow_duplicate_common_name: Allow to duplicate common name
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] auto_approve_warnings: List of warnings to be automatically approved
         :param pulumi.Input[str] certificate_chain_type: Certificate trust chain type
-        :param pulumi.Input[str] certificate_type: Certificate type of enrollment
+        :param pulumi.Input[bool] change_management: When set to false, the certificate will be deployed to both staging and production networks
         :param pulumi.Input[str] common_name: Common name used for enrollment
         :param pulumi.Input[str] contract_id: Contract ID for which enrollment is retrieved
-        :param pulumi.Input['CpsDvEnrollmentCsrArgs'] csr: Certificate signing request generated during enrollment creation
-        :param pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentDnsChallengeArgs']]] dns_challenges: DNS challenge information
-        :param pulumi.Input[bool] enable_multi_stacked_certificates: Enable Dual-Stacked certificate deployment for enrollment
-        :param pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentHttpChallengeArgs']]] http_challenges: HTTP challenge information
-        :param pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs'] network_configuration: Settings containing network information and TLS Metadata used by CPS
-        :param pulumi.Input['CpsDvEnrollmentOrganizationArgs'] organization: Organization information
-        :param pulumi.Input[str] registration_authority: The registration authority or certificate authority (CA) used to obtain a certificate
+        :param pulumi.Input['CpsThirdPartyEnrollmentCsrArgs'] csr: Data used for generation of Certificate Signing Request
+        :param pulumi.Input[bool] exclude_sans: When true, SANs are excluded from the CSR
+        :param pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs'] network_configuration: Settings containing network information and TLS metadata used by CPS
+        :param pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs'] organization: Organization information
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sans: List of SANs
         :param pulumi.Input[str] secure_network: Type of TLS deployment network
-        :param pulumi.Input[str] signature_algorithm: SHA algorithm type
+        :param pulumi.Input[str] signature_algorithm: The SHA function. Changing this value may require running terraform destroy, terraform apply
         :param pulumi.Input[bool] sni_only: Whether Server Name Indication is used for enrollment
-        :param pulumi.Input['CpsDvEnrollmentTechContactArgs'] tech_contact: Contact information for an administrator at Akamai
-        :param pulumi.Input[str] validation_type: Enrolment validation type
+        :param pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs'] tech_contact: Contact information for an administrator at Akamai
         """
         if acknowledge_pre_verification_warnings is not None:
             pulumi.set(__self__, "acknowledge_pre_verification_warnings", acknowledge_pre_verification_warnings)
         if admin_contact is not None:
             pulumi.set(__self__, "admin_contact", admin_contact)
         if allow_duplicate_common_name is not None:
             pulumi.set(__self__, "allow_duplicate_common_name", allow_duplicate_common_name)
+        if auto_approve_warnings is not None:
+            pulumi.set(__self__, "auto_approve_warnings", auto_approve_warnings)
         if certificate_chain_type is not None:
             pulumi.set(__self__, "certificate_chain_type", certificate_chain_type)
-        if certificate_type is not None:
-            pulumi.set(__self__, "certificate_type", certificate_type)
+        if change_management is not None:
+            pulumi.set(__self__, "change_management", change_management)
         if common_name is not None:
             pulumi.set(__self__, "common_name", common_name)
         if contract_id is not None:
             pulumi.set(__self__, "contract_id", contract_id)
         if csr is not None:
             pulumi.set(__self__, "csr", csr)
-        if dns_challenges is not None:
-            pulumi.set(__self__, "dns_challenges", dns_challenges)
-        if enable_multi_stacked_certificates is not None:
-            warnings.warn("""Deprecated, don't use; always false""", DeprecationWarning)
-            pulumi.log.warn("""enable_multi_stacked_certificates is deprecated: Deprecated, don't use; always false""")
-        if enable_multi_stacked_certificates is not None:
-            pulumi.set(__self__, "enable_multi_stacked_certificates", enable_multi_stacked_certificates)
-        if http_challenges is not None:
-            pulumi.set(__self__, "http_challenges", http_challenges)
+        if exclude_sans is not None:
+            pulumi.set(__self__, "exclude_sans", exclude_sans)
         if network_configuration is not None:
             pulumi.set(__self__, "network_configuration", network_configuration)
         if organization is not None:
             pulumi.set(__self__, "organization", organization)
-        if registration_authority is not None:
-            pulumi.set(__self__, "registration_authority", registration_authority)
         if sans is not None:
             pulumi.set(__self__, "sans", sans)
         if secure_network is not None:
             pulumi.set(__self__, "secure_network", secure_network)
         if signature_algorithm is not None:
             pulumi.set(__self__, "signature_algorithm", signature_algorithm)
         if sni_only is not None:
             pulumi.set(__self__, "sni_only", sni_only)
         if tech_contact is not None:
             pulumi.set(__self__, "tech_contact", tech_contact)
-        if validation_type is not None:
-            pulumi.set(__self__, "validation_type", validation_type)
 
     @property
     @pulumi.getter(name="acknowledgePreVerificationWarnings")
     def acknowledge_pre_verification_warnings(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether acknowledge warnings before certificate verification
         """
@@ -357,22 +369,22 @@
 
     @acknowledge_pre_verification_warnings.setter
     def acknowledge_pre_verification_warnings(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "acknowledge_pre_verification_warnings", value)
 
     @property
     @pulumi.getter(name="adminContact")
-    def admin_contact(self) -> Optional[pulumi.Input['CpsDvEnrollmentAdminContactArgs']]:
+    def admin_contact(self) -> Optional[pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs']]:
         """
         Contact information for the certificate administrator to use at organization
         """
         return pulumi.get(self, "admin_contact")
 
     @admin_contact.setter
-    def admin_contact(self, value: Optional[pulumi.Input['CpsDvEnrollmentAdminContactArgs']]):
+    def admin_contact(self, value: Optional[pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs']]):
         pulumi.set(self, "admin_contact", value)
 
     @property
     @pulumi.getter(name="allowDuplicateCommonName")
     def allow_duplicate_common_name(self) -> Optional[pulumi.Input[bool]]:
         """
         Allow to duplicate common name
@@ -380,36 +392,48 @@
         return pulumi.get(self, "allow_duplicate_common_name")
 
     @allow_duplicate_common_name.setter
     def allow_duplicate_common_name(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_duplicate_common_name", value)
 
     @property
+    @pulumi.getter(name="autoApproveWarnings")
+    def auto_approve_warnings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of warnings to be automatically approved
+        """
+        return pulumi.get(self, "auto_approve_warnings")
+
+    @auto_approve_warnings.setter
+    def auto_approve_warnings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "auto_approve_warnings", value)
+
+    @property
     @pulumi.getter(name="certificateChainType")
     def certificate_chain_type(self) -> Optional[pulumi.Input[str]]:
         """
         Certificate trust chain type
         """
         return pulumi.get(self, "certificate_chain_type")
 
     @certificate_chain_type.setter
     def certificate_chain_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "certificate_chain_type", value)
 
     @property
-    @pulumi.getter(name="certificateType")
-    def certificate_type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="changeManagement")
+    def change_management(self) -> Optional[pulumi.Input[bool]]:
         """
-        Certificate type of enrollment
+        When set to false, the certificate will be deployed to both staging and production networks
         """
-        return pulumi.get(self, "certificate_type")
+        return pulumi.get(self, "change_management")
 
-    @certificate_type.setter
-    def certificate_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "certificate_type", value)
+    @change_management.setter
+    def change_management(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "change_management", value)
 
     @property
     @pulumi.getter(name="commonName")
     def common_name(self) -> Optional[pulumi.Input[str]]:
         """
         Common name used for enrollment
         """
@@ -429,100 +453,61 @@
 
     @contract_id.setter
     def contract_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract_id", value)
 
     @property
     @pulumi.getter
-    def csr(self) -> Optional[pulumi.Input['CpsDvEnrollmentCsrArgs']]:
+    def csr(self) -> Optional[pulumi.Input['CpsThirdPartyEnrollmentCsrArgs']]:
         """
-        Certificate signing request generated during enrollment creation
+        Data used for generation of Certificate Signing Request
         """
         return pulumi.get(self, "csr")
 
     @csr.setter
-    def csr(self, value: Optional[pulumi.Input['CpsDvEnrollmentCsrArgs']]):
+    def csr(self, value: Optional[pulumi.Input['CpsThirdPartyEnrollmentCsrArgs']]):
         pulumi.set(self, "csr", value)
 
     @property
-    @pulumi.getter(name="dnsChallenges")
-    def dns_challenges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentDnsChallengeArgs']]]]:
+    @pulumi.getter(name="excludeSans")
+    def exclude_sans(self) -> Optional[pulumi.Input[bool]]:
         """
-        DNS challenge information
+        When true, SANs are excluded from the CSR
         """
-        return pulumi.get(self, "dns_challenges")
+        return pulumi.get(self, "exclude_sans")
 
-    @dns_challenges.setter
-    def dns_challenges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentDnsChallengeArgs']]]]):
-        pulumi.set(self, "dns_challenges", value)
-
-    @property
-    @pulumi.getter(name="enableMultiStackedCertificates")
-    def enable_multi_stacked_certificates(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable Dual-Stacked certificate deployment for enrollment
-        """
-        warnings.warn("""Deprecated, don't use; always false""", DeprecationWarning)
-        pulumi.log.warn("""enable_multi_stacked_certificates is deprecated: Deprecated, don't use; always false""")
-
-        return pulumi.get(self, "enable_multi_stacked_certificates")
-
-    @enable_multi_stacked_certificates.setter
-    def enable_multi_stacked_certificates(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enable_multi_stacked_certificates", value)
-
-    @property
-    @pulumi.getter(name="httpChallenges")
-    def http_challenges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentHttpChallengeArgs']]]]:
-        """
-        HTTP challenge information
-        """
-        return pulumi.get(self, "http_challenges")
-
-    @http_challenges.setter
-    def http_challenges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentHttpChallengeArgs']]]]):
-        pulumi.set(self, "http_challenges", value)
+    @exclude_sans.setter
+    def exclude_sans(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "exclude_sans", value)
 
     @property
     @pulumi.getter(name="networkConfiguration")
-    def network_configuration(self) -> Optional[pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs']]:
+    def network_configuration(self) -> Optional[pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs']]:
         """
-        Settings containing network information and TLS Metadata used by CPS
+        Settings containing network information and TLS metadata used by CPS
         """
         return pulumi.get(self, "network_configuration")
 
     @network_configuration.setter
-    def network_configuration(self, value: Optional[pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs']]):
+    def network_configuration(self, value: Optional[pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs']]):
         pulumi.set(self, "network_configuration", value)
 
     @property
     @pulumi.getter
-    def organization(self) -> Optional[pulumi.Input['CpsDvEnrollmentOrganizationArgs']]:
+    def organization(self) -> Optional[pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs']]:
         """
         Organization information
         """
         return pulumi.get(self, "organization")
 
     @organization.setter
-    def organization(self, value: Optional[pulumi.Input['CpsDvEnrollmentOrganizationArgs']]):
+    def organization(self, value: Optional[pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs']]):
         pulumi.set(self, "organization", value)
 
     @property
-    @pulumi.getter(name="registrationAuthority")
-    def registration_authority(self) -> Optional[pulumi.Input[str]]:
-        """
-        The registration authority or certificate authority (CA) used to obtain a certificate
-        """
-        return pulumi.get(self, "registration_authority")
-
-    @registration_authority.setter
-    def registration_authority(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "registration_authority", value)
-
-    @property
     @pulumi.getter
     def sans(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of SANs
         """
         return pulumi.get(self, "sans")
 
@@ -542,15 +527,15 @@
     def secure_network(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secure_network", value)
 
     @property
     @pulumi.getter(name="signatureAlgorithm")
     def signature_algorithm(self) -> Optional[pulumi.Input[str]]:
         """
-        SHA algorithm type
+        The SHA function. Changing this value may require running terraform destroy, terraform apply
         """
         return pulumi.get(self, "signature_algorithm")
 
     @signature_algorithm.setter
     def signature_algorithm(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signature_algorithm", value)
 
@@ -564,291 +549,276 @@
 
     @sni_only.setter
     def sni_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "sni_only", value)
 
     @property
     @pulumi.getter(name="techContact")
-    def tech_contact(self) -> Optional[pulumi.Input['CpsDvEnrollmentTechContactArgs']]:
+    def tech_contact(self) -> Optional[pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs']]:
         """
         Contact information for an administrator at Akamai
         """
         return pulumi.get(self, "tech_contact")
 
     @tech_contact.setter
-    def tech_contact(self, value: Optional[pulumi.Input['CpsDvEnrollmentTechContactArgs']]):
+    def tech_contact(self, value: Optional[pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs']]):
         pulumi.set(self, "tech_contact", value)
 
-    @property
-    @pulumi.getter(name="validationType")
-    def validation_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        Enrolment validation type
-        """
-        return pulumi.get(self, "validation_type")
-
-    @validation_type.setter
-    def validation_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "validation_type", value)
-
 
-class CpsDvEnrollment(pulumi.CustomResource):
+class CpsThirdPartyEnrollment(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  acknowledge_pre_verification_warnings: Optional[pulumi.Input[bool]] = None,
-                 admin_contact: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentAdminContactArgs']]] = None,
+                 admin_contact: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentAdminContactArgs']]] = None,
                  allow_duplicate_common_name: Optional[pulumi.Input[bool]] = None,
+                 auto_approve_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  certificate_chain_type: Optional[pulumi.Input[str]] = None,
+                 change_management: Optional[pulumi.Input[bool]] = None,
                  common_name: Optional[pulumi.Input[str]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
-                 csr: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentCsrArgs']]] = None,
-                 enable_multi_stacked_certificates: Optional[pulumi.Input[bool]] = None,
-                 network_configuration: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentNetworkConfigurationArgs']]] = None,
-                 organization: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentOrganizationArgs']]] = None,
+                 csr: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentCsrArgs']]] = None,
+                 exclude_sans: Optional[pulumi.Input[bool]] = None,
+                 network_configuration: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentNetworkConfigurationArgs']]] = None,
+                 organization: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentOrganizationArgs']]] = None,
                  sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  secure_network: Optional[pulumi.Input[str]] = None,
                  signature_algorithm: Optional[pulumi.Input[str]] = None,
                  sni_only: Optional[pulumi.Input[bool]] = None,
-                 tech_contact: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentTechContactArgs']]] = None,
+                 tech_contact: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentTechContactArgs']]] = None,
                  __props__=None):
         """
-        Create a CpsDvEnrollment resource with the given unique name, props, and options.
+        Create a CpsThirdPartyEnrollment resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] acknowledge_pre_verification_warnings: Whether acknowledge warnings before certificate verification
-        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentAdminContactArgs']] admin_contact: Contact information for the certificate administrator to use at organization
+        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentAdminContactArgs']] admin_contact: Contact information for the certificate administrator to use at organization
         :param pulumi.Input[bool] allow_duplicate_common_name: Allow to duplicate common name
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] auto_approve_warnings: List of warnings to be automatically approved
         :param pulumi.Input[str] certificate_chain_type: Certificate trust chain type
+        :param pulumi.Input[bool] change_management: When set to false, the certificate will be deployed to both staging and production networks
         :param pulumi.Input[str] common_name: Common name used for enrollment
         :param pulumi.Input[str] contract_id: Contract ID for which enrollment is retrieved
-        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentCsrArgs']] csr: Certificate signing request generated during enrollment creation
-        :param pulumi.Input[bool] enable_multi_stacked_certificates: Enable Dual-Stacked certificate deployment for enrollment
-        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentNetworkConfigurationArgs']] network_configuration: Settings containing network information and TLS Metadata used by CPS
-        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentOrganizationArgs']] organization: Organization information
+        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentCsrArgs']] csr: Data used for generation of Certificate Signing Request
+        :param pulumi.Input[bool] exclude_sans: When true, SANs are excluded from the CSR
+        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentNetworkConfigurationArgs']] network_configuration: Settings containing network information and TLS metadata used by CPS
+        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentOrganizationArgs']] organization: Organization information
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sans: List of SANs
         :param pulumi.Input[str] secure_network: Type of TLS deployment network
-        :param pulumi.Input[str] signature_algorithm: SHA algorithm type
+        :param pulumi.Input[str] signature_algorithm: The SHA function. Changing this value may require running terraform destroy, terraform apply
         :param pulumi.Input[bool] sni_only: Whether Server Name Indication is used for enrollment
-        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentTechContactArgs']] tech_contact: Contact information for an administrator at Akamai
+        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentTechContactArgs']] tech_contact: Contact information for an administrator at Akamai
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: CpsDvEnrollmentArgs,
+                 args: CpsThirdPartyEnrollmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a CpsDvEnrollment resource with the given unique name, props, and options.
+        Create a CpsThirdPartyEnrollment resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param CpsDvEnrollmentArgs args: The arguments to use to populate this resource's properties.
+        :param CpsThirdPartyEnrollmentArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CpsDvEnrollmentArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(CpsThirdPartyEnrollmentArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  acknowledge_pre_verification_warnings: Optional[pulumi.Input[bool]] = None,
-                 admin_contact: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentAdminContactArgs']]] = None,
+                 admin_contact: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentAdminContactArgs']]] = None,
                  allow_duplicate_common_name: Optional[pulumi.Input[bool]] = None,
+                 auto_approve_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  certificate_chain_type: Optional[pulumi.Input[str]] = None,
+                 change_management: Optional[pulumi.Input[bool]] = None,
                  common_name: Optional[pulumi.Input[str]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
-                 csr: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentCsrArgs']]] = None,
-                 enable_multi_stacked_certificates: Optional[pulumi.Input[bool]] = None,
-                 network_configuration: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentNetworkConfigurationArgs']]] = None,
-                 organization: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentOrganizationArgs']]] = None,
+                 csr: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentCsrArgs']]] = None,
+                 exclude_sans: Optional[pulumi.Input[bool]] = None,
+                 network_configuration: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentNetworkConfigurationArgs']]] = None,
+                 organization: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentOrganizationArgs']]] = None,
                  sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  secure_network: Optional[pulumi.Input[str]] = None,
                  signature_algorithm: Optional[pulumi.Input[str]] = None,
                  sni_only: Optional[pulumi.Input[bool]] = None,
-                 tech_contact: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentTechContactArgs']]] = None,
+                 tech_contact: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentTechContactArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CpsDvEnrollmentArgs.__new__(CpsDvEnrollmentArgs)
+            __props__ = CpsThirdPartyEnrollmentArgs.__new__(CpsThirdPartyEnrollmentArgs)
 
             __props__.__dict__["acknowledge_pre_verification_warnings"] = acknowledge_pre_verification_warnings
             if admin_contact is None and not opts.urn:
                 raise TypeError("Missing required property 'admin_contact'")
             __props__.__dict__["admin_contact"] = admin_contact
             __props__.__dict__["allow_duplicate_common_name"] = allow_duplicate_common_name
+            __props__.__dict__["auto_approve_warnings"] = auto_approve_warnings
             __props__.__dict__["certificate_chain_type"] = certificate_chain_type
+            __props__.__dict__["change_management"] = change_management
             if common_name is None and not opts.urn:
                 raise TypeError("Missing required property 'common_name'")
             __props__.__dict__["common_name"] = common_name
             if contract_id is None and not opts.urn:
                 raise TypeError("Missing required property 'contract_id'")
             __props__.__dict__["contract_id"] = contract_id
             if csr is None and not opts.urn:
                 raise TypeError("Missing required property 'csr'")
             __props__.__dict__["csr"] = csr
-            if enable_multi_stacked_certificates is not None and not opts.urn:
-                warnings.warn("""Deprecated, don't use; always false""", DeprecationWarning)
-                pulumi.log.warn("""enable_multi_stacked_certificates is deprecated: Deprecated, don't use; always false""")
-            __props__.__dict__["enable_multi_stacked_certificates"] = enable_multi_stacked_certificates
+            __props__.__dict__["exclude_sans"] = exclude_sans
             if network_configuration is None and not opts.urn:
                 raise TypeError("Missing required property 'network_configuration'")
             __props__.__dict__["network_configuration"] = network_configuration
             if organization is None and not opts.urn:
                 raise TypeError("Missing required property 'organization'")
             __props__.__dict__["organization"] = organization
             __props__.__dict__["sans"] = sans
             if secure_network is None and not opts.urn:
                 raise TypeError("Missing required property 'secure_network'")
             __props__.__dict__["secure_network"] = secure_network
-            if signature_algorithm is None and not opts.urn:
-                raise TypeError("Missing required property 'signature_algorithm'")
             __props__.__dict__["signature_algorithm"] = signature_algorithm
             if sni_only is None and not opts.urn:
                 raise TypeError("Missing required property 'sni_only'")
             __props__.__dict__["sni_only"] = sni_only
             if tech_contact is None and not opts.urn:
                 raise TypeError("Missing required property 'tech_contact'")
             __props__.__dict__["tech_contact"] = tech_contact
-            __props__.__dict__["certificate_type"] = None
-            __props__.__dict__["dns_challenges"] = None
-            __props__.__dict__["http_challenges"] = None
-            __props__.__dict__["registration_authority"] = None
-            __props__.__dict__["validation_type"] = None
-        super(CpsDvEnrollment, __self__).__init__(
-            'akamai:index/cpsDvEnrollment:CpsDvEnrollment',
+        super(CpsThirdPartyEnrollment, __self__).__init__(
+            'akamai:index/cpsThirdPartyEnrollment:CpsThirdPartyEnrollment',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             acknowledge_pre_verification_warnings: Optional[pulumi.Input[bool]] = None,
-            admin_contact: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentAdminContactArgs']]] = None,
+            admin_contact: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentAdminContactArgs']]] = None,
             allow_duplicate_common_name: Optional[pulumi.Input[bool]] = None,
+            auto_approve_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             certificate_chain_type: Optional[pulumi.Input[str]] = None,
-            certificate_type: Optional[pulumi.Input[str]] = None,
+            change_management: Optional[pulumi.Input[bool]] = None,
             common_name: Optional[pulumi.Input[str]] = None,
             contract_id: Optional[pulumi.Input[str]] = None,
-            csr: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentCsrArgs']]] = None,
-            dns_challenges: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CpsDvEnrollmentDnsChallengeArgs']]]]] = None,
-            enable_multi_stacked_certificates: Optional[pulumi.Input[bool]] = None,
-            http_challenges: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CpsDvEnrollmentHttpChallengeArgs']]]]] = None,
-            network_configuration: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentNetworkConfigurationArgs']]] = None,
-            organization: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentOrganizationArgs']]] = None,
-            registration_authority: Optional[pulumi.Input[str]] = None,
+            csr: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentCsrArgs']]] = None,
+            exclude_sans: Optional[pulumi.Input[bool]] = None,
+            network_configuration: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentNetworkConfigurationArgs']]] = None,
+            organization: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentOrganizationArgs']]] = None,
             sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             secure_network: Optional[pulumi.Input[str]] = None,
             signature_algorithm: Optional[pulumi.Input[str]] = None,
             sni_only: Optional[pulumi.Input[bool]] = None,
-            tech_contact: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentTechContactArgs']]] = None,
-            validation_type: Optional[pulumi.Input[str]] = None) -> 'CpsDvEnrollment':
+            tech_contact: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentTechContactArgs']]] = None) -> 'CpsThirdPartyEnrollment':
         """
-        Get an existing CpsDvEnrollment resource's state with the given name, id, and optional extra
+        Get an existing CpsThirdPartyEnrollment resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] acknowledge_pre_verification_warnings: Whether acknowledge warnings before certificate verification
-        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentAdminContactArgs']] admin_contact: Contact information for the certificate administrator to use at organization
+        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentAdminContactArgs']] admin_contact: Contact information for the certificate administrator to use at organization
         :param pulumi.Input[bool] allow_duplicate_common_name: Allow to duplicate common name
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] auto_approve_warnings: List of warnings to be automatically approved
         :param pulumi.Input[str] certificate_chain_type: Certificate trust chain type
-        :param pulumi.Input[str] certificate_type: Certificate type of enrollment
+        :param pulumi.Input[bool] change_management: When set to false, the certificate will be deployed to both staging and production networks
         :param pulumi.Input[str] common_name: Common name used for enrollment
         :param pulumi.Input[str] contract_id: Contract ID for which enrollment is retrieved
-        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentCsrArgs']] csr: Certificate signing request generated during enrollment creation
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CpsDvEnrollmentDnsChallengeArgs']]]] dns_challenges: DNS challenge information
-        :param pulumi.Input[bool] enable_multi_stacked_certificates: Enable Dual-Stacked certificate deployment for enrollment
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CpsDvEnrollmentHttpChallengeArgs']]]] http_challenges: HTTP challenge information
-        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentNetworkConfigurationArgs']] network_configuration: Settings containing network information and TLS Metadata used by CPS
-        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentOrganizationArgs']] organization: Organization information
-        :param pulumi.Input[str] registration_authority: The registration authority or certificate authority (CA) used to obtain a certificate
+        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentCsrArgs']] csr: Data used for generation of Certificate Signing Request
+        :param pulumi.Input[bool] exclude_sans: When true, SANs are excluded from the CSR
+        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentNetworkConfigurationArgs']] network_configuration: Settings containing network information and TLS metadata used by CPS
+        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentOrganizationArgs']] organization: Organization information
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sans: List of SANs
         :param pulumi.Input[str] secure_network: Type of TLS deployment network
-        :param pulumi.Input[str] signature_algorithm: SHA algorithm type
+        :param pulumi.Input[str] signature_algorithm: The SHA function. Changing this value may require running terraform destroy, terraform apply
         :param pulumi.Input[bool] sni_only: Whether Server Name Indication is used for enrollment
-        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentTechContactArgs']] tech_contact: Contact information for an administrator at Akamai
-        :param pulumi.Input[str] validation_type: Enrolment validation type
+        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentTechContactArgs']] tech_contact: Contact information for an administrator at Akamai
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _CpsDvEnrollmentState.__new__(_CpsDvEnrollmentState)
+        __props__ = _CpsThirdPartyEnrollmentState.__new__(_CpsThirdPartyEnrollmentState)
 
         __props__.__dict__["acknowledge_pre_verification_warnings"] = acknowledge_pre_verification_warnings
         __props__.__dict__["admin_contact"] = admin_contact
         __props__.__dict__["allow_duplicate_common_name"] = allow_duplicate_common_name
+        __props__.__dict__["auto_approve_warnings"] = auto_approve_warnings
         __props__.__dict__["certificate_chain_type"] = certificate_chain_type
-        __props__.__dict__["certificate_type"] = certificate_type
+        __props__.__dict__["change_management"] = change_management
         __props__.__dict__["common_name"] = common_name
         __props__.__dict__["contract_id"] = contract_id
         __props__.__dict__["csr"] = csr
-        __props__.__dict__["dns_challenges"] = dns_challenges
-        __props__.__dict__["enable_multi_stacked_certificates"] = enable_multi_stacked_certificates
-        __props__.__dict__["http_challenges"] = http_challenges
+        __props__.__dict__["exclude_sans"] = exclude_sans
         __props__.__dict__["network_configuration"] = network_configuration
         __props__.__dict__["organization"] = organization
-        __props__.__dict__["registration_authority"] = registration_authority
         __props__.__dict__["sans"] = sans
         __props__.__dict__["secure_network"] = secure_network
         __props__.__dict__["signature_algorithm"] = signature_algorithm
         __props__.__dict__["sni_only"] = sni_only
         __props__.__dict__["tech_contact"] = tech_contact
-        __props__.__dict__["validation_type"] = validation_type
-        return CpsDvEnrollment(resource_name, opts=opts, __props__=__props__)
+        return CpsThirdPartyEnrollment(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="acknowledgePreVerificationWarnings")
     def acknowledge_pre_verification_warnings(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether acknowledge warnings before certificate verification
         """
         return pulumi.get(self, "acknowledge_pre_verification_warnings")
 
     @property
     @pulumi.getter(name="adminContact")
-    def admin_contact(self) -> pulumi.Output['outputs.CpsDvEnrollmentAdminContact']:
+    def admin_contact(self) -> pulumi.Output['outputs.CpsThirdPartyEnrollmentAdminContact']:
         """
         Contact information for the certificate administrator to use at organization
         """
         return pulumi.get(self, "admin_contact")
 
     @property
     @pulumi.getter(name="allowDuplicateCommonName")
     def allow_duplicate_common_name(self) -> pulumi.Output[Optional[bool]]:
         """
         Allow to duplicate common name
         """
         return pulumi.get(self, "allow_duplicate_common_name")
 
     @property
+    @pulumi.getter(name="autoApproveWarnings")
+    def auto_approve_warnings(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        List of warnings to be automatically approved
+        """
+        return pulumi.get(self, "auto_approve_warnings")
+
+    @property
     @pulumi.getter(name="certificateChainType")
     def certificate_chain_type(self) -> pulumi.Output[Optional[str]]:
         """
         Certificate trust chain type
         """
         return pulumi.get(self, "certificate_chain_type")
 
     @property
-    @pulumi.getter(name="certificateType")
-    def certificate_type(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="changeManagement")
+    def change_management(self) -> pulumi.Output[Optional[bool]]:
         """
-        Certificate type of enrollment
+        When set to false, the certificate will be deployed to both staging and production networks
         """
-        return pulumi.get(self, "certificate_type")
+        return pulumi.get(self, "change_management")
 
     @property
     @pulumi.getter(name="commonName")
     def common_name(self) -> pulumi.Output[str]:
         """
         Common name used for enrollment
         """
@@ -860,72 +830,45 @@
         """
         Contract ID for which enrollment is retrieved
         """
         return pulumi.get(self, "contract_id")
 
     @property
     @pulumi.getter
-    def csr(self) -> pulumi.Output['outputs.CpsDvEnrollmentCsr']:
+    def csr(self) -> pulumi.Output['outputs.CpsThirdPartyEnrollmentCsr']:
         """
-        Certificate signing request generated during enrollment creation
+        Data used for generation of Certificate Signing Request
         """
         return pulumi.get(self, "csr")
 
     @property
-    @pulumi.getter(name="dnsChallenges")
-    def dns_challenges(self) -> pulumi.Output[Sequence['outputs.CpsDvEnrollmentDnsChallenge']]:
-        """
-        DNS challenge information
-        """
-        return pulumi.get(self, "dns_challenges")
-
-    @property
-    @pulumi.getter(name="enableMultiStackedCertificates")
-    def enable_multi_stacked_certificates(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="excludeSans")
+    def exclude_sans(self) -> pulumi.Output[Optional[bool]]:
         """
-        Enable Dual-Stacked certificate deployment for enrollment
+        When true, SANs are excluded from the CSR
         """
-        warnings.warn("""Deprecated, don't use; always false""", DeprecationWarning)
-        pulumi.log.warn("""enable_multi_stacked_certificates is deprecated: Deprecated, don't use; always false""")
-
-        return pulumi.get(self, "enable_multi_stacked_certificates")
-
-    @property
-    @pulumi.getter(name="httpChallenges")
-    def http_challenges(self) -> pulumi.Output[Sequence['outputs.CpsDvEnrollmentHttpChallenge']]:
-        """
-        HTTP challenge information
-        """
-        return pulumi.get(self, "http_challenges")
+        return pulumi.get(self, "exclude_sans")
 
     @property
     @pulumi.getter(name="networkConfiguration")
-    def network_configuration(self) -> pulumi.Output['outputs.CpsDvEnrollmentNetworkConfiguration']:
+    def network_configuration(self) -> pulumi.Output['outputs.CpsThirdPartyEnrollmentNetworkConfiguration']:
         """
-        Settings containing network information and TLS Metadata used by CPS
+        Settings containing network information and TLS metadata used by CPS
         """
         return pulumi.get(self, "network_configuration")
 
     @property
     @pulumi.getter
-    def organization(self) -> pulumi.Output['outputs.CpsDvEnrollmentOrganization']:
+    def organization(self) -> pulumi.Output['outputs.CpsThirdPartyEnrollmentOrganization']:
         """
         Organization information
         """
         return pulumi.get(self, "organization")
 
     @property
-    @pulumi.getter(name="registrationAuthority")
-    def registration_authority(self) -> pulumi.Output[str]:
-        """
-        The registration authority or certificate authority (CA) used to obtain a certificate
-        """
-        return pulumi.get(self, "registration_authority")
-
-    @property
     @pulumi.getter
     def sans(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         List of SANs
         """
         return pulumi.get(self, "sans")
 
@@ -935,37 +878,29 @@
         """
         Type of TLS deployment network
         """
         return pulumi.get(self, "secure_network")
 
     @property
     @pulumi.getter(name="signatureAlgorithm")
-    def signature_algorithm(self) -> pulumi.Output[str]:
+    def signature_algorithm(self) -> pulumi.Output[Optional[str]]:
         """
-        SHA algorithm type
+        The SHA function. Changing this value may require running terraform destroy, terraform apply
         """
         return pulumi.get(self, "signature_algorithm")
 
     @property
     @pulumi.getter(name="sniOnly")
     def sni_only(self) -> pulumi.Output[bool]:
         """
         Whether Server Name Indication is used for enrollment
         """
         return pulumi.get(self, "sni_only")
 
     @property
     @pulumi.getter(name="techContact")
-    def tech_contact(self) -> pulumi.Output['outputs.CpsDvEnrollmentTechContact']:
+    def tech_contact(self) -> pulumi.Output['outputs.CpsThirdPartyEnrollmentTechContact']:
         """
         Contact information for an administrator at Akamai
         """
         return pulumi.get(self, "tech_contact")
 
-    @property
-    @pulumi.getter(name="validationType")
-    def validation_type(self) -> pulumi.Output[str]:
-        """
-        Enrolment validation type
-        """
-        return pulumi.get(self, "validation_type")
-
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cps_dv_validation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cps_dv_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cps_third_party_enrollment.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cps_dv_enrollment.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,92 +7,79 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['CpsThirdPartyEnrollmentArgs', 'CpsThirdPartyEnrollment']
+__all__ = ['CpsDvEnrollmentArgs', 'CpsDvEnrollment']
 
 @pulumi.input_type
-class CpsThirdPartyEnrollmentArgs:
+class CpsDvEnrollmentArgs:
     def __init__(__self__, *,
-                 admin_contact: pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs'],
+                 admin_contact: pulumi.Input['CpsDvEnrollmentAdminContactArgs'],
                  common_name: pulumi.Input[str],
                  contract_id: pulumi.Input[str],
-                 csr: pulumi.Input['CpsThirdPartyEnrollmentCsrArgs'],
-                 network_configuration: pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs'],
-                 organization: pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs'],
+                 csr: pulumi.Input['CpsDvEnrollmentCsrArgs'],
+                 network_configuration: pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs'],
+                 organization: pulumi.Input['CpsDvEnrollmentOrganizationArgs'],
                  secure_network: pulumi.Input[str],
+                 signature_algorithm: pulumi.Input[str],
                  sni_only: pulumi.Input[bool],
-                 tech_contact: pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs'],
+                 tech_contact: pulumi.Input['CpsDvEnrollmentTechContactArgs'],
                  acknowledge_pre_verification_warnings: Optional[pulumi.Input[bool]] = None,
                  allow_duplicate_common_name: Optional[pulumi.Input[bool]] = None,
-                 auto_approve_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  certificate_chain_type: Optional[pulumi.Input[str]] = None,
-                 change_management: Optional[pulumi.Input[bool]] = None,
-                 exclude_sans: Optional[pulumi.Input[bool]] = None,
-                 sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 signature_algorithm: Optional[pulumi.Input[str]] = None):
+                 sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        The set of arguments for constructing a CpsThirdPartyEnrollment resource.
-        :param pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs'] admin_contact: Contact information for the certificate administrator to use at organization
+        The set of arguments for constructing a CpsDvEnrollment resource.
+        :param pulumi.Input['CpsDvEnrollmentAdminContactArgs'] admin_contact: Contact information for the certificate administrator to use at organization
         :param pulumi.Input[str] common_name: Common name used for enrollment
         :param pulumi.Input[str] contract_id: Contract ID for which enrollment is retrieved
-        :param pulumi.Input['CpsThirdPartyEnrollmentCsrArgs'] csr: Data used for generation of Certificate Signing Request
-        :param pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs'] network_configuration: Settings containing network information and TLS metadata used by CPS
-        :param pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs'] organization: Organization information
+        :param pulumi.Input['CpsDvEnrollmentCsrArgs'] csr: Certificate signing request generated during enrollment creation
+        :param pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs'] network_configuration: Settings containing network information and TLS Metadata used by CPS
+        :param pulumi.Input['CpsDvEnrollmentOrganizationArgs'] organization: Organization information
         :param pulumi.Input[str] secure_network: Type of TLS deployment network
+        :param pulumi.Input[str] signature_algorithm: SHA algorithm type
         :param pulumi.Input[bool] sni_only: Whether Server Name Indication is used for enrollment
-        :param pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs'] tech_contact: Contact information for an administrator at Akamai
+        :param pulumi.Input['CpsDvEnrollmentTechContactArgs'] tech_contact: Contact information for an administrator at Akamai
         :param pulumi.Input[bool] acknowledge_pre_verification_warnings: Whether acknowledge warnings before certificate verification
         :param pulumi.Input[bool] allow_duplicate_common_name: Allow to duplicate common name
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] auto_approve_warnings: List of warnings to be automatically approved
         :param pulumi.Input[str] certificate_chain_type: Certificate trust chain type
-        :param pulumi.Input[bool] change_management: When set to false, the certificate will be deployed to both staging and production networks
-        :param pulumi.Input[bool] exclude_sans: When true, SANs are excluded from the CSR
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sans: List of SANs
-        :param pulumi.Input[str] signature_algorithm: The SHA function. Changing this value may require running terraform destroy, terraform apply
         """
         pulumi.set(__self__, "admin_contact", admin_contact)
         pulumi.set(__self__, "common_name", common_name)
         pulumi.set(__self__, "contract_id", contract_id)
         pulumi.set(__self__, "csr", csr)
         pulumi.set(__self__, "network_configuration", network_configuration)
         pulumi.set(__self__, "organization", organization)
         pulumi.set(__self__, "secure_network", secure_network)
+        pulumi.set(__self__, "signature_algorithm", signature_algorithm)
         pulumi.set(__self__, "sni_only", sni_only)
         pulumi.set(__self__, "tech_contact", tech_contact)
         if acknowledge_pre_verification_warnings is not None:
             pulumi.set(__self__, "acknowledge_pre_verification_warnings", acknowledge_pre_verification_warnings)
         if allow_duplicate_common_name is not None:
             pulumi.set(__self__, "allow_duplicate_common_name", allow_duplicate_common_name)
-        if auto_approve_warnings is not None:
-            pulumi.set(__self__, "auto_approve_warnings", auto_approve_warnings)
         if certificate_chain_type is not None:
             pulumi.set(__self__, "certificate_chain_type", certificate_chain_type)
-        if change_management is not None:
-            pulumi.set(__self__, "change_management", change_management)
-        if exclude_sans is not None:
-            pulumi.set(__self__, "exclude_sans", exclude_sans)
         if sans is not None:
             pulumi.set(__self__, "sans", sans)
-        if signature_algorithm is not None:
-            pulumi.set(__self__, "signature_algorithm", signature_algorithm)
 
     @property
     @pulumi.getter(name="adminContact")
-    def admin_contact(self) -> pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs']:
+    def admin_contact(self) -> pulumi.Input['CpsDvEnrollmentAdminContactArgs']:
         """
         Contact information for the certificate administrator to use at organization
         """
         return pulumi.get(self, "admin_contact")
 
     @admin_contact.setter
-    def admin_contact(self, value: pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs']):
+    def admin_contact(self, value: pulumi.Input['CpsDvEnrollmentAdminContactArgs']):
         pulumi.set(self, "admin_contact", value)
 
     @property
     @pulumi.getter(name="commonName")
     def common_name(self) -> pulumi.Input[str]:
         """
         Common name used for enrollment
@@ -113,46 +100,46 @@
 
     @contract_id.setter
     def contract_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "contract_id", value)
 
     @property
     @pulumi.getter
-    def csr(self) -> pulumi.Input['CpsThirdPartyEnrollmentCsrArgs']:
+    def csr(self) -> pulumi.Input['CpsDvEnrollmentCsrArgs']:
         """
-        Data used for generation of Certificate Signing Request
+        Certificate signing request generated during enrollment creation
         """
         return pulumi.get(self, "csr")
 
     @csr.setter
-    def csr(self, value: pulumi.Input['CpsThirdPartyEnrollmentCsrArgs']):
+    def csr(self, value: pulumi.Input['CpsDvEnrollmentCsrArgs']):
         pulumi.set(self, "csr", value)
 
     @property
     @pulumi.getter(name="networkConfiguration")
-    def network_configuration(self) -> pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs']:
+    def network_configuration(self) -> pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs']:
         """
-        Settings containing network information and TLS metadata used by CPS
+        Settings containing network information and TLS Metadata used by CPS
         """
         return pulumi.get(self, "network_configuration")
 
     @network_configuration.setter
-    def network_configuration(self, value: pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs']):
+    def network_configuration(self, value: pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs']):
         pulumi.set(self, "network_configuration", value)
 
     @property
     @pulumi.getter
-    def organization(self) -> pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs']:
+    def organization(self) -> pulumi.Input['CpsDvEnrollmentOrganizationArgs']:
         """
         Organization information
         """
         return pulumi.get(self, "organization")
 
     @organization.setter
-    def organization(self, value: pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs']):
+    def organization(self, value: pulumi.Input['CpsDvEnrollmentOrganizationArgs']):
         pulumi.set(self, "organization", value)
 
     @property
     @pulumi.getter(name="secureNetwork")
     def secure_network(self) -> pulumi.Input[str]:
         """
         Type of TLS deployment network
@@ -160,35 +147,47 @@
         return pulumi.get(self, "secure_network")
 
     @secure_network.setter
     def secure_network(self, value: pulumi.Input[str]):
         pulumi.set(self, "secure_network", value)
 
     @property
+    @pulumi.getter(name="signatureAlgorithm")
+    def signature_algorithm(self) -> pulumi.Input[str]:
+        """
+        SHA algorithm type
+        """
+        return pulumi.get(self, "signature_algorithm")
+
+    @signature_algorithm.setter
+    def signature_algorithm(self, value: pulumi.Input[str]):
+        pulumi.set(self, "signature_algorithm", value)
+
+    @property
     @pulumi.getter(name="sniOnly")
     def sni_only(self) -> pulumi.Input[bool]:
         """
         Whether Server Name Indication is used for enrollment
         """
         return pulumi.get(self, "sni_only")
 
     @sni_only.setter
     def sni_only(self, value: pulumi.Input[bool]):
         pulumi.set(self, "sni_only", value)
 
     @property
     @pulumi.getter(name="techContact")
-    def tech_contact(self) -> pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs']:
+    def tech_contact(self) -> pulumi.Input['CpsDvEnrollmentTechContactArgs']:
         """
         Contact information for an administrator at Akamai
         """
         return pulumi.get(self, "tech_contact")
 
     @tech_contact.setter
-    def tech_contact(self, value: pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs']):
+    def tech_contact(self, value: pulumi.Input['CpsDvEnrollmentTechContactArgs']):
         pulumi.set(self, "tech_contact", value)
 
     @property
     @pulumi.getter(name="acknowledgePreVerificationWarnings")
     def acknowledge_pre_verification_warnings(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether acknowledge warnings before certificate verification
@@ -208,160 +207,120 @@
         return pulumi.get(self, "allow_duplicate_common_name")
 
     @allow_duplicate_common_name.setter
     def allow_duplicate_common_name(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_duplicate_common_name", value)
 
     @property
-    @pulumi.getter(name="autoApproveWarnings")
-    def auto_approve_warnings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        List of warnings to be automatically approved
-        """
-        return pulumi.get(self, "auto_approve_warnings")
-
-    @auto_approve_warnings.setter
-    def auto_approve_warnings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "auto_approve_warnings", value)
-
-    @property
     @pulumi.getter(name="certificateChainType")
     def certificate_chain_type(self) -> Optional[pulumi.Input[str]]:
         """
         Certificate trust chain type
         """
         return pulumi.get(self, "certificate_chain_type")
 
     @certificate_chain_type.setter
     def certificate_chain_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "certificate_chain_type", value)
 
     @property
-    @pulumi.getter(name="changeManagement")
-    def change_management(self) -> Optional[pulumi.Input[bool]]:
-        """
-        When set to false, the certificate will be deployed to both staging and production networks
-        """
-        return pulumi.get(self, "change_management")
-
-    @change_management.setter
-    def change_management(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "change_management", value)
-
-    @property
-    @pulumi.getter(name="excludeSans")
-    def exclude_sans(self) -> Optional[pulumi.Input[bool]]:
-        """
-        When true, SANs are excluded from the CSR
-        """
-        return pulumi.get(self, "exclude_sans")
-
-    @exclude_sans.setter
-    def exclude_sans(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "exclude_sans", value)
-
-    @property
     @pulumi.getter
     def sans(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of SANs
         """
         return pulumi.get(self, "sans")
 
     @sans.setter
     def sans(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "sans", value)
 
-    @property
-    @pulumi.getter(name="signatureAlgorithm")
-    def signature_algorithm(self) -> Optional[pulumi.Input[str]]:
-        """
-        The SHA function. Changing this value may require running terraform destroy, terraform apply
-        """
-        return pulumi.get(self, "signature_algorithm")
-
-    @signature_algorithm.setter
-    def signature_algorithm(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "signature_algorithm", value)
-
 
 @pulumi.input_type
-class _CpsThirdPartyEnrollmentState:
+class _CpsDvEnrollmentState:
     def __init__(__self__, *,
                  acknowledge_pre_verification_warnings: Optional[pulumi.Input[bool]] = None,
-                 admin_contact: Optional[pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs']] = None,
+                 admin_contact: Optional[pulumi.Input['CpsDvEnrollmentAdminContactArgs']] = None,
                  allow_duplicate_common_name: Optional[pulumi.Input[bool]] = None,
-                 auto_approve_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  certificate_chain_type: Optional[pulumi.Input[str]] = None,
-                 change_management: Optional[pulumi.Input[bool]] = None,
+                 certificate_type: Optional[pulumi.Input[str]] = None,
                  common_name: Optional[pulumi.Input[str]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
-                 csr: Optional[pulumi.Input['CpsThirdPartyEnrollmentCsrArgs']] = None,
-                 exclude_sans: Optional[pulumi.Input[bool]] = None,
-                 network_configuration: Optional[pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs']] = None,
-                 organization: Optional[pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs']] = None,
+                 csr: Optional[pulumi.Input['CpsDvEnrollmentCsrArgs']] = None,
+                 dns_challenges: Optional[pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentDnsChallengeArgs']]]] = None,
+                 http_challenges: Optional[pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentHttpChallengeArgs']]]] = None,
+                 network_configuration: Optional[pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs']] = None,
+                 organization: Optional[pulumi.Input['CpsDvEnrollmentOrganizationArgs']] = None,
+                 registration_authority: Optional[pulumi.Input[str]] = None,
                  sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  secure_network: Optional[pulumi.Input[str]] = None,
                  signature_algorithm: Optional[pulumi.Input[str]] = None,
                  sni_only: Optional[pulumi.Input[bool]] = None,
-                 tech_contact: Optional[pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs']] = None):
+                 tech_contact: Optional[pulumi.Input['CpsDvEnrollmentTechContactArgs']] = None,
+                 validation_type: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering CpsThirdPartyEnrollment resources.
+        Input properties used for looking up and filtering CpsDvEnrollment resources.
         :param pulumi.Input[bool] acknowledge_pre_verification_warnings: Whether acknowledge warnings before certificate verification
-        :param pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs'] admin_contact: Contact information for the certificate administrator to use at organization
+        :param pulumi.Input['CpsDvEnrollmentAdminContactArgs'] admin_contact: Contact information for the certificate administrator to use at organization
         :param pulumi.Input[bool] allow_duplicate_common_name: Allow to duplicate common name
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] auto_approve_warnings: List of warnings to be automatically approved
         :param pulumi.Input[str] certificate_chain_type: Certificate trust chain type
-        :param pulumi.Input[bool] change_management: When set to false, the certificate will be deployed to both staging and production networks
+        :param pulumi.Input[str] certificate_type: Certificate type of enrollment
         :param pulumi.Input[str] common_name: Common name used for enrollment
         :param pulumi.Input[str] contract_id: Contract ID for which enrollment is retrieved
-        :param pulumi.Input['CpsThirdPartyEnrollmentCsrArgs'] csr: Data used for generation of Certificate Signing Request
-        :param pulumi.Input[bool] exclude_sans: When true, SANs are excluded from the CSR
-        :param pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs'] network_configuration: Settings containing network information and TLS metadata used by CPS
-        :param pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs'] organization: Organization information
+        :param pulumi.Input['CpsDvEnrollmentCsrArgs'] csr: Certificate signing request generated during enrollment creation
+        :param pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentDnsChallengeArgs']]] dns_challenges: DNS challenge information
+        :param pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentHttpChallengeArgs']]] http_challenges: HTTP challenge information
+        :param pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs'] network_configuration: Settings containing network information and TLS Metadata used by CPS
+        :param pulumi.Input['CpsDvEnrollmentOrganizationArgs'] organization: Organization information
+        :param pulumi.Input[str] registration_authority: The registration authority or certificate authority (CA) used to obtain a certificate
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sans: List of SANs
         :param pulumi.Input[str] secure_network: Type of TLS deployment network
-        :param pulumi.Input[str] signature_algorithm: The SHA function. Changing this value may require running terraform destroy, terraform apply
+        :param pulumi.Input[str] signature_algorithm: SHA algorithm type
         :param pulumi.Input[bool] sni_only: Whether Server Name Indication is used for enrollment
-        :param pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs'] tech_contact: Contact information for an administrator at Akamai
+        :param pulumi.Input['CpsDvEnrollmentTechContactArgs'] tech_contact: Contact information for an administrator at Akamai
+        :param pulumi.Input[str] validation_type: Enrolment validation type
         """
         if acknowledge_pre_verification_warnings is not None:
             pulumi.set(__self__, "acknowledge_pre_verification_warnings", acknowledge_pre_verification_warnings)
         if admin_contact is not None:
             pulumi.set(__self__, "admin_contact", admin_contact)
         if allow_duplicate_common_name is not None:
             pulumi.set(__self__, "allow_duplicate_common_name", allow_duplicate_common_name)
-        if auto_approve_warnings is not None:
-            pulumi.set(__self__, "auto_approve_warnings", auto_approve_warnings)
         if certificate_chain_type is not None:
             pulumi.set(__self__, "certificate_chain_type", certificate_chain_type)
-        if change_management is not None:
-            pulumi.set(__self__, "change_management", change_management)
+        if certificate_type is not None:
+            pulumi.set(__self__, "certificate_type", certificate_type)
         if common_name is not None:
             pulumi.set(__self__, "common_name", common_name)
         if contract_id is not None:
             pulumi.set(__self__, "contract_id", contract_id)
         if csr is not None:
             pulumi.set(__self__, "csr", csr)
-        if exclude_sans is not None:
-            pulumi.set(__self__, "exclude_sans", exclude_sans)
+        if dns_challenges is not None:
+            pulumi.set(__self__, "dns_challenges", dns_challenges)
+        if http_challenges is not None:
+            pulumi.set(__self__, "http_challenges", http_challenges)
         if network_configuration is not None:
             pulumi.set(__self__, "network_configuration", network_configuration)
         if organization is not None:
             pulumi.set(__self__, "organization", organization)
+        if registration_authority is not None:
+            pulumi.set(__self__, "registration_authority", registration_authority)
         if sans is not None:
             pulumi.set(__self__, "sans", sans)
         if secure_network is not None:
             pulumi.set(__self__, "secure_network", secure_network)
         if signature_algorithm is not None:
             pulumi.set(__self__, "signature_algorithm", signature_algorithm)
         if sni_only is not None:
             pulumi.set(__self__, "sni_only", sni_only)
         if tech_contact is not None:
             pulumi.set(__self__, "tech_contact", tech_contact)
+        if validation_type is not None:
+            pulumi.set(__self__, "validation_type", validation_type)
 
     @property
     @pulumi.getter(name="acknowledgePreVerificationWarnings")
     def acknowledge_pre_verification_warnings(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether acknowledge warnings before certificate verification
         """
@@ -369,22 +328,22 @@
 
     @acknowledge_pre_verification_warnings.setter
     def acknowledge_pre_verification_warnings(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "acknowledge_pre_verification_warnings", value)
 
     @property
     @pulumi.getter(name="adminContact")
-    def admin_contact(self) -> Optional[pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs']]:
+    def admin_contact(self) -> Optional[pulumi.Input['CpsDvEnrollmentAdminContactArgs']]:
         """
         Contact information for the certificate administrator to use at organization
         """
         return pulumi.get(self, "admin_contact")
 
     @admin_contact.setter
-    def admin_contact(self, value: Optional[pulumi.Input['CpsThirdPartyEnrollmentAdminContactArgs']]):
+    def admin_contact(self, value: Optional[pulumi.Input['CpsDvEnrollmentAdminContactArgs']]):
         pulumi.set(self, "admin_contact", value)
 
     @property
     @pulumi.getter(name="allowDuplicateCommonName")
     def allow_duplicate_common_name(self) -> Optional[pulumi.Input[bool]]:
         """
         Allow to duplicate common name
@@ -392,48 +351,36 @@
         return pulumi.get(self, "allow_duplicate_common_name")
 
     @allow_duplicate_common_name.setter
     def allow_duplicate_common_name(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_duplicate_common_name", value)
 
     @property
-    @pulumi.getter(name="autoApproveWarnings")
-    def auto_approve_warnings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        List of warnings to be automatically approved
-        """
-        return pulumi.get(self, "auto_approve_warnings")
-
-    @auto_approve_warnings.setter
-    def auto_approve_warnings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "auto_approve_warnings", value)
-
-    @property
     @pulumi.getter(name="certificateChainType")
     def certificate_chain_type(self) -> Optional[pulumi.Input[str]]:
         """
         Certificate trust chain type
         """
         return pulumi.get(self, "certificate_chain_type")
 
     @certificate_chain_type.setter
     def certificate_chain_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "certificate_chain_type", value)
 
     @property
-    @pulumi.getter(name="changeManagement")
-    def change_management(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="certificateType")
+    def certificate_type(self) -> Optional[pulumi.Input[str]]:
         """
-        When set to false, the certificate will be deployed to both staging and production networks
+        Certificate type of enrollment
         """
-        return pulumi.get(self, "change_management")
+        return pulumi.get(self, "certificate_type")
 
-    @change_management.setter
-    def change_management(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "change_management", value)
+    @certificate_type.setter
+    def certificate_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "certificate_type", value)
 
     @property
     @pulumi.getter(name="commonName")
     def common_name(self) -> Optional[pulumi.Input[str]]:
         """
         Common name used for enrollment
         """
@@ -453,61 +400,85 @@
 
     @contract_id.setter
     def contract_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract_id", value)
 
     @property
     @pulumi.getter
-    def csr(self) -> Optional[pulumi.Input['CpsThirdPartyEnrollmentCsrArgs']]:
+    def csr(self) -> Optional[pulumi.Input['CpsDvEnrollmentCsrArgs']]:
         """
-        Data used for generation of Certificate Signing Request
+        Certificate signing request generated during enrollment creation
         """
         return pulumi.get(self, "csr")
 
     @csr.setter
-    def csr(self, value: Optional[pulumi.Input['CpsThirdPartyEnrollmentCsrArgs']]):
+    def csr(self, value: Optional[pulumi.Input['CpsDvEnrollmentCsrArgs']]):
         pulumi.set(self, "csr", value)
 
     @property
-    @pulumi.getter(name="excludeSans")
-    def exclude_sans(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="dnsChallenges")
+    def dns_challenges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentDnsChallengeArgs']]]]:
         """
-        When true, SANs are excluded from the CSR
+        DNS challenge information
         """
-        return pulumi.get(self, "exclude_sans")
+        return pulumi.get(self, "dns_challenges")
 
-    @exclude_sans.setter
-    def exclude_sans(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "exclude_sans", value)
+    @dns_challenges.setter
+    def dns_challenges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentDnsChallengeArgs']]]]):
+        pulumi.set(self, "dns_challenges", value)
+
+    @property
+    @pulumi.getter(name="httpChallenges")
+    def http_challenges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentHttpChallengeArgs']]]]:
+        """
+        HTTP challenge information
+        """
+        return pulumi.get(self, "http_challenges")
+
+    @http_challenges.setter
+    def http_challenges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CpsDvEnrollmentHttpChallengeArgs']]]]):
+        pulumi.set(self, "http_challenges", value)
 
     @property
     @pulumi.getter(name="networkConfiguration")
-    def network_configuration(self) -> Optional[pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs']]:
+    def network_configuration(self) -> Optional[pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs']]:
         """
-        Settings containing network information and TLS metadata used by CPS
+        Settings containing network information and TLS Metadata used by CPS
         """
         return pulumi.get(self, "network_configuration")
 
     @network_configuration.setter
-    def network_configuration(self, value: Optional[pulumi.Input['CpsThirdPartyEnrollmentNetworkConfigurationArgs']]):
+    def network_configuration(self, value: Optional[pulumi.Input['CpsDvEnrollmentNetworkConfigurationArgs']]):
         pulumi.set(self, "network_configuration", value)
 
     @property
     @pulumi.getter
-    def organization(self) -> Optional[pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs']]:
+    def organization(self) -> Optional[pulumi.Input['CpsDvEnrollmentOrganizationArgs']]:
         """
         Organization information
         """
         return pulumi.get(self, "organization")
 
     @organization.setter
-    def organization(self, value: Optional[pulumi.Input['CpsThirdPartyEnrollmentOrganizationArgs']]):
+    def organization(self, value: Optional[pulumi.Input['CpsDvEnrollmentOrganizationArgs']]):
         pulumi.set(self, "organization", value)
 
     @property
+    @pulumi.getter(name="registrationAuthority")
+    def registration_authority(self) -> Optional[pulumi.Input[str]]:
+        """
+        The registration authority or certificate authority (CA) used to obtain a certificate
+        """
+        return pulumi.get(self, "registration_authority")
+
+    @registration_authority.setter
+    def registration_authority(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "registration_authority", value)
+
+    @property
     @pulumi.getter
     def sans(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of SANs
         """
         return pulumi.get(self, "sans")
 
@@ -527,15 +498,15 @@
     def secure_network(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secure_network", value)
 
     @property
     @pulumi.getter(name="signatureAlgorithm")
     def signature_algorithm(self) -> Optional[pulumi.Input[str]]:
         """
-        The SHA function. Changing this value may require running terraform destroy, terraform apply
+        SHA algorithm type
         """
         return pulumi.get(self, "signature_algorithm")
 
     @signature_algorithm.setter
     def signature_algorithm(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signature_algorithm", value)
 
@@ -549,276 +520,281 @@
 
     @sni_only.setter
     def sni_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "sni_only", value)
 
     @property
     @pulumi.getter(name="techContact")
-    def tech_contact(self) -> Optional[pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs']]:
+    def tech_contact(self) -> Optional[pulumi.Input['CpsDvEnrollmentTechContactArgs']]:
         """
         Contact information for an administrator at Akamai
         """
         return pulumi.get(self, "tech_contact")
 
     @tech_contact.setter
-    def tech_contact(self, value: Optional[pulumi.Input['CpsThirdPartyEnrollmentTechContactArgs']]):
+    def tech_contact(self, value: Optional[pulumi.Input['CpsDvEnrollmentTechContactArgs']]):
         pulumi.set(self, "tech_contact", value)
 
+    @property
+    @pulumi.getter(name="validationType")
+    def validation_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Enrolment validation type
+        """
+        return pulumi.get(self, "validation_type")
 
-class CpsThirdPartyEnrollment(pulumi.CustomResource):
+    @validation_type.setter
+    def validation_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "validation_type", value)
+
+
+class CpsDvEnrollment(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  acknowledge_pre_verification_warnings: Optional[pulumi.Input[bool]] = None,
-                 admin_contact: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentAdminContactArgs']]] = None,
+                 admin_contact: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentAdminContactArgs']]] = None,
                  allow_duplicate_common_name: Optional[pulumi.Input[bool]] = None,
-                 auto_approve_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  certificate_chain_type: Optional[pulumi.Input[str]] = None,
-                 change_management: Optional[pulumi.Input[bool]] = None,
                  common_name: Optional[pulumi.Input[str]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
-                 csr: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentCsrArgs']]] = None,
-                 exclude_sans: Optional[pulumi.Input[bool]] = None,
-                 network_configuration: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentNetworkConfigurationArgs']]] = None,
-                 organization: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentOrganizationArgs']]] = None,
+                 csr: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentCsrArgs']]] = None,
+                 network_configuration: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentNetworkConfigurationArgs']]] = None,
+                 organization: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentOrganizationArgs']]] = None,
                  sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  secure_network: Optional[pulumi.Input[str]] = None,
                  signature_algorithm: Optional[pulumi.Input[str]] = None,
                  sni_only: Optional[pulumi.Input[bool]] = None,
-                 tech_contact: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentTechContactArgs']]] = None,
+                 tech_contact: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentTechContactArgs']]] = None,
                  __props__=None):
         """
-        Create a CpsThirdPartyEnrollment resource with the given unique name, props, and options.
+        Create a CpsDvEnrollment resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] acknowledge_pre_verification_warnings: Whether acknowledge warnings before certificate verification
-        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentAdminContactArgs']] admin_contact: Contact information for the certificate administrator to use at organization
+        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentAdminContactArgs']] admin_contact: Contact information for the certificate administrator to use at organization
         :param pulumi.Input[bool] allow_duplicate_common_name: Allow to duplicate common name
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] auto_approve_warnings: List of warnings to be automatically approved
         :param pulumi.Input[str] certificate_chain_type: Certificate trust chain type
-        :param pulumi.Input[bool] change_management: When set to false, the certificate will be deployed to both staging and production networks
         :param pulumi.Input[str] common_name: Common name used for enrollment
         :param pulumi.Input[str] contract_id: Contract ID for which enrollment is retrieved
-        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentCsrArgs']] csr: Data used for generation of Certificate Signing Request
-        :param pulumi.Input[bool] exclude_sans: When true, SANs are excluded from the CSR
-        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentNetworkConfigurationArgs']] network_configuration: Settings containing network information and TLS metadata used by CPS
-        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentOrganizationArgs']] organization: Organization information
+        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentCsrArgs']] csr: Certificate signing request generated during enrollment creation
+        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentNetworkConfigurationArgs']] network_configuration: Settings containing network information and TLS Metadata used by CPS
+        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentOrganizationArgs']] organization: Organization information
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sans: List of SANs
         :param pulumi.Input[str] secure_network: Type of TLS deployment network
-        :param pulumi.Input[str] signature_algorithm: The SHA function. Changing this value may require running terraform destroy, terraform apply
+        :param pulumi.Input[str] signature_algorithm: SHA algorithm type
         :param pulumi.Input[bool] sni_only: Whether Server Name Indication is used for enrollment
-        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentTechContactArgs']] tech_contact: Contact information for an administrator at Akamai
+        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentTechContactArgs']] tech_contact: Contact information for an administrator at Akamai
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: CpsThirdPartyEnrollmentArgs,
+                 args: CpsDvEnrollmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a CpsThirdPartyEnrollment resource with the given unique name, props, and options.
+        Create a CpsDvEnrollment resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param CpsThirdPartyEnrollmentArgs args: The arguments to use to populate this resource's properties.
+        :param CpsDvEnrollmentArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CpsThirdPartyEnrollmentArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(CpsDvEnrollmentArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  acknowledge_pre_verification_warnings: Optional[pulumi.Input[bool]] = None,
-                 admin_contact: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentAdminContactArgs']]] = None,
+                 admin_contact: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentAdminContactArgs']]] = None,
                  allow_duplicate_common_name: Optional[pulumi.Input[bool]] = None,
-                 auto_approve_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  certificate_chain_type: Optional[pulumi.Input[str]] = None,
-                 change_management: Optional[pulumi.Input[bool]] = None,
                  common_name: Optional[pulumi.Input[str]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
-                 csr: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentCsrArgs']]] = None,
-                 exclude_sans: Optional[pulumi.Input[bool]] = None,
-                 network_configuration: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentNetworkConfigurationArgs']]] = None,
-                 organization: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentOrganizationArgs']]] = None,
+                 csr: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentCsrArgs']]] = None,
+                 network_configuration: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentNetworkConfigurationArgs']]] = None,
+                 organization: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentOrganizationArgs']]] = None,
                  sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  secure_network: Optional[pulumi.Input[str]] = None,
                  signature_algorithm: Optional[pulumi.Input[str]] = None,
                  sni_only: Optional[pulumi.Input[bool]] = None,
-                 tech_contact: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentTechContactArgs']]] = None,
+                 tech_contact: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentTechContactArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CpsThirdPartyEnrollmentArgs.__new__(CpsThirdPartyEnrollmentArgs)
+            __props__ = CpsDvEnrollmentArgs.__new__(CpsDvEnrollmentArgs)
 
             __props__.__dict__["acknowledge_pre_verification_warnings"] = acknowledge_pre_verification_warnings
             if admin_contact is None and not opts.urn:
                 raise TypeError("Missing required property 'admin_contact'")
             __props__.__dict__["admin_contact"] = admin_contact
             __props__.__dict__["allow_duplicate_common_name"] = allow_duplicate_common_name
-            __props__.__dict__["auto_approve_warnings"] = auto_approve_warnings
             __props__.__dict__["certificate_chain_type"] = certificate_chain_type
-            __props__.__dict__["change_management"] = change_management
             if common_name is None and not opts.urn:
                 raise TypeError("Missing required property 'common_name'")
             __props__.__dict__["common_name"] = common_name
             if contract_id is None and not opts.urn:
                 raise TypeError("Missing required property 'contract_id'")
             __props__.__dict__["contract_id"] = contract_id
             if csr is None and not opts.urn:
                 raise TypeError("Missing required property 'csr'")
             __props__.__dict__["csr"] = csr
-            __props__.__dict__["exclude_sans"] = exclude_sans
             if network_configuration is None and not opts.urn:
                 raise TypeError("Missing required property 'network_configuration'")
             __props__.__dict__["network_configuration"] = network_configuration
             if organization is None and not opts.urn:
                 raise TypeError("Missing required property 'organization'")
             __props__.__dict__["organization"] = organization
             __props__.__dict__["sans"] = sans
             if secure_network is None and not opts.urn:
                 raise TypeError("Missing required property 'secure_network'")
             __props__.__dict__["secure_network"] = secure_network
+            if signature_algorithm is None and not opts.urn:
+                raise TypeError("Missing required property 'signature_algorithm'")
             __props__.__dict__["signature_algorithm"] = signature_algorithm
             if sni_only is None and not opts.urn:
                 raise TypeError("Missing required property 'sni_only'")
             __props__.__dict__["sni_only"] = sni_only
             if tech_contact is None and not opts.urn:
                 raise TypeError("Missing required property 'tech_contact'")
             __props__.__dict__["tech_contact"] = tech_contact
-        super(CpsThirdPartyEnrollment, __self__).__init__(
-            'akamai:index/cpsThirdPartyEnrollment:CpsThirdPartyEnrollment',
+            __props__.__dict__["certificate_type"] = None
+            __props__.__dict__["dns_challenges"] = None
+            __props__.__dict__["http_challenges"] = None
+            __props__.__dict__["registration_authority"] = None
+            __props__.__dict__["validation_type"] = None
+        super(CpsDvEnrollment, __self__).__init__(
+            'akamai:index/cpsDvEnrollment:CpsDvEnrollment',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             acknowledge_pre_verification_warnings: Optional[pulumi.Input[bool]] = None,
-            admin_contact: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentAdminContactArgs']]] = None,
+            admin_contact: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentAdminContactArgs']]] = None,
             allow_duplicate_common_name: Optional[pulumi.Input[bool]] = None,
-            auto_approve_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             certificate_chain_type: Optional[pulumi.Input[str]] = None,
-            change_management: Optional[pulumi.Input[bool]] = None,
+            certificate_type: Optional[pulumi.Input[str]] = None,
             common_name: Optional[pulumi.Input[str]] = None,
             contract_id: Optional[pulumi.Input[str]] = None,
-            csr: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentCsrArgs']]] = None,
-            exclude_sans: Optional[pulumi.Input[bool]] = None,
-            network_configuration: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentNetworkConfigurationArgs']]] = None,
-            organization: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentOrganizationArgs']]] = None,
+            csr: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentCsrArgs']]] = None,
+            dns_challenges: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CpsDvEnrollmentDnsChallengeArgs']]]]] = None,
+            http_challenges: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CpsDvEnrollmentHttpChallengeArgs']]]]] = None,
+            network_configuration: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentNetworkConfigurationArgs']]] = None,
+            organization: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentOrganizationArgs']]] = None,
+            registration_authority: Optional[pulumi.Input[str]] = None,
             sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             secure_network: Optional[pulumi.Input[str]] = None,
             signature_algorithm: Optional[pulumi.Input[str]] = None,
             sni_only: Optional[pulumi.Input[bool]] = None,
-            tech_contact: Optional[pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentTechContactArgs']]] = None) -> 'CpsThirdPartyEnrollment':
+            tech_contact: Optional[pulumi.Input[pulumi.InputType['CpsDvEnrollmentTechContactArgs']]] = None,
+            validation_type: Optional[pulumi.Input[str]] = None) -> 'CpsDvEnrollment':
         """
-        Get an existing CpsThirdPartyEnrollment resource's state with the given name, id, and optional extra
+        Get an existing CpsDvEnrollment resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] acknowledge_pre_verification_warnings: Whether acknowledge warnings before certificate verification
-        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentAdminContactArgs']] admin_contact: Contact information for the certificate administrator to use at organization
+        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentAdminContactArgs']] admin_contact: Contact information for the certificate administrator to use at organization
         :param pulumi.Input[bool] allow_duplicate_common_name: Allow to duplicate common name
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] auto_approve_warnings: List of warnings to be automatically approved
         :param pulumi.Input[str] certificate_chain_type: Certificate trust chain type
-        :param pulumi.Input[bool] change_management: When set to false, the certificate will be deployed to both staging and production networks
+        :param pulumi.Input[str] certificate_type: Certificate type of enrollment
         :param pulumi.Input[str] common_name: Common name used for enrollment
         :param pulumi.Input[str] contract_id: Contract ID for which enrollment is retrieved
-        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentCsrArgs']] csr: Data used for generation of Certificate Signing Request
-        :param pulumi.Input[bool] exclude_sans: When true, SANs are excluded from the CSR
-        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentNetworkConfigurationArgs']] network_configuration: Settings containing network information and TLS metadata used by CPS
-        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentOrganizationArgs']] organization: Organization information
+        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentCsrArgs']] csr: Certificate signing request generated during enrollment creation
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CpsDvEnrollmentDnsChallengeArgs']]]] dns_challenges: DNS challenge information
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CpsDvEnrollmentHttpChallengeArgs']]]] http_challenges: HTTP challenge information
+        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentNetworkConfigurationArgs']] network_configuration: Settings containing network information and TLS Metadata used by CPS
+        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentOrganizationArgs']] organization: Organization information
+        :param pulumi.Input[str] registration_authority: The registration authority or certificate authority (CA) used to obtain a certificate
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sans: List of SANs
         :param pulumi.Input[str] secure_network: Type of TLS deployment network
-        :param pulumi.Input[str] signature_algorithm: The SHA function. Changing this value may require running terraform destroy, terraform apply
+        :param pulumi.Input[str] signature_algorithm: SHA algorithm type
         :param pulumi.Input[bool] sni_only: Whether Server Name Indication is used for enrollment
-        :param pulumi.Input[pulumi.InputType['CpsThirdPartyEnrollmentTechContactArgs']] tech_contact: Contact information for an administrator at Akamai
+        :param pulumi.Input[pulumi.InputType['CpsDvEnrollmentTechContactArgs']] tech_contact: Contact information for an administrator at Akamai
+        :param pulumi.Input[str] validation_type: Enrolment validation type
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _CpsThirdPartyEnrollmentState.__new__(_CpsThirdPartyEnrollmentState)
+        __props__ = _CpsDvEnrollmentState.__new__(_CpsDvEnrollmentState)
 
         __props__.__dict__["acknowledge_pre_verification_warnings"] = acknowledge_pre_verification_warnings
         __props__.__dict__["admin_contact"] = admin_contact
         __props__.__dict__["allow_duplicate_common_name"] = allow_duplicate_common_name
-        __props__.__dict__["auto_approve_warnings"] = auto_approve_warnings
         __props__.__dict__["certificate_chain_type"] = certificate_chain_type
-        __props__.__dict__["change_management"] = change_management
+        __props__.__dict__["certificate_type"] = certificate_type
         __props__.__dict__["common_name"] = common_name
         __props__.__dict__["contract_id"] = contract_id
         __props__.__dict__["csr"] = csr
-        __props__.__dict__["exclude_sans"] = exclude_sans
+        __props__.__dict__["dns_challenges"] = dns_challenges
+        __props__.__dict__["http_challenges"] = http_challenges
         __props__.__dict__["network_configuration"] = network_configuration
         __props__.__dict__["organization"] = organization
+        __props__.__dict__["registration_authority"] = registration_authority
         __props__.__dict__["sans"] = sans
         __props__.__dict__["secure_network"] = secure_network
         __props__.__dict__["signature_algorithm"] = signature_algorithm
         __props__.__dict__["sni_only"] = sni_only
         __props__.__dict__["tech_contact"] = tech_contact
-        return CpsThirdPartyEnrollment(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["validation_type"] = validation_type
+        return CpsDvEnrollment(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="acknowledgePreVerificationWarnings")
     def acknowledge_pre_verification_warnings(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether acknowledge warnings before certificate verification
         """
         return pulumi.get(self, "acknowledge_pre_verification_warnings")
 
     @property
     @pulumi.getter(name="adminContact")
-    def admin_contact(self) -> pulumi.Output['outputs.CpsThirdPartyEnrollmentAdminContact']:
+    def admin_contact(self) -> pulumi.Output['outputs.CpsDvEnrollmentAdminContact']:
         """
         Contact information for the certificate administrator to use at organization
         """
         return pulumi.get(self, "admin_contact")
 
     @property
     @pulumi.getter(name="allowDuplicateCommonName")
     def allow_duplicate_common_name(self) -> pulumi.Output[Optional[bool]]:
         """
         Allow to duplicate common name
         """
         return pulumi.get(self, "allow_duplicate_common_name")
 
     @property
-    @pulumi.getter(name="autoApproveWarnings")
-    def auto_approve_warnings(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        """
-        List of warnings to be automatically approved
-        """
-        return pulumi.get(self, "auto_approve_warnings")
-
-    @property
     @pulumi.getter(name="certificateChainType")
     def certificate_chain_type(self) -> pulumi.Output[Optional[str]]:
         """
         Certificate trust chain type
         """
         return pulumi.get(self, "certificate_chain_type")
 
     @property
-    @pulumi.getter(name="changeManagement")
-    def change_management(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="certificateType")
+    def certificate_type(self) -> pulumi.Output[str]:
         """
-        When set to false, the certificate will be deployed to both staging and production networks
+        Certificate type of enrollment
         """
-        return pulumi.get(self, "change_management")
+        return pulumi.get(self, "certificate_type")
 
     @property
     @pulumi.getter(name="commonName")
     def common_name(self) -> pulumi.Output[str]:
         """
         Common name used for enrollment
         """
@@ -830,45 +806,61 @@
         """
         Contract ID for which enrollment is retrieved
         """
         return pulumi.get(self, "contract_id")
 
     @property
     @pulumi.getter
-    def csr(self) -> pulumi.Output['outputs.CpsThirdPartyEnrollmentCsr']:
+    def csr(self) -> pulumi.Output['outputs.CpsDvEnrollmentCsr']:
         """
-        Data used for generation of Certificate Signing Request
+        Certificate signing request generated during enrollment creation
         """
         return pulumi.get(self, "csr")
 
     @property
-    @pulumi.getter(name="excludeSans")
-    def exclude_sans(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="dnsChallenges")
+    def dns_challenges(self) -> pulumi.Output[Sequence['outputs.CpsDvEnrollmentDnsChallenge']]:
+        """
+        DNS challenge information
+        """
+        return pulumi.get(self, "dns_challenges")
+
+    @property
+    @pulumi.getter(name="httpChallenges")
+    def http_challenges(self) -> pulumi.Output[Sequence['outputs.CpsDvEnrollmentHttpChallenge']]:
         """
-        When true, SANs are excluded from the CSR
+        HTTP challenge information
         """
-        return pulumi.get(self, "exclude_sans")
+        return pulumi.get(self, "http_challenges")
 
     @property
     @pulumi.getter(name="networkConfiguration")
-    def network_configuration(self) -> pulumi.Output['outputs.CpsThirdPartyEnrollmentNetworkConfiguration']:
+    def network_configuration(self) -> pulumi.Output['outputs.CpsDvEnrollmentNetworkConfiguration']:
         """
-        Settings containing network information and TLS metadata used by CPS
+        Settings containing network information and TLS Metadata used by CPS
         """
         return pulumi.get(self, "network_configuration")
 
     @property
     @pulumi.getter
-    def organization(self) -> pulumi.Output['outputs.CpsThirdPartyEnrollmentOrganization']:
+    def organization(self) -> pulumi.Output['outputs.CpsDvEnrollmentOrganization']:
         """
         Organization information
         """
         return pulumi.get(self, "organization")
 
     @property
+    @pulumi.getter(name="registrationAuthority")
+    def registration_authority(self) -> pulumi.Output[str]:
+        """
+        The registration authority or certificate authority (CA) used to obtain a certificate
+        """
+        return pulumi.get(self, "registration_authority")
+
+    @property
     @pulumi.getter
     def sans(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         List of SANs
         """
         return pulumi.get(self, "sans")
 
@@ -878,29 +870,37 @@
         """
         Type of TLS deployment network
         """
         return pulumi.get(self, "secure_network")
 
     @property
     @pulumi.getter(name="signatureAlgorithm")
-    def signature_algorithm(self) -> pulumi.Output[Optional[str]]:
+    def signature_algorithm(self) -> pulumi.Output[str]:
         """
-        The SHA function. Changing this value may require running terraform destroy, terraform apply
+        SHA algorithm type
         """
         return pulumi.get(self, "signature_algorithm")
 
     @property
     @pulumi.getter(name="sniOnly")
     def sni_only(self) -> pulumi.Output[bool]:
         """
         Whether Server Name Indication is used for enrollment
         """
         return pulumi.get(self, "sni_only")
 
     @property
     @pulumi.getter(name="techContact")
-    def tech_contact(self) -> pulumi.Output['outputs.CpsThirdPartyEnrollmentTechContact']:
+    def tech_contact(self) -> pulumi.Output['outputs.CpsDvEnrollmentTechContact']:
         """
         Contact information for an administrator at Akamai
         """
         return pulumi.get(self, "tech_contact")
 
+    @property
+    @pulumi.getter(name="validationType")
+    def validation_type(self) -> pulumi.Output[str]:
+        """
+        Enrolment validation type
+        """
+        return pulumi.get(self, "validation_type")
+
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/cps_upload_certificate.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/cps_upload_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/datastream.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/datastream.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,73 +13,71 @@
 
 __all__ = ['DatastreamArgs', 'Datastream']
 
 @pulumi.input_type
 class DatastreamArgs:
     def __init__(__self__, *,
                  active: pulumi.Input[bool],
-                 config: pulumi.Input['DatastreamConfigArgs'],
                  contract_id: pulumi.Input[str],
-                 dataset_fields_ids: pulumi.Input[Sequence[pulumi.Input[int]]],
+                 dataset_fields: pulumi.Input[Sequence[pulumi.Input[int]]],
+                 delivery_configuration: pulumi.Input['DatastreamDeliveryConfigurationArgs'],
                  group_id: pulumi.Input[str],
-                 property_ids: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 properties: pulumi.Input[Sequence[pulumi.Input[str]]],
                  stream_name: pulumi.Input[str],
-                 stream_type: pulumi.Input[str],
-                 template_name: pulumi.Input[str],
                  azure_connector: Optional[pulumi.Input['DatastreamAzureConnectorArgs']] = None,
+                 collect_midgress: Optional[pulumi.Input[bool]] = None,
                  datadog_connector: Optional[pulumi.Input['DatastreamDatadogConnectorArgs']] = None,
                  elasticsearch_connector: Optional[pulumi.Input['DatastreamElasticsearchConnectorArgs']] = None,
-                 email_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  gcs_connector: Optional[pulumi.Input['DatastreamGcsConnectorArgs']] = None,
                  https_connector: Optional[pulumi.Input['DatastreamHttpsConnectorArgs']] = None,
                  loggly_connector: Optional[pulumi.Input['DatastreamLogglyConnectorArgs']] = None,
                  new_relic_connector: Optional[pulumi.Input['DatastreamNewRelicConnectorArgs']] = None,
+                 notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  oracle_connector: Optional[pulumi.Input['DatastreamOracleConnectorArgs']] = None,
                  s3_connector: Optional[pulumi.Input['DatastreamS3ConnectorArgs']] = None,
                  splunk_connector: Optional[pulumi.Input['DatastreamSplunkConnectorArgs']] = None,
                  sumologic_connector: Optional[pulumi.Input['DatastreamSumologicConnectorArgs']] = None):
         """
         The set of arguments for constructing a Datastream resource.
         :param pulumi.Input[bool] active: Defining if stream should be active or not
-        :param pulumi.Input['DatastreamConfigArgs'] config: Provides information about the configuration related to logs (format, file names, delivery frequency)
         :param pulumi.Input[str] contract_id: Identifies the contract that has access to the product
-        :param pulumi.Input[Sequence[pulumi.Input[int]]] dataset_fields_ids: A list of data set fields selected from the associated template that the stream monitors in logs. The order of the
+        :param pulumi.Input[Sequence[pulumi.Input[int]]] dataset_fields: A list of data set fields selected from the associated template that the stream monitors in logs. The order of the
                identifiers define how the value for these fields appear in the log lines
+        :param pulumi.Input['DatastreamDeliveryConfigurationArgs'] delivery_configuration: Provides information about the configuration related to logs (format, file names, delivery frequency)
         :param pulumi.Input[str] group_id: Identifies the group that has access to the product and for which the stream configuration was created
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] property_ids: Identifies the properties monitored in the stream
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] properties: Identifies the properties monitored in the stream
         :param pulumi.Input[str] stream_name: The name of the stream
-        :param pulumi.Input[str] stream_type: Specifies the type of the data stream
-        :param pulumi.Input[str] template_name: The name of the template associated with the stream
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] email_ids: List of email addresses where the system sends notifications about activations and deactivations of the stream
+        :param pulumi.Input[bool] collect_midgress: Identifies if stream needs to collect midgress data
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_emails: List of email addresses where the system sends notifications about activations and deactivations of the stream
         """
         pulumi.set(__self__, "active", active)
-        pulumi.set(__self__, "config", config)
         pulumi.set(__self__, "contract_id", contract_id)
-        pulumi.set(__self__, "dataset_fields_ids", dataset_fields_ids)
+        pulumi.set(__self__, "dataset_fields", dataset_fields)
+        pulumi.set(__self__, "delivery_configuration", delivery_configuration)
         pulumi.set(__self__, "group_id", group_id)
-        pulumi.set(__self__, "property_ids", property_ids)
+        pulumi.set(__self__, "properties", properties)
         pulumi.set(__self__, "stream_name", stream_name)
-        pulumi.set(__self__, "stream_type", stream_type)
-        pulumi.set(__self__, "template_name", template_name)
         if azure_connector is not None:
             pulumi.set(__self__, "azure_connector", azure_connector)
+        if collect_midgress is not None:
+            pulumi.set(__self__, "collect_midgress", collect_midgress)
         if datadog_connector is not None:
             pulumi.set(__self__, "datadog_connector", datadog_connector)
         if elasticsearch_connector is not None:
             pulumi.set(__self__, "elasticsearch_connector", elasticsearch_connector)
-        if email_ids is not None:
-            pulumi.set(__self__, "email_ids", email_ids)
         if gcs_connector is not None:
             pulumi.set(__self__, "gcs_connector", gcs_connector)
         if https_connector is not None:
             pulumi.set(__self__, "https_connector", https_connector)
         if loggly_connector is not None:
             pulumi.set(__self__, "loggly_connector", loggly_connector)
         if new_relic_connector is not None:
             pulumi.set(__self__, "new_relic_connector", new_relic_connector)
+        if notification_emails is not None:
+            pulumi.set(__self__, "notification_emails", notification_emails)
         if oracle_connector is not None:
             pulumi.set(__self__, "oracle_connector", oracle_connector)
         if s3_connector is not None:
             pulumi.set(__self__, "s3_connector", s3_connector)
         if splunk_connector is not None:
             pulumi.set(__self__, "splunk_connector", splunk_connector)
         if sumologic_connector is not None:
@@ -94,120 +92,108 @@
         return pulumi.get(self, "active")
 
     @active.setter
     def active(self, value: pulumi.Input[bool]):
         pulumi.set(self, "active", value)
 
     @property
-    @pulumi.getter
-    def config(self) -> pulumi.Input['DatastreamConfigArgs']:
-        """
-        Provides information about the configuration related to logs (format, file names, delivery frequency)
-        """
-        return pulumi.get(self, "config")
-
-    @config.setter
-    def config(self, value: pulumi.Input['DatastreamConfigArgs']):
-        pulumi.set(self, "config", value)
-
-    @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> pulumi.Input[str]:
         """
         Identifies the contract that has access to the product
         """
         return pulumi.get(self, "contract_id")
 
     @contract_id.setter
     def contract_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "contract_id", value)
 
     @property
-    @pulumi.getter(name="datasetFieldsIds")
-    def dataset_fields_ids(self) -> pulumi.Input[Sequence[pulumi.Input[int]]]:
+    @pulumi.getter(name="datasetFields")
+    def dataset_fields(self) -> pulumi.Input[Sequence[pulumi.Input[int]]]:
         """
         A list of data set fields selected from the associated template that the stream monitors in logs. The order of the
         identifiers define how the value for these fields appear in the log lines
         """
-        return pulumi.get(self, "dataset_fields_ids")
+        return pulumi.get(self, "dataset_fields")
+
+    @dataset_fields.setter
+    def dataset_fields(self, value: pulumi.Input[Sequence[pulumi.Input[int]]]):
+        pulumi.set(self, "dataset_fields", value)
+
+    @property
+    @pulumi.getter(name="deliveryConfiguration")
+    def delivery_configuration(self) -> pulumi.Input['DatastreamDeliveryConfigurationArgs']:
+        """
+        Provides information about the configuration related to logs (format, file names, delivery frequency)
+        """
+        return pulumi.get(self, "delivery_configuration")
 
-    @dataset_fields_ids.setter
-    def dataset_fields_ids(self, value: pulumi.Input[Sequence[pulumi.Input[int]]]):
-        pulumi.set(self, "dataset_fields_ids", value)
+    @delivery_configuration.setter
+    def delivery_configuration(self, value: pulumi.Input['DatastreamDeliveryConfigurationArgs']):
+        pulumi.set(self, "delivery_configuration", value)
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> pulumi.Input[str]:
         """
         Identifies the group that has access to the product and for which the stream configuration was created
         """
         return pulumi.get(self, "group_id")
 
     @group_id.setter
     def group_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "group_id", value)
 
     @property
-    @pulumi.getter(name="propertyIds")
-    def property_ids(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+    @pulumi.getter
+    def properties(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
         Identifies the properties monitored in the stream
         """
-        return pulumi.get(self, "property_ids")
+        return pulumi.get(self, "properties")
 
-    @property_ids.setter
-    def property_ids(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "property_ids", value)
+    @properties.setter
+    def properties(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "properties", value)
 
     @property
     @pulumi.getter(name="streamName")
     def stream_name(self) -> pulumi.Input[str]:
         """
         The name of the stream
         """
         return pulumi.get(self, "stream_name")
 
     @stream_name.setter
     def stream_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "stream_name", value)
 
     @property
-    @pulumi.getter(name="streamType")
-    def stream_type(self) -> pulumi.Input[str]:
-        """
-        Specifies the type of the data stream
-        """
-        return pulumi.get(self, "stream_type")
-
-    @stream_type.setter
-    def stream_type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "stream_type", value)
-
-    @property
-    @pulumi.getter(name="templateName")
-    def template_name(self) -> pulumi.Input[str]:
-        """
-        The name of the template associated with the stream
-        """
-        return pulumi.get(self, "template_name")
-
-    @template_name.setter
-    def template_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "template_name", value)
-
-    @property
     @pulumi.getter(name="azureConnector")
     def azure_connector(self) -> Optional[pulumi.Input['DatastreamAzureConnectorArgs']]:
         return pulumi.get(self, "azure_connector")
 
     @azure_connector.setter
     def azure_connector(self, value: Optional[pulumi.Input['DatastreamAzureConnectorArgs']]):
         pulumi.set(self, "azure_connector", value)
 
     @property
+    @pulumi.getter(name="collectMidgress")
+    def collect_midgress(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Identifies if stream needs to collect midgress data
+        """
+        return pulumi.get(self, "collect_midgress")
+
+    @collect_midgress.setter
+    def collect_midgress(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "collect_midgress", value)
+
+    @property
     @pulumi.getter(name="datadogConnector")
     def datadog_connector(self) -> Optional[pulumi.Input['DatastreamDatadogConnectorArgs']]:
         return pulumi.get(self, "datadog_connector")
 
     @datadog_connector.setter
     def datadog_connector(self, value: Optional[pulumi.Input['DatastreamDatadogConnectorArgs']]):
         pulumi.set(self, "datadog_connector", value)
@@ -218,26 +204,14 @@
         return pulumi.get(self, "elasticsearch_connector")
 
     @elasticsearch_connector.setter
     def elasticsearch_connector(self, value: Optional[pulumi.Input['DatastreamElasticsearchConnectorArgs']]):
         pulumi.set(self, "elasticsearch_connector", value)
 
     @property
-    @pulumi.getter(name="emailIds")
-    def email_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        List of email addresses where the system sends notifications about activations and deactivations of the stream
-        """
-        return pulumi.get(self, "email_ids")
-
-    @email_ids.setter
-    def email_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "email_ids", value)
-
-    @property
     @pulumi.getter(name="gcsConnector")
     def gcs_connector(self) -> Optional[pulumi.Input['DatastreamGcsConnectorArgs']]:
         return pulumi.get(self, "gcs_connector")
 
     @gcs_connector.setter
     def gcs_connector(self, value: Optional[pulumi.Input['DatastreamGcsConnectorArgs']]):
         pulumi.set(self, "gcs_connector", value)
@@ -266,14 +240,26 @@
         return pulumi.get(self, "new_relic_connector")
 
     @new_relic_connector.setter
     def new_relic_connector(self, value: Optional[pulumi.Input['DatastreamNewRelicConnectorArgs']]):
         pulumi.set(self, "new_relic_connector", value)
 
     @property
+    @pulumi.getter(name="notificationEmails")
+    def notification_emails(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of email addresses where the system sends notifications about activations and deactivations of the stream
+        """
+        return pulumi.get(self, "notification_emails")
+
+    @notification_emails.setter
+    def notification_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "notification_emails", value)
+
+    @property
     @pulumi.getter(name="oracleConnector")
     def oracle_connector(self) -> Optional[pulumi.Input['DatastreamOracleConnectorArgs']]:
         return pulumi.get(self, "oracle_connector")
 
     @oracle_connector.setter
     def oracle_connector(self, value: Optional[pulumi.Input['DatastreamOracleConnectorArgs']]):
         pulumi.set(self, "oracle_connector", value)
@@ -307,125 +293,117 @@
 
 
 @pulumi.input_type
 class _DatastreamState:
     def __init__(__self__, *,
                  active: Optional[pulumi.Input[bool]] = None,
                  azure_connector: Optional[pulumi.Input['DatastreamAzureConnectorArgs']] = None,
-                 config: Optional[pulumi.Input['DatastreamConfigArgs']] = None,
+                 collect_midgress: Optional[pulumi.Input[bool]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
                  created_by: Optional[pulumi.Input[str]] = None,
                  created_date: Optional[pulumi.Input[str]] = None,
                  datadog_connector: Optional[pulumi.Input['DatastreamDatadogConnectorArgs']] = None,
-                 dataset_fields_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+                 dataset_fields: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+                 delivery_configuration: Optional[pulumi.Input['DatastreamDeliveryConfigurationArgs']] = None,
                  elasticsearch_connector: Optional[pulumi.Input['DatastreamElasticsearchConnectorArgs']] = None,
-                 email_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  gcs_connector: Optional[pulumi.Input['DatastreamGcsConnectorArgs']] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
-                 group_name: Optional[pulumi.Input[str]] = None,
                  https_connector: Optional[pulumi.Input['DatastreamHttpsConnectorArgs']] = None,
+                 latest_version: Optional[pulumi.Input[int]] = None,
                  loggly_connector: Optional[pulumi.Input['DatastreamLogglyConnectorArgs']] = None,
                  modified_by: Optional[pulumi.Input[str]] = None,
                  modified_date: Optional[pulumi.Input[str]] = None,
                  new_relic_connector: Optional[pulumi.Input['DatastreamNewRelicConnectorArgs']] = None,
+                 notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  oracle_connector: Optional[pulumi.Input['DatastreamOracleConnectorArgs']] = None,
                  papi_json: Optional[pulumi.Input[str]] = None,
                  product_id: Optional[pulumi.Input[str]] = None,
-                 product_name: Optional[pulumi.Input[str]] = None,
-                 property_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  s3_connector: Optional[pulumi.Input['DatastreamS3ConnectorArgs']] = None,
                  splunk_connector: Optional[pulumi.Input['DatastreamSplunkConnectorArgs']] = None,
                  stream_name: Optional[pulumi.Input[str]] = None,
-                 stream_type: Optional[pulumi.Input[str]] = None,
-                 stream_version_id: Optional[pulumi.Input[int]] = None,
-                 sumologic_connector: Optional[pulumi.Input['DatastreamSumologicConnectorArgs']] = None,
-                 template_name: Optional[pulumi.Input[str]] = None):
+                 stream_version: Optional[pulumi.Input[int]] = None,
+                 sumologic_connector: Optional[pulumi.Input['DatastreamSumologicConnectorArgs']] = None):
         """
         Input properties used for looking up and filtering Datastream resources.
         :param pulumi.Input[bool] active: Defining if stream should be active or not
-        :param pulumi.Input['DatastreamConfigArgs'] config: Provides information about the configuration related to logs (format, file names, delivery frequency)
+        :param pulumi.Input[bool] collect_midgress: Identifies if stream needs to collect midgress data
         :param pulumi.Input[str] contract_id: Identifies the contract that has access to the product
         :param pulumi.Input[str] created_by: The username who created the stream
         :param pulumi.Input[str] created_date: The date and time when the stream was created
-        :param pulumi.Input[Sequence[pulumi.Input[int]]] dataset_fields_ids: A list of data set fields selected from the associated template that the stream monitors in logs. The order of the
+        :param pulumi.Input[Sequence[pulumi.Input[int]]] dataset_fields: A list of data set fields selected from the associated template that the stream monitors in logs. The order of the
                identifiers define how the value for these fields appear in the log lines
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] email_ids: List of email addresses where the system sends notifications about activations and deactivations of the stream
+        :param pulumi.Input['DatastreamDeliveryConfigurationArgs'] delivery_configuration: Provides information about the configuration related to logs (format, file names, delivery frequency)
         :param pulumi.Input[str] group_id: Identifies the group that has access to the product and for which the stream configuration was created
-        :param pulumi.Input[str] group_name: The name of the user group for which the stream was created
+        :param pulumi.Input[int] latest_version: Identifies the latest active configuration version of the stream
         :param pulumi.Input[str] modified_by: The username who modified the stream
         :param pulumi.Input[str] modified_date: The date and time when the stream was modified
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_emails: List of email addresses where the system sends notifications about activations and deactivations of the stream
         :param pulumi.Input[str] papi_json: The configuration in JSON format that can be copy-pasted into PAPI configuration to enable datastream behavior
         :param pulumi.Input[str] product_id: The ID of the product for which the stream was created
-        :param pulumi.Input[str] product_name: The name of the product for which the stream was created
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] property_ids: Identifies the properties monitored in the stream
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] properties: Identifies the properties monitored in the stream
         :param pulumi.Input[str] stream_name: The name of the stream
-        :param pulumi.Input[str] stream_type: Specifies the type of the data stream
-        :param pulumi.Input[int] stream_version_id: Identifies the configuration version of the stream
-        :param pulumi.Input[str] template_name: The name of the template associated with the stream
+        :param pulumi.Input[int] stream_version: Identifies the configuration version of the stream
         """
         if active is not None:
             pulumi.set(__self__, "active", active)
         if azure_connector is not None:
             pulumi.set(__self__, "azure_connector", azure_connector)
-        if config is not None:
-            pulumi.set(__self__, "config", config)
+        if collect_midgress is not None:
+            pulumi.set(__self__, "collect_midgress", collect_midgress)
         if contract_id is not None:
             pulumi.set(__self__, "contract_id", contract_id)
         if created_by is not None:
             pulumi.set(__self__, "created_by", created_by)
         if created_date is not None:
             pulumi.set(__self__, "created_date", created_date)
         if datadog_connector is not None:
             pulumi.set(__self__, "datadog_connector", datadog_connector)
-        if dataset_fields_ids is not None:
-            pulumi.set(__self__, "dataset_fields_ids", dataset_fields_ids)
+        if dataset_fields is not None:
+            pulumi.set(__self__, "dataset_fields", dataset_fields)
+        if delivery_configuration is not None:
+            pulumi.set(__self__, "delivery_configuration", delivery_configuration)
         if elasticsearch_connector is not None:
             pulumi.set(__self__, "elasticsearch_connector", elasticsearch_connector)
-        if email_ids is not None:
-            pulumi.set(__self__, "email_ids", email_ids)
         if gcs_connector is not None:
             pulumi.set(__self__, "gcs_connector", gcs_connector)
         if group_id is not None:
             pulumi.set(__self__, "group_id", group_id)
-        if group_name is not None:
-            pulumi.set(__self__, "group_name", group_name)
         if https_connector is not None:
             pulumi.set(__self__, "https_connector", https_connector)
+        if latest_version is not None:
+            pulumi.set(__self__, "latest_version", latest_version)
         if loggly_connector is not None:
             pulumi.set(__self__, "loggly_connector", loggly_connector)
         if modified_by is not None:
             pulumi.set(__self__, "modified_by", modified_by)
         if modified_date is not None:
             pulumi.set(__self__, "modified_date", modified_date)
         if new_relic_connector is not None:
             pulumi.set(__self__, "new_relic_connector", new_relic_connector)
+        if notification_emails is not None:
+            pulumi.set(__self__, "notification_emails", notification_emails)
         if oracle_connector is not None:
             pulumi.set(__self__, "oracle_connector", oracle_connector)
         if papi_json is not None:
             pulumi.set(__self__, "papi_json", papi_json)
         if product_id is not None:
             pulumi.set(__self__, "product_id", product_id)
-        if product_name is not None:
-            pulumi.set(__self__, "product_name", product_name)
-        if property_ids is not None:
-            pulumi.set(__self__, "property_ids", property_ids)
+        if properties is not None:
+            pulumi.set(__self__, "properties", properties)
         if s3_connector is not None:
             pulumi.set(__self__, "s3_connector", s3_connector)
         if splunk_connector is not None:
             pulumi.set(__self__, "splunk_connector", splunk_connector)
         if stream_name is not None:
             pulumi.set(__self__, "stream_name", stream_name)
-        if stream_type is not None:
-            pulumi.set(__self__, "stream_type", stream_type)
-        if stream_version_id is not None:
-            pulumi.set(__self__, "stream_version_id", stream_version_id)
+        if stream_version is not None:
+            pulumi.set(__self__, "stream_version", stream_version)
         if sumologic_connector is not None:
             pulumi.set(__self__, "sumologic_connector", sumologic_connector)
-        if template_name is not None:
-            pulumi.set(__self__, "template_name", template_name)
 
     @property
     @pulumi.getter
     def active(self) -> Optional[pulumi.Input[bool]]:
         """
         Defining if stream should be active or not
         """
@@ -441,24 +419,24 @@
         return pulumi.get(self, "azure_connector")
 
     @azure_connector.setter
     def azure_connector(self, value: Optional[pulumi.Input['DatastreamAzureConnectorArgs']]):
         pulumi.set(self, "azure_connector", value)
 
     @property
-    @pulumi.getter
-    def config(self) -> Optional[pulumi.Input['DatastreamConfigArgs']]:
+    @pulumi.getter(name="collectMidgress")
+    def collect_midgress(self) -> Optional[pulumi.Input[bool]]:
         """
-        Provides information about the configuration related to logs (format, file names, delivery frequency)
+        Identifies if stream needs to collect midgress data
         """
-        return pulumi.get(self, "config")
+        return pulumi.get(self, "collect_midgress")
 
-    @config.setter
-    def config(self, value: Optional[pulumi.Input['DatastreamConfigArgs']]):
-        pulumi.set(self, "config", value)
+    @collect_midgress.setter
+    def collect_midgress(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "collect_midgress", value)
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> Optional[pulumi.Input[str]]:
         """
         Identifies the contract that has access to the product
         """
@@ -498,48 +476,48 @@
         return pulumi.get(self, "datadog_connector")
 
     @datadog_connector.setter
     def datadog_connector(self, value: Optional[pulumi.Input['DatastreamDatadogConnectorArgs']]):
         pulumi.set(self, "datadog_connector", value)
 
     @property
-    @pulumi.getter(name="datasetFieldsIds")
-    def dataset_fields_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]:
+    @pulumi.getter(name="datasetFields")
+    def dataset_fields(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]:
         """
         A list of data set fields selected from the associated template that the stream monitors in logs. The order of the
         identifiers define how the value for these fields appear in the log lines
         """
-        return pulumi.get(self, "dataset_fields_ids")
+        return pulumi.get(self, "dataset_fields")
 
-    @dataset_fields_ids.setter
-    def dataset_fields_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]):
-        pulumi.set(self, "dataset_fields_ids", value)
+    @dataset_fields.setter
+    def dataset_fields(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]):
+        pulumi.set(self, "dataset_fields", value)
+
+    @property
+    @pulumi.getter(name="deliveryConfiguration")
+    def delivery_configuration(self) -> Optional[pulumi.Input['DatastreamDeliveryConfigurationArgs']]:
+        """
+        Provides information about the configuration related to logs (format, file names, delivery frequency)
+        """
+        return pulumi.get(self, "delivery_configuration")
+
+    @delivery_configuration.setter
+    def delivery_configuration(self, value: Optional[pulumi.Input['DatastreamDeliveryConfigurationArgs']]):
+        pulumi.set(self, "delivery_configuration", value)
 
     @property
     @pulumi.getter(name="elasticsearchConnector")
     def elasticsearch_connector(self) -> Optional[pulumi.Input['DatastreamElasticsearchConnectorArgs']]:
         return pulumi.get(self, "elasticsearch_connector")
 
     @elasticsearch_connector.setter
     def elasticsearch_connector(self, value: Optional[pulumi.Input['DatastreamElasticsearchConnectorArgs']]):
         pulumi.set(self, "elasticsearch_connector", value)
 
     @property
-    @pulumi.getter(name="emailIds")
-    def email_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        List of email addresses where the system sends notifications about activations and deactivations of the stream
-        """
-        return pulumi.get(self, "email_ids")
-
-    @email_ids.setter
-    def email_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "email_ids", value)
-
-    @property
     @pulumi.getter(name="gcsConnector")
     def gcs_connector(self) -> Optional[pulumi.Input['DatastreamGcsConnectorArgs']]:
         return pulumi.get(self, "gcs_connector")
 
     @gcs_connector.setter
     def gcs_connector(self, value: Optional[pulumi.Input['DatastreamGcsConnectorArgs']]):
         pulumi.set(self, "gcs_connector", value)
@@ -553,35 +531,35 @@
         return pulumi.get(self, "group_id")
 
     @group_id.setter
     def group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group_id", value)
 
     @property
-    @pulumi.getter(name="groupName")
-    def group_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The name of the user group for which the stream was created
-        """
-        return pulumi.get(self, "group_name")
-
-    @group_name.setter
-    def group_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group_name", value)
-
-    @property
     @pulumi.getter(name="httpsConnector")
     def https_connector(self) -> Optional[pulumi.Input['DatastreamHttpsConnectorArgs']]:
         return pulumi.get(self, "https_connector")
 
     @https_connector.setter
     def https_connector(self, value: Optional[pulumi.Input['DatastreamHttpsConnectorArgs']]):
         pulumi.set(self, "https_connector", value)
 
     @property
+    @pulumi.getter(name="latestVersion")
+    def latest_version(self) -> Optional[pulumi.Input[int]]:
+        """
+        Identifies the latest active configuration version of the stream
+        """
+        return pulumi.get(self, "latest_version")
+
+    @latest_version.setter
+    def latest_version(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "latest_version", value)
+
+    @property
     @pulumi.getter(name="logglyConnector")
     def loggly_connector(self) -> Optional[pulumi.Input['DatastreamLogglyConnectorArgs']]:
         return pulumi.get(self, "loggly_connector")
 
     @loggly_connector.setter
     def loggly_connector(self, value: Optional[pulumi.Input['DatastreamLogglyConnectorArgs']]):
         pulumi.set(self, "loggly_connector", value)
@@ -616,14 +594,26 @@
         return pulumi.get(self, "new_relic_connector")
 
     @new_relic_connector.setter
     def new_relic_connector(self, value: Optional[pulumi.Input['DatastreamNewRelicConnectorArgs']]):
         pulumi.set(self, "new_relic_connector", value)
 
     @property
+    @pulumi.getter(name="notificationEmails")
+    def notification_emails(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of email addresses where the system sends notifications about activations and deactivations of the stream
+        """
+        return pulumi.get(self, "notification_emails")
+
+    @notification_emails.setter
+    def notification_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "notification_emails", value)
+
+    @property
     @pulumi.getter(name="oracleConnector")
     def oracle_connector(self) -> Optional[pulumi.Input['DatastreamOracleConnectorArgs']]:
         return pulumi.get(self, "oracle_connector")
 
     @oracle_connector.setter
     def oracle_connector(self, value: Optional[pulumi.Input['DatastreamOracleConnectorArgs']]):
         pulumi.set(self, "oracle_connector", value)
@@ -649,36 +639,24 @@
         return pulumi.get(self, "product_id")
 
     @product_id.setter
     def product_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "product_id", value)
 
     @property
-    @pulumi.getter(name="productName")
-    def product_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The name of the product for which the stream was created
-        """
-        return pulumi.get(self, "product_name")
-
-    @product_name.setter
-    def product_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "product_name", value)
-
-    @property
-    @pulumi.getter(name="propertyIds")
-    def property_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter
+    def properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Identifies the properties monitored in the stream
         """
-        return pulumi.get(self, "property_ids")
+        return pulumi.get(self, "properties")
 
-    @property_ids.setter
-    def property_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "property_ids", value)
+    @properties.setter
+    def properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "properties", value)
 
     @property
     @pulumi.getter(name="s3Connector")
     def s3_connector(self) -> Optional[pulumi.Input['DatastreamS3ConnectorArgs']]:
         return pulumi.get(self, "s3_connector")
 
     @s3_connector.setter
@@ -703,101 +681,75 @@
         return pulumi.get(self, "stream_name")
 
     @stream_name.setter
     def stream_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stream_name", value)
 
     @property
-    @pulumi.getter(name="streamType")
-    def stream_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        Specifies the type of the data stream
-        """
-        return pulumi.get(self, "stream_type")
-
-    @stream_type.setter
-    def stream_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "stream_type", value)
-
-    @property
-    @pulumi.getter(name="streamVersionId")
-    def stream_version_id(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="streamVersion")
+    def stream_version(self) -> Optional[pulumi.Input[int]]:
         """
         Identifies the configuration version of the stream
         """
-        return pulumi.get(self, "stream_version_id")
+        return pulumi.get(self, "stream_version")
 
-    @stream_version_id.setter
-    def stream_version_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "stream_version_id", value)
+    @stream_version.setter
+    def stream_version(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "stream_version", value)
 
     @property
     @pulumi.getter(name="sumologicConnector")
     def sumologic_connector(self) -> Optional[pulumi.Input['DatastreamSumologicConnectorArgs']]:
         return pulumi.get(self, "sumologic_connector")
 
     @sumologic_connector.setter
     def sumologic_connector(self, value: Optional[pulumi.Input['DatastreamSumologicConnectorArgs']]):
         pulumi.set(self, "sumologic_connector", value)
 
-    @property
-    @pulumi.getter(name="templateName")
-    def template_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The name of the template associated with the stream
-        """
-        return pulumi.get(self, "template_name")
-
-    @template_name.setter
-    def template_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "template_name", value)
-
 
 class Datastream(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  active: Optional[pulumi.Input[bool]] = None,
                  azure_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamAzureConnectorArgs']]] = None,
-                 config: Optional[pulumi.Input[pulumi.InputType['DatastreamConfigArgs']]] = None,
+                 collect_midgress: Optional[pulumi.Input[bool]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
                  datadog_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamDatadogConnectorArgs']]] = None,
-                 dataset_fields_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+                 dataset_fields: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+                 delivery_configuration: Optional[pulumi.Input[pulumi.InputType['DatastreamDeliveryConfigurationArgs']]] = None,
                  elasticsearch_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamElasticsearchConnectorArgs']]] = None,
-                 email_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  gcs_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamGcsConnectorArgs']]] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  https_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamHttpsConnectorArgs']]] = None,
                  loggly_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamLogglyConnectorArgs']]] = None,
                  new_relic_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamNewRelicConnectorArgs']]] = None,
+                 notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  oracle_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamOracleConnectorArgs']]] = None,
-                 property_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  s3_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamS3ConnectorArgs']]] = None,
                  splunk_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamSplunkConnectorArgs']]] = None,
                  stream_name: Optional[pulumi.Input[str]] = None,
-                 stream_type: Optional[pulumi.Input[str]] = None,
                  sumologic_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamSumologicConnectorArgs']]] = None,
-                 template_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a Datastream resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Defining if stream should be active or not
-        :param pulumi.Input[pulumi.InputType['DatastreamConfigArgs']] config: Provides information about the configuration related to logs (format, file names, delivery frequency)
+        :param pulumi.Input[bool] collect_midgress: Identifies if stream needs to collect midgress data
         :param pulumi.Input[str] contract_id: Identifies the contract that has access to the product
-        :param pulumi.Input[Sequence[pulumi.Input[int]]] dataset_fields_ids: A list of data set fields selected from the associated template that the stream monitors in logs. The order of the
+        :param pulumi.Input[Sequence[pulumi.Input[int]]] dataset_fields: A list of data set fields selected from the associated template that the stream monitors in logs. The order of the
                identifiers define how the value for these fields appear in the log lines
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] email_ids: List of email addresses where the system sends notifications about activations and deactivations of the stream
+        :param pulumi.Input[pulumi.InputType['DatastreamDeliveryConfigurationArgs']] delivery_configuration: Provides information about the configuration related to logs (format, file names, delivery frequency)
         :param pulumi.Input[str] group_id: Identifies the group that has access to the product and for which the stream configuration was created
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] property_ids: Identifies the properties monitored in the stream
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_emails: List of email addresses where the system sends notifications about activations and deactivations of the stream
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] properties: Identifies the properties monitored in the stream
         :param pulumi.Input[str] stream_name: The name of the stream
-        :param pulumi.Input[str] stream_type: Specifies the type of the data stream
-        :param pulumi.Input[str] template_name: The name of the template associated with the stream
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DatastreamArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -816,192 +768,179 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  active: Optional[pulumi.Input[bool]] = None,
                  azure_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamAzureConnectorArgs']]] = None,
-                 config: Optional[pulumi.Input[pulumi.InputType['DatastreamConfigArgs']]] = None,
+                 collect_midgress: Optional[pulumi.Input[bool]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
                  datadog_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamDatadogConnectorArgs']]] = None,
-                 dataset_fields_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+                 dataset_fields: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+                 delivery_configuration: Optional[pulumi.Input[pulumi.InputType['DatastreamDeliveryConfigurationArgs']]] = None,
                  elasticsearch_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamElasticsearchConnectorArgs']]] = None,
-                 email_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  gcs_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamGcsConnectorArgs']]] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  https_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamHttpsConnectorArgs']]] = None,
                  loggly_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamLogglyConnectorArgs']]] = None,
                  new_relic_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamNewRelicConnectorArgs']]] = None,
+                 notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  oracle_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamOracleConnectorArgs']]] = None,
-                 property_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  s3_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamS3ConnectorArgs']]] = None,
                  splunk_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamSplunkConnectorArgs']]] = None,
                  stream_name: Optional[pulumi.Input[str]] = None,
-                 stream_type: Optional[pulumi.Input[str]] = None,
                  sumologic_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamSumologicConnectorArgs']]] = None,
-                 template_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DatastreamArgs.__new__(DatastreamArgs)
 
             if active is None and not opts.urn:
                 raise TypeError("Missing required property 'active'")
             __props__.__dict__["active"] = active
             __props__.__dict__["azure_connector"] = azure_connector
-            if config is None and not opts.urn:
-                raise TypeError("Missing required property 'config'")
-            __props__.__dict__["config"] = config
+            __props__.__dict__["collect_midgress"] = collect_midgress
             if contract_id is None and not opts.urn:
                 raise TypeError("Missing required property 'contract_id'")
             __props__.__dict__["contract_id"] = contract_id
             __props__.__dict__["datadog_connector"] = datadog_connector
-            if dataset_fields_ids is None and not opts.urn:
-                raise TypeError("Missing required property 'dataset_fields_ids'")
-            __props__.__dict__["dataset_fields_ids"] = dataset_fields_ids
+            if dataset_fields is None and not opts.urn:
+                raise TypeError("Missing required property 'dataset_fields'")
+            __props__.__dict__["dataset_fields"] = dataset_fields
+            if delivery_configuration is None and not opts.urn:
+                raise TypeError("Missing required property 'delivery_configuration'")
+            __props__.__dict__["delivery_configuration"] = delivery_configuration
             __props__.__dict__["elasticsearch_connector"] = elasticsearch_connector
-            __props__.__dict__["email_ids"] = email_ids
             __props__.__dict__["gcs_connector"] = gcs_connector
             if group_id is None and not opts.urn:
                 raise TypeError("Missing required property 'group_id'")
             __props__.__dict__["group_id"] = group_id
             __props__.__dict__["https_connector"] = https_connector
             __props__.__dict__["loggly_connector"] = loggly_connector
             __props__.__dict__["new_relic_connector"] = new_relic_connector
+            __props__.__dict__["notification_emails"] = notification_emails
             __props__.__dict__["oracle_connector"] = oracle_connector
-            if property_ids is None and not opts.urn:
-                raise TypeError("Missing required property 'property_ids'")
-            __props__.__dict__["property_ids"] = property_ids
+            if properties is None and not opts.urn:
+                raise TypeError("Missing required property 'properties'")
+            __props__.__dict__["properties"] = properties
             __props__.__dict__["s3_connector"] = s3_connector
             __props__.__dict__["splunk_connector"] = splunk_connector
             if stream_name is None and not opts.urn:
                 raise TypeError("Missing required property 'stream_name'")
             __props__.__dict__["stream_name"] = stream_name
-            if stream_type is None and not opts.urn:
-                raise TypeError("Missing required property 'stream_type'")
-            __props__.__dict__["stream_type"] = stream_type
             __props__.__dict__["sumologic_connector"] = sumologic_connector
-            if template_name is None and not opts.urn:
-                raise TypeError("Missing required property 'template_name'")
-            __props__.__dict__["template_name"] = template_name
             __props__.__dict__["created_by"] = None
             __props__.__dict__["created_date"] = None
-            __props__.__dict__["group_name"] = None
+            __props__.__dict__["latest_version"] = None
             __props__.__dict__["modified_by"] = None
             __props__.__dict__["modified_date"] = None
             __props__.__dict__["papi_json"] = None
             __props__.__dict__["product_id"] = None
-            __props__.__dict__["product_name"] = None
-            __props__.__dict__["stream_version_id"] = None
+            __props__.__dict__["stream_version"] = None
         super(Datastream, __self__).__init__(
             'akamai:index/datastream:Datastream',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             active: Optional[pulumi.Input[bool]] = None,
             azure_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamAzureConnectorArgs']]] = None,
-            config: Optional[pulumi.Input[pulumi.InputType['DatastreamConfigArgs']]] = None,
+            collect_midgress: Optional[pulumi.Input[bool]] = None,
             contract_id: Optional[pulumi.Input[str]] = None,
             created_by: Optional[pulumi.Input[str]] = None,
             created_date: Optional[pulumi.Input[str]] = None,
             datadog_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamDatadogConnectorArgs']]] = None,
-            dataset_fields_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+            dataset_fields: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+            delivery_configuration: Optional[pulumi.Input[pulumi.InputType['DatastreamDeliveryConfigurationArgs']]] = None,
             elasticsearch_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamElasticsearchConnectorArgs']]] = None,
-            email_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             gcs_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamGcsConnectorArgs']]] = None,
             group_id: Optional[pulumi.Input[str]] = None,
-            group_name: Optional[pulumi.Input[str]] = None,
             https_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamHttpsConnectorArgs']]] = None,
+            latest_version: Optional[pulumi.Input[int]] = None,
             loggly_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamLogglyConnectorArgs']]] = None,
             modified_by: Optional[pulumi.Input[str]] = None,
             modified_date: Optional[pulumi.Input[str]] = None,
             new_relic_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamNewRelicConnectorArgs']]] = None,
+            notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             oracle_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamOracleConnectorArgs']]] = None,
             papi_json: Optional[pulumi.Input[str]] = None,
             product_id: Optional[pulumi.Input[str]] = None,
-            product_name: Optional[pulumi.Input[str]] = None,
-            property_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             s3_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamS3ConnectorArgs']]] = None,
             splunk_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamSplunkConnectorArgs']]] = None,
             stream_name: Optional[pulumi.Input[str]] = None,
-            stream_type: Optional[pulumi.Input[str]] = None,
-            stream_version_id: Optional[pulumi.Input[int]] = None,
-            sumologic_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamSumologicConnectorArgs']]] = None,
-            template_name: Optional[pulumi.Input[str]] = None) -> 'Datastream':
+            stream_version: Optional[pulumi.Input[int]] = None,
+            sumologic_connector: Optional[pulumi.Input[pulumi.InputType['DatastreamSumologicConnectorArgs']]] = None) -> 'Datastream':
         """
         Get an existing Datastream resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Defining if stream should be active or not
-        :param pulumi.Input[pulumi.InputType['DatastreamConfigArgs']] config: Provides information about the configuration related to logs (format, file names, delivery frequency)
+        :param pulumi.Input[bool] collect_midgress: Identifies if stream needs to collect midgress data
         :param pulumi.Input[str] contract_id: Identifies the contract that has access to the product
         :param pulumi.Input[str] created_by: The username who created the stream
         :param pulumi.Input[str] created_date: The date and time when the stream was created
-        :param pulumi.Input[Sequence[pulumi.Input[int]]] dataset_fields_ids: A list of data set fields selected from the associated template that the stream monitors in logs. The order of the
+        :param pulumi.Input[Sequence[pulumi.Input[int]]] dataset_fields: A list of data set fields selected from the associated template that the stream monitors in logs. The order of the
                identifiers define how the value for these fields appear in the log lines
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] email_ids: List of email addresses where the system sends notifications about activations and deactivations of the stream
+        :param pulumi.Input[pulumi.InputType['DatastreamDeliveryConfigurationArgs']] delivery_configuration: Provides information about the configuration related to logs (format, file names, delivery frequency)
         :param pulumi.Input[str] group_id: Identifies the group that has access to the product and for which the stream configuration was created
-        :param pulumi.Input[str] group_name: The name of the user group for which the stream was created
+        :param pulumi.Input[int] latest_version: Identifies the latest active configuration version of the stream
         :param pulumi.Input[str] modified_by: The username who modified the stream
         :param pulumi.Input[str] modified_date: The date and time when the stream was modified
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_emails: List of email addresses where the system sends notifications about activations and deactivations of the stream
         :param pulumi.Input[str] papi_json: The configuration in JSON format that can be copy-pasted into PAPI configuration to enable datastream behavior
         :param pulumi.Input[str] product_id: The ID of the product for which the stream was created
-        :param pulumi.Input[str] product_name: The name of the product for which the stream was created
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] property_ids: Identifies the properties monitored in the stream
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] properties: Identifies the properties monitored in the stream
         :param pulumi.Input[str] stream_name: The name of the stream
-        :param pulumi.Input[str] stream_type: Specifies the type of the data stream
-        :param pulumi.Input[int] stream_version_id: Identifies the configuration version of the stream
-        :param pulumi.Input[str] template_name: The name of the template associated with the stream
+        :param pulumi.Input[int] stream_version: Identifies the configuration version of the stream
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DatastreamState.__new__(_DatastreamState)
 
         __props__.__dict__["active"] = active
         __props__.__dict__["azure_connector"] = azure_connector
-        __props__.__dict__["config"] = config
+        __props__.__dict__["collect_midgress"] = collect_midgress
         __props__.__dict__["contract_id"] = contract_id
         __props__.__dict__["created_by"] = created_by
         __props__.__dict__["created_date"] = created_date
         __props__.__dict__["datadog_connector"] = datadog_connector
-        __props__.__dict__["dataset_fields_ids"] = dataset_fields_ids
+        __props__.__dict__["dataset_fields"] = dataset_fields
+        __props__.__dict__["delivery_configuration"] = delivery_configuration
         __props__.__dict__["elasticsearch_connector"] = elasticsearch_connector
-        __props__.__dict__["email_ids"] = email_ids
         __props__.__dict__["gcs_connector"] = gcs_connector
         __props__.__dict__["group_id"] = group_id
-        __props__.__dict__["group_name"] = group_name
         __props__.__dict__["https_connector"] = https_connector
+        __props__.__dict__["latest_version"] = latest_version
         __props__.__dict__["loggly_connector"] = loggly_connector
         __props__.__dict__["modified_by"] = modified_by
         __props__.__dict__["modified_date"] = modified_date
         __props__.__dict__["new_relic_connector"] = new_relic_connector
+        __props__.__dict__["notification_emails"] = notification_emails
         __props__.__dict__["oracle_connector"] = oracle_connector
         __props__.__dict__["papi_json"] = papi_json
         __props__.__dict__["product_id"] = product_id
-        __props__.__dict__["product_name"] = product_name
-        __props__.__dict__["property_ids"] = property_ids
+        __props__.__dict__["properties"] = properties
         __props__.__dict__["s3_connector"] = s3_connector
         __props__.__dict__["splunk_connector"] = splunk_connector
         __props__.__dict__["stream_name"] = stream_name
-        __props__.__dict__["stream_type"] = stream_type
-        __props__.__dict__["stream_version_id"] = stream_version_id
+        __props__.__dict__["stream_version"] = stream_version
         __props__.__dict__["sumologic_connector"] = sumologic_connector
-        __props__.__dict__["template_name"] = template_name
         return Datastream(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def active(self) -> pulumi.Output[bool]:
         """
         Defining if stream should be active or not
@@ -1010,20 +949,20 @@
 
     @property
     @pulumi.getter(name="azureConnector")
     def azure_connector(self) -> pulumi.Output[Optional['outputs.DatastreamAzureConnector']]:
         return pulumi.get(self, "azure_connector")
 
     @property
-    @pulumi.getter
-    def config(self) -> pulumi.Output['outputs.DatastreamConfig']:
+    @pulumi.getter(name="collectMidgress")
+    def collect_midgress(self) -> pulumi.Output[Optional[bool]]:
         """
-        Provides information about the configuration related to logs (format, file names, delivery frequency)
+        Identifies if stream needs to collect midgress data
         """
-        return pulumi.get(self, "config")
+        return pulumi.get(self, "collect_midgress")
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> pulumi.Output[str]:
         """
         Identifies the contract that has access to the product
         """
@@ -1047,62 +986,62 @@
 
     @property
     @pulumi.getter(name="datadogConnector")
     def datadog_connector(self) -> pulumi.Output[Optional['outputs.DatastreamDatadogConnector']]:
         return pulumi.get(self, "datadog_connector")
 
     @property
-    @pulumi.getter(name="datasetFieldsIds")
-    def dataset_fields_ids(self) -> pulumi.Output[Sequence[int]]:
+    @pulumi.getter(name="datasetFields")
+    def dataset_fields(self) -> pulumi.Output[Sequence[int]]:
         """
         A list of data set fields selected from the associated template that the stream monitors in logs. The order of the
         identifiers define how the value for these fields appear in the log lines
         """
-        return pulumi.get(self, "dataset_fields_ids")
+        return pulumi.get(self, "dataset_fields")
+
+    @property
+    @pulumi.getter(name="deliveryConfiguration")
+    def delivery_configuration(self) -> pulumi.Output['outputs.DatastreamDeliveryConfiguration']:
+        """
+        Provides information about the configuration related to logs (format, file names, delivery frequency)
+        """
+        return pulumi.get(self, "delivery_configuration")
 
     @property
     @pulumi.getter(name="elasticsearchConnector")
     def elasticsearch_connector(self) -> pulumi.Output[Optional['outputs.DatastreamElasticsearchConnector']]:
         return pulumi.get(self, "elasticsearch_connector")
 
     @property
-    @pulumi.getter(name="emailIds")
-    def email_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        """
-        List of email addresses where the system sends notifications about activations and deactivations of the stream
-        """
-        return pulumi.get(self, "email_ids")
-
-    @property
     @pulumi.getter(name="gcsConnector")
     def gcs_connector(self) -> pulumi.Output[Optional['outputs.DatastreamGcsConnector']]:
         return pulumi.get(self, "gcs_connector")
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> pulumi.Output[str]:
         """
         Identifies the group that has access to the product and for which the stream configuration was created
         """
         return pulumi.get(self, "group_id")
 
     @property
-    @pulumi.getter(name="groupName")
-    def group_name(self) -> pulumi.Output[str]:
-        """
-        The name of the user group for which the stream was created
-        """
-        return pulumi.get(self, "group_name")
-
-    @property
     @pulumi.getter(name="httpsConnector")
     def https_connector(self) -> pulumi.Output[Optional['outputs.DatastreamHttpsConnector']]:
         return pulumi.get(self, "https_connector")
 
     @property
+    @pulumi.getter(name="latestVersion")
+    def latest_version(self) -> pulumi.Output[int]:
+        """
+        Identifies the latest active configuration version of the stream
+        """
+        return pulumi.get(self, "latest_version")
+
+    @property
     @pulumi.getter(name="logglyConnector")
     def loggly_connector(self) -> pulumi.Output[Optional['outputs.DatastreamLogglyConnector']]:
         return pulumi.get(self, "loggly_connector")
 
     @property
     @pulumi.getter(name="modifiedBy")
     def modified_by(self) -> pulumi.Output[str]:
@@ -1121,14 +1060,22 @@
 
     @property
     @pulumi.getter(name="newRelicConnector")
     def new_relic_connector(self) -> pulumi.Output[Optional['outputs.DatastreamNewRelicConnector']]:
         return pulumi.get(self, "new_relic_connector")
 
     @property
+    @pulumi.getter(name="notificationEmails")
+    def notification_emails(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        List of email addresses where the system sends notifications about activations and deactivations of the stream
+        """
+        return pulumi.get(self, "notification_emails")
+
+    @property
     @pulumi.getter(name="oracleConnector")
     def oracle_connector(self) -> pulumi.Output[Optional['outputs.DatastreamOracleConnector']]:
         return pulumi.get(self, "oracle_connector")
 
     @property
     @pulumi.getter(name="papiJson")
     def papi_json(self) -> pulumi.Output[str]:
@@ -1142,28 +1089,20 @@
     def product_id(self) -> pulumi.Output[str]:
         """
         The ID of the product for which the stream was created
         """
         return pulumi.get(self, "product_id")
 
     @property
-    @pulumi.getter(name="productName")
-    def product_name(self) -> pulumi.Output[str]:
-        """
-        The name of the product for which the stream was created
-        """
-        return pulumi.get(self, "product_name")
-
-    @property
-    @pulumi.getter(name="propertyIds")
-    def property_ids(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter
+    def properties(self) -> pulumi.Output[Sequence[str]]:
         """
         Identifies the properties monitored in the stream
         """
-        return pulumi.get(self, "property_ids")
+        return pulumi.get(self, "properties")
 
     @property
     @pulumi.getter(name="s3Connector")
     def s3_connector(self) -> pulumi.Output[Optional['outputs.DatastreamS3Connector']]:
         return pulumi.get(self, "s3_connector")
 
     @property
@@ -1176,35 +1115,19 @@
     def stream_name(self) -> pulumi.Output[str]:
         """
         The name of the stream
         """
         return pulumi.get(self, "stream_name")
 
     @property
-    @pulumi.getter(name="streamType")
-    def stream_type(self) -> pulumi.Output[str]:
-        """
-        Specifies the type of the data stream
-        """
-        return pulumi.get(self, "stream_type")
-
-    @property
-    @pulumi.getter(name="streamVersionId")
-    def stream_version_id(self) -> pulumi.Output[int]:
+    @pulumi.getter(name="streamVersion")
+    def stream_version(self) -> pulumi.Output[int]:
         """
         Identifies the configuration version of the stream
         """
-        return pulumi.get(self, "stream_version_id")
+        return pulumi.get(self, "stream_version")
 
     @property
     @pulumi.getter(name="sumologicConnector")
     def sumologic_connector(self) -> pulumi.Output[Optional['outputs.DatastreamSumologicConnector']]:
         return pulumi.get(self, "sumologic_connector")
 
-    @property
-    @pulumi.getter(name="templateName")
-    def template_name(self) -> pulumi.Output[str]:
-        """
-        The name of the template associated with the stream
-        """
-        return pulumi.get(self, "template_name")
-
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/dns_record.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/dns_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
         """
         The set of arguments for constructing a DnsRecord resource.
         """
         pulumi.set(__self__, "recordtype", recordtype)
         pulumi.set(__self__, "ttl", ttl)
         pulumi.set(__self__, "zone", zone)
         if active is not None:
+            warnings.warn("""Field 'active' has been deprecated. Setting it has no effect""", DeprecationWarning)
+            pulumi.log.warn("""active is deprecated: Field 'active' has been deprecated. Setting it has no effect""")
+        if active is not None:
             pulumi.set(__self__, "active", active)
         if algorithm is not None:
             pulumi.set(__self__, "algorithm", algorithm)
         if certificate is not None:
             pulumi.set(__self__, "certificate", certificate)
         if digest is not None:
             pulumi.set(__self__, "digest", digest)
@@ -209,14 +212,17 @@
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter
     def active(self) -> Optional[pulumi.Input[bool]]:
+        warnings.warn("""Field 'active' has been deprecated. Setting it has no effect""", DeprecationWarning)
+        pulumi.log.warn("""active is deprecated: Field 'active' has been deprecated. Setting it has no effect""")
+
         return pulumi.get(self, "active")
 
     @active.setter
     def active(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "active", value)
 
     @property
@@ -751,14 +757,17 @@
                  usage: Optional[pulumi.Input[int]] = None,
                  weight: Optional[pulumi.Input[int]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering DnsRecord resources.
         """
         if active is not None:
+            warnings.warn("""Field 'active' has been deprecated. Setting it has no effect""", DeprecationWarning)
+            pulumi.log.warn("""active is deprecated: Field 'active' has been deprecated. Setting it has no effect""")
+        if active is not None:
             pulumi.set(__self__, "active", active)
         if algorithm is not None:
             pulumi.set(__self__, "algorithm", algorithm)
         if answer_type is not None:
             pulumi.set(__self__, "answer_type", answer_type)
         if certificate is not None:
             pulumi.set(__self__, "certificate", certificate)
@@ -874,14 +883,17 @@
             pulumi.set(__self__, "weight", weight)
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter
     def active(self) -> Optional[pulumi.Input[bool]]:
+        warnings.warn("""Field 'active' has been deprecated. Setting it has no effect""", DeprecationWarning)
+        pulumi.log.warn("""active is deprecated: Field 'active' has been deprecated. Setting it has no effect""")
+
         return pulumi.get(self, "active")
 
     @active.setter
     def active(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "active", value)
 
     @property
@@ -1567,14 +1579,17 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DnsRecordArgs.__new__(DnsRecordArgs)
 
+            if active is not None and not opts.urn:
+                warnings.warn("""Field 'active' has been deprecated. Setting it has no effect""", DeprecationWarning)
+                pulumi.log.warn("""active is deprecated: Field 'active' has been deprecated. Setting it has no effect""")
             __props__.__dict__["active"] = active
             __props__.__dict__["algorithm"] = algorithm
             __props__.__dict__["certificate"] = certificate
             __props__.__dict__["digest"] = digest
             __props__.__dict__["digest_type"] = digest_type
             __props__.__dict__["email_address"] = email_address
             __props__.__dict__["expiration"] = expiration
@@ -1782,14 +1797,17 @@
         __props__.__dict__["weight"] = weight
         __props__.__dict__["zone"] = zone
         return DnsRecord(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def active(self) -> pulumi.Output[Optional[bool]]:
+        warnings.warn("""Field 'active' has been deprecated. Setting it has no effect""", DeprecationWarning)
+        pulumi.log.warn("""active is deprecated: Field 'active' has been deprecated. Setting it has no effect""")
+
         return pulumi.get(self, "active")
 
     @property
     @pulumi.getter
     def algorithm(self) -> pulumi.Output[Optional[int]]:
         return pulumi.get(self, "algorithm")
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/dns_zone.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/dns_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edge_host_name.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_resource.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,551 +4,610 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = ['EdgeHostNameArgs', 'EdgeHostName']
+__all__ = ['GtmResourceArgs', 'GtmResource']
 
 @pulumi.input_type
-class EdgeHostNameArgs:
+class GtmResourceArgs:
     def __init__(__self__, *,
-                 edge_hostname: pulumi.Input[str],
-                 ip_behavior: pulumi.Input[str],
-                 certificate: Optional[pulumi.Input[int]] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
-                 contract_id: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 group_id: Optional[pulumi.Input[str]] = None,
-                 product: Optional[pulumi.Input[str]] = None,
-                 product_id: Optional[pulumi.Input[str]] = None,
-                 status_update_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 use_cases: Optional[pulumi.Input[str]] = None):
+                 aggregation_type: pulumi.Input[str],
+                 domain: pulumi.Input[str],
+                 type: pulumi.Input[str],
+                 constrained_property: Optional[pulumi.Input[str]] = None,
+                 decay_rate: Optional[pulumi.Input[float]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 host_header: Optional[pulumi.Input[str]] = None,
+                 leader_string: Optional[pulumi.Input[str]] = None,
+                 least_squares_decay: Optional[pulumi.Input[float]] = None,
+                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
+                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]] = None,
+                 upper_bound: Optional[pulumi.Input[int]] = None,
+                 wait_on_complete: Optional[pulumi.Input[bool]] = None):
         """
-        The set of arguments for constructing a EdgeHostName resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] status_update_emails: Email address that should receive updates on the IP behavior update request. Required for update operation.
-        :param pulumi.Input[str] use_cases: A JSON encoded list of use cases
+        The set of arguments for constructing a GtmResource resource.
         """
-        pulumi.set(__self__, "edge_hostname", edge_hostname)
-        pulumi.set(__self__, "ip_behavior", ip_behavior)
-        if certificate is not None:
-            pulumi.set(__self__, "certificate", certificate)
-        if contract is not None:
-            warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-        if contract is not None:
-            pulumi.set(__self__, "contract", contract)
-        if contract_id is not None:
-            pulumi.set(__self__, "contract_id", contract_id)
-        if group is not None:
-            warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-        if group is not None:
-            pulumi.set(__self__, "group", group)
-        if group_id is not None:
-            pulumi.set(__self__, "group_id", group_id)
-        if product is not None:
-            warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
-        if product is not None:
-            pulumi.set(__self__, "product", product)
-        if product_id is not None:
-            pulumi.set(__self__, "product_id", product_id)
-        if status_update_emails is not None:
-            pulumi.set(__self__, "status_update_emails", status_update_emails)
-        if use_cases is not None:
-            pulumi.set(__self__, "use_cases", use_cases)
+        pulumi.set(__self__, "aggregation_type", aggregation_type)
+        pulumi.set(__self__, "domain", domain)
+        pulumi.set(__self__, "type", type)
+        if constrained_property is not None:
+            pulumi.set(__self__, "constrained_property", constrained_property)
+        if decay_rate is not None:
+            pulumi.set(__self__, "decay_rate", decay_rate)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if host_header is not None:
+            pulumi.set(__self__, "host_header", host_header)
+        if leader_string is not None:
+            pulumi.set(__self__, "leader_string", leader_string)
+        if least_squares_decay is not None:
+            pulumi.set(__self__, "least_squares_decay", least_squares_decay)
+        if load_imbalance_percentage is not None:
+            pulumi.set(__self__, "load_imbalance_percentage", load_imbalance_percentage)
+        if max_u_multiplicative_increment is not None:
+            pulumi.set(__self__, "max_u_multiplicative_increment", max_u_multiplicative_increment)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if resource_instances is not None:
+            pulumi.set(__self__, "resource_instances", resource_instances)
+        if upper_bound is not None:
+            pulumi.set(__self__, "upper_bound", upper_bound)
+        if wait_on_complete is not None:
+            pulumi.set(__self__, "wait_on_complete", wait_on_complete)
 
     @property
-    @pulumi.getter(name="edgeHostname")
-    def edge_hostname(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "edge_hostname")
+    @pulumi.getter(name="aggregationType")
+    def aggregation_type(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "aggregation_type")
 
-    @edge_hostname.setter
-    def edge_hostname(self, value: pulumi.Input[str]):
-        pulumi.set(self, "edge_hostname", value)
+    @aggregation_type.setter
+    def aggregation_type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "aggregation_type", value)
 
     @property
-    @pulumi.getter(name="ipBehavior")
-    def ip_behavior(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "ip_behavior")
+    @pulumi.getter
+    def domain(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "domain")
 
-    @ip_behavior.setter
-    def ip_behavior(self, value: pulumi.Input[str]):
-        pulumi.set(self, "ip_behavior", value)
+    @domain.setter
+    def domain(self, value: pulumi.Input[str]):
+        pulumi.set(self, "domain", value)
 
     @property
     @pulumi.getter
-    def certificate(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "certificate")
+    def type(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "type", value)
+
+    @property
+    @pulumi.getter(name="constrainedProperty")
+    def constrained_property(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "constrained_property")
+
+    @constrained_property.setter
+    def constrained_property(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "constrained_property", value)
+
+    @property
+    @pulumi.getter(name="decayRate")
+    def decay_rate(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "decay_rate")
 
-    @certificate.setter
-    def certificate(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "certificate", value)
+    @decay_rate.setter
+    def decay_rate(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "decay_rate", value)
 
     @property
     @pulumi.getter
-    def contract(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+    def description(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "description")
 
-        return pulumi.get(self, "contract")
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
-    @contract.setter
-    def contract(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "contract", value)
+    @property
+    @pulumi.getter(name="hostHeader")
+    def host_header(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "host_header")
+
+    @host_header.setter
+    def host_header(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "host_header", value)
 
     @property
-    @pulumi.getter(name="contractId")
-    def contract_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "contract_id")
+    @pulumi.getter(name="leaderString")
+    def leader_string(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "leader_string")
 
-    @contract_id.setter
-    def contract_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "contract_id", value)
+    @leader_string.setter
+    def leader_string(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "leader_string", value)
 
     @property
-    @pulumi.getter
-    def group(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+    @pulumi.getter(name="leastSquaresDecay")
+    def least_squares_decay(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "least_squares_decay")
 
-        return pulumi.get(self, "group")
+    @least_squares_decay.setter
+    def least_squares_decay(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "least_squares_decay", value)
 
-    @group.setter
-    def group(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group", value)
+    @property
+    @pulumi.getter(name="loadImbalancePercentage")
+    def load_imbalance_percentage(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "load_imbalance_percentage")
+
+    @load_imbalance_percentage.setter
+    def load_imbalance_percentage(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "load_imbalance_percentage", value)
 
     @property
-    @pulumi.getter(name="groupId")
-    def group_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "group_id")
+    @pulumi.getter(name="maxUMultiplicativeIncrement")
+    def max_u_multiplicative_increment(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "max_u_multiplicative_increment")
 
-    @group_id.setter
-    def group_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group_id", value)
+    @max_u_multiplicative_increment.setter
+    def max_u_multiplicative_increment(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "max_u_multiplicative_increment", value)
 
     @property
     @pulumi.getter
-    def product(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
-
-        return pulumi.get(self, "product")
+    def name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "name")
 
-    @product.setter
-    def product(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "product", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="productId")
-    def product_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "product_id")
+    @pulumi.getter(name="resourceInstances")
+    def resource_instances(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]:
+        return pulumi.get(self, "resource_instances")
 
-    @product_id.setter
-    def product_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "product_id", value)
+    @resource_instances.setter
+    def resource_instances(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]):
+        pulumi.set(self, "resource_instances", value)
 
     @property
-    @pulumi.getter(name="statusUpdateEmails")
-    def status_update_emails(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Email address that should receive updates on the IP behavior update request. Required for update operation.
-        """
-        return pulumi.get(self, "status_update_emails")
+    @pulumi.getter(name="upperBound")
+    def upper_bound(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "upper_bound")
 
-    @status_update_emails.setter
-    def status_update_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "status_update_emails", value)
+    @upper_bound.setter
+    def upper_bound(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "upper_bound", value)
 
     @property
-    @pulumi.getter(name="useCases")
-    def use_cases(self) -> Optional[pulumi.Input[str]]:
-        """
-        A JSON encoded list of use cases
-        """
-        return pulumi.get(self, "use_cases")
+    @pulumi.getter(name="waitOnComplete")
+    def wait_on_complete(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "wait_on_complete")
 
-    @use_cases.setter
-    def use_cases(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "use_cases", value)
+    @wait_on_complete.setter
+    def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "wait_on_complete", value)
 
 
 @pulumi.input_type
-class _EdgeHostNameState:
+class _GtmResourceState:
     def __init__(__self__, *,
-                 certificate: Optional[pulumi.Input[int]] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
-                 contract_id: Optional[pulumi.Input[str]] = None,
-                 edge_hostname: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 group_id: Optional[pulumi.Input[str]] = None,
-                 ip_behavior: Optional[pulumi.Input[str]] = None,
-                 product: Optional[pulumi.Input[str]] = None,
-                 product_id: Optional[pulumi.Input[str]] = None,
-                 status_update_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 use_cases: Optional[pulumi.Input[str]] = None):
+                 aggregation_type: Optional[pulumi.Input[str]] = None,
+                 constrained_property: Optional[pulumi.Input[str]] = None,
+                 decay_rate: Optional[pulumi.Input[float]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 domain: Optional[pulumi.Input[str]] = None,
+                 host_header: Optional[pulumi.Input[str]] = None,
+                 leader_string: Optional[pulumi.Input[str]] = None,
+                 least_squares_decay: Optional[pulumi.Input[float]] = None,
+                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
+                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
+                 upper_bound: Optional[pulumi.Input[int]] = None,
+                 wait_on_complete: Optional[pulumi.Input[bool]] = None):
         """
-        Input properties used for looking up and filtering EdgeHostName resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] status_update_emails: Email address that should receive updates on the IP behavior update request. Required for update operation.
-        :param pulumi.Input[str] use_cases: A JSON encoded list of use cases
+        Input properties used for looking up and filtering GtmResource resources.
         """
-        if certificate is not None:
-            pulumi.set(__self__, "certificate", certificate)
-        if contract is not None:
-            warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-        if contract is not None:
-            pulumi.set(__self__, "contract", contract)
-        if contract_id is not None:
-            pulumi.set(__self__, "contract_id", contract_id)
-        if edge_hostname is not None:
-            pulumi.set(__self__, "edge_hostname", edge_hostname)
-        if group is not None:
-            warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-        if group is not None:
-            pulumi.set(__self__, "group", group)
-        if group_id is not None:
-            pulumi.set(__self__, "group_id", group_id)
-        if ip_behavior is not None:
-            pulumi.set(__self__, "ip_behavior", ip_behavior)
-        if product is not None:
-            warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
-        if product is not None:
-            pulumi.set(__self__, "product", product)
-        if product_id is not None:
-            pulumi.set(__self__, "product_id", product_id)
-        if status_update_emails is not None:
-            pulumi.set(__self__, "status_update_emails", status_update_emails)
-        if use_cases is not None:
-            pulumi.set(__self__, "use_cases", use_cases)
+        if aggregation_type is not None:
+            pulumi.set(__self__, "aggregation_type", aggregation_type)
+        if constrained_property is not None:
+            pulumi.set(__self__, "constrained_property", constrained_property)
+        if decay_rate is not None:
+            pulumi.set(__self__, "decay_rate", decay_rate)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if domain is not None:
+            pulumi.set(__self__, "domain", domain)
+        if host_header is not None:
+            pulumi.set(__self__, "host_header", host_header)
+        if leader_string is not None:
+            pulumi.set(__self__, "leader_string", leader_string)
+        if least_squares_decay is not None:
+            pulumi.set(__self__, "least_squares_decay", least_squares_decay)
+        if load_imbalance_percentage is not None:
+            pulumi.set(__self__, "load_imbalance_percentage", load_imbalance_percentage)
+        if max_u_multiplicative_increment is not None:
+            pulumi.set(__self__, "max_u_multiplicative_increment", max_u_multiplicative_increment)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if resource_instances is not None:
+            pulumi.set(__self__, "resource_instances", resource_instances)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+        if upper_bound is not None:
+            pulumi.set(__self__, "upper_bound", upper_bound)
+        if wait_on_complete is not None:
+            pulumi.set(__self__, "wait_on_complete", wait_on_complete)
 
     @property
-    @pulumi.getter
-    def certificate(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "certificate")
+    @pulumi.getter(name="aggregationType")
+    def aggregation_type(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "aggregation_type")
 
-    @certificate.setter
-    def certificate(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "certificate", value)
+    @aggregation_type.setter
+    def aggregation_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "aggregation_type", value)
 
     @property
-    @pulumi.getter
-    def contract(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-
-        return pulumi.get(self, "contract")
+    @pulumi.getter(name="constrainedProperty")
+    def constrained_property(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "constrained_property")
 
-    @contract.setter
-    def contract(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "contract", value)
+    @constrained_property.setter
+    def constrained_property(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "constrained_property", value)
 
     @property
-    @pulumi.getter(name="contractId")
-    def contract_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "contract_id")
+    @pulumi.getter(name="decayRate")
+    def decay_rate(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "decay_rate")
 
-    @contract_id.setter
-    def contract_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "contract_id", value)
+    @decay_rate.setter
+    def decay_rate(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "decay_rate", value)
 
     @property
-    @pulumi.getter(name="edgeHostname")
-    def edge_hostname(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "edge_hostname")
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "description")
 
-    @edge_hostname.setter
-    def edge_hostname(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "edge_hostname", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
-    def group(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+    def domain(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "domain")
+
+    @domain.setter
+    def domain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "domain", value)
+
+    @property
+    @pulumi.getter(name="hostHeader")
+    def host_header(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "host_header")
+
+    @host_header.setter
+    def host_header(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "host_header", value)
 
-        return pulumi.get(self, "group")
+    @property
+    @pulumi.getter(name="leaderString")
+    def leader_string(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "leader_string")
 
-    @group.setter
-    def group(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group", value)
+    @leader_string.setter
+    def leader_string(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "leader_string", value)
 
     @property
-    @pulumi.getter(name="groupId")
-    def group_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "group_id")
+    @pulumi.getter(name="leastSquaresDecay")
+    def least_squares_decay(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "least_squares_decay")
 
-    @group_id.setter
-    def group_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group_id", value)
+    @least_squares_decay.setter
+    def least_squares_decay(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "least_squares_decay", value)
 
     @property
-    @pulumi.getter(name="ipBehavior")
-    def ip_behavior(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "ip_behavior")
+    @pulumi.getter(name="loadImbalancePercentage")
+    def load_imbalance_percentage(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "load_imbalance_percentage")
 
-    @ip_behavior.setter
-    def ip_behavior(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ip_behavior", value)
+    @load_imbalance_percentage.setter
+    def load_imbalance_percentage(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "load_imbalance_percentage", value)
+
+    @property
+    @pulumi.getter(name="maxUMultiplicativeIncrement")
+    def max_u_multiplicative_increment(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "max_u_multiplicative_increment")
+
+    @max_u_multiplicative_increment.setter
+    def max_u_multiplicative_increment(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "max_u_multiplicative_increment", value)
 
     @property
     @pulumi.getter
-    def product(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
+    def name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "name")
 
-        return pulumi.get(self, "product")
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
-    @product.setter
-    def product(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "product", value)
+    @property
+    @pulumi.getter(name="resourceInstances")
+    def resource_instances(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]:
+        return pulumi.get(self, "resource_instances")
+
+    @resource_instances.setter
+    def resource_instances(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]):
+        pulumi.set(self, "resource_instances", value)
 
     @property
-    @pulumi.getter(name="productId")
-    def product_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "product_id")
+    @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "type")
 
-    @product_id.setter
-    def product_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "product_id", value)
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
 
     @property
-    @pulumi.getter(name="statusUpdateEmails")
-    def status_update_emails(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Email address that should receive updates on the IP behavior update request. Required for update operation.
-        """
-        return pulumi.get(self, "status_update_emails")
+    @pulumi.getter(name="upperBound")
+    def upper_bound(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "upper_bound")
 
-    @status_update_emails.setter
-    def status_update_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "status_update_emails", value)
+    @upper_bound.setter
+    def upper_bound(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "upper_bound", value)
 
     @property
-    @pulumi.getter(name="useCases")
-    def use_cases(self) -> Optional[pulumi.Input[str]]:
-        """
-        A JSON encoded list of use cases
-        """
-        return pulumi.get(self, "use_cases")
+    @pulumi.getter(name="waitOnComplete")
+    def wait_on_complete(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "wait_on_complete")
 
-    @use_cases.setter
-    def use_cases(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "use_cases", value)
+    @wait_on_complete.setter
+    def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "wait_on_complete", value)
 
 
-class EdgeHostName(pulumi.CustomResource):
+class GtmResource(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 certificate: Optional[pulumi.Input[int]] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
-                 contract_id: Optional[pulumi.Input[str]] = None,
-                 edge_hostname: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 group_id: Optional[pulumi.Input[str]] = None,
-                 ip_behavior: Optional[pulumi.Input[str]] = None,
-                 product: Optional[pulumi.Input[str]] = None,
-                 product_id: Optional[pulumi.Input[str]] = None,
-                 status_update_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 use_cases: Optional[pulumi.Input[str]] = None,
+                 aggregation_type: Optional[pulumi.Input[str]] = None,
+                 constrained_property: Optional[pulumi.Input[str]] = None,
+                 decay_rate: Optional[pulumi.Input[float]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 domain: Optional[pulumi.Input[str]] = None,
+                 host_header: Optional[pulumi.Input[str]] = None,
+                 leader_string: Optional[pulumi.Input[str]] = None,
+                 least_squares_decay: Optional[pulumi.Input[float]] = None,
+                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
+                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
+                 upper_bound: Optional[pulumi.Input[int]] = None,
+                 wait_on_complete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        Create a EdgeHostName resource with the given unique name, props, and options.
+        Create a GtmResource resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] status_update_emails: Email address that should receive updates on the IP behavior update request. Required for update operation.
-        :param pulumi.Input[str] use_cases: A JSON encoded list of use cases
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: EdgeHostNameArgs,
+                 args: GtmResourceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a EdgeHostName resource with the given unique name, props, and options.
+        Create a GtmResource resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param EdgeHostNameArgs args: The arguments to use to populate this resource's properties.
+        :param GtmResourceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(EdgeHostNameArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(GtmResourceArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 certificate: Optional[pulumi.Input[int]] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
-                 contract_id: Optional[pulumi.Input[str]] = None,
-                 edge_hostname: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 group_id: Optional[pulumi.Input[str]] = None,
-                 ip_behavior: Optional[pulumi.Input[str]] = None,
-                 product: Optional[pulumi.Input[str]] = None,
-                 product_id: Optional[pulumi.Input[str]] = None,
-                 status_update_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 use_cases: Optional[pulumi.Input[str]] = None,
+                 aggregation_type: Optional[pulumi.Input[str]] = None,
+                 constrained_property: Optional[pulumi.Input[str]] = None,
+                 decay_rate: Optional[pulumi.Input[float]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 domain: Optional[pulumi.Input[str]] = None,
+                 host_header: Optional[pulumi.Input[str]] = None,
+                 leader_string: Optional[pulumi.Input[str]] = None,
+                 least_squares_decay: Optional[pulumi.Input[float]] = None,
+                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
+                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
+                 upper_bound: Optional[pulumi.Input[int]] = None,
+                 wait_on_complete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = EdgeHostNameArgs.__new__(EdgeHostNameArgs)
+            __props__ = GtmResourceArgs.__new__(GtmResourceArgs)
 
-            __props__.__dict__["certificate"] = certificate
-            if contract is not None and not opts.urn:
-                warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-                pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-            __props__.__dict__["contract"] = contract
-            __props__.__dict__["contract_id"] = contract_id
-            if edge_hostname is None and not opts.urn:
-                raise TypeError("Missing required property 'edge_hostname'")
-            __props__.__dict__["edge_hostname"] = edge_hostname
-            if group is not None and not opts.urn:
-                warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-                pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-            __props__.__dict__["group"] = group
-            __props__.__dict__["group_id"] = group_id
-            if ip_behavior is None and not opts.urn:
-                raise TypeError("Missing required property 'ip_behavior'")
-            __props__.__dict__["ip_behavior"] = ip_behavior
-            if product is not None and not opts.urn:
-                warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-                pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
-            __props__.__dict__["product"] = product
-            __props__.__dict__["product_id"] = product_id
-            __props__.__dict__["status_update_emails"] = status_update_emails
-            __props__.__dict__["use_cases"] = use_cases
-        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="akamai:properties/edgeHostName:EdgeHostName")])
+            if aggregation_type is None and not opts.urn:
+                raise TypeError("Missing required property 'aggregation_type'")
+            __props__.__dict__["aggregation_type"] = aggregation_type
+            __props__.__dict__["constrained_property"] = constrained_property
+            __props__.__dict__["decay_rate"] = decay_rate
+            __props__.__dict__["description"] = description
+            if domain is None and not opts.urn:
+                raise TypeError("Missing required property 'domain'")
+            __props__.__dict__["domain"] = domain
+            __props__.__dict__["host_header"] = host_header
+            __props__.__dict__["leader_string"] = leader_string
+            __props__.__dict__["least_squares_decay"] = least_squares_decay
+            __props__.__dict__["load_imbalance_percentage"] = load_imbalance_percentage
+            __props__.__dict__["max_u_multiplicative_increment"] = max_u_multiplicative_increment
+            __props__.__dict__["name"] = name
+            __props__.__dict__["resource_instances"] = resource_instances
+            if type is None and not opts.urn:
+                raise TypeError("Missing required property 'type'")
+            __props__.__dict__["type"] = type
+            __props__.__dict__["upper_bound"] = upper_bound
+            __props__.__dict__["wait_on_complete"] = wait_on_complete
+        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="akamai:trafficmanagement/gtmResource:GtmResource")])
         opts = pulumi.ResourceOptions.merge(opts, alias_opts)
-        super(EdgeHostName, __self__).__init__(
-            'akamai:index/edgeHostName:EdgeHostName',
+        super(GtmResource, __self__).__init__(
+            'akamai:index/gtmResource:GtmResource',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            certificate: Optional[pulumi.Input[int]] = None,
-            contract: Optional[pulumi.Input[str]] = None,
-            contract_id: Optional[pulumi.Input[str]] = None,
-            edge_hostname: Optional[pulumi.Input[str]] = None,
-            group: Optional[pulumi.Input[str]] = None,
-            group_id: Optional[pulumi.Input[str]] = None,
-            ip_behavior: Optional[pulumi.Input[str]] = None,
-            product: Optional[pulumi.Input[str]] = None,
-            product_id: Optional[pulumi.Input[str]] = None,
-            status_update_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            use_cases: Optional[pulumi.Input[str]] = None) -> 'EdgeHostName':
+            aggregation_type: Optional[pulumi.Input[str]] = None,
+            constrained_property: Optional[pulumi.Input[str]] = None,
+            decay_rate: Optional[pulumi.Input[float]] = None,
+            description: Optional[pulumi.Input[str]] = None,
+            domain: Optional[pulumi.Input[str]] = None,
+            host_header: Optional[pulumi.Input[str]] = None,
+            leader_string: Optional[pulumi.Input[str]] = None,
+            least_squares_decay: Optional[pulumi.Input[float]] = None,
+            load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
+            max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
+            type: Optional[pulumi.Input[str]] = None,
+            upper_bound: Optional[pulumi.Input[int]] = None,
+            wait_on_complete: Optional[pulumi.Input[bool]] = None) -> 'GtmResource':
         """
-        Get an existing EdgeHostName resource's state with the given name, id, and optional extra
+        Get an existing GtmResource resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] status_update_emails: Email address that should receive updates on the IP behavior update request. Required for update operation.
-        :param pulumi.Input[str] use_cases: A JSON encoded list of use cases
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _EdgeHostNameState.__new__(_EdgeHostNameState)
+        __props__ = _GtmResourceState.__new__(_GtmResourceState)
 
-        __props__.__dict__["certificate"] = certificate
-        __props__.__dict__["contract"] = contract
-        __props__.__dict__["contract_id"] = contract_id
-        __props__.__dict__["edge_hostname"] = edge_hostname
-        __props__.__dict__["group"] = group
-        __props__.__dict__["group_id"] = group_id
-        __props__.__dict__["ip_behavior"] = ip_behavior
-        __props__.__dict__["product"] = product
-        __props__.__dict__["product_id"] = product_id
-        __props__.__dict__["status_update_emails"] = status_update_emails
-        __props__.__dict__["use_cases"] = use_cases
-        return EdgeHostName(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["aggregation_type"] = aggregation_type
+        __props__.__dict__["constrained_property"] = constrained_property
+        __props__.__dict__["decay_rate"] = decay_rate
+        __props__.__dict__["description"] = description
+        __props__.__dict__["domain"] = domain
+        __props__.__dict__["host_header"] = host_header
+        __props__.__dict__["leader_string"] = leader_string
+        __props__.__dict__["least_squares_decay"] = least_squares_decay
+        __props__.__dict__["load_imbalance_percentage"] = load_imbalance_percentage
+        __props__.__dict__["max_u_multiplicative_increment"] = max_u_multiplicative_increment
+        __props__.__dict__["name"] = name
+        __props__.__dict__["resource_instances"] = resource_instances
+        __props__.__dict__["type"] = type
+        __props__.__dict__["upper_bound"] = upper_bound
+        __props__.__dict__["wait_on_complete"] = wait_on_complete
+        return GtmResource(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def certificate(self) -> pulumi.Output[Optional[int]]:
-        return pulumi.get(self, "certificate")
+    @pulumi.getter(name="aggregationType")
+    def aggregation_type(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "aggregation_type")
 
     @property
-    @pulumi.getter
-    def contract(self) -> pulumi.Output[str]:
-        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-
-        return pulumi.get(self, "contract")
+    @pulumi.getter(name="constrainedProperty")
+    def constrained_property(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "constrained_property")
 
     @property
-    @pulumi.getter(name="contractId")
-    def contract_id(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "contract_id")
+    @pulumi.getter(name="decayRate")
+    def decay_rate(self) -> pulumi.Output[Optional[float]]:
+        return pulumi.get(self, "decay_rate")
 
     @property
-    @pulumi.getter(name="edgeHostname")
-    def edge_hostname(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "edge_hostname")
+    @pulumi.getter
+    def description(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
-    def group(self) -> pulumi.Output[str]:
-        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+    def domain(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "domain")
+
+    @property
+    @pulumi.getter(name="hostHeader")
+    def host_header(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "host_header")
 
-        return pulumi.get(self, "group")
+    @property
+    @pulumi.getter(name="leaderString")
+    def leader_string(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "leader_string")
+
+    @property
+    @pulumi.getter(name="leastSquaresDecay")
+    def least_squares_decay(self) -> pulumi.Output[Optional[float]]:
+        return pulumi.get(self, "least_squares_decay")
 
     @property
-    @pulumi.getter(name="groupId")
-    def group_id(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "group_id")
+    @pulumi.getter(name="loadImbalancePercentage")
+    def load_imbalance_percentage(self) -> pulumi.Output[Optional[float]]:
+        return pulumi.get(self, "load_imbalance_percentage")
 
     @property
-    @pulumi.getter(name="ipBehavior")
-    def ip_behavior(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "ip_behavior")
+    @pulumi.getter(name="maxUMultiplicativeIncrement")
+    def max_u_multiplicative_increment(self) -> pulumi.Output[Optional[float]]:
+        return pulumi.get(self, "max_u_multiplicative_increment")
 
     @property
     @pulumi.getter
-    def product(self) -> pulumi.Output[str]:
-        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
+    def name(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "name")
 
-        return pulumi.get(self, "product")
+    @property
+    @pulumi.getter(name="resourceInstances")
+    def resource_instances(self) -> pulumi.Output[Optional[Sequence['outputs.GtmResourceResourceInstance']]]:
+        return pulumi.get(self, "resource_instances")
 
     @property
-    @pulumi.getter(name="productId")
-    def product_id(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "product_id")
+    @pulumi.getter
+    def type(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "type")
 
     @property
-    @pulumi.getter(name="statusUpdateEmails")
-    def status_update_emails(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        """
-        Email address that should receive updates on the IP behavior update request. Required for update operation.
-        """
-        return pulumi.get(self, "status_update_emails")
+    @pulumi.getter(name="upperBound")
+    def upper_bound(self) -> pulumi.Output[Optional[int]]:
+        return pulumi.get(self, "upper_bound")
 
     @property
-    @pulumi.getter(name="useCases")
-    def use_cases(self) -> pulumi.Output[Optional[str]]:
-        """
-        A JSON encoded list of use cases
-        """
-        return pulumi.get(self, "use_cases")
+    @pulumi.getter(name="waitOnComplete")
+    def wait_on_complete(self) -> pulumi.Output[Optional[bool]]:
+        return pulumi.get(self, "wait_on_complete")
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edge_kv.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edge_kv.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edge_worker.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edge_worker.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edge_workers_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edge_workers_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edgedns/get_authorities_set.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edgedns/get_authorities_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edgedns/get_dns_record_set.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edgedns/get_dns_record_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/edgekv_group_items.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/edgekv_group_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_advanced_settings_logging.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_advanced_settings_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_api_endpoints.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_api_endpoints.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_api_request_constraints.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_api_request_constraints.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_attack_groups.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_attack_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_bypass_network_lists.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_bypass_network_lists.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_configuration.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_configuration_version.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_configuration_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_contracts_groups.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_contracts_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_custom_deny.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_custom_deny.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_custom_rule_actions.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_custom_rule_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_custom_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_custom_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_eval.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_eval.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_eval_groups.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_eval_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_eval_penalty_box.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_eval_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_eval_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_eval_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_export_configuration.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_export_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_failover_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_failover_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_hostname_coverage.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_hostname_coverage.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_ip_geo.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_ip_geo.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 
 @pulumi.output_type
 class GetAppSecIPGeoResult:
     """
     A collection of values returned by getAppSecIPGeo.
     """
-    def __init__(__self__, config_id=None, exception_ip_network_lists=None, geo_network_lists=None, id=None, ip_network_lists=None, mode=None, output_text=None, security_policy_id=None):
+    def __init__(__self__, config_id=None, exception_ip_network_lists=None, geo_network_lists=None, id=None, ip_network_lists=None, mode=None, output_text=None, security_policy_id=None, ukraine_geo_control_action=None):
         if config_id and not isinstance(config_id, int):
             raise TypeError("Expected argument 'config_id' to be a int")
         pulumi.set(__self__, "config_id", config_id)
         if exception_ip_network_lists and not isinstance(exception_ip_network_lists, list):
             raise TypeError("Expected argument 'exception_ip_network_lists' to be a list")
         pulumi.set(__self__, "exception_ip_network_lists", exception_ip_network_lists)
         if geo_network_lists and not isinstance(geo_network_lists, list):
@@ -42,14 +42,17 @@
         pulumi.set(__self__, "mode", mode)
         if output_text and not isinstance(output_text, str):
             raise TypeError("Expected argument 'output_text' to be a str")
         pulumi.set(__self__, "output_text", output_text)
         if security_policy_id and not isinstance(security_policy_id, str):
             raise TypeError("Expected argument 'security_policy_id' to be a str")
         pulumi.set(__self__, "security_policy_id", security_policy_id)
+        if ukraine_geo_control_action and not isinstance(ukraine_geo_control_action, str):
+            raise TypeError("Expected argument 'ukraine_geo_control_action' to be a str")
+        pulumi.set(__self__, "ukraine_geo_control_action", ukraine_geo_control_action)
 
     @property
     @pulumi.getter(name="configId")
     def config_id(self) -> int:
         return pulumi.get(self, "config_id")
 
     @property
@@ -86,29 +89,35 @@
         return pulumi.get(self, "output_text")
 
     @property
     @pulumi.getter(name="securityPolicyId")
     def security_policy_id(self) -> str:
         return pulumi.get(self, "security_policy_id")
 
+    @property
+    @pulumi.getter(name="ukraineGeoControlAction")
+    def ukraine_geo_control_action(self) -> str:
+        return pulumi.get(self, "ukraine_geo_control_action")
+
 
 class AwaitableGetAppSecIPGeoResult(GetAppSecIPGeoResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetAppSecIPGeoResult(
             config_id=self.config_id,
             exception_ip_network_lists=self.exception_ip_network_lists,
             geo_network_lists=self.geo_network_lists,
             id=self.id,
             ip_network_lists=self.ip_network_lists,
             mode=self.mode,
             output_text=self.output_text,
-            security_policy_id=self.security_policy_id)
+            security_policy_id=self.security_policy_id,
+            ukraine_geo_control_action=self.ukraine_geo_control_action)
 
 
 def get_app_sec_ip_geo(config_id: Optional[int] = None,
                        security_policy_id: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAppSecIPGeoResult:
     """
     Use this data source to access information about an existing resource.
@@ -123,15 +132,16 @@
         config_id=pulumi.get(__ret__, 'config_id'),
         exception_ip_network_lists=pulumi.get(__ret__, 'exception_ip_network_lists'),
         geo_network_lists=pulumi.get(__ret__, 'geo_network_lists'),
         id=pulumi.get(__ret__, 'id'),
         ip_network_lists=pulumi.get(__ret__, 'ip_network_lists'),
         mode=pulumi.get(__ret__, 'mode'),
         output_text=pulumi.get(__ret__, 'output_text'),
-        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'),
+        ukraine_geo_control_action=pulumi.get(__ret__, 'ukraine_geo_control_action'))
 
 
 @_utilities.lift_output_func(get_app_sec_ip_geo)
 def get_app_sec_ip_geo_output(config_id: Optional[pulumi.Input[int]] = None,
                               security_policy_id: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecIPGeoResult]:
     """
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_malware_content_types.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_malware_content_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_malware_policies.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_malware_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_malware_policy_actions.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_malware_policy_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_match_targets.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_match_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_penalty_box.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_rate_policies.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_rate_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_rate_policy_actions.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_rate_policy_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_reputation_profile_actions.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_reputation_profile_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_reputation_profile_analysis.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_reputation_profile_analysis.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_reputation_profiles.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_reputation_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_rule_upgrade_details.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_rule_upgrade_details.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_security_policy.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_security_policy_protections.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_security_policy_protections.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_selectable_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_selectable_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_selected_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_siem_definitions.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_siem_definitions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_siem_settings.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_siem_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_slow_post.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_slow_post.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_threat_intel.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_threat_intel.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_tuning_recommendations.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_tuning_recommendations.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_version_notes.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_version_notes.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_waf_mode.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_waf_mode.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_app_sec_wap_selected_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_app_sec_wap_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_appsec_advanced_settings_request_body.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_appsec_advanced_settings_request_body.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_authorities_set.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_authorities_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_akamai_bot_category.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_akamai_bot_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_akamai_bot_category_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_akamai_bot_category_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_akamai_defined_bot.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_akamai_defined_bot.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_analytics_cookie.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_analytics_cookie.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_analytics_cookie_values.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_analytics_cookie_values.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_category_exception.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_category_exception.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_detection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_detection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_detection_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_detection_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_endpoint_coverage_report.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_endpoint_coverage_report.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_bot_management_settings.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_bot_management_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_challenge_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_challenge_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_challenge_interception_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_challenge_interception_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_client_side_security.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_client_side_security.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_conditional_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_conditional_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_custom_bot_category.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_bot_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_custom_bot_category_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_bot_category_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_custom_bot_category_sequence.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_bot_category_sequence.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_custom_client.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_custom_defined_bot.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_defined_bot.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_custom_deny_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_custom_deny_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_javascript_injection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_javascript_injection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_recategorized_akamai_defined_bot.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_recategorized_akamai_defined_bot.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_response_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_response_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_serve_alternate_action.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_serve_alternate_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_transactional_endpoint.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_transactional_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_botman_transactional_endpoint_protection.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_botman_transactional_endpoint_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_application_load_balancer.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_application_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_phased_release_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_phased_release_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_policy.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_request_control_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_request_control_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_contract.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_properties.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,103 +4,98 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
 
 __all__ = [
-    'GetContractResult',
-    'AwaitableGetContractResult',
-    'get_contract',
-    'get_contract_output',
+    'GetPropertiesResult',
+    'AwaitableGetPropertiesResult',
+    'get_properties',
+    'get_properties_output',
 ]
 
 @pulumi.output_type
-class GetContractResult:
+class GetPropertiesResult:
     """
-    A collection of values returned by getContract.
+    A collection of values returned by getProperties.
     """
-    def __init__(__self__, group=None, group_id=None, group_name=None, id=None):
-        if group and not isinstance(group, str):
-            raise TypeError("Expected argument 'group' to be a str")
-        pulumi.set(__self__, "group", group)
+    def __init__(__self__, contract_id=None, group_id=None, id=None, properties=None):
+        if contract_id and not isinstance(contract_id, str):
+            raise TypeError("Expected argument 'contract_id' to be a str")
+        pulumi.set(__self__, "contract_id", contract_id)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
-        if group_name and not isinstance(group_name, str):
-            raise TypeError("Expected argument 'group_name' to be a str")
-        pulumi.set(__self__, "group_name", group_name)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if properties and not isinstance(properties, list):
+            raise TypeError("Expected argument 'properties' to be a list")
+        pulumi.set(__self__, "properties", properties)
 
     @property
-    @pulumi.getter
-    def group(self) -> Optional[str]:
-        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-
-        return pulumi.get(self, "group")
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> str:
+        return pulumi.get(self, "contract_id")
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> str:
         return pulumi.get(self, "group_id")
 
     @property
-    @pulumi.getter(name="groupName")
-    def group_name(self) -> str:
-        return pulumi.get(self, "group_name")
-
-    @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
+    @property
+    @pulumi.getter
+    def properties(self) -> Sequence['outputs.GetPropertiesPropertyResult']:
+        return pulumi.get(self, "properties")
+
 
-class AwaitableGetContractResult(GetContractResult):
+class AwaitableGetPropertiesResult(GetPropertiesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetContractResult(
-            group=self.group,
+        return GetPropertiesResult(
+            contract_id=self.contract_id,
             group_id=self.group_id,
-            group_name=self.group_name,
-            id=self.id)
+            id=self.id,
+            properties=self.properties)
 
 
-def get_contract(group: Optional[str] = None,
-                 group_id: Optional[str] = None,
-                 group_name: Optional[str] = None,
-                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetContractResult:
+def get_properties(contract_id: Optional[str] = None,
+                   group_id: Optional[str] = None,
+                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertiesResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
-    __args__['group'] = group
+    __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
-    __args__['groupName'] = group_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getContract:getContract', __args__, opts=opts, typ=GetContractResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getProperties:getProperties', __args__, opts=opts, typ=GetPropertiesResult).value
 
-    return AwaitableGetContractResult(
-        group=pulumi.get(__ret__, 'group'),
+    return AwaitableGetPropertiesResult(
+        contract_id=pulumi.get(__ret__, 'contract_id'),
         group_id=pulumi.get(__ret__, 'group_id'),
-        group_name=pulumi.get(__ret__, 'group_name'),
-        id=pulumi.get(__ret__, 'id'))
+        id=pulumi.get(__ret__, 'id'),
+        properties=pulumi.get(__ret__, 'properties'))
 
 
-@_utilities.lift_output_func(get_contract)
-def get_contract_output(group: Optional[pulumi.Input[Optional[str]]] = None,
-                        group_id: Optional[pulumi.Input[Optional[str]]] = None,
-                        group_name: Optional[pulumi.Input[Optional[str]]] = None,
-                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetContractResult]:
+@_utilities.lift_output_func(get_properties)
+def get_properties_output(contract_id: Optional[pulumi.Input[str]] = None,
+                          group_id: Optional[pulumi.Input[str]] = None,
+                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertiesResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_contracts.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_contracts.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cp_code.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_include.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,140 +6,145 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetCpCodeResult',
-    'AwaitableGetCpCodeResult',
-    'get_cp_code',
-    'get_cp_code_output',
+    'GetPropertyIncludeResult',
+    'AwaitableGetPropertyIncludeResult',
+    'get_property_include',
+    'get_property_include_output',
 ]
 
 @pulumi.output_type
-class GetCpCodeResult:
+class GetPropertyIncludeResult:
     """
-    A collection of values returned by getCpCode.
+    A collection of values returned by getPropertyInclude.
     """
-    def __init__(__self__, contract=None, contract_id=None, group=None, group_id=None, id=None, name=None, product_ids=None):
-        if contract and not isinstance(contract, str):
-            raise TypeError("Expected argument 'contract' to be a str")
-        pulumi.set(__self__, "contract", contract)
+    def __init__(__self__, contract_id=None, group_id=None, id=None, include_id=None, latest_version=None, name=None, production_version=None, staging_version=None, type=None):
         if contract_id and not isinstance(contract_id, str):
             raise TypeError("Expected argument 'contract_id' to be a str")
         pulumi.set(__self__, "contract_id", contract_id)
-        if group and not isinstance(group, str):
-            raise TypeError("Expected argument 'group' to be a str")
-        pulumi.set(__self__, "group", group)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if include_id and not isinstance(include_id, str):
+            raise TypeError("Expected argument 'include_id' to be a str")
+        pulumi.set(__self__, "include_id", include_id)
+        if latest_version and not isinstance(latest_version, int):
+            raise TypeError("Expected argument 'latest_version' to be a int")
+        pulumi.set(__self__, "latest_version", latest_version)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
-        if product_ids and not isinstance(product_ids, list):
-            raise TypeError("Expected argument 'product_ids' to be a list")
-        pulumi.set(__self__, "product_ids", product_ids)
-
-    @property
-    @pulumi.getter
-    def contract(self) -> str:
-        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-
-        return pulumi.get(self, "contract")
+        if production_version and not isinstance(production_version, int):
+            raise TypeError("Expected argument 'production_version' to be a int")
+        pulumi.set(__self__, "production_version", production_version)
+        if staging_version and not isinstance(staging_version, int):
+            raise TypeError("Expected argument 'staging_version' to be a int")
+        pulumi.set(__self__, "staging_version", staging_version)
+        if type and not isinstance(type, str):
+            raise TypeError("Expected argument 'type' to be a str")
+        pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> str:
         return pulumi.get(self, "contract_id")
 
     @property
-    @pulumi.getter
-    def group(self) -> str:
-        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-
-        return pulumi.get(self, "group")
-
-    @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> str:
         return pulumi.get(self, "group_id")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="includeId")
+    def include_id(self) -> str:
+        return pulumi.get(self, "include_id")
+
+    @property
+    @pulumi.getter(name="latestVersion")
+    def latest_version(self) -> int:
+        return pulumi.get(self, "latest_version")
+
+    @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="productIds")
-    def product_ids(self) -> Sequence[str]:
-        return pulumi.get(self, "product_ids")
+    @pulumi.getter(name="productionVersion")
+    def production_version(self) -> int:
+        return pulumi.get(self, "production_version")
+
+    @property
+    @pulumi.getter(name="stagingVersion")
+    def staging_version(self) -> int:
+        return pulumi.get(self, "staging_version")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        return pulumi.get(self, "type")
 
 
-class AwaitableGetCpCodeResult(GetCpCodeResult):
+class AwaitableGetPropertyIncludeResult(GetPropertyIncludeResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetCpCodeResult(
-            contract=self.contract,
+        return GetPropertyIncludeResult(
             contract_id=self.contract_id,
-            group=self.group,
             group_id=self.group_id,
             id=self.id,
+            include_id=self.include_id,
+            latest_version=self.latest_version,
             name=self.name,
-            product_ids=self.product_ids)
+            production_version=self.production_version,
+            staging_version=self.staging_version,
+            type=self.type)
 
 
-def get_cp_code(contract: Optional[str] = None,
-                contract_id: Optional[str] = None,
-                group: Optional[str] = None,
-                group_id: Optional[str] = None,
-                name: Optional[str] = None,
-                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCpCodeResult:
+def get_property_include(contract_id: Optional[str] = None,
+                         group_id: Optional[str] = None,
+                         include_id: Optional[str] = None,
+                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyIncludeResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
-    __args__['contract'] = contract
     __args__['contractId'] = contract_id
-    __args__['group'] = group
     __args__['groupId'] = group_id
-    __args__['name'] = name
+    __args__['includeId'] = include_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getCpCode:getCpCode', __args__, opts=opts, typ=GetCpCodeResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyInclude:getPropertyInclude', __args__, opts=opts, typ=GetPropertyIncludeResult).value
 
-    return AwaitableGetCpCodeResult(
-        contract=pulumi.get(__ret__, 'contract'),
+    return AwaitableGetPropertyIncludeResult(
         contract_id=pulumi.get(__ret__, 'contract_id'),
-        group=pulumi.get(__ret__, 'group'),
         group_id=pulumi.get(__ret__, 'group_id'),
         id=pulumi.get(__ret__, 'id'),
+        include_id=pulumi.get(__ret__, 'include_id'),
+        latest_version=pulumi.get(__ret__, 'latest_version'),
         name=pulumi.get(__ret__, 'name'),
-        product_ids=pulumi.get(__ret__, 'product_ids'))
+        production_version=pulumi.get(__ret__, 'production_version'),
+        staging_version=pulumi.get(__ret__, 'staging_version'),
+        type=pulumi.get(__ret__, 'type'))
 
 
-@_utilities.lift_output_func(get_cp_code)
-def get_cp_code_output(contract: Optional[pulumi.Input[Optional[str]]] = None,
-                       contract_id: Optional[pulumi.Input[Optional[str]]] = None,
-                       group: Optional[pulumi.Input[Optional[str]]] = None,
-                       group_id: Optional[pulumi.Input[Optional[str]]] = None,
-                       name: Optional[pulumi.Input[str]] = None,
-                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCpCodeResult]:
+@_utilities.lift_output_func(get_property_include)
+def get_property_include_output(contract_id: Optional[pulumi.Input[str]] = None,
+                                group_id: Optional[pulumi.Input[str]] = None,
+                                include_id: Optional[pulumi.Input[str]] = None,
+                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyIncludeResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cps_csr.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_csr.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cps_deployments.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_deployments.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cps_enrollment.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cps_enrollments.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_enrollments.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_cps_warnings.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cps_warnings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_datastream_activation_history.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_datastream_activation_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_datastream_dataset_fields.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_datastream_dataset_fields.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,71 +18,71 @@
 ]
 
 @pulumi.output_type
 class GetDatastreamDatasetFieldsResult:
     """
     A collection of values returned by getDatastreamDatasetFields.
     """
-    def __init__(__self__, fields=None, id=None, template_name=None):
-        if fields and not isinstance(fields, list):
-            raise TypeError("Expected argument 'fields' to be a list")
-        pulumi.set(__self__, "fields", fields)
+    def __init__(__self__, dataset_fields=None, id=None, product_id=None):
+        if dataset_fields and not isinstance(dataset_fields, list):
+            raise TypeError("Expected argument 'dataset_fields' to be a list")
+        pulumi.set(__self__, "dataset_fields", dataset_fields)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if template_name and not isinstance(template_name, str):
-            raise TypeError("Expected argument 'template_name' to be a str")
-        pulumi.set(__self__, "template_name", template_name)
+        if product_id and not isinstance(product_id, str):
+            raise TypeError("Expected argument 'product_id' to be a str")
+        pulumi.set(__self__, "product_id", product_id)
 
     @property
-    @pulumi.getter
-    def fields(self) -> Sequence['outputs.GetDatastreamDatasetFieldsFieldResult']:
-        return pulumi.get(self, "fields")
+    @pulumi.getter(name="datasetFields")
+    def dataset_fields(self) -> Sequence['outputs.GetDatastreamDatasetFieldsDatasetFieldResult']:
+        return pulumi.get(self, "dataset_fields")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="templateName")
-    def template_name(self) -> Optional[str]:
-        return pulumi.get(self, "template_name")
+    @pulumi.getter(name="productId")
+    def product_id(self) -> Optional[str]:
+        return pulumi.get(self, "product_id")
 
 
 class AwaitableGetDatastreamDatasetFieldsResult(GetDatastreamDatasetFieldsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetDatastreamDatasetFieldsResult(
-            fields=self.fields,
+            dataset_fields=self.dataset_fields,
             id=self.id,
-            template_name=self.template_name)
+            product_id=self.product_id)
 
 
-def get_datastream_dataset_fields(template_name: Optional[str] = None,
+def get_datastream_dataset_fields(product_id: Optional[str] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatastreamDatasetFieldsResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
-    __args__['templateName'] = template_name
+    __args__['productId'] = product_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getDatastreamDatasetFields:getDatastreamDatasetFields', __args__, opts=opts, typ=GetDatastreamDatasetFieldsResult).value
 
     return AwaitableGetDatastreamDatasetFieldsResult(
-        fields=pulumi.get(__ret__, 'fields'),
+        dataset_fields=pulumi.get(__ret__, 'dataset_fields'),
         id=pulumi.get(__ret__, 'id'),
-        template_name=pulumi.get(__ret__, 'template_name'))
+        product_id=pulumi.get(__ret__, 'product_id'))
 
 
 @_utilities.lift_output_func(get_datastream_dataset_fields)
-def get_datastream_dataset_fields_output(template_name: Optional[pulumi.Input[Optional[str]]] = None,
+def get_datastream_dataset_fields_output(product_id: Optional[pulumi.Input[Optional[str]]] = None,
                                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatastreamDatasetFieldsResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_datastreams.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_datastreams.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,71 +18,71 @@
 ]
 
 @pulumi.output_type
 class GetDatastreamsResult:
     """
     A collection of values returned by getDatastreams.
     """
-    def __init__(__self__, group_id=None, id=None, streams=None):
-        if group_id and not isinstance(group_id, str):
-            raise TypeError("Expected argument 'group_id' to be a str")
+    def __init__(__self__, group_id=None, id=None, streams_details=None):
+        if group_id and not isinstance(group_id, int):
+            raise TypeError("Expected argument 'group_id' to be a int")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if streams and not isinstance(streams, list):
-            raise TypeError("Expected argument 'streams' to be a list")
-        pulumi.set(__self__, "streams", streams)
+        if streams_details and not isinstance(streams_details, list):
+            raise TypeError("Expected argument 'streams_details' to be a list")
+        pulumi.set(__self__, "streams_details", streams_details)
 
     @property
     @pulumi.getter(name="groupId")
-    def group_id(self) -> Optional[str]:
+    def group_id(self) -> Optional[int]:
         return pulumi.get(self, "group_id")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter
-    def streams(self) -> Sequence['outputs.GetDatastreamsStreamResult']:
-        return pulumi.get(self, "streams")
+    @pulumi.getter(name="streamsDetails")
+    def streams_details(self) -> Sequence['outputs.GetDatastreamsStreamsDetailResult']:
+        return pulumi.get(self, "streams_details")
 
 
 class AwaitableGetDatastreamsResult(GetDatastreamsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetDatastreamsResult(
             group_id=self.group_id,
             id=self.id,
-            streams=self.streams)
+            streams_details=self.streams_details)
 
 
-def get_datastreams(group_id: Optional[str] = None,
+def get_datastreams(group_id: Optional[int] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatastreamsResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     __args__['groupId'] = group_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getDatastreams:getDatastreams', __args__, opts=opts, typ=GetDatastreamsResult).value
 
     return AwaitableGetDatastreamsResult(
         group_id=pulumi.get(__ret__, 'group_id'),
         id=pulumi.get(__ret__, 'id'),
-        streams=pulumi.get(__ret__, 'streams'))
+        streams_details=pulumi.get(__ret__, 'streams_details'))
 
 
 @_utilities.lift_output_func(get_datastreams)
-def get_datastreams_output(group_id: Optional[pulumi.Input[Optional[str]]] = None,
+def get_datastreams_output(group_id: Optional[pulumi.Input[Optional[int]]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatastreamsResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_dns_record_set.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_dns_record_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_edge_worker.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edge_worker.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_edge_worker_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edge_worker_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_edge_workers_property_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edge_workers_property_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_edge_workers_resource_tier.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edge_workers_resource_tier.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_edgekv_group_items.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edgekv_group_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_edgekv_groups.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_edgekv_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_group.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_hostnames.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,119 +4,121 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
 
 __all__ = [
-    'GetGroupResult',
-    'AwaitableGetGroupResult',
-    'get_group',
-    'get_group_output',
+    'GetPropertyHostnamesResult',
+    'AwaitableGetPropertyHostnamesResult',
+    'get_property_hostnames',
+    'get_property_hostnames_output',
 ]
 
 @pulumi.output_type
-class GetGroupResult:
+class GetPropertyHostnamesResult:
     """
-    A collection of values returned by getGroup.
+    A collection of values returned by getPropertyHostnames.
     """
-    def __init__(__self__, contract=None, contract_id=None, group_name=None, id=None, name=None):
-        if contract and not isinstance(contract, str):
-            raise TypeError("Expected argument 'contract' to be a str")
-        pulumi.set(__self__, "contract", contract)
+    def __init__(__self__, contract_id=None, group_id=None, hostnames=None, id=None, property_id=None, version=None):
         if contract_id and not isinstance(contract_id, str):
             raise TypeError("Expected argument 'contract_id' to be a str")
         pulumi.set(__self__, "contract_id", contract_id)
-        if group_name and not isinstance(group_name, str):
-            raise TypeError("Expected argument 'group_name' to be a str")
-        pulumi.set(__self__, "group_name", group_name)
+        if group_id and not isinstance(group_id, str):
+            raise TypeError("Expected argument 'group_id' to be a str")
+        pulumi.set(__self__, "group_id", group_id)
+        if hostnames and not isinstance(hostnames, list):
+            raise TypeError("Expected argument 'hostnames' to be a list")
+        pulumi.set(__self__, "hostnames", hostnames)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if name and not isinstance(name, str):
-            raise TypeError("Expected argument 'name' to be a str")
-        pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter
-    def contract(self) -> str:
-        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-
-        return pulumi.get(self, "contract")
+        if property_id and not isinstance(property_id, str):
+            raise TypeError("Expected argument 'property_id' to be a str")
+        pulumi.set(__self__, "property_id", property_id)
+        if version and not isinstance(version, int):
+            raise TypeError("Expected argument 'version' to be a int")
+        pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> str:
         return pulumi.get(self, "contract_id")
 
     @property
-    @pulumi.getter(name="groupName")
-    def group_name(self) -> str:
-        return pulumi.get(self, "group_name")
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> str:
+        return pulumi.get(self, "group_id")
+
+    @property
+    @pulumi.getter
+    def hostnames(self) -> Sequence['outputs.GetPropertyHostnamesHostnameResult']:
+        return pulumi.get(self, "hostnames")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter
-    def name(self) -> str:
-        warnings.warn("""The setting \"name\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""name is deprecated: The setting \"name\" has been deprecated.""")
+    @pulumi.getter(name="propertyId")
+    def property_id(self) -> str:
+        return pulumi.get(self, "property_id")
 
-        return pulumi.get(self, "name")
+    @property
+    @pulumi.getter
+    def version(self) -> int:
+        return pulumi.get(self, "version")
 
 
-class AwaitableGetGroupResult(GetGroupResult):
+class AwaitableGetPropertyHostnamesResult(GetPropertyHostnamesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetGroupResult(
-            contract=self.contract,
+        return GetPropertyHostnamesResult(
             contract_id=self.contract_id,
-            group_name=self.group_name,
+            group_id=self.group_id,
+            hostnames=self.hostnames,
             id=self.id,
-            name=self.name)
+            property_id=self.property_id,
+            version=self.version)
 
 
-def get_group(contract: Optional[str] = None,
-              contract_id: Optional[str] = None,
-              group_name: Optional[str] = None,
-              name: Optional[str] = None,
-              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGroupResult:
+def get_property_hostnames(contract_id: Optional[str] = None,
+                           group_id: Optional[str] = None,
+                           property_id: Optional[str] = None,
+                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyHostnamesResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
-    __args__['contract'] = contract
     __args__['contractId'] = contract_id
-    __args__['groupName'] = group_name
-    __args__['name'] = name
+    __args__['groupId'] = group_id
+    __args__['propertyId'] = property_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getGroup:getGroup', __args__, opts=opts, typ=GetGroupResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyHostnames:getPropertyHostnames', __args__, opts=opts, typ=GetPropertyHostnamesResult).value
 
-    return AwaitableGetGroupResult(
-        contract=pulumi.get(__ret__, 'contract'),
+    return AwaitableGetPropertyHostnamesResult(
         contract_id=pulumi.get(__ret__, 'contract_id'),
-        group_name=pulumi.get(__ret__, 'group_name'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        hostnames=pulumi.get(__ret__, 'hostnames'),
         id=pulumi.get(__ret__, 'id'),
-        name=pulumi.get(__ret__, 'name'))
+        property_id=pulumi.get(__ret__, 'property_id'),
+        version=pulumi.get(__ret__, 'version'))
 
 
-@_utilities.lift_output_func(get_group)
-def get_group_output(contract: Optional[pulumi.Input[Optional[str]]] = None,
-                     contract_id: Optional[pulumi.Input[Optional[str]]] = None,
-                     group_name: Optional[pulumi.Input[Optional[str]]] = None,
-                     name: Optional[pulumi.Input[Optional[str]]] = None,
-                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupResult]:
+@_utilities.lift_output_func(get_property_hostnames)
+def get_property_hostnames_output(contract_id: Optional[pulumi.Input[str]] = None,
+                                  group_id: Optional[pulumi.Input[str]] = None,
+                                  property_id: Optional[pulumi.Input[str]] = None,
+                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyHostnamesResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_groups.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_gtm_datacenter.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_gtm_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_gtm_datacenters.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_gtm_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_gtm_default_datacenter.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_gtm_default_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_contact_types.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_contact_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_countries.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_countries.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_grantable_roles.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_grantable_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_roles.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_states.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_states.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_supported_langs.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_supported_langs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_timeout_policies.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_timeout_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_iam_timezones.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_iam_timezones.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_network_lists.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_network_lists.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_properties.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,98 +4,97 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
-from . import outputs
 
 __all__ = [
-    'GetPropertiesResult',
-    'AwaitableGetPropertiesResult',
-    'get_properties',
-    'get_properties_output',
+    'GetPropertyResult',
+    'AwaitableGetPropertyResult',
+    'get_property',
+    'get_property_output',
 ]
 
 @pulumi.output_type
-class GetPropertiesResult:
+class GetPropertyResult:
     """
-    A collection of values returned by getProperties.
+    A collection of values returned by getProperty.
     """
-    def __init__(__self__, contract_id=None, group_id=None, id=None, properties=None):
-        if contract_id and not isinstance(contract_id, str):
-            raise TypeError("Expected argument 'contract_id' to be a str")
-        pulumi.set(__self__, "contract_id", contract_id)
-        if group_id and not isinstance(group_id, str):
-            raise TypeError("Expected argument 'group_id' to be a str")
-        pulumi.set(__self__, "group_id", group_id)
+    def __init__(__self__, id=None, name=None, rules=None, version=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if properties and not isinstance(properties, list):
-            raise TypeError("Expected argument 'properties' to be a list")
-        pulumi.set(__self__, "properties", properties)
-
-    @property
-    @pulumi.getter(name="contractId")
-    def contract_id(self) -> str:
-        return pulumi.get(self, "contract_id")
-
-    @property
-    @pulumi.getter(name="groupId")
-    def group_id(self) -> str:
-        return pulumi.get(self, "group_id")
+        if name and not isinstance(name, str):
+            raise TypeError("Expected argument 'name' to be a str")
+        pulumi.set(__self__, "name", name)
+        if rules and not isinstance(rules, str):
+            raise TypeError("Expected argument 'rules' to be a str")
+        pulumi.set(__self__, "rules", rules)
+        if version and not isinstance(version, int):
+            raise TypeError("Expected argument 'version' to be a int")
+        pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def properties(self) -> Sequence['outputs.GetPropertiesPropertyResult']:
-        return pulumi.get(self, "properties")
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def rules(self) -> str:
+        return pulumi.get(self, "rules")
+
+    @property
+    @pulumi.getter
+    def version(self) -> Optional[int]:
+        return pulumi.get(self, "version")
 
 
-class AwaitableGetPropertiesResult(GetPropertiesResult):
+class AwaitableGetPropertyResult(GetPropertyResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPropertiesResult(
-            contract_id=self.contract_id,
-            group_id=self.group_id,
+        return GetPropertyResult(
             id=self.id,
-            properties=self.properties)
+            name=self.name,
+            rules=self.rules,
+            version=self.version)
 
 
-def get_properties(contract_id: Optional[str] = None,
-                   group_id: Optional[str] = None,
-                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertiesResult:
+def get_property(name: Optional[str] = None,
+                 version: Optional[int] = None,
+                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
-    __args__['contractId'] = contract_id
-    __args__['groupId'] = group_id
+    __args__['name'] = name
+    __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getProperties:getProperties', __args__, opts=opts, typ=GetPropertiesResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getProperty:getProperty', __args__, opts=opts, typ=GetPropertyResult).value
 
-    return AwaitableGetPropertiesResult(
-        contract_id=pulumi.get(__ret__, 'contract_id'),
-        group_id=pulumi.get(__ret__, 'group_id'),
+    return AwaitableGetPropertyResult(
         id=pulumi.get(__ret__, 'id'),
-        properties=pulumi.get(__ret__, 'properties'))
+        name=pulumi.get(__ret__, 'name'),
+        rules=pulumi.get(__ret__, 'rules'),
+        version=pulumi.get(__ret__, 'version'))
 
 
-@_utilities.lift_output_func(get_properties)
-def get_properties_output(contract_id: Optional[pulumi.Input[str]] = None,
-                          group_id: Optional[pulumi.Input[str]] = None,
-                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertiesResult]:
+@_utilities.lift_output_func(get_property)
+def get_property_output(name: Optional[pulumi.Input[str]] = None,
+                        version: Optional[pulumi.Input[Optional[int]]] = None,
+                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_properties_search.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_properties_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/get_property.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
 __all__ = [
     'GetPropertyResult',
     'AwaitableGetPropertyResult',
     'get_property',
     'get_property_output',
 ]
 
+warnings.warn("""akamai.properties/getproperty.getProperty has been deprecated in favor of akamai.index/getproperty.getProperty""", DeprecationWarning)
+
 @pulumi.output_type
 class GetPropertyResult:
     """
     A collection of values returned by getProperty.
     """
     def __init__(__self__, id=None, name=None, rules=None, version=None):
         if id and not isinstance(id, str):
@@ -73,19 +75,20 @@
 
 def get_property(name: Optional[str] = None,
                  version: Optional[int] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyResult:
     """
     Use this data source to access information about an existing resource.
     """
+    pulumi.log.warn("""get_property is deprecated: akamai.properties/getproperty.getProperty has been deprecated in favor of akamai.index/getproperty.getProperty""")
     __args__ = dict()
     __args__['name'] = name
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getProperty:getProperty', __args__, opts=opts, typ=GetPropertyResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:properties/getProperty:getProperty', __args__, opts=opts, typ=GetPropertyResult).value
 
     return AwaitableGetPropertyResult(
         id=pulumi.get(__ret__, 'id'),
         name=pulumi.get(__ret__, 'name'),
         rules=pulumi.get(__ret__, 'rules'),
         version=pulumi.get(__ret__, 'version'))
 
@@ -93,8 +96,9 @@
 @_utilities.lift_output_func(get_property)
 def get_property_output(name: Optional[pulumi.Input[str]] = None,
                         version: Optional[pulumi.Input[Optional[int]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyResult]:
     """
     Use this data source to access information about an existing resource.
     """
+    pulumi.log.warn("""get_property is deprecated: akamai.properties/getproperty.getProperty has been deprecated in favor of akamai.index/getproperty.getProperty""")
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_hostnames.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_include_parents.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,118 +7,108 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
-    'GetPropertyHostnamesResult',
-    'AwaitableGetPropertyHostnamesResult',
-    'get_property_hostnames',
-    'get_property_hostnames_output',
+    'GetPropertyIncludeParentsResult',
+    'AwaitableGetPropertyIncludeParentsResult',
+    'get_property_include_parents',
+    'get_property_include_parents_output',
 ]
 
 @pulumi.output_type
-class GetPropertyHostnamesResult:
+class GetPropertyIncludeParentsResult:
     """
-    A collection of values returned by getPropertyHostnames.
+    A collection of values returned by getPropertyIncludeParents.
     """
-    def __init__(__self__, contract_id=None, group_id=None, hostnames=None, id=None, property_id=None, version=None):
+    def __init__(__self__, contract_id=None, group_id=None, id=None, include_id=None, parents=None):
         if contract_id and not isinstance(contract_id, str):
             raise TypeError("Expected argument 'contract_id' to be a str")
         pulumi.set(__self__, "contract_id", contract_id)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
-        if hostnames and not isinstance(hostnames, list):
-            raise TypeError("Expected argument 'hostnames' to be a list")
-        pulumi.set(__self__, "hostnames", hostnames)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if property_id and not isinstance(property_id, str):
-            raise TypeError("Expected argument 'property_id' to be a str")
-        pulumi.set(__self__, "property_id", property_id)
-        if version and not isinstance(version, int):
-            raise TypeError("Expected argument 'version' to be a int")
-        pulumi.set(__self__, "version", version)
+        if include_id and not isinstance(include_id, str):
+            raise TypeError("Expected argument 'include_id' to be a str")
+        pulumi.set(__self__, "include_id", include_id)
+        if parents and not isinstance(parents, list):
+            raise TypeError("Expected argument 'parents' to be a list")
+        pulumi.set(__self__, "parents", parents)
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> str:
         return pulumi.get(self, "contract_id")
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> str:
         return pulumi.get(self, "group_id")
 
     @property
     @pulumi.getter
-    def hostnames(self) -> Sequence['outputs.GetPropertyHostnamesHostnameResult']:
-        return pulumi.get(self, "hostnames")
-
-    @property
-    @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="propertyId")
-    def property_id(self) -> str:
-        return pulumi.get(self, "property_id")
+    @pulumi.getter(name="includeId")
+    def include_id(self) -> str:
+        return pulumi.get(self, "include_id")
 
     @property
     @pulumi.getter
-    def version(self) -> int:
-        return pulumi.get(self, "version")
+    def parents(self) -> Sequence['outputs.GetPropertyIncludeParentsParentResult']:
+        return pulumi.get(self, "parents")
 
 
-class AwaitableGetPropertyHostnamesResult(GetPropertyHostnamesResult):
+class AwaitableGetPropertyIncludeParentsResult(GetPropertyIncludeParentsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPropertyHostnamesResult(
+        return GetPropertyIncludeParentsResult(
             contract_id=self.contract_id,
             group_id=self.group_id,
-            hostnames=self.hostnames,
             id=self.id,
-            property_id=self.property_id,
-            version=self.version)
+            include_id=self.include_id,
+            parents=self.parents)
 
 
-def get_property_hostnames(contract_id: Optional[str] = None,
-                           group_id: Optional[str] = None,
-                           property_id: Optional[str] = None,
-                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyHostnamesResult:
+def get_property_include_parents(contract_id: Optional[str] = None,
+                                 group_id: Optional[str] = None,
+                                 include_id: Optional[str] = None,
+                                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyIncludeParentsResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
-    __args__['propertyId'] = property_id
+    __args__['includeId'] = include_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyHostnames:getPropertyHostnames', __args__, opts=opts, typ=GetPropertyHostnamesResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyIncludeParents:getPropertyIncludeParents', __args__, opts=opts, typ=GetPropertyIncludeParentsResult).value
 
-    return AwaitableGetPropertyHostnamesResult(
+    return AwaitableGetPropertyIncludeParentsResult(
         contract_id=pulumi.get(__ret__, 'contract_id'),
         group_id=pulumi.get(__ret__, 'group_id'),
-        hostnames=pulumi.get(__ret__, 'hostnames'),
         id=pulumi.get(__ret__, 'id'),
-        property_id=pulumi.get(__ret__, 'property_id'),
-        version=pulumi.get(__ret__, 'version'))
+        include_id=pulumi.get(__ret__, 'include_id'),
+        parents=pulumi.get(__ret__, 'parents'))
 
 
-@_utilities.lift_output_func(get_property_hostnames)
-def get_property_hostnames_output(contract_id: Optional[pulumi.Input[str]] = None,
-                                  group_id: Optional[pulumi.Input[str]] = None,
-                                  property_id: Optional[pulumi.Input[str]] = None,
-                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyHostnamesResult]:
+@_utilities.lift_output_func(get_property_include_parents)
+def get_property_include_parents_output(contract_id: Optional[pulumi.Input[str]] = None,
+                                        group_id: Optional[pulumi.Input[str]] = None,
+                                        include_id: Optional[pulumi.Input[str]] = None,
+                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyIncludeParentsResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_include.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_rules.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,148 +6,144 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetPropertyIncludeResult',
-    'AwaitableGetPropertyIncludeResult',
-    'get_property_include',
-    'get_property_include_output',
+    'GetPropertyRulesResult',
+    'AwaitableGetPropertyRulesResult',
+    'get_property_rules',
+    'get_property_rules_output',
 ]
 
 @pulumi.output_type
-class GetPropertyIncludeResult:
+class GetPropertyRulesResult:
     """
-    A collection of values returned by getPropertyInclude.
+    A collection of values returned by getPropertyRules.
     """
-    def __init__(__self__, contract_id=None, group_id=None, id=None, include_id=None, latest_version=None, name=None, production_version=None, staging_version=None, type=None):
+    def __init__(__self__, contract_id=None, errors=None, group_id=None, id=None, property_id=None, rule_format=None, rules=None, version=None):
         if contract_id and not isinstance(contract_id, str):
             raise TypeError("Expected argument 'contract_id' to be a str")
         pulumi.set(__self__, "contract_id", contract_id)
+        if errors and not isinstance(errors, str):
+            raise TypeError("Expected argument 'errors' to be a str")
+        pulumi.set(__self__, "errors", errors)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if include_id and not isinstance(include_id, str):
-            raise TypeError("Expected argument 'include_id' to be a str")
-        pulumi.set(__self__, "include_id", include_id)
-        if latest_version and not isinstance(latest_version, int):
-            raise TypeError("Expected argument 'latest_version' to be a int")
-        pulumi.set(__self__, "latest_version", latest_version)
-        if name and not isinstance(name, str):
-            raise TypeError("Expected argument 'name' to be a str")
-        pulumi.set(__self__, "name", name)
-        if production_version and not isinstance(production_version, int):
-            raise TypeError("Expected argument 'production_version' to be a int")
-        pulumi.set(__self__, "production_version", production_version)
-        if staging_version and not isinstance(staging_version, int):
-            raise TypeError("Expected argument 'staging_version' to be a int")
-        pulumi.set(__self__, "staging_version", staging_version)
-        if type and not isinstance(type, str):
-            raise TypeError("Expected argument 'type' to be a str")
-        pulumi.set(__self__, "type", type)
+        if property_id and not isinstance(property_id, str):
+            raise TypeError("Expected argument 'property_id' to be a str")
+        pulumi.set(__self__, "property_id", property_id)
+        if rule_format and not isinstance(rule_format, str):
+            raise TypeError("Expected argument 'rule_format' to be a str")
+        pulumi.set(__self__, "rule_format", rule_format)
+        if rules and not isinstance(rules, str):
+            raise TypeError("Expected argument 'rules' to be a str")
+        pulumi.set(__self__, "rules", rules)
+        if version and not isinstance(version, int):
+            raise TypeError("Expected argument 'version' to be a int")
+        pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> str:
         return pulumi.get(self, "contract_id")
 
     @property
+    @pulumi.getter
+    def errors(self) -> str:
+        return pulumi.get(self, "errors")
+
+    @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> str:
         return pulumi.get(self, "group_id")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="includeId")
-    def include_id(self) -> str:
-        return pulumi.get(self, "include_id")
+    @pulumi.getter(name="propertyId")
+    def property_id(self) -> str:
+        return pulumi.get(self, "property_id")
 
     @property
-    @pulumi.getter(name="latestVersion")
-    def latest_version(self) -> int:
-        return pulumi.get(self, "latest_version")
+    @pulumi.getter(name="ruleFormat")
+    def rule_format(self) -> Optional[str]:
+        return pulumi.get(self, "rule_format")
 
     @property
     @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter(name="productionVersion")
-    def production_version(self) -> int:
-        return pulumi.get(self, "production_version")
-
-    @property
-    @pulumi.getter(name="stagingVersion")
-    def staging_version(self) -> int:
-        return pulumi.get(self, "staging_version")
+    def rules(self) -> str:
+        return pulumi.get(self, "rules")
 
     @property
     @pulumi.getter
-    def type(self) -> str:
-        return pulumi.get(self, "type")
+    def version(self) -> int:
+        return pulumi.get(self, "version")
 
 
-class AwaitableGetPropertyIncludeResult(GetPropertyIncludeResult):
+class AwaitableGetPropertyRulesResult(GetPropertyRulesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPropertyIncludeResult(
+        return GetPropertyRulesResult(
             contract_id=self.contract_id,
+            errors=self.errors,
             group_id=self.group_id,
             id=self.id,
-            include_id=self.include_id,
-            latest_version=self.latest_version,
-            name=self.name,
-            production_version=self.production_version,
-            staging_version=self.staging_version,
-            type=self.type)
+            property_id=self.property_id,
+            rule_format=self.rule_format,
+            rules=self.rules,
+            version=self.version)
 
 
-def get_property_include(contract_id: Optional[str] = None,
-                         group_id: Optional[str] = None,
-                         include_id: Optional[str] = None,
-                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyIncludeResult:
+def get_property_rules(contract_id: Optional[str] = None,
+                       group_id: Optional[str] = None,
+                       property_id: Optional[str] = None,
+                       rule_format: Optional[str] = None,
+                       version: Optional[int] = None,
+                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyRulesResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
-    __args__['includeId'] = include_id
+    __args__['propertyId'] = property_id
+    __args__['ruleFormat'] = rule_format
+    __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyInclude:getPropertyInclude', __args__, opts=opts, typ=GetPropertyIncludeResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyRules:getPropertyRules', __args__, opts=opts, typ=GetPropertyRulesResult).value
 
-    return AwaitableGetPropertyIncludeResult(
+    return AwaitableGetPropertyRulesResult(
         contract_id=pulumi.get(__ret__, 'contract_id'),
+        errors=pulumi.get(__ret__, 'errors'),
         group_id=pulumi.get(__ret__, 'group_id'),
         id=pulumi.get(__ret__, 'id'),
-        include_id=pulumi.get(__ret__, 'include_id'),
-        latest_version=pulumi.get(__ret__, 'latest_version'),
-        name=pulumi.get(__ret__, 'name'),
-        production_version=pulumi.get(__ret__, 'production_version'),
-        staging_version=pulumi.get(__ret__, 'staging_version'),
-        type=pulumi.get(__ret__, 'type'))
+        property_id=pulumi.get(__ret__, 'property_id'),
+        rule_format=pulumi.get(__ret__, 'rule_format'),
+        rules=pulumi.get(__ret__, 'rules'),
+        version=pulumi.get(__ret__, 'version'))
 
 
-@_utilities.lift_output_func(get_property_include)
-def get_property_include_output(contract_id: Optional[pulumi.Input[str]] = None,
-                                group_id: Optional[pulumi.Input[str]] = None,
-                                include_id: Optional[pulumi.Input[str]] = None,
-                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyIncludeResult]:
+@_utilities.lift_output_func(get_property_rules)
+def get_property_rules_output(contract_id: Optional[pulumi.Input[Optional[str]]] = None,
+                              group_id: Optional[pulumi.Input[Optional[str]]] = None,
+                              property_id: Optional[pulumi.Input[str]] = None,
+                              rule_format: Optional[pulumi.Input[Optional[str]]] = None,
+                              version: Optional[pulumi.Input[Optional[int]]] = None,
+                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyRulesResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_include_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_include_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_include_parents.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_cp_code.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,44 +4,43 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
-from . import outputs
 
 __all__ = [
-    'GetPropertyIncludeParentsResult',
-    'AwaitableGetPropertyIncludeParentsResult',
-    'get_property_include_parents',
-    'get_property_include_parents_output',
+    'GetCpCodeResult',
+    'AwaitableGetCpCodeResult',
+    'get_cp_code',
+    'get_cp_code_output',
 ]
 
 @pulumi.output_type
-class GetPropertyIncludeParentsResult:
+class GetCpCodeResult:
     """
-    A collection of values returned by getPropertyIncludeParents.
+    A collection of values returned by getCpCode.
     """
-    def __init__(__self__, contract_id=None, group_id=None, id=None, include_id=None, parents=None):
+    def __init__(__self__, contract_id=None, group_id=None, id=None, name=None, product_ids=None):
         if contract_id and not isinstance(contract_id, str):
             raise TypeError("Expected argument 'contract_id' to be a str")
         pulumi.set(__self__, "contract_id", contract_id)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if include_id and not isinstance(include_id, str):
-            raise TypeError("Expected argument 'include_id' to be a str")
-        pulumi.set(__self__, "include_id", include_id)
-        if parents and not isinstance(parents, list):
-            raise TypeError("Expected argument 'parents' to be a list")
-        pulumi.set(__self__, "parents", parents)
+        if name and not isinstance(name, str):
+            raise TypeError("Expected argument 'name' to be a str")
+        pulumi.set(__self__, "name", name)
+        if product_ids and not isinstance(product_ids, list):
+            raise TypeError("Expected argument 'product_ids' to be a list")
+        pulumi.set(__self__, "product_ids", product_ids)
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> str:
         return pulumi.get(self, "contract_id")
 
     @property
@@ -54,61 +53,61 @@
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="includeId")
-    def include_id(self) -> str:
-        return pulumi.get(self, "include_id")
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter
-    def parents(self) -> Sequence['outputs.GetPropertyIncludeParentsParentResult']:
-        return pulumi.get(self, "parents")
+    @pulumi.getter(name="productIds")
+    def product_ids(self) -> Sequence[str]:
+        return pulumi.get(self, "product_ids")
 
 
-class AwaitableGetPropertyIncludeParentsResult(GetPropertyIncludeParentsResult):
+class AwaitableGetCpCodeResult(GetCpCodeResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPropertyIncludeParentsResult(
+        return GetCpCodeResult(
             contract_id=self.contract_id,
             group_id=self.group_id,
             id=self.id,
-            include_id=self.include_id,
-            parents=self.parents)
+            name=self.name,
+            product_ids=self.product_ids)
 
 
-def get_property_include_parents(contract_id: Optional[str] = None,
-                                 group_id: Optional[str] = None,
-                                 include_id: Optional[str] = None,
-                                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyIncludeParentsResult:
+def get_cp_code(contract_id: Optional[str] = None,
+                group_id: Optional[str] = None,
+                name: Optional[str] = None,
+                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCpCodeResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
-    __args__['includeId'] = include_id
+    __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyIncludeParents:getPropertyIncludeParents', __args__, opts=opts, typ=GetPropertyIncludeParentsResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getCpCode:getCpCode', __args__, opts=opts, typ=GetCpCodeResult).value
 
-    return AwaitableGetPropertyIncludeParentsResult(
+    return AwaitableGetCpCodeResult(
         contract_id=pulumi.get(__ret__, 'contract_id'),
         group_id=pulumi.get(__ret__, 'group_id'),
         id=pulumi.get(__ret__, 'id'),
-        include_id=pulumi.get(__ret__, 'include_id'),
-        parents=pulumi.get(__ret__, 'parents'))
+        name=pulumi.get(__ret__, 'name'),
+        product_ids=pulumi.get(__ret__, 'product_ids'))
 
 
-@_utilities.lift_output_func(get_property_include_parents)
-def get_property_include_parents_output(contract_id: Optional[pulumi.Input[str]] = None,
-                                        group_id: Optional[pulumi.Input[str]] = None,
-                                        include_id: Optional[pulumi.Input[str]] = None,
-                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyIncludeParentsResult]:
+@_utilities.lift_output_func(get_cp_code)
+def get_cp_code_output(contract_id: Optional[pulumi.Input[str]] = None,
+                       group_id: Optional[pulumi.Input[str]] = None,
+                       name: Optional[pulumi.Input[str]] = None,
+                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCpCodeResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_include_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_include_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_includes.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_includes.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_products.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_products.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_rule_formats.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_rule_formats.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/get_property_rules.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
 __all__ = [
     'GetPropertyRulesResult',
     'AwaitableGetPropertyRulesResult',
     'get_property_rules',
     'get_property_rules_output',
 ]
 
+warnings.warn("""akamai.properties/getpropertyrules.getPropertyRules has been deprecated in favor of akamai.index/getpropertyrules.getPropertyRules""", DeprecationWarning)
+
 @pulumi.output_type
 class GetPropertyRulesResult:
     """
     A collection of values returned by getPropertyRules.
     """
     def __init__(__self__, contract_id=None, errors=None, group_id=None, id=None, property_id=None, rule_format=None, rules=None, version=None):
         if contract_id and not isinstance(contract_id, str):
@@ -112,22 +114,23 @@
                        property_id: Optional[str] = None,
                        rule_format: Optional[str] = None,
                        version: Optional[int] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyRulesResult:
     """
     Use this data source to access information about an existing resource.
     """
+    pulumi.log.warn("""get_property_rules is deprecated: akamai.properties/getpropertyrules.getPropertyRules has been deprecated in favor of akamai.index/getpropertyrules.getPropertyRules""")
     __args__ = dict()
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
     __args__['propertyId'] = property_id
     __args__['ruleFormat'] = rule_format
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyRules:getPropertyRules', __args__, opts=opts, typ=GetPropertyRulesResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:properties/getPropertyRules:getPropertyRules', __args__, opts=opts, typ=GetPropertyRulesResult).value
 
     return AwaitableGetPropertyRulesResult(
         contract_id=pulumi.get(__ret__, 'contract_id'),
         errors=pulumi.get(__ret__, 'errors'),
         group_id=pulumi.get(__ret__, 'group_id'),
         id=pulumi.get(__ret__, 'id'),
         property_id=pulumi.get(__ret__, 'property_id'),
@@ -142,8 +145,9 @@
                               property_id: Optional[pulumi.Input[str]] = None,
                               rule_format: Optional[pulumi.Input[Optional[str]]] = None,
                               version: Optional[pulumi.Input[Optional[int]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyRulesResult]:
     """
     Use this data source to access information about an existing resource.
     """
+    pulumi.log.warn("""get_property_rules is deprecated: akamai.properties/getpropertyrules.getPropertyRules has been deprecated in favor of akamai.index/getpropertyrules.getPropertyRules""")
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_rules_builder.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_rules_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,27 +19,30 @@
 ]
 
 @pulumi.output_type
 class GetPropertyRulesBuilderResult:
     """
     A collection of values returned by getPropertyRulesBuilder.
     """
-    def __init__(__self__, id=None, json=None, rule_format=None, rules_v20230105=None):
+    def __init__(__self__, id=None, json=None, rule_format=None, rules_v20230105=None, rules_v20230530=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if json and not isinstance(json, str):
             raise TypeError("Expected argument 'json' to be a str")
         pulumi.set(__self__, "json", json)
         if rule_format and not isinstance(rule_format, str):
             raise TypeError("Expected argument 'rule_format' to be a str")
         pulumi.set(__self__, "rule_format", rule_format)
         if rules_v20230105 and not isinstance(rules_v20230105, dict):
             raise TypeError("Expected argument 'rules_v20230105' to be a dict")
         pulumi.set(__self__, "rules_v20230105", rules_v20230105)
+        if rules_v20230530 and not isinstance(rules_v20230530, dict):
+            raise TypeError("Expected argument 'rules_v20230530' to be a dict")
+        pulumi.set(__self__, "rules_v20230530", rules_v20230530)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
@@ -56,44 +59,54 @@
         return pulumi.get(self, "rule_format")
 
     @property
     @pulumi.getter(name="rulesV20230105")
     def rules_v20230105(self) -> Optional['outputs.GetPropertyRulesBuilderRulesV20230105Result']:
         return pulumi.get(self, "rules_v20230105")
 
+    @property
+    @pulumi.getter(name="rulesV20230530")
+    def rules_v20230530(self) -> Optional['outputs.GetPropertyRulesBuilderRulesV20230530Result']:
+        return pulumi.get(self, "rules_v20230530")
+
 
 class AwaitableGetPropertyRulesBuilderResult(GetPropertyRulesBuilderResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetPropertyRulesBuilderResult(
             id=self.id,
             json=self.json,
             rule_format=self.rule_format,
-            rules_v20230105=self.rules_v20230105)
+            rules_v20230105=self.rules_v20230105,
+            rules_v20230530=self.rules_v20230530)
 
 
 def get_property_rules_builder(rules_v20230105: Optional[pulumi.InputType['GetPropertyRulesBuilderRulesV20230105Args']] = None,
+                               rules_v20230530: Optional[pulumi.InputType['GetPropertyRulesBuilderRulesV20230530Args']] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyRulesBuilderResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     __args__['rulesV20230105'] = rules_v20230105
+    __args__['rulesV20230530'] = rules_v20230530
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyRulesBuilder:getPropertyRulesBuilder', __args__, opts=opts, typ=GetPropertyRulesBuilderResult).value
 
     return AwaitableGetPropertyRulesBuilderResult(
         id=pulumi.get(__ret__, 'id'),
         json=pulumi.get(__ret__, 'json'),
         rule_format=pulumi.get(__ret__, 'rule_format'),
-        rules_v20230105=pulumi.get(__ret__, 'rules_v20230105'))
+        rules_v20230105=pulumi.get(__ret__, 'rules_v20230105'),
+        rules_v20230530=pulumi.get(__ret__, 'rules_v20230530'))
 
 
 @_utilities.lift_output_func(get_property_rules_builder)
 def get_property_rules_builder_output(rules_v20230105: Optional[pulumi.Input[Optional[pulumi.InputType['GetPropertyRulesBuilderRulesV20230105Args']]]] = None,
+                                      rules_v20230530: Optional[pulumi.Input[Optional[pulumi.InputType['GetPropertyRulesBuilderRulesV20230530Args']]]] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyRulesBuilderResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/get_property_rules_template.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/get_property_rules_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_asmap.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_asmap.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_cidrmap.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_cidrmap.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_datacenter.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_domain.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_geomap.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_geomap.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_property.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/gtm_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/gtm_resource.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/property_activation.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,607 +7,502 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['GtmResourceArgs', 'GtmResource']
+__all__ = ['PropertyActivationArgs', 'PropertyActivation']
 
 @pulumi.input_type
-class GtmResourceArgs:
+class PropertyActivationArgs:
     def __init__(__self__, *,
-                 aggregation_type: pulumi.Input[str],
-                 domain: pulumi.Input[str],
-                 type: pulumi.Input[str],
-                 constrained_property: Optional[pulumi.Input[str]] = None,
-                 decay_rate: Optional[pulumi.Input[float]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 host_header: Optional[pulumi.Input[str]] = None,
-                 leader_string: Optional[pulumi.Input[str]] = None,
-                 least_squares_decay: Optional[pulumi.Input[float]] = None,
-                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
-                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]] = None,
-                 upper_bound: Optional[pulumi.Input[int]] = None,
-                 wait_on_complete: Optional[pulumi.Input[bool]] = None):
+                 contacts: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 property_id: pulumi.Input[str],
+                 version: pulumi.Input[int],
+                 activation_id: Optional[pulumi.Input[str]] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]] = None):
         """
-        The set of arguments for constructing a GtmResource resource.
+        The set of arguments for constructing a PropertyActivation resource.
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: Automatically acknowledge all rule warnings for activation to continue. Default is false
+        :param pulumi.Input['PropertyActivationComplianceRecordArgs'] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] note: assigns a log message to the activation request
         """
-        pulumi.set(__self__, "aggregation_type", aggregation_type)
-        pulumi.set(__self__, "domain", domain)
-        pulumi.set(__self__, "type", type)
-        if constrained_property is not None:
-            pulumi.set(__self__, "constrained_property", constrained_property)
-        if decay_rate is not None:
-            pulumi.set(__self__, "decay_rate", decay_rate)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if host_header is not None:
-            pulumi.set(__self__, "host_header", host_header)
-        if leader_string is not None:
-            pulumi.set(__self__, "leader_string", leader_string)
-        if least_squares_decay is not None:
-            pulumi.set(__self__, "least_squares_decay", least_squares_decay)
-        if load_imbalance_percentage is not None:
-            pulumi.set(__self__, "load_imbalance_percentage", load_imbalance_percentage)
-        if max_u_multiplicative_increment is not None:
-            pulumi.set(__self__, "max_u_multiplicative_increment", max_u_multiplicative_increment)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if resource_instances is not None:
-            pulumi.set(__self__, "resource_instances", resource_instances)
-        if upper_bound is not None:
-            pulumi.set(__self__, "upper_bound", upper_bound)
-        if wait_on_complete is not None:
-            pulumi.set(__self__, "wait_on_complete", wait_on_complete)
-
-    @property
-    @pulumi.getter(name="aggregationType")
-    def aggregation_type(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "aggregation_type")
-
-    @aggregation_type.setter
-    def aggregation_type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "aggregation_type", value)
-
-    @property
-    @pulumi.getter
-    def domain(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "domain")
-
-    @domain.setter
-    def domain(self, value: pulumi.Input[str]):
-        pulumi.set(self, "domain", value)
+        pulumi.set(__self__, "contacts", contacts)
+        pulumi.set(__self__, "property_id", property_id)
+        pulumi.set(__self__, "version", version)
+        if activation_id is not None:
+            pulumi.set(__self__, "activation_id", activation_id)
+        if auto_acknowledge_rule_warnings is not None:
+            pulumi.set(__self__, "auto_acknowledge_rule_warnings", auto_acknowledge_rule_warnings)
+        if compliance_record is not None:
+            pulumi.set(__self__, "compliance_record", compliance_record)
+        if network is not None:
+            pulumi.set(__self__, "network", network)
+        if note is not None:
+            pulumi.set(__self__, "note", note)
+        if rule_errors is not None:
+            pulumi.set(__self__, "rule_errors", rule_errors)
 
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "type", value)
+    def contacts(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        return pulumi.get(self, "contacts")
 
-    @property
-    @pulumi.getter(name="constrainedProperty")
-    def constrained_property(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "constrained_property")
-
-    @constrained_property.setter
-    def constrained_property(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "constrained_property", value)
+    @contacts.setter
+    def contacts(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "contacts", value)
 
     @property
-    @pulumi.getter(name="decayRate")
-    def decay_rate(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "decay_rate")
+    @pulumi.getter(name="propertyId")
+    def property_id(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "property_id")
 
-    @decay_rate.setter
-    def decay_rate(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "decay_rate", value)
+    @property_id.setter
+    def property_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "property_id", value)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "description")
-
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
-
-    @property
-    @pulumi.getter(name="hostHeader")
-    def host_header(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "host_header")
-
-    @host_header.setter
-    def host_header(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "host_header", value)
-
-    @property
-    @pulumi.getter(name="leaderString")
-    def leader_string(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "leader_string")
+    def version(self) -> pulumi.Input[int]:
+        return pulumi.get(self, "version")
 
-    @leader_string.setter
-    def leader_string(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "leader_string", value)
+    @version.setter
+    def version(self, value: pulumi.Input[int]):
+        pulumi.set(self, "version", value)
 
     @property
-    @pulumi.getter(name="leastSquaresDecay")
-    def least_squares_decay(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "least_squares_decay")
+    @pulumi.getter(name="activationId")
+    def activation_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "activation_id")
 
-    @least_squares_decay.setter
-    def least_squares_decay(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "least_squares_decay", value)
+    @activation_id.setter
+    def activation_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "activation_id", value)
 
     @property
-    @pulumi.getter(name="loadImbalancePercentage")
-    def load_imbalance_percentage(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "load_imbalance_percentage")
+    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
+    def auto_acknowledge_rule_warnings(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Automatically acknowledge all rule warnings for activation to continue. Default is false
+        """
+        return pulumi.get(self, "auto_acknowledge_rule_warnings")
 
-    @load_imbalance_percentage.setter
-    def load_imbalance_percentage(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "load_imbalance_percentage", value)
+    @auto_acknowledge_rule_warnings.setter
+    def auto_acknowledge_rule_warnings(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "auto_acknowledge_rule_warnings", value)
 
     @property
-    @pulumi.getter(name="maxUMultiplicativeIncrement")
-    def max_u_multiplicative_increment(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "max_u_multiplicative_increment")
+    @pulumi.getter(name="complianceRecord")
+    def compliance_record(self) -> Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']]:
+        """
+        Provides an audit record when activating on a production network
+        """
+        return pulumi.get(self, "compliance_record")
 
-    @max_u_multiplicative_increment.setter
-    def max_u_multiplicative_increment(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "max_u_multiplicative_increment", value)
+    @compliance_record.setter
+    def compliance_record(self, value: Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']]):
+        pulumi.set(self, "compliance_record", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "name")
+    def network(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "network")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @network.setter
+    def network(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network", value)
 
     @property
-    @pulumi.getter(name="resourceInstances")
-    def resource_instances(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]:
-        return pulumi.get(self, "resource_instances")
-
-    @resource_instances.setter
-    def resource_instances(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]):
-        pulumi.set(self, "resource_instances", value)
-
-    @property
-    @pulumi.getter(name="upperBound")
-    def upper_bound(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "upper_bound")
+    @pulumi.getter
+    def note(self) -> Optional[pulumi.Input[str]]:
+        """
+        assigns a log message to the activation request
+        """
+        return pulumi.get(self, "note")
 
-    @upper_bound.setter
-    def upper_bound(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "upper_bound", value)
+    @note.setter
+    def note(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "note", value)
 
     @property
-    @pulumi.getter(name="waitOnComplete")
-    def wait_on_complete(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "wait_on_complete")
+    @pulumi.getter(name="ruleErrors")
+    def rule_errors(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]]:
+        return pulumi.get(self, "rule_errors")
 
-    @wait_on_complete.setter
-    def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "wait_on_complete", value)
+    @rule_errors.setter
+    def rule_errors(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]]):
+        pulumi.set(self, "rule_errors", value)
 
 
 @pulumi.input_type
-class _GtmResourceState:
+class _PropertyActivationState:
     def __init__(__self__, *,
-                 aggregation_type: Optional[pulumi.Input[str]] = None,
-                 constrained_property: Optional[pulumi.Input[str]] = None,
-                 decay_rate: Optional[pulumi.Input[float]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 host_header: Optional[pulumi.Input[str]] = None,
-                 leader_string: Optional[pulumi.Input[str]] = None,
-                 least_squares_decay: Optional[pulumi.Input[float]] = None,
-                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
-                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 upper_bound: Optional[pulumi.Input[int]] = None,
-                 wait_on_complete: Optional[pulumi.Input[bool]] = None):
+                 activation_id: Optional[pulumi.Input[str]] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']] = None,
+                 contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 errors: Optional[pulumi.Input[str]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 property_id: Optional[pulumi.Input[str]] = None,
+                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
+                 version: Optional[pulumi.Input[int]] = None,
+                 warnings: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering GtmResource resources.
+        Input properties used for looking up and filtering PropertyActivation resources.
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: Automatically acknowledge all rule warnings for activation to continue. Default is false
+        :param pulumi.Input['PropertyActivationComplianceRecordArgs'] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] note: assigns a log message to the activation request
         """
-        if aggregation_type is not None:
-            pulumi.set(__self__, "aggregation_type", aggregation_type)
-        if constrained_property is not None:
-            pulumi.set(__self__, "constrained_property", constrained_property)
-        if decay_rate is not None:
-            pulumi.set(__self__, "decay_rate", decay_rate)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if domain is not None:
-            pulumi.set(__self__, "domain", domain)
-        if host_header is not None:
-            pulumi.set(__self__, "host_header", host_header)
-        if leader_string is not None:
-            pulumi.set(__self__, "leader_string", leader_string)
-        if least_squares_decay is not None:
-            pulumi.set(__self__, "least_squares_decay", least_squares_decay)
-        if load_imbalance_percentage is not None:
-            pulumi.set(__self__, "load_imbalance_percentage", load_imbalance_percentage)
-        if max_u_multiplicative_increment is not None:
-            pulumi.set(__self__, "max_u_multiplicative_increment", max_u_multiplicative_increment)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if resource_instances is not None:
-            pulumi.set(__self__, "resource_instances", resource_instances)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-        if upper_bound is not None:
-            pulumi.set(__self__, "upper_bound", upper_bound)
-        if wait_on_complete is not None:
-            pulumi.set(__self__, "wait_on_complete", wait_on_complete)
-
-    @property
-    @pulumi.getter(name="aggregationType")
-    def aggregation_type(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "aggregation_type")
-
-    @aggregation_type.setter
-    def aggregation_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "aggregation_type", value)
+        if activation_id is not None:
+            pulumi.set(__self__, "activation_id", activation_id)
+        if auto_acknowledge_rule_warnings is not None:
+            pulumi.set(__self__, "auto_acknowledge_rule_warnings", auto_acknowledge_rule_warnings)
+        if compliance_record is not None:
+            pulumi.set(__self__, "compliance_record", compliance_record)
+        if contacts is not None:
+            pulumi.set(__self__, "contacts", contacts)
+        if errors is not None:
+            pulumi.set(__self__, "errors", errors)
+        if network is not None:
+            pulumi.set(__self__, "network", network)
+        if note is not None:
+            pulumi.set(__self__, "note", note)
+        if property_id is not None:
+            pulumi.set(__self__, "property_id", property_id)
+        if rule_errors is not None:
+            pulumi.set(__self__, "rule_errors", rule_errors)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
+        if warnings is not None:
+            pulumi.set(__self__, "warnings", warnings)
+
+    @property
+    @pulumi.getter(name="activationId")
+    def activation_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "activation_id")
+
+    @activation_id.setter
+    def activation_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "activation_id", value)
 
     @property
-    @pulumi.getter(name="constrainedProperty")
-    def constrained_property(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "constrained_property")
+    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
+    def auto_acknowledge_rule_warnings(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Automatically acknowledge all rule warnings for activation to continue. Default is false
+        """
+        return pulumi.get(self, "auto_acknowledge_rule_warnings")
 
-    @constrained_property.setter
-    def constrained_property(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "constrained_property", value)
+    @auto_acknowledge_rule_warnings.setter
+    def auto_acknowledge_rule_warnings(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "auto_acknowledge_rule_warnings", value)
 
     @property
-    @pulumi.getter(name="decayRate")
-    def decay_rate(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "decay_rate")
+    @pulumi.getter(name="complianceRecord")
+    def compliance_record(self) -> Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']]:
+        """
+        Provides an audit record when activating on a production network
+        """
+        return pulumi.get(self, "compliance_record")
 
-    @decay_rate.setter
-    def decay_rate(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "decay_rate", value)
+    @compliance_record.setter
+    def compliance_record(self, value: Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']]):
+        pulumi.set(self, "compliance_record", value)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "description")
+    def contacts(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "contacts")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @contacts.setter
+    def contacts(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "contacts", value)
 
     @property
     @pulumi.getter
-    def domain(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "domain")
-
-    @domain.setter
-    def domain(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "domain", value)
-
-    @property
-    @pulumi.getter(name="hostHeader")
-    def host_header(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "host_header")
+    def errors(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "errors")
 
-    @host_header.setter
-    def host_header(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "host_header", value)
+    @errors.setter
+    def errors(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "errors", value)
 
     @property
-    @pulumi.getter(name="leaderString")
-    def leader_string(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "leader_string")
+    @pulumi.getter
+    def network(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "network")
 
-    @leader_string.setter
-    def leader_string(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "leader_string", value)
+    @network.setter
+    def network(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network", value)
 
     @property
-    @pulumi.getter(name="leastSquaresDecay")
-    def least_squares_decay(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "least_squares_decay")
+    @pulumi.getter
+    def note(self) -> Optional[pulumi.Input[str]]:
+        """
+        assigns a log message to the activation request
+        """
+        return pulumi.get(self, "note")
 
-    @least_squares_decay.setter
-    def least_squares_decay(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "least_squares_decay", value)
+    @note.setter
+    def note(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "note", value)
 
     @property
-    @pulumi.getter(name="loadImbalancePercentage")
-    def load_imbalance_percentage(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "load_imbalance_percentage")
+    @pulumi.getter(name="propertyId")
+    def property_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "property_id")
 
-    @load_imbalance_percentage.setter
-    def load_imbalance_percentage(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "load_imbalance_percentage", value)
+    @property_id.setter
+    def property_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "property_id", value)
 
     @property
-    @pulumi.getter(name="maxUMultiplicativeIncrement")
-    def max_u_multiplicative_increment(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "max_u_multiplicative_increment")
+    @pulumi.getter(name="ruleErrors")
+    def rule_errors(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]]:
+        return pulumi.get(self, "rule_errors")
 
-    @max_u_multiplicative_increment.setter
-    def max_u_multiplicative_increment(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "max_u_multiplicative_increment", value)
+    @rule_errors.setter
+    def rule_errors(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]]):
+        pulumi.set(self, "rule_errors", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "name")
+    def status(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "status")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter(name="resourceInstances")
-    def resource_instances(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]:
-        return pulumi.get(self, "resource_instances")
-
-    @resource_instances.setter
-    def resource_instances(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]):
-        pulumi.set(self, "resource_instances", value)
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
 
     @property
     @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
+    def version(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "version")
 
-    @property
-    @pulumi.getter(name="upperBound")
-    def upper_bound(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "upper_bound")
-
-    @upper_bound.setter
-    def upper_bound(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "upper_bound", value)
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "version", value)
 
     @property
-    @pulumi.getter(name="waitOnComplete")
-    def wait_on_complete(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "wait_on_complete")
+    @pulumi.getter
+    def warnings(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "warnings")
 
-    @wait_on_complete.setter
-    def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "wait_on_complete", value)
+    @warnings.setter
+    def warnings(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "warnings", value)
 
 
-class GtmResource(pulumi.CustomResource):
+class PropertyActivation(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 aggregation_type: Optional[pulumi.Input[str]] = None,
-                 constrained_property: Optional[pulumi.Input[str]] = None,
-                 decay_rate: Optional[pulumi.Input[float]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 host_header: Optional[pulumi.Input[str]] = None,
-                 leader_string: Optional[pulumi.Input[str]] = None,
-                 least_squares_decay: Optional[pulumi.Input[float]] = None,
-                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
-                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 upper_bound: Optional[pulumi.Input[int]] = None,
-                 wait_on_complete: Optional[pulumi.Input[bool]] = None,
+                 activation_id: Optional[pulumi.Input[str]] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']]] = None,
+                 contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 property_id: Optional[pulumi.Input[str]] = None,
+                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleErrorArgs']]]]] = None,
+                 version: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Create a GtmResource resource with the given unique name, props, and options.
+        Create a PropertyActivation resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: Automatically acknowledge all rule warnings for activation to continue. Default is false
+        :param pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] note: assigns a log message to the activation request
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: GtmResourceArgs,
+                 args: PropertyActivationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a GtmResource resource with the given unique name, props, and options.
+        Create a PropertyActivation resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param GtmResourceArgs args: The arguments to use to populate this resource's properties.
+        :param PropertyActivationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(GtmResourceArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(PropertyActivationArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 aggregation_type: Optional[pulumi.Input[str]] = None,
-                 constrained_property: Optional[pulumi.Input[str]] = None,
-                 decay_rate: Optional[pulumi.Input[float]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 host_header: Optional[pulumi.Input[str]] = None,
-                 leader_string: Optional[pulumi.Input[str]] = None,
-                 least_squares_decay: Optional[pulumi.Input[float]] = None,
-                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
-                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 upper_bound: Optional[pulumi.Input[int]] = None,
-                 wait_on_complete: Optional[pulumi.Input[bool]] = None,
+                 activation_id: Optional[pulumi.Input[str]] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']]] = None,
+                 contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 property_id: Optional[pulumi.Input[str]] = None,
+                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleErrorArgs']]]]] = None,
+                 version: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = GtmResourceArgs.__new__(GtmResourceArgs)
+            __props__ = PropertyActivationArgs.__new__(PropertyActivationArgs)
 
-            if aggregation_type is None and not opts.urn:
-                raise TypeError("Missing required property 'aggregation_type'")
-            __props__.__dict__["aggregation_type"] = aggregation_type
-            __props__.__dict__["constrained_property"] = constrained_property
-            __props__.__dict__["decay_rate"] = decay_rate
-            __props__.__dict__["description"] = description
-            if domain is None and not opts.urn:
-                raise TypeError("Missing required property 'domain'")
-            __props__.__dict__["domain"] = domain
-            __props__.__dict__["host_header"] = host_header
-            __props__.__dict__["leader_string"] = leader_string
-            __props__.__dict__["least_squares_decay"] = least_squares_decay
-            __props__.__dict__["load_imbalance_percentage"] = load_imbalance_percentage
-            __props__.__dict__["max_u_multiplicative_increment"] = max_u_multiplicative_increment
-            __props__.__dict__["name"] = name
-            __props__.__dict__["resource_instances"] = resource_instances
-            if type is None and not opts.urn:
-                raise TypeError("Missing required property 'type'")
-            __props__.__dict__["type"] = type
-            __props__.__dict__["upper_bound"] = upper_bound
-            __props__.__dict__["wait_on_complete"] = wait_on_complete
-        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="akamai:trafficmanagement/gtmResource:GtmResource")])
+            __props__.__dict__["activation_id"] = activation_id
+            __props__.__dict__["auto_acknowledge_rule_warnings"] = auto_acknowledge_rule_warnings
+            __props__.__dict__["compliance_record"] = compliance_record
+            if contacts is None and not opts.urn:
+                raise TypeError("Missing required property 'contacts'")
+            __props__.__dict__["contacts"] = contacts
+            __props__.__dict__["network"] = network
+            __props__.__dict__["note"] = note
+            if property_id is None and not opts.urn:
+                raise TypeError("Missing required property 'property_id'")
+            __props__.__dict__["property_id"] = property_id
+            __props__.__dict__["rule_errors"] = rule_errors
+            if version is None and not opts.urn:
+                raise TypeError("Missing required property 'version'")
+            __props__.__dict__["version"] = version
+            __props__.__dict__["errors"] = None
+            __props__.__dict__["status"] = None
+            __props__.__dict__["warnings"] = None
+        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="akamai:properties/propertyActivation:PropertyActivation")])
         opts = pulumi.ResourceOptions.merge(opts, alias_opts)
-        super(GtmResource, __self__).__init__(
-            'akamai:index/gtmResource:GtmResource',
+        super(PropertyActivation, __self__).__init__(
+            'akamai:index/propertyActivation:PropertyActivation',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            aggregation_type: Optional[pulumi.Input[str]] = None,
-            constrained_property: Optional[pulumi.Input[str]] = None,
-            decay_rate: Optional[pulumi.Input[float]] = None,
-            description: Optional[pulumi.Input[str]] = None,
-            domain: Optional[pulumi.Input[str]] = None,
-            host_header: Optional[pulumi.Input[str]] = None,
-            leader_string: Optional[pulumi.Input[str]] = None,
-            least_squares_decay: Optional[pulumi.Input[float]] = None,
-            load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
-            max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
-            name: Optional[pulumi.Input[str]] = None,
-            resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
-            type: Optional[pulumi.Input[str]] = None,
-            upper_bound: Optional[pulumi.Input[int]] = None,
-            wait_on_complete: Optional[pulumi.Input[bool]] = None) -> 'GtmResource':
+            activation_id: Optional[pulumi.Input[str]] = None,
+            auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+            compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']]] = None,
+            contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            errors: Optional[pulumi.Input[str]] = None,
+            network: Optional[pulumi.Input[str]] = None,
+            note: Optional[pulumi.Input[str]] = None,
+            property_id: Optional[pulumi.Input[str]] = None,
+            rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleErrorArgs']]]]] = None,
+            status: Optional[pulumi.Input[str]] = None,
+            version: Optional[pulumi.Input[int]] = None,
+            warnings: Optional[pulumi.Input[str]] = None) -> 'PropertyActivation':
         """
-        Get an existing GtmResource resource's state with the given name, id, and optional extra
+        Get an existing PropertyActivation resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: Automatically acknowledge all rule warnings for activation to continue. Default is false
+        :param pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] note: assigns a log message to the activation request
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _GtmResourceState.__new__(_GtmResourceState)
-
-        __props__.__dict__["aggregation_type"] = aggregation_type
-        __props__.__dict__["constrained_property"] = constrained_property
-        __props__.__dict__["decay_rate"] = decay_rate
-        __props__.__dict__["description"] = description
-        __props__.__dict__["domain"] = domain
-        __props__.__dict__["host_header"] = host_header
-        __props__.__dict__["leader_string"] = leader_string
-        __props__.__dict__["least_squares_decay"] = least_squares_decay
-        __props__.__dict__["load_imbalance_percentage"] = load_imbalance_percentage
-        __props__.__dict__["max_u_multiplicative_increment"] = max_u_multiplicative_increment
-        __props__.__dict__["name"] = name
-        __props__.__dict__["resource_instances"] = resource_instances
-        __props__.__dict__["type"] = type
-        __props__.__dict__["upper_bound"] = upper_bound
-        __props__.__dict__["wait_on_complete"] = wait_on_complete
-        return GtmResource(resource_name, opts=opts, __props__=__props__)
+        __props__ = _PropertyActivationState.__new__(_PropertyActivationState)
 
-    @property
-    @pulumi.getter(name="aggregationType")
-    def aggregation_type(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "aggregation_type")
+        __props__.__dict__["activation_id"] = activation_id
+        __props__.__dict__["auto_acknowledge_rule_warnings"] = auto_acknowledge_rule_warnings
+        __props__.__dict__["compliance_record"] = compliance_record
+        __props__.__dict__["contacts"] = contacts
+        __props__.__dict__["errors"] = errors
+        __props__.__dict__["network"] = network
+        __props__.__dict__["note"] = note
+        __props__.__dict__["property_id"] = property_id
+        __props__.__dict__["rule_errors"] = rule_errors
+        __props__.__dict__["status"] = status
+        __props__.__dict__["version"] = version
+        __props__.__dict__["warnings"] = warnings
+        return PropertyActivation(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter(name="activationId")
+    def activation_id(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "activation_id")
 
     @property
-    @pulumi.getter(name="constrainedProperty")
-    def constrained_property(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "constrained_property")
+    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
+    def auto_acknowledge_rule_warnings(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Automatically acknowledge all rule warnings for activation to continue. Default is false
+        """
+        return pulumi.get(self, "auto_acknowledge_rule_warnings")
 
     @property
-    @pulumi.getter(name="decayRate")
-    def decay_rate(self) -> pulumi.Output[Optional[float]]:
-        return pulumi.get(self, "decay_rate")
+    @pulumi.getter(name="complianceRecord")
+    def compliance_record(self) -> pulumi.Output[Optional['outputs.PropertyActivationComplianceRecord']]:
+        """
+        Provides an audit record when activating on a production network
+        """
+        return pulumi.get(self, "compliance_record")
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "description")
+    def contacts(self) -> pulumi.Output[Sequence[str]]:
+        return pulumi.get(self, "contacts")
 
     @property
     @pulumi.getter
-    def domain(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "domain")
-
-    @property
-    @pulumi.getter(name="hostHeader")
-    def host_header(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "host_header")
+    def errors(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "errors")
 
     @property
-    @pulumi.getter(name="leaderString")
-    def leader_string(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "leader_string")
+    @pulumi.getter
+    def network(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "network")
 
     @property
-    @pulumi.getter(name="leastSquaresDecay")
-    def least_squares_decay(self) -> pulumi.Output[Optional[float]]:
-        return pulumi.get(self, "least_squares_decay")
+    @pulumi.getter
+    def note(self) -> pulumi.Output[Optional[str]]:
+        """
+        assigns a log message to the activation request
+        """
+        return pulumi.get(self, "note")
 
     @property
-    @pulumi.getter(name="loadImbalancePercentage")
-    def load_imbalance_percentage(self) -> pulumi.Output[Optional[float]]:
-        return pulumi.get(self, "load_imbalance_percentage")
+    @pulumi.getter(name="propertyId")
+    def property_id(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "property_id")
 
     @property
-    @pulumi.getter(name="maxUMultiplicativeIncrement")
-    def max_u_multiplicative_increment(self) -> pulumi.Output[Optional[float]]:
-        return pulumi.get(self, "max_u_multiplicative_increment")
+    @pulumi.getter(name="ruleErrors")
+    def rule_errors(self) -> pulumi.Output[Sequence['outputs.PropertyActivationRuleError']]:
+        return pulumi.get(self, "rule_errors")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter(name="resourceInstances")
-    def resource_instances(self) -> pulumi.Output[Optional[Sequence['outputs.GtmResourceResourceInstance']]]:
-        return pulumi.get(self, "resource_instances")
+    def status(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "status")
 
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "type")
-
-    @property
-    @pulumi.getter(name="upperBound")
-    def upper_bound(self) -> pulumi.Output[Optional[int]]:
-        return pulumi.get(self, "upper_bound")
+    def version(self) -> pulumi.Output[int]:
+        return pulumi.get(self, "version")
 
     @property
-    @pulumi.getter(name="waitOnComplete")
-    def wait_on_complete(self) -> pulumi.Output[Optional[bool]]:
-        return pulumi.get(self, "wait_on_complete")
+    @pulumi.getter
+    def warnings(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "warnings")
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/iam_blocked_user_properties.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/iam_blocked_user_properties.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/iam_group.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/iam_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/iam_role.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/iam_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/iam_user.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/iam_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,14 @@
                  city: Optional[pulumi.Input[str]] = None,
                  contact_type: Optional[pulumi.Input[str]] = None,
                  country: Optional[pulumi.Input[str]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  email_update_pending: Optional[pulumi.Input[bool]] = None,
                  enable_tfa: Optional[pulumi.Input[bool]] = None,
                  first_name: Optional[pulumi.Input[str]] = None,
-                 is_locked: Optional[pulumi.Input[bool]] = None,
                  job_title: Optional[pulumi.Input[str]] = None,
                  last_login: Optional[pulumi.Input[str]] = None,
                  last_name: Optional[pulumi.Input[str]] = None,
                  lock: Optional[pulumi.Input[bool]] = None,
                  mobile_phone: Optional[pulumi.Input[str]] = None,
                  password_expired_after: Optional[pulumi.Input[str]] = None,
                  phone: Optional[pulumi.Input[str]] = None,
@@ -351,15 +350,14 @@
         :param pulumi.Input[str] city: The user's city
         :param pulumi.Input[str] contact_type: To help characterize the user, the value can be any that are available from the view-contact-types operation
         :param pulumi.Input[str] country: As part of the user's location, the value can be any that are available from the view-supported-countries operation
         :param pulumi.Input[str] email: The user's email address
         :param pulumi.Input[bool] email_update_pending: Indicates whether email update is pending
         :param pulumi.Input[bool] enable_tfa: Indicates whether two-factor authentication is allowed
         :param pulumi.Input[str] first_name: The user's first name
-        :param pulumi.Input[bool] is_locked: The user's lock status
         :param pulumi.Input[str] job_title: The user's position at your company
         :param pulumi.Input[str] last_login: ISO 8601 timestamp indicating when the user last logged in
         :param pulumi.Input[str] last_name: The user's surname
         :param pulumi.Input[bool] lock: Flag to block a user account
         :param pulumi.Input[str] mobile_phone: The user's mobile phone number
         :param pulumi.Input[str] password_expired_after: The date a user's password expires
         :param pulumi.Input[str] phone: The user's main phone number
@@ -386,19 +384,14 @@
             pulumi.set(__self__, "email", email)
         if email_update_pending is not None:
             pulumi.set(__self__, "email_update_pending", email_update_pending)
         if enable_tfa is not None:
             pulumi.set(__self__, "enable_tfa", enable_tfa)
         if first_name is not None:
             pulumi.set(__self__, "first_name", first_name)
-        if is_locked is not None:
-            warnings.warn("""The setting \"is_locked\" has been deprecated. Please use \"lock\" setting instead""", DeprecationWarning)
-            pulumi.log.warn("""is_locked is deprecated: The setting \"is_locked\" has been deprecated. Please use \"lock\" setting instead""")
-        if is_locked is not None:
-            pulumi.set(__self__, "is_locked", is_locked)
         if job_title is not None:
             pulumi.set(__self__, "job_title", job_title)
         if last_login is not None:
             pulumi.set(__self__, "last_login", last_login)
         if last_name is not None:
             pulumi.set(__self__, "last_name", last_name)
         if lock is not None:
@@ -531,29 +524,14 @@
         return pulumi.get(self, "first_name")
 
     @first_name.setter
     def first_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "first_name", value)
 
     @property
-    @pulumi.getter(name="isLocked")
-    def is_locked(self) -> Optional[pulumi.Input[bool]]:
-        """
-        The user's lock status
-        """
-        warnings.warn("""The setting \"is_locked\" has been deprecated. Please use \"lock\" setting instead""", DeprecationWarning)
-        pulumi.log.warn("""is_locked is deprecated: The setting \"is_locked\" has been deprecated. Please use \"lock\" setting instead""")
-
-        return pulumi.get(self, "is_locked")
-
-    @is_locked.setter
-    def is_locked(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "is_locked", value)
-
-    @property
     @pulumi.getter(name="jobTitle")
     def job_title(self) -> Optional[pulumi.Input[str]]:
         """
         The user's position at your company
         """
         return pulumi.get(self, "job_title")
 
@@ -860,15 +838,14 @@
             __props__.__dict__["preferred_language"] = preferred_language
             __props__.__dict__["secondary_email"] = secondary_email
             __props__.__dict__["session_timeout"] = session_timeout
             __props__.__dict__["state"] = state
             __props__.__dict__["time_zone"] = time_zone
             __props__.__dict__["zip_code"] = zip_code
             __props__.__dict__["email_update_pending"] = None
-            __props__.__dict__["is_locked"] = None
             __props__.__dict__["last_login"] = None
             __props__.__dict__["password_expired_after"] = None
             __props__.__dict__["tfa_configured"] = None
             __props__.__dict__["user_name"] = None
         super(IamUser, __self__).__init__(
             'akamai:index/iamUser:IamUser',
             resource_name,
@@ -884,15 +861,14 @@
             city: Optional[pulumi.Input[str]] = None,
             contact_type: Optional[pulumi.Input[str]] = None,
             country: Optional[pulumi.Input[str]] = None,
             email: Optional[pulumi.Input[str]] = None,
             email_update_pending: Optional[pulumi.Input[bool]] = None,
             enable_tfa: Optional[pulumi.Input[bool]] = None,
             first_name: Optional[pulumi.Input[str]] = None,
-            is_locked: Optional[pulumi.Input[bool]] = None,
             job_title: Optional[pulumi.Input[str]] = None,
             last_login: Optional[pulumi.Input[str]] = None,
             last_name: Optional[pulumi.Input[str]] = None,
             lock: Optional[pulumi.Input[bool]] = None,
             mobile_phone: Optional[pulumi.Input[str]] = None,
             password_expired_after: Optional[pulumi.Input[str]] = None,
             phone: Optional[pulumi.Input[str]] = None,
@@ -916,15 +892,14 @@
         :param pulumi.Input[str] city: The user's city
         :param pulumi.Input[str] contact_type: To help characterize the user, the value can be any that are available from the view-contact-types operation
         :param pulumi.Input[str] country: As part of the user's location, the value can be any that are available from the view-supported-countries operation
         :param pulumi.Input[str] email: The user's email address
         :param pulumi.Input[bool] email_update_pending: Indicates whether email update is pending
         :param pulumi.Input[bool] enable_tfa: Indicates whether two-factor authentication is allowed
         :param pulumi.Input[str] first_name: The user's first name
-        :param pulumi.Input[bool] is_locked: The user's lock status
         :param pulumi.Input[str] job_title: The user's position at your company
         :param pulumi.Input[str] last_login: ISO 8601 timestamp indicating when the user last logged in
         :param pulumi.Input[str] last_name: The user's surname
         :param pulumi.Input[bool] lock: Flag to block a user account
         :param pulumi.Input[str] mobile_phone: The user's mobile phone number
         :param pulumi.Input[str] password_expired_after: The date a user's password expires
         :param pulumi.Input[str] phone: The user's main phone number
@@ -946,15 +921,14 @@
         __props__.__dict__["city"] = city
         __props__.__dict__["contact_type"] = contact_type
         __props__.__dict__["country"] = country
         __props__.__dict__["email"] = email
         __props__.__dict__["email_update_pending"] = email_update_pending
         __props__.__dict__["enable_tfa"] = enable_tfa
         __props__.__dict__["first_name"] = first_name
-        __props__.__dict__["is_locked"] = is_locked
         __props__.__dict__["job_title"] = job_title
         __props__.__dict__["last_login"] = last_login
         __props__.__dict__["last_name"] = last_name
         __props__.__dict__["lock"] = lock
         __props__.__dict__["mobile_phone"] = mobile_phone
         __props__.__dict__["password_expired_after"] = password_expired_after
         __props__.__dict__["phone"] = phone
@@ -1037,25 +1011,14 @@
     def first_name(self) -> pulumi.Output[str]:
         """
         The user's first name
         """
         return pulumi.get(self, "first_name")
 
     @property
-    @pulumi.getter(name="isLocked")
-    def is_locked(self) -> pulumi.Output[bool]:
-        """
-        The user's lock status
-        """
-        warnings.warn("""The setting \"is_locked\" has been deprecated. Please use \"lock\" setting instead""", DeprecationWarning)
-        pulumi.log.warn("""is_locked is deprecated: The setting \"is_locked\" has been deprecated. Please use \"lock\" setting instead""")
-
-        return pulumi.get(self, "is_locked")
-
-    @property
     @pulumi.getter(name="jobTitle")
     def job_title(self) -> pulumi.Output[Optional[str]]:
         """
         The user's position at your company
         """
         return pulumi.get(self, "job_title")
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/network_list.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/network_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/network_list_activations.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/network_list_activations.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,33 +13,27 @@
 
 @pulumi.input_type
 class NetworkListActivationsArgs:
     def __init__(__self__, *,
                  network_list_id: pulumi.Input[str],
                  notification_emails: pulumi.Input[Sequence[pulumi.Input[str]]],
                  sync_point: pulumi.Input[int],
-                 activate: Optional[pulumi.Input[bool]] = None,
                  network: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a NetworkListActivations resource.
         :param pulumi.Input[str] network_list_id: Unique identifier of the network list
         :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_emails: List of email addresses of Control Center users who receive an email when activation of this list is complete
         :param pulumi.Input[int] sync_point: Identifies the sync point of the network list to be activated
         :param pulumi.Input[str] network: The Akamai network on which the list is activated: STAGING or PRODUCTION
         :param pulumi.Input[str] notes: Descriptive text to accompany the activation
         """
         pulumi.set(__self__, "network_list_id", network_list_id)
         pulumi.set(__self__, "notification_emails", notification_emails)
         pulumi.set(__self__, "sync_point", sync_point)
-        if activate is not None:
-            warnings.warn("""The setting \"activate\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""activate is deprecated: The setting \"activate\" has been deprecated.""")
-        if activate is not None:
-            pulumi.set(__self__, "activate", activate)
         if network is not None:
             pulumi.set(__self__, "network", network)
         if notes is not None:
             pulumi.set(__self__, "notes", notes)
 
     @property
     @pulumi.getter(name="networkListId")
@@ -75,26 +69,14 @@
 
     @sync_point.setter
     def sync_point(self, value: pulumi.Input[int]):
         pulumi.set(self, "sync_point", value)
 
     @property
     @pulumi.getter
-    def activate(self) -> Optional[pulumi.Input[bool]]:
-        warnings.warn("""The setting \"activate\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""activate is deprecated: The setting \"activate\" has been deprecated.""")
-
-        return pulumi.get(self, "activate")
-
-    @activate.setter
-    def activate(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "activate", value)
-
-    @property
-    @pulumi.getter
     def network(self) -> Optional[pulumi.Input[str]]:
         """
         The Akamai network on which the list is activated: STAGING or PRODUCTION
         """
         return pulumi.get(self, "network")
 
     @network.setter
@@ -113,15 +95,14 @@
     def notes(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "notes", value)
 
 
 @pulumi.input_type
 class _NetworkListActivationsState:
     def __init__(__self__, *,
-                 activate: Optional[pulumi.Input[bool]] = None,
                  network: Optional[pulumi.Input[str]] = None,
                  network_list_id: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  sync_point: Optional[pulumi.Input[int]] = None):
         """
@@ -129,19 +110,14 @@
         :param pulumi.Input[str] network: The Akamai network on which the list is activated: STAGING or PRODUCTION
         :param pulumi.Input[str] network_list_id: Unique identifier of the network list
         :param pulumi.Input[str] notes: Descriptive text to accompany the activation
         :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_emails: List of email addresses of Control Center users who receive an email when activation of this list is complete
         :param pulumi.Input[str] status: This network list's current activation status in the environment specified by the "network" attribute
         :param pulumi.Input[int] sync_point: Identifies the sync point of the network list to be activated
         """
-        if activate is not None:
-            warnings.warn("""The setting \"activate\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""activate is deprecated: The setting \"activate\" has been deprecated.""")
-        if activate is not None:
-            pulumi.set(__self__, "activate", activate)
         if network is not None:
             pulumi.set(__self__, "network", network)
         if network_list_id is not None:
             pulumi.set(__self__, "network_list_id", network_list_id)
         if notes is not None:
             pulumi.set(__self__, "notes", notes)
         if notification_emails is not None:
@@ -149,26 +125,14 @@
         if status is not None:
             pulumi.set(__self__, "status", status)
         if sync_point is not None:
             pulumi.set(__self__, "sync_point", sync_point)
 
     @property
     @pulumi.getter
-    def activate(self) -> Optional[pulumi.Input[bool]]:
-        warnings.warn("""The setting \"activate\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""activate is deprecated: The setting \"activate\" has been deprecated.""")
-
-        return pulumi.get(self, "activate")
-
-    @activate.setter
-    def activate(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "activate", value)
-
-    @property
-    @pulumi.getter
     def network(self) -> Optional[pulumi.Input[str]]:
         """
         The Akamai network on which the list is activated: STAGING or PRODUCTION
         """
         return pulumi.get(self, "network")
 
     @network.setter
@@ -237,15 +201,14 @@
 
 
 class NetworkListActivations(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 activate: Optional[pulumi.Input[bool]] = None,
                  network: Optional[pulumi.Input[str]] = None,
                  network_list_id: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  sync_point: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
@@ -277,33 +240,28 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 activate: Optional[pulumi.Input[bool]] = None,
                  network: Optional[pulumi.Input[str]] = None,
                  network_list_id: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  sync_point: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NetworkListActivationsArgs.__new__(NetworkListActivationsArgs)
 
-            if activate is not None and not opts.urn:
-                warnings.warn("""The setting \"activate\" has been deprecated.""", DeprecationWarning)
-                pulumi.log.warn("""activate is deprecated: The setting \"activate\" has been deprecated.""")
-            __props__.__dict__["activate"] = activate
             __props__.__dict__["network"] = network
             if network_list_id is None and not opts.urn:
                 raise TypeError("Missing required property 'network_list_id'")
             __props__.__dict__["network_list_id"] = network_list_id
             __props__.__dict__["notes"] = notes
             if notification_emails is None and not opts.urn:
                 raise TypeError("Missing required property 'notification_emails'")
@@ -318,15 +276,14 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            activate: Optional[pulumi.Input[bool]] = None,
             network: Optional[pulumi.Input[str]] = None,
             network_list_id: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             notification_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             status: Optional[pulumi.Input[str]] = None,
             sync_point: Optional[pulumi.Input[int]] = None) -> 'NetworkListActivations':
         """
@@ -343,33 +300,24 @@
         :param pulumi.Input[str] status: This network list's current activation status in the environment specified by the "network" attribute
         :param pulumi.Input[int] sync_point: Identifies the sync point of the network list to be activated
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _NetworkListActivationsState.__new__(_NetworkListActivationsState)
 
-        __props__.__dict__["activate"] = activate
         __props__.__dict__["network"] = network
         __props__.__dict__["network_list_id"] = network_list_id
         __props__.__dict__["notes"] = notes
         __props__.__dict__["notification_emails"] = notification_emails
         __props__.__dict__["status"] = status
         __props__.__dict__["sync_point"] = sync_point
         return NetworkListActivations(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def activate(self) -> pulumi.Output[Optional[bool]]:
-        warnings.warn("""The setting \"activate\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""activate is deprecated: The setting \"activate\" has been deprecated.""")
-
-        return pulumi.get(self, "activate")
-
-    @property
-    @pulumi.getter
     def network(self) -> pulumi.Output[Optional[str]]:
         """
         The Akamai network on which the list is activated: STAGING or PRODUCTION
         """
         return pulumi.get(self, "network")
 
     @property
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/network_list_description.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/network_list_description.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/network_list_subscription.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/network_list_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/properties/get_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/get_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/properties/get_property_rules.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/properties/get_cp_code.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,148 +6,112 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'GetPropertyRulesResult',
-    'AwaitableGetPropertyRulesResult',
-    'get_property_rules',
-    'get_property_rules_output',
+    'GetCpCodeResult',
+    'AwaitableGetCpCodeResult',
+    'get_cp_code',
+    'get_cp_code_output',
 ]
 
-warnings.warn("""akamai.properties/getpropertyrules.getPropertyRules has been deprecated in favor of akamai.index/getpropertyrules.getPropertyRules""", DeprecationWarning)
+warnings.warn("""akamai.properties/getcpcode.getCpCode has been deprecated in favor of akamai.index/getcpcode.getCpCode""", DeprecationWarning)
 
 @pulumi.output_type
-class GetPropertyRulesResult:
+class GetCpCodeResult:
     """
-    A collection of values returned by getPropertyRules.
+    A collection of values returned by getCpCode.
     """
-    def __init__(__self__, contract_id=None, errors=None, group_id=None, id=None, property_id=None, rule_format=None, rules=None, version=None):
+    def __init__(__self__, contract_id=None, group_id=None, id=None, name=None, product_ids=None):
         if contract_id and not isinstance(contract_id, str):
             raise TypeError("Expected argument 'contract_id' to be a str")
         pulumi.set(__self__, "contract_id", contract_id)
-        if errors and not isinstance(errors, str):
-            raise TypeError("Expected argument 'errors' to be a str")
-        pulumi.set(__self__, "errors", errors)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if property_id and not isinstance(property_id, str):
-            raise TypeError("Expected argument 'property_id' to be a str")
-        pulumi.set(__self__, "property_id", property_id)
-        if rule_format and not isinstance(rule_format, str):
-            raise TypeError("Expected argument 'rule_format' to be a str")
-        pulumi.set(__self__, "rule_format", rule_format)
-        if rules and not isinstance(rules, str):
-            raise TypeError("Expected argument 'rules' to be a str")
-        pulumi.set(__self__, "rules", rules)
-        if version and not isinstance(version, int):
-            raise TypeError("Expected argument 'version' to be a int")
-        pulumi.set(__self__, "version", version)
+        if name and not isinstance(name, str):
+            raise TypeError("Expected argument 'name' to be a str")
+        pulumi.set(__self__, "name", name)
+        if product_ids and not isinstance(product_ids, list):
+            raise TypeError("Expected argument 'product_ids' to be a list")
+        pulumi.set(__self__, "product_ids", product_ids)
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> str:
         return pulumi.get(self, "contract_id")
 
     @property
-    @pulumi.getter
-    def errors(self) -> str:
-        return pulumi.get(self, "errors")
-
-    @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> str:
         return pulumi.get(self, "group_id")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="propertyId")
-    def property_id(self) -> str:
-        return pulumi.get(self, "property_id")
-
-    @property
-    @pulumi.getter(name="ruleFormat")
-    def rule_format(self) -> Optional[str]:
-        return pulumi.get(self, "rule_format")
-
-    @property
     @pulumi.getter
-    def rules(self) -> str:
-        return pulumi.get(self, "rules")
+    def name(self) -> str:
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter
-    def version(self) -> int:
-        return pulumi.get(self, "version")
+    @pulumi.getter(name="productIds")
+    def product_ids(self) -> Sequence[str]:
+        return pulumi.get(self, "product_ids")
 
 
-class AwaitableGetPropertyRulesResult(GetPropertyRulesResult):
+class AwaitableGetCpCodeResult(GetCpCodeResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPropertyRulesResult(
+        return GetCpCodeResult(
             contract_id=self.contract_id,
-            errors=self.errors,
             group_id=self.group_id,
             id=self.id,
-            property_id=self.property_id,
-            rule_format=self.rule_format,
-            rules=self.rules,
-            version=self.version)
+            name=self.name,
+            product_ids=self.product_ids)
 
 
-def get_property_rules(contract_id: Optional[str] = None,
-                       group_id: Optional[str] = None,
-                       property_id: Optional[str] = None,
-                       rule_format: Optional[str] = None,
-                       version: Optional[int] = None,
-                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyRulesResult:
+def get_cp_code(contract_id: Optional[str] = None,
+                group_id: Optional[str] = None,
+                name: Optional[str] = None,
+                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCpCodeResult:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_property_rules is deprecated: akamai.properties/getpropertyrules.getPropertyRules has been deprecated in favor of akamai.index/getpropertyrules.getPropertyRules""")
+    pulumi.log.warn("""get_cp_code is deprecated: akamai.properties/getcpcode.getCpCode has been deprecated in favor of akamai.index/getcpcode.getCpCode""")
     __args__ = dict()
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
-    __args__['propertyId'] = property_id
-    __args__['ruleFormat'] = rule_format
-    __args__['version'] = version
+    __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:properties/getPropertyRules:getPropertyRules', __args__, opts=opts, typ=GetPropertyRulesResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:properties/getCpCode:getCpCode', __args__, opts=opts, typ=GetCpCodeResult).value
 
-    return AwaitableGetPropertyRulesResult(
+    return AwaitableGetCpCodeResult(
         contract_id=pulumi.get(__ret__, 'contract_id'),
-        errors=pulumi.get(__ret__, 'errors'),
         group_id=pulumi.get(__ret__, 'group_id'),
         id=pulumi.get(__ret__, 'id'),
-        property_id=pulumi.get(__ret__, 'property_id'),
-        rule_format=pulumi.get(__ret__, 'rule_format'),
-        rules=pulumi.get(__ret__, 'rules'),
-        version=pulumi.get(__ret__, 'version'))
+        name=pulumi.get(__ret__, 'name'),
+        product_ids=pulumi.get(__ret__, 'product_ids'))
 
 
-@_utilities.lift_output_func(get_property_rules)
-def get_property_rules_output(contract_id: Optional[pulumi.Input[Optional[str]]] = None,
-                              group_id: Optional[pulumi.Input[Optional[str]]] = None,
-                              property_id: Optional[pulumi.Input[str]] = None,
-                              rule_format: Optional[pulumi.Input[Optional[str]]] = None,
-                              version: Optional[pulumi.Input[Optional[int]]] = None,
-                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyRulesResult]:
+@_utilities.lift_output_func(get_cp_code)
+def get_cp_code_output(contract_id: Optional[pulumi.Input[str]] = None,
+                       group_id: Optional[pulumi.Input[str]] = None,
+                       name: Optional[pulumi.Input[str]] = None,
+                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCpCodeResult]:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_property_rules is deprecated: akamai.properties/getpropertyrules.getPropertyRules has been deprecated in favor of akamai.index/getpropertyrules.getPropertyRules""")
+    pulumi.log.warn("""get_cp_code is deprecated: akamai.properties/getcpcode.getCpCode has been deprecated in favor of akamai.index/getcpcode.getCpCode""")
     ...
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/property_activation.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/property.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,605 +7,545 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['PropertyActivationArgs', 'PropertyActivation']
+__all__ = ['PropertyArgs', 'Property']
 
 @pulumi.input_type
-class PropertyActivationArgs:
+class PropertyArgs:
     def __init__(__self__, *,
-                 contacts: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 version: pulumi.Input[int],
-                 activation_id: Optional[pulumi.Input[str]] = None,
-                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
-                 compliance_record: Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']] = None,
-                 network: Optional[pulumi.Input[str]] = None,
-                 note: Optional[pulumi.Input[str]] = None,
-                 property: Optional[pulumi.Input[str]] = None,
-                 property_id: Optional[pulumi.Input[str]] = None,
-                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]] = None,
-                 rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleWarningArgs']]]] = None):
-        """
-        The set of arguments for constructing a PropertyActivation resource.
-        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: automatically acknowledge all rule warnings for activation to continue. default is true
-        :param pulumi.Input['PropertyActivationComplianceRecordArgs'] compliance_record: Provides an audit record when activating on a production network
-        :param pulumi.Input[str] note: assigns a log message to the activation request
-        """
-        pulumi.set(__self__, "contacts", contacts)
-        pulumi.set(__self__, "version", version)
-        if activation_id is not None:
-            pulumi.set(__self__, "activation_id", activation_id)
-        if auto_acknowledge_rule_warnings is not None:
-            pulumi.set(__self__, "auto_acknowledge_rule_warnings", auto_acknowledge_rule_warnings)
-        if compliance_record is not None:
-            pulumi.set(__self__, "compliance_record", compliance_record)
-        if network is not None:
-            pulumi.set(__self__, "network", network)
-        if note is not None:
-            pulumi.set(__self__, "note", note)
-        if property is not None:
-            warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
-        if property is not None:
-            pulumi.set(__self__, "property", property)
-        if property_id is not None:
-            pulumi.set(__self__, "property_id", property_id)
-        if rule_errors is not None:
-            pulumi.set(__self__, "rule_errors", rule_errors)
-        if rule_warnings is not None:
-            warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
-            pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
-        if rule_warnings is not None:
-            pulumi.set(__self__, "rule_warnings", rule_warnings)
-
-    @property
-    @pulumi.getter
-    def contacts(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        return pulumi.get(self, "contacts")
-
-    @contacts.setter
-    def contacts(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "contacts", value)
-
-    @property
-    @pulumi.getter
-    def version(self) -> pulumi.Input[int]:
-        return pulumi.get(self, "version")
-
-    @version.setter
-    def version(self, value: pulumi.Input[int]):
-        pulumi.set(self, "version", value)
+                 contract_id: pulumi.Input[str],
+                 group_id: pulumi.Input[str],
+                 product_id: pulumi.Input[str],
+                 hostnames: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyHostnameArgs']]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 rule_format: Optional[pulumi.Input[str]] = None,
+                 rules: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a Property resource.
+        :param pulumi.Input[str] contract_id: Contract ID to be assigned to the Property
+        :param pulumi.Input[str] group_id: Group ID to be assigned to the Property
+        :param pulumi.Input[str] product_id: Product ID to be assigned to the Property
+        :param pulumi.Input[str] name: Name to give to the Property (must be unique)
+        :param pulumi.Input[str] rule_format: Specify the rule format version (defaults to latest version available when created)
+        :param pulumi.Input[str] rules: Property Rules as JSON
+        """
+        pulumi.set(__self__, "contract_id", contract_id)
+        pulumi.set(__self__, "group_id", group_id)
+        pulumi.set(__self__, "product_id", product_id)
+        if hostnames is not None:
+            pulumi.set(__self__, "hostnames", hostnames)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if rule_format is not None:
+            pulumi.set(__self__, "rule_format", rule_format)
+        if rules is not None:
+            pulumi.set(__self__, "rules", rules)
 
     @property
-    @pulumi.getter(name="activationId")
-    def activation_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "activation_id")
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> pulumi.Input[str]:
+        """
+        Contract ID to be assigned to the Property
+        """
+        return pulumi.get(self, "contract_id")
 
-    @activation_id.setter
-    def activation_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "activation_id", value)
+    @contract_id.setter
+    def contract_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "contract_id", value)
 
     @property
-    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
-    def auto_acknowledge_rule_warnings(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> pulumi.Input[str]:
         """
-        automatically acknowledge all rule warnings for activation to continue. default is true
+        Group ID to be assigned to the Property
         """
-        return pulumi.get(self, "auto_acknowledge_rule_warnings")
+        return pulumi.get(self, "group_id")
 
-    @auto_acknowledge_rule_warnings.setter
-    def auto_acknowledge_rule_warnings(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "auto_acknowledge_rule_warnings", value)
+    @group_id.setter
+    def group_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "group_id", value)
 
     @property
-    @pulumi.getter(name="complianceRecord")
-    def compliance_record(self) -> Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']]:
+    @pulumi.getter(name="productId")
+    def product_id(self) -> pulumi.Input[str]:
         """
-        Provides an audit record when activating on a production network
+        Product ID to be assigned to the Property
         """
-        return pulumi.get(self, "compliance_record")
+        return pulumi.get(self, "product_id")
 
-    @compliance_record.setter
-    def compliance_record(self, value: Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']]):
-        pulumi.set(self, "compliance_record", value)
+    @product_id.setter
+    def product_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "product_id", value)
 
     @property
     @pulumi.getter
-    def network(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "network")
+    def hostnames(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyHostnameArgs']]]]:
+        return pulumi.get(self, "hostnames")
 
-    @network.setter
-    def network(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "network", value)
+    @hostnames.setter
+    def hostnames(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyHostnameArgs']]]]):
+        pulumi.set(self, "hostnames", value)
 
     @property
     @pulumi.getter
-    def note(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        assigns a log message to the activation request
+        Name to give to the Property (must be unique)
         """
-        return pulumi.get(self, "note")
-
-    @note.setter
-    def note(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "note", value)
-
-    @property
-    @pulumi.getter(name="propertyId")
-    def property_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "property_id")
+        return pulumi.get(self, "name")
 
-    @property_id.setter
-    def property_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "property_id", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="ruleErrors")
-    def rule_errors(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]]:
-        return pulumi.get(self, "rule_errors")
-
-    @rule_errors.setter
-    def rule_errors(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]]):
-        pulumi.set(self, "rule_errors", value)
+    @pulumi.getter(name="ruleFormat")
+    def rule_format(self) -> Optional[pulumi.Input[str]]:
+        """
+        Specify the rule format version (defaults to latest version available when created)
+        """
+        return pulumi.get(self, "rule_format")
 
-    @property
-    @pulumi.getter(name="ruleWarnings")
-    def rule_warnings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleWarningArgs']]]]:
-        warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
-        pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
-
-        return pulumi.get(self, "rule_warnings")
-
-    @rule_warnings.setter
-    def rule_warnings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleWarningArgs']]]]):
-        pulumi.set(self, "rule_warnings", value)
+    @rule_format.setter
+    def rule_format(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rule_format", value)
 
     @property
     @pulumi.getter
-    def property(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
-
-        return pulumi.get(self, "property")
-
-    @property.setter
-    def property(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "property", value)
+    def rules(self) -> Optional[pulumi.Input[str]]:
+        """
+        Property Rules as JSON
+        """
+        return pulumi.get(self, "rules")
+
+    @rules.setter
+    def rules(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rules", value)
 
 
 @pulumi.input_type
-class _PropertyActivationState:
+class _PropertyState:
     def __init__(__self__, *,
-                 activation_id: Optional[pulumi.Input[str]] = None,
-                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
-                 compliance_record: Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']] = None,
-                 contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 errors: Optional[pulumi.Input[str]] = None,
-                 network: Optional[pulumi.Input[str]] = None,
-                 note: Optional[pulumi.Input[str]] = None,
-                 property: Optional[pulumi.Input[str]] = None,
-                 property_id: Optional[pulumi.Input[str]] = None,
-                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]] = None,
-                 rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleWarningArgs']]]] = None,
-                 status: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[int]] = None,
-                 warnings: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering PropertyActivation resources.
-        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: automatically acknowledge all rule warnings for activation to continue. default is true
-        :param pulumi.Input['PropertyActivationComplianceRecordArgs'] compliance_record: Provides an audit record when activating on a production network
-        :param pulumi.Input[str] note: assigns a log message to the activation request
-        """
-        if activation_id is not None:
-            pulumi.set(__self__, "activation_id", activation_id)
-        if auto_acknowledge_rule_warnings is not None:
-            pulumi.set(__self__, "auto_acknowledge_rule_warnings", auto_acknowledge_rule_warnings)
-        if compliance_record is not None:
-            pulumi.set(__self__, "compliance_record", compliance_record)
-        if contacts is not None:
-            pulumi.set(__self__, "contacts", contacts)
-        if errors is not None:
-            pulumi.set(__self__, "errors", errors)
-        if network is not None:
-            pulumi.set(__self__, "network", network)
-        if note is not None:
-            pulumi.set(__self__, "note", note)
-        if property is not None:
-            warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
-        if property is not None:
-            pulumi.set(__self__, "property", property)
-        if property_id is not None:
-            pulumi.set(__self__, "property_id", property_id)
+                 contract_id: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[str]] = None,
+                 hostnames: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyHostnameArgs']]]] = None,
+                 latest_version: Optional[pulumi.Input[int]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 product_id: Optional[pulumi.Input[str]] = None,
+                 production_version: Optional[pulumi.Input[int]] = None,
+                 read_version: Optional[pulumi.Input[int]] = None,
+                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyRuleErrorArgs']]]] = None,
+                 rule_format: Optional[pulumi.Input[str]] = None,
+                 rules: Optional[pulumi.Input[str]] = None,
+                 staging_version: Optional[pulumi.Input[int]] = None):
+        """
+        Input properties used for looking up and filtering Property resources.
+        :param pulumi.Input[str] contract_id: Contract ID to be assigned to the Property
+        :param pulumi.Input[str] group_id: Group ID to be assigned to the Property
+        :param pulumi.Input[int] latest_version: Property's current latest version number
+        :param pulumi.Input[str] name: Name to give to the Property (must be unique)
+        :param pulumi.Input[str] product_id: Product ID to be assigned to the Property
+        :param pulumi.Input[int] production_version: Property's version currently activated in production (zero when not active in production)
+        :param pulumi.Input[int] read_version: Required property's version to be read
+        :param pulumi.Input[str] rule_format: Specify the rule format version (defaults to latest version available when created)
+        :param pulumi.Input[str] rules: Property Rules as JSON
+        :param pulumi.Input[int] staging_version: Property's version currently activated in staging (zero when not active in staging)
+        """
+        if contract_id is not None:
+            pulumi.set(__self__, "contract_id", contract_id)
+        if group_id is not None:
+            pulumi.set(__self__, "group_id", group_id)
+        if hostnames is not None:
+            pulumi.set(__self__, "hostnames", hostnames)
+        if latest_version is not None:
+            pulumi.set(__self__, "latest_version", latest_version)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if product_id is not None:
+            pulumi.set(__self__, "product_id", product_id)
+        if production_version is not None:
+            pulumi.set(__self__, "production_version", production_version)
+        if read_version is not None:
+            pulumi.set(__self__, "read_version", read_version)
         if rule_errors is not None:
             pulumi.set(__self__, "rule_errors", rule_errors)
-        if rule_warnings is not None:
-            warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
-            pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
-        if rule_warnings is not None:
-            pulumi.set(__self__, "rule_warnings", rule_warnings)
-        if status is not None:
-            pulumi.set(__self__, "status", status)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
-        if warnings is not None:
-            pulumi.set(__self__, "warnings", warnings)
+        if rule_format is not None:
+            pulumi.set(__self__, "rule_format", rule_format)
+        if rules is not None:
+            pulumi.set(__self__, "rules", rules)
+        if staging_version is not None:
+            pulumi.set(__self__, "staging_version", staging_version)
 
     @property
-    @pulumi.getter(name="activationId")
-    def activation_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "activation_id")
-
-    @activation_id.setter
-    def activation_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "activation_id", value)
-
-    @property
-    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
-    def auto_acknowledge_rule_warnings(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> Optional[pulumi.Input[str]]:
         """
-        automatically acknowledge all rule warnings for activation to continue. default is true
+        Contract ID to be assigned to the Property
         """
-        return pulumi.get(self, "auto_acknowledge_rule_warnings")
+        return pulumi.get(self, "contract_id")
 
-    @auto_acknowledge_rule_warnings.setter
-    def auto_acknowledge_rule_warnings(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "auto_acknowledge_rule_warnings", value)
+    @contract_id.setter
+    def contract_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "contract_id", value)
 
     @property
-    @pulumi.getter(name="complianceRecord")
-    def compliance_record(self) -> Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']]:
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Provides an audit record when activating on a production network
+        Group ID to be assigned to the Property
         """
-        return pulumi.get(self, "compliance_record")
+        return pulumi.get(self, "group_id")
 
-    @compliance_record.setter
-    def compliance_record(self, value: Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']]):
-        pulumi.set(self, "compliance_record", value)
+    @group_id.setter
+    def group_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "group_id", value)
 
     @property
     @pulumi.getter
-    def contacts(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "contacts")
+    def hostnames(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyHostnameArgs']]]]:
+        return pulumi.get(self, "hostnames")
 
-    @contacts.setter
-    def contacts(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "contacts", value)
+    @hostnames.setter
+    def hostnames(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyHostnameArgs']]]]):
+        pulumi.set(self, "hostnames", value)
 
     @property
-    @pulumi.getter
-    def errors(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "errors")
+    @pulumi.getter(name="latestVersion")
+    def latest_version(self) -> Optional[pulumi.Input[int]]:
+        """
+        Property's current latest version number
+        """
+        return pulumi.get(self, "latest_version")
 
-    @errors.setter
-    def errors(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "errors", value)
+    @latest_version.setter
+    def latest_version(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "latest_version", value)
 
     @property
     @pulumi.getter
-    def network(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "network")
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name to give to the Property (must be unique)
+        """
+        return pulumi.get(self, "name")
 
-    @network.setter
-    def network(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "network", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def note(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="productId")
+    def product_id(self) -> Optional[pulumi.Input[str]]:
         """
-        assigns a log message to the activation request
+        Product ID to be assigned to the Property
         """
-        return pulumi.get(self, "note")
+        return pulumi.get(self, "product_id")
 
-    @note.setter
-    def note(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "note", value)
+    @product_id.setter
+    def product_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "product_id", value)
 
     @property
-    @pulumi.getter(name="propertyId")
-    def property_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "property_id")
+    @pulumi.getter(name="productionVersion")
+    def production_version(self) -> Optional[pulumi.Input[int]]:
+        """
+        Property's version currently activated in production (zero when not active in production)
+        """
+        return pulumi.get(self, "production_version")
+
+    @production_version.setter
+    def production_version(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "production_version", value)
+
+    @property
+    @pulumi.getter(name="readVersion")
+    def read_version(self) -> Optional[pulumi.Input[int]]:
+        """
+        Required property's version to be read
+        """
+        return pulumi.get(self, "read_version")
 
-    @property_id.setter
-    def property_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "property_id", value)
+    @read_version.setter
+    def read_version(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "read_version", value)
 
     @property
     @pulumi.getter(name="ruleErrors")
-    def rule_errors(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]]:
+    def rule_errors(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyRuleErrorArgs']]]]:
         return pulumi.get(self, "rule_errors")
 
     @rule_errors.setter
-    def rule_errors(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]]):
+    def rule_errors(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyRuleErrorArgs']]]]):
         pulumi.set(self, "rule_errors", value)
 
     @property
-    @pulumi.getter(name="ruleWarnings")
-    def rule_warnings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleWarningArgs']]]]:
-        warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
-        pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
-
-        return pulumi.get(self, "rule_warnings")
-
-    @rule_warnings.setter
-    def rule_warnings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleWarningArgs']]]]):
-        pulumi.set(self, "rule_warnings", value)
-
-    @property
-    @pulumi.getter
-    def status(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "status")
-
-    @status.setter
-    def status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "status", value)
-
-    @property
-    @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "version")
+    @pulumi.getter(name="ruleFormat")
+    def rule_format(self) -> Optional[pulumi.Input[str]]:
+        """
+        Specify the rule format version (defaults to latest version available when created)
+        """
+        return pulumi.get(self, "rule_format")
 
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "version", value)
+    @rule_format.setter
+    def rule_format(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rule_format", value)
 
     @property
     @pulumi.getter
-    def warnings(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "warnings")
+    def rules(self) -> Optional[pulumi.Input[str]]:
+        """
+        Property Rules as JSON
+        """
+        return pulumi.get(self, "rules")
 
-    @warnings.setter
-    def warnings(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "warnings", value)
+    @rules.setter
+    def rules(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rules", value)
 
     @property
-    @pulumi.getter
-    def property(self) -> Optional[pulumi.Input[str]]:
-        warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
-
-        return pulumi.get(self, "property")
+    @pulumi.getter(name="stagingVersion")
+    def staging_version(self) -> Optional[pulumi.Input[int]]:
+        """
+        Property's version currently activated in staging (zero when not active in staging)
+        """
+        return pulumi.get(self, "staging_version")
 
-    @property.setter
-    def property(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "property", value)
+    @staging_version.setter
+    def staging_version(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "staging_version", value)
 
 
-class PropertyActivation(pulumi.CustomResource):
+class Property(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 activation_id: Optional[pulumi.Input[str]] = None,
-                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
-                 compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']]] = None,
-                 contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 network: Optional[pulumi.Input[str]] = None,
-                 note: Optional[pulumi.Input[str]] = None,
-                 property: Optional[pulumi.Input[str]] = None,
-                 property_id: Optional[pulumi.Input[str]] = None,
-                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleErrorArgs']]]]] = None,
-                 rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleWarningArgs']]]]] = None,
-                 version: Optional[pulumi.Input[int]] = None,
+                 contract_id: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[str]] = None,
+                 hostnames: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyHostnameArgs']]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 product_id: Optional[pulumi.Input[str]] = None,
+                 rule_format: Optional[pulumi.Input[str]] = None,
+                 rules: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a PropertyActivation resource with the given unique name, props, and options.
+        Create a Property resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: automatically acknowledge all rule warnings for activation to continue. default is true
-        :param pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']] compliance_record: Provides an audit record when activating on a production network
-        :param pulumi.Input[str] note: assigns a log message to the activation request
+        :param pulumi.Input[str] contract_id: Contract ID to be assigned to the Property
+        :param pulumi.Input[str] group_id: Group ID to be assigned to the Property
+        :param pulumi.Input[str] name: Name to give to the Property (must be unique)
+        :param pulumi.Input[str] product_id: Product ID to be assigned to the Property
+        :param pulumi.Input[str] rule_format: Specify the rule format version (defaults to latest version available when created)
+        :param pulumi.Input[str] rules: Property Rules as JSON
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: PropertyActivationArgs,
+                 args: PropertyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a PropertyActivation resource with the given unique name, props, and options.
+        Create a Property resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param PropertyActivationArgs args: The arguments to use to populate this resource's properties.
+        :param PropertyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(PropertyActivationArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(PropertyArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 activation_id: Optional[pulumi.Input[str]] = None,
-                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
-                 compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']]] = None,
-                 contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 network: Optional[pulumi.Input[str]] = None,
-                 note: Optional[pulumi.Input[str]] = None,
-                 property: Optional[pulumi.Input[str]] = None,
-                 property_id: Optional[pulumi.Input[str]] = None,
-                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleErrorArgs']]]]] = None,
-                 rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleWarningArgs']]]]] = None,
-                 version: Optional[pulumi.Input[int]] = None,
+                 contract_id: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[str]] = None,
+                 hostnames: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyHostnameArgs']]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 product_id: Optional[pulumi.Input[str]] = None,
+                 rule_format: Optional[pulumi.Input[str]] = None,
+                 rules: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = PropertyActivationArgs.__new__(PropertyActivationArgs)
+            __props__ = PropertyArgs.__new__(PropertyArgs)
 
-            __props__.__dict__["activation_id"] = activation_id
-            __props__.__dict__["auto_acknowledge_rule_warnings"] = auto_acknowledge_rule_warnings
-            __props__.__dict__["compliance_record"] = compliance_record
-            if contacts is None and not opts.urn:
-                raise TypeError("Missing required property 'contacts'")
-            __props__.__dict__["contacts"] = contacts
-            __props__.__dict__["network"] = network
-            __props__.__dict__["note"] = note
-            if property is not None and not opts.urn:
-                warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
-                pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
-            __props__.__dict__["property"] = property
-            __props__.__dict__["property_id"] = property_id
-            __props__.__dict__["rule_errors"] = rule_errors
-            if rule_warnings is not None and not opts.urn:
-                warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
-                pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
-            __props__.__dict__["rule_warnings"] = rule_warnings
-            if version is None and not opts.urn:
-                raise TypeError("Missing required property 'version'")
-            __props__.__dict__["version"] = version
-            __props__.__dict__["errors"] = None
-            __props__.__dict__["status"] = None
-            __props__.__dict__["warnings"] = None
-        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="akamai:properties/propertyActivation:PropertyActivation")])
+            if contract_id is None and not opts.urn:
+                raise TypeError("Missing required property 'contract_id'")
+            __props__.__dict__["contract_id"] = contract_id
+            if group_id is None and not opts.urn:
+                raise TypeError("Missing required property 'group_id'")
+            __props__.__dict__["group_id"] = group_id
+            __props__.__dict__["hostnames"] = hostnames
+            __props__.__dict__["name"] = name
+            if product_id is None and not opts.urn:
+                raise TypeError("Missing required property 'product_id'")
+            __props__.__dict__["product_id"] = product_id
+            __props__.__dict__["rule_format"] = rule_format
+            __props__.__dict__["rules"] = rules
+            __props__.__dict__["latest_version"] = None
+            __props__.__dict__["production_version"] = None
+            __props__.__dict__["read_version"] = None
+            __props__.__dict__["rule_errors"] = None
+            __props__.__dict__["staging_version"] = None
+        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="akamai:properties/property:Property")])
         opts = pulumi.ResourceOptions.merge(opts, alias_opts)
-        super(PropertyActivation, __self__).__init__(
-            'akamai:index/propertyActivation:PropertyActivation',
+        super(Property, __self__).__init__(
+            'akamai:index/property:Property',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            activation_id: Optional[pulumi.Input[str]] = None,
-            auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
-            compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']]] = None,
-            contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            errors: Optional[pulumi.Input[str]] = None,
-            network: Optional[pulumi.Input[str]] = None,
-            note: Optional[pulumi.Input[str]] = None,
-            property: Optional[pulumi.Input[str]] = None,
-            property_id: Optional[pulumi.Input[str]] = None,
-            rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleErrorArgs']]]]] = None,
-            rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleWarningArgs']]]]] = None,
-            status: Optional[pulumi.Input[str]] = None,
-            version: Optional[pulumi.Input[int]] = None,
-            warnings: Optional[pulumi.Input[str]] = None) -> 'PropertyActivation':
+            contract_id: Optional[pulumi.Input[str]] = None,
+            group_id: Optional[pulumi.Input[str]] = None,
+            hostnames: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyHostnameArgs']]]]] = None,
+            latest_version: Optional[pulumi.Input[int]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            product_id: Optional[pulumi.Input[str]] = None,
+            production_version: Optional[pulumi.Input[int]] = None,
+            read_version: Optional[pulumi.Input[int]] = None,
+            rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyRuleErrorArgs']]]]] = None,
+            rule_format: Optional[pulumi.Input[str]] = None,
+            rules: Optional[pulumi.Input[str]] = None,
+            staging_version: Optional[pulumi.Input[int]] = None) -> 'Property':
         """
-        Get an existing PropertyActivation resource's state with the given name, id, and optional extra
+        Get an existing Property resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: automatically acknowledge all rule warnings for activation to continue. default is true
-        :param pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']] compliance_record: Provides an audit record when activating on a production network
-        :param pulumi.Input[str] note: assigns a log message to the activation request
+        :param pulumi.Input[str] contract_id: Contract ID to be assigned to the Property
+        :param pulumi.Input[str] group_id: Group ID to be assigned to the Property
+        :param pulumi.Input[int] latest_version: Property's current latest version number
+        :param pulumi.Input[str] name: Name to give to the Property (must be unique)
+        :param pulumi.Input[str] product_id: Product ID to be assigned to the Property
+        :param pulumi.Input[int] production_version: Property's version currently activated in production (zero when not active in production)
+        :param pulumi.Input[int] read_version: Required property's version to be read
+        :param pulumi.Input[str] rule_format: Specify the rule format version (defaults to latest version available when created)
+        :param pulumi.Input[str] rules: Property Rules as JSON
+        :param pulumi.Input[int] staging_version: Property's version currently activated in staging (zero when not active in staging)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _PropertyActivationState.__new__(_PropertyActivationState)
+        __props__ = _PropertyState.__new__(_PropertyState)
 
-        __props__.__dict__["activation_id"] = activation_id
-        __props__.__dict__["auto_acknowledge_rule_warnings"] = auto_acknowledge_rule_warnings
-        __props__.__dict__["compliance_record"] = compliance_record
-        __props__.__dict__["contacts"] = contacts
-        __props__.__dict__["errors"] = errors
-        __props__.__dict__["network"] = network
-        __props__.__dict__["note"] = note
-        __props__.__dict__["property"] = property
-        __props__.__dict__["property_id"] = property_id
+        __props__.__dict__["contract_id"] = contract_id
+        __props__.__dict__["group_id"] = group_id
+        __props__.__dict__["hostnames"] = hostnames
+        __props__.__dict__["latest_version"] = latest_version
+        __props__.__dict__["name"] = name
+        __props__.__dict__["product_id"] = product_id
+        __props__.__dict__["production_version"] = production_version
+        __props__.__dict__["read_version"] = read_version
         __props__.__dict__["rule_errors"] = rule_errors
-        __props__.__dict__["rule_warnings"] = rule_warnings
-        __props__.__dict__["status"] = status
-        __props__.__dict__["version"] = version
-        __props__.__dict__["warnings"] = warnings
-        return PropertyActivation(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter(name="activationId")
-    def activation_id(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "activation_id")
+        __props__.__dict__["rule_format"] = rule_format
+        __props__.__dict__["rules"] = rules
+        __props__.__dict__["staging_version"] = staging_version
+        return Property(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
-    def auto_acknowledge_rule_warnings(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> pulumi.Output[str]:
         """
-        automatically acknowledge all rule warnings for activation to continue. default is true
+        Contract ID to be assigned to the Property
         """
-        return pulumi.get(self, "auto_acknowledge_rule_warnings")
+        return pulumi.get(self, "contract_id")
 
     @property
-    @pulumi.getter(name="complianceRecord")
-    def compliance_record(self) -> pulumi.Output[Optional['outputs.PropertyActivationComplianceRecord']]:
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> pulumi.Output[str]:
         """
-        Provides an audit record when activating on a production network
+        Group ID to be assigned to the Property
         """
-        return pulumi.get(self, "compliance_record")
+        return pulumi.get(self, "group_id")
 
     @property
     @pulumi.getter
-    def contacts(self) -> pulumi.Output[Sequence[str]]:
-        return pulumi.get(self, "contacts")
+    def hostnames(self) -> pulumi.Output[Optional[Sequence['outputs.PropertyHostname']]]:
+        return pulumi.get(self, "hostnames")
 
     @property
-    @pulumi.getter
-    def errors(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "errors")
-
-    @property
-    @pulumi.getter
-    def network(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "network")
+    @pulumi.getter(name="latestVersion")
+    def latest_version(self) -> pulumi.Output[int]:
+        """
+        Property's current latest version number
+        """
+        return pulumi.get(self, "latest_version")
 
     @property
     @pulumi.getter
-    def note(self) -> pulumi.Output[Optional[str]]:
+    def name(self) -> pulumi.Output[str]:
         """
-        assigns a log message to the activation request
+        Name to give to the Property (must be unique)
         """
-        return pulumi.get(self, "note")
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="propertyId")
-    def property_id(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "property_id")
+    @pulumi.getter(name="productId")
+    def product_id(self) -> pulumi.Output[str]:
+        """
+        Product ID to be assigned to the Property
+        """
+        return pulumi.get(self, "product_id")
 
     @property
-    @pulumi.getter(name="ruleErrors")
-    def rule_errors(self) -> pulumi.Output[Sequence['outputs.PropertyActivationRuleError']]:
-        return pulumi.get(self, "rule_errors")
+    @pulumi.getter(name="productionVersion")
+    def production_version(self) -> pulumi.Output[int]:
+        """
+        Property's version currently activated in production (zero when not active in production)
+        """
+        return pulumi.get(self, "production_version")
 
     @property
-    @pulumi.getter(name="ruleWarnings")
-    def rule_warnings(self) -> pulumi.Output[Sequence['outputs.PropertyActivationRuleWarning']]:
-        warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
-        pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
-
-        return pulumi.get(self, "rule_warnings")
+    @pulumi.getter(name="readVersion")
+    def read_version(self) -> pulumi.Output[int]:
+        """
+        Required property's version to be read
+        """
+        return pulumi.get(self, "read_version")
 
     @property
-    @pulumi.getter
-    def status(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "status")
+    @pulumi.getter(name="ruleErrors")
+    def rule_errors(self) -> pulumi.Output[Sequence['outputs.PropertyRuleError']]:
+        return pulumi.get(self, "rule_errors")
 
     @property
-    @pulumi.getter
-    def version(self) -> pulumi.Output[int]:
-        return pulumi.get(self, "version")
+    @pulumi.getter(name="ruleFormat")
+    def rule_format(self) -> pulumi.Output[str]:
+        """
+        Specify the rule format version (defaults to latest version available when created)
+        """
+        return pulumi.get(self, "rule_format")
 
     @property
     @pulumi.getter
-    def warnings(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "warnings")
+    def rules(self) -> pulumi.Output[str]:
+        """
+        Property Rules as JSON
+        """
+        return pulumi.get(self, "rules")
 
     @property
-    @pulumi.getter
-    def property(self) -> pulumi.Output[str]:
-        warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
-        pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
-
-        return pulumi.get(self, "property")
+    @pulumi.getter(name="stagingVersion")
+    def staging_version(self) -> pulumi.Output[int]:
+        """
+        Property's version currently activated in staging (zero when not active in staging)
+        """
+        return pulumi.get(self, "staging_version")
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai.egg-info/PKG-INFO` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-akamai
-Version: 5.1.0a1689311902
+Version: 6.0.0a1690300875
 Summary: A Pulumi package for creating and managing akamai cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-akamai
 Keywords: pulumi akamai
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -34,15 +34,15 @@
 
     $ pip install pulumi_akamai
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-akamai/sdk/v5
+    $ go get github.com/pulumi/pulumi-akamai/sdk/v6
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Akamai
```

### Comparing `pulumi_akamai-5.1.0a1689311902/pulumi_akamai.egg-info/SOURCES.txt` & `pulumi_akamai-6.0.0a1690300875/pulumi_akamai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 pulumi_akamai/app_sec_slow_post_protection.py
 pulumi_akamai/app_sec_threat_intel.py
 pulumi_akamai/app_sec_version_nodes.py
 pulumi_akamai/app_sec_waf_mode.py
 pulumi_akamai/app_sec_waf_protection.py
 pulumi_akamai/app_sec_wap_selected_hostnames.py
 pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py
+pulumi_akamai/appsec_advanced_settings_pii_learning.py
 pulumi_akamai/appsec_advanced_settings_request_body.py
 pulumi_akamai/botman_akamai_bot_category_action.py
 pulumi_akamai/botman_bot_analytics_cookie.py
 pulumi_akamai/botman_bot_category_exception.py
 pulumi_akamai/botman_bot_detection_action.py
 pulumi_akamai/botman_bot_management_settings.py
 pulumi_akamai/botman_challenge_action.py
@@ -134,14 +135,15 @@
 pulumi_akamai/get_app_sec_slow_post.py
 pulumi_akamai/get_app_sec_threat_intel.py
 pulumi_akamai/get_app_sec_tuning_recommendations.py
 pulumi_akamai/get_app_sec_version_notes.py
 pulumi_akamai/get_app_sec_waf_mode.py
 pulumi_akamai/get_app_sec_wap_selected_hostnames.py
 pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py
+pulumi_akamai/get_appsec_advanced_settings_pii_learning.py
 pulumi_akamai/get_appsec_advanced_settings_request_body.py
 pulumi_akamai/get_authorities_set.py
 pulumi_akamai/get_botman_akamai_bot_category.py
 pulumi_akamai/get_botman_akamai_bot_category_action.py
 pulumi_akamai/get_botman_akamai_defined_bot.py
 pulumi_akamai/get_botman_bot_analytics_cookie.py
 pulumi_akamai/get_botman_bot_analytics_cookie_values.py
@@ -203,14 +205,16 @@
 pulumi_akamai/get_iam_countries.py
 pulumi_akamai/get_iam_grantable_roles.py
 pulumi_akamai/get_iam_roles.py
 pulumi_akamai/get_iam_states.py
 pulumi_akamai/get_iam_supported_langs.py
 pulumi_akamai/get_iam_timeout_policies.py
 pulumi_akamai/get_iam_timezones.py
+pulumi_akamai/get_imaging_policy_image.py
+pulumi_akamai/get_imaging_policy_video.py
 pulumi_akamai/get_network_lists.py
 pulumi_akamai/get_properties.py
 pulumi_akamai/get_properties_search.py
 pulumi_akamai/get_property.py
 pulumi_akamai/get_property_activation.py
 pulumi_akamai/get_property_hostnames.py
 pulumi_akamai/get_property_include.py
@@ -230,14 +234,17 @@
 pulumi_akamai/gtm_geomap.py
 pulumi_akamai/gtm_property.py
 pulumi_akamai/gtm_resource.py
 pulumi_akamai/iam_blocked_user_properties.py
 pulumi_akamai/iam_group.py
 pulumi_akamai/iam_role.py
 pulumi_akamai/iam_user.py
+pulumi_akamai/imaging_policy_image.py
+pulumi_akamai/imaging_policy_set.py
+pulumi_akamai/imaging_policy_video.py
 pulumi_akamai/network_list.py
 pulumi_akamai/network_list_activations.py
 pulumi_akamai/network_list_description.py
 pulumi_akamai/network_list_subscription.py
 pulumi_akamai/outputs.py
 pulumi_akamai/property.py
 pulumi_akamai/property_activation.py
```

### Comparing `pulumi_akamai-5.1.0a1689311902/setup.py` & `pulumi_akamai-6.0.0a1690300875/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.1.0a1689311902"
-PLUGIN_VERSION = "5.1.0-alpha.1689311902+24f24382"
+VERSION = "6.0.0a1690300875"
+PLUGIN_VERSION = "6.0.0-alpha.1690300875+c3feb58e"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'akamai', PLUGIN_VERSION])
         except OSError as error:
```

