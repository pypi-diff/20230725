# Comparing `tmp/scs-analysis-2.7.7.tar.gz` & `tmp/scs-analysis-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-analysis-2.7.7.tar", last modified: Fri Jun 30 08:21:15 2023, max compression
+gzip compressed data, was "scs-analysis-2.8.5.tar", last modified: Tue Jul 25 12:39:48 2023, max compression
```

## Comparing `scs-analysis-2.7.7.tar` & `scs-analysis-2.8.5.tar`

### file list

```diff
@@ -1,166 +1,164 @@
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.425173 scs-analysis-2.7.7/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/LICENSE
--rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/MANIFEST.in
--rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-30 08:21:15.425173 scs-analysis-2.7.7/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)      766 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/README.md
--rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/README.rst
--rw-rw-r--   0 jade      (1002) jade      (1002)      232 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/requirements.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-30 08:21:15.425173 scs-analysis-2.7.7/setup.cfg
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5196 2023-06-30 08:21:07.000000 scs-analysis-2.7.7/setup.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.409173 scs-analysis-2.7.7/src/
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.417173 scs-analysis-2.7.7/src/scs_analysis/
--rwxrwxr-x   0 jade      (1002) jade      (1002)      183 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/__init__.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2467 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/access_key.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)    10112 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/alert.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4013 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/alert_status.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2235 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/aws_api_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4611 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/aws_byline.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2655 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/aws_client_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7224 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/aws_mqtt_client.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7079 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/aws_topic_history.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2139 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/aws_topic_publisher.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2918 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/aws_upload_interval.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)    14469 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/baseline.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5964 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/baseline_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.417173 scs-analysis-2.7.7/src/scs_analysis/chart/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/chart/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1630 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/chart/chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4546 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/chart/histo_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4249 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/chart/multi_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4317 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/chart/single_chart.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.425173 scs-analysis-2.7.7/src/scs_analysis/cmd/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1966 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_access_key.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9948 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_alert.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5170 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_alert_status.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2713 2022-11-09 12:09:25.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_api_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3826 2022-11-09 12:09:25.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_byline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3092 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_client_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7868 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_topic_history.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1522 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7348 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6605 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_baseline_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4665 2023-06-26 13:23:15.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_devices.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3043 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_email.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3570 2023-03-20 10:12:25.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3183 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_user_identity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7027 2023-03-20 10:12:25.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_users.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5419 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_configuration_csv.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4707 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_configuration_monitor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4426 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3321 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_collation_summary.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2867 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_join.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2774 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2761 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_segmentor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3372 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_writer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3657 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_device_controller.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5046 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_device_monitor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3267 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_device_monitor_status.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4066 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_histo_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3039 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_localised_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2011 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_monitor_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5603 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_mqtt_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3378 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_multi_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3490 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_node.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5404 2023-03-20 10:12:25.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_devices.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4524 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_path_roots.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4630 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_user_paths.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6422 2023-03-20 10:12:25.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_users.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4992 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisations.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3560 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_aggregate.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3536 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2628 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_concentration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2813 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_distance.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2189 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_duplicates.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3020 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_error.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1677 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1688 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4763 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_iso_8601.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_low_pass.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2312 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_median.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2782 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_nullify.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1224 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_paths.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1579 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3899 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_slope.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1577 2022-09-20 10:07:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_sort.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3100 2022-09-20 10:07:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_stats.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5204 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_subset.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2264 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_tally.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_time_shift.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2325 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_timezone.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3701 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_single_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1441 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_socket_receiver.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1540 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_uds.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5425 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cognito_devices.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6472 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cognito_email.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5460 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cognito_user_credentials.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7844 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cognito_user_identity.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     8291 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cognito_users.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7435 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/configuration_csv.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3511 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/configuration_monitor.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3859 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/configuration_monitor_check.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6401 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/csv_collation_summary.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3967 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/csv_collator.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6835 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/csv_join.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5065 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/csv_reader.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4697 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/csv_segmentor.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3800 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/csv_writer.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6115 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/device_controller.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4288 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/device_monitor.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4456 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/device_monitor_status.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.425173 scs-analysis-2.7.7/src/scs_analysis/handler/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4051 2023-03-20 10:12:25.000000 scs-analysis-2.7.7/src/scs_analysis/handler/aws_mqtt_publisher.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2329 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/batch_download_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1436 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/configuration_csv_generator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/csv_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5893 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/csv_segmentor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1184 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/mqtt_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2007 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/sample_midpoint.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/sample_regression.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4308 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/histo_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2127 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/localised_datetime.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2544 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/monitor_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4367 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/multi_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5982 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/node.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5896 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/organisation_devices.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4713 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/organisation_path_roots.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4925 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/organisation_user_paths.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5783 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/organisation_users.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5300 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/organisations.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7233 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/sample_aggregate.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4821 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_average.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5162 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_collator.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5566 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_concentration.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3970 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/sample_distance.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3765 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/sample_duplicates.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4685 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_error.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3102 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_interval.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7990 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_iso_8601.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3802 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_low_pass.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3571 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_max.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3776 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_median.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3529 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_midpoint.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3570 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_min.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5072 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/sample_noise.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4017 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_nullify.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1667 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/sample_paths.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3320 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_regression.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5707 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/sample_slope.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2502 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_sort.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5928 2022-09-20 10:07:36.000000 scs-analysis-2.7.7/src/scs_analysis/sample_stats.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6001 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_subset.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2897 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_time_shift.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4732 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/sample_timezone.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4463 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/single_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2451 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/socket_receiver.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1891 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/timer.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1849 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/uds_receiver.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.417173 scs-analysis-2.7.7/src/scs_analysis.egg-info/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-30 08:21:15.000000 scs-analysis-2.7.7/src/scs_analysis.egg-info/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)     6034 2023-06-30 08:21:15.000000 scs-analysis-2.7.7/src/scs_analysis.egg-info/SOURCES.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-30 08:21:15.000000 scs-analysis-2.7.7/src/scs_analysis.egg-info/dependency_links.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)      247 2023-06-30 08:21:15.000000 scs-analysis-2.7.7/src/scs_analysis.egg-info/requires.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       13 2023-06-30 08:21:15.000000 scs-analysis-2.7.7/src/scs_analysis.egg-info/top_level.txt
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:48.612063 scs-analysis-2.8.5/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/LICENSE
+-rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/MANIFEST.in
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-07-25 12:39:48.612063 scs-analysis-2.8.5/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)      766 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/README.md
+-rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/README.rst
+-rw-rw-r--   0 jade      (1002) jade      (1002)      232 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/requirements.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-07-25 12:39:48.616063 scs-analysis-2.8.5/setup.cfg
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5164 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/setup.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:48.600063 scs-analysis-2.8.5/src/
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:48.608063 scs-analysis-2.8.5/src/scs_analysis/
+-rwxrwxr-x   0 jade      (1002) jade      (1002)      241 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/__init__.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)    11141 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/alert.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4013 2023-06-30 08:17:13.000000 scs-analysis-2.8.5/src/scs_analysis/alert_status.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5387 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/aws_byline.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2655 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/aws_client_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7224 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/aws_mqtt_client.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7481 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/aws_topic_history.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2139 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/aws_topic_publisher.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2918 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/aws_upload_interval.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)    14679 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/baseline.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6682 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/baseline_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:48.608063 scs-analysis-2.8.5/src/scs_analysis/chart/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/chart/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1630 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/chart/chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4546 2023-04-17 09:22:53.000000 scs-analysis-2.8.5/src/scs_analysis/chart/histo_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4249 2023-04-17 09:22:53.000000 scs-analysis-2.8.5/src/scs_analysis/chart/multi_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4317 2023-04-17 09:22:53.000000 scs-analysis-2.8.5/src/scs_analysis/chart/single_chart.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:48.612063 scs-analysis-2.8.5/src/scs_analysis/cmd/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11254 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_alert.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5146 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_alert_status.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4651 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_aws_byline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3135 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_aws_client_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8364 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_aws_topic_history.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1539 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7342 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6435 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_baseline_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4689 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_cognito_devices.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3076 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_cognito_email.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3602 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3206 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_cognito_user_identity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7049 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_cognito_users.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5451 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_configuration_csv.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4729 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_configuration_monitor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4439 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3327 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_csv_collation_summary.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2856 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_csv_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3444 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_csv_join.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2813 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_csv_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2758 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_csv_segmentor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3399 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_csv_writer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3671 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_device_controller.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5972 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_device_monitor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3290 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_device_monitor_status.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4078 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_histo_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3073 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_localised_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2038 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_monitor_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5637 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_mqtt_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3408 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_multi_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3499 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_node.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5372 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_organisation_devices.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4547 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_organisation_path_roots.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4653 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_organisation_user_paths.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6445 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_organisation_users.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5015 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_organisations.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3579 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_aggregate.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3534 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2847 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_distance.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2237 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_duplicates.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3035 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_error.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1698 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2688 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_gas_concentration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1952 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_gas_density.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1709 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4825 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_iso_8601.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2569 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_low_pass.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2346 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_median.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2794 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_nullify.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1256 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_paths.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1609 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3899 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_slope.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1609 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_sort.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3114 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_stats.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5210 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_subset.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2294 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_tally.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2597 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_time_shift.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2385 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_timezone.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3731 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_single_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1481 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_socket_receiver.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1570 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_uds.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5476 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cognito_devices.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6472 2023-06-30 08:17:13.000000 scs-analysis-2.8.5/src/scs_analysis/cognito_email.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5460 2023-06-30 08:17:13.000000 scs-analysis-2.8.5/src/scs_analysis/cognito_user_credentials.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7993 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cognito_user_identity.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     8291 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/cognito_users.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7435 2023-06-30 08:17:13.000000 scs-analysis-2.8.5/src/scs_analysis/configuration_csv.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3511 2023-06-30 08:17:13.000000 scs-analysis-2.8.5/src/scs_analysis/configuration_monitor.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3859 2023-06-30 08:17:13.000000 scs-analysis-2.8.5/src/scs_analysis/configuration_monitor_check.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6401 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/csv_collation_summary.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3967 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/csv_collator.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6835 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/csv_join.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5065 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/csv_reader.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4697 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/csv_segmentor.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3800 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/csv_writer.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6344 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/device_controller.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4537 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/device_monitor.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4456 2023-06-30 08:17:13.000000 scs-analysis-2.8.5/src/scs_analysis/device_monitor_status.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:48.612063 scs-analysis-2.8.5/src/scs_analysis/handler/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/handler/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4051 2023-03-20 10:12:25.000000 scs-analysis-2.8.5/src/scs_analysis/handler/aws_mqtt_publisher.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2329 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/handler/batch_download_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1436 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/handler/configuration_csv_generator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/handler/csv_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5893 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/handler/csv_segmentor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1184 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/handler/mqtt_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2007 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/handler/sample_midpoint.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/handler/sample_regression.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4308 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/histo_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2127 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/localised_datetime.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2544 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/monitor_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4367 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/multi_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5982 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/node.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5976 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/organisation_devices.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4713 2023-06-26 09:33:48.000000 scs-analysis-2.8.5/src/scs_analysis/organisation_path_roots.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4925 2023-06-26 09:33:48.000000 scs-analysis-2.8.5/src/scs_analysis/organisation_user_paths.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5783 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/organisation_users.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5300 2023-06-26 09:33:48.000000 scs-analysis-2.8.5/src/scs_analysis/organisations.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7233 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/sample_aggregate.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4821 2023-06-26 09:33:48.000000 scs-analysis-2.8.5/src/scs_analysis/sample_average.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5162 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/sample_collator.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3970 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/sample_distance.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3765 2023-04-17 09:22:53.000000 scs-analysis-2.8.5/src/scs_analysis/sample_duplicates.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4685 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/sample_error.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5606 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/sample_gas_concentration.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3561 2023-07-25 12:37:52.000000 scs-analysis-2.8.5/src/scs_analysis/sample_gas_density.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3102 2023-06-26 09:33:48.000000 scs-analysis-2.8.5/src/scs_analysis/sample_interval.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7990 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/sample_iso_8601.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3802 2023-06-26 09:33:48.000000 scs-analysis-2.8.5/src/scs_analysis/sample_low_pass.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3571 2023-06-26 09:33:48.000000 scs-analysis-2.8.5/src/scs_analysis/sample_max.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3776 2023-06-26 09:33:48.000000 scs-analysis-2.8.5/src/scs_analysis/sample_median.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3529 2023-06-26 09:33:48.000000 scs-analysis-2.8.5/src/scs_analysis/sample_midpoint.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3570 2023-06-26 09:33:48.000000 scs-analysis-2.8.5/src/scs_analysis/sample_min.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5072 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/sample_noise.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4017 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/sample_nullify.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1667 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/sample_paths.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3320 2023-06-26 09:33:48.000000 scs-analysis-2.8.5/src/scs_analysis/sample_regression.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5707 2023-04-17 09:22:53.000000 scs-analysis-2.8.5/src/scs_analysis/sample_slope.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2502 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/sample_sort.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5928 2022-09-20 10:07:36.000000 scs-analysis-2.8.5/src/scs_analysis/sample_stats.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6001 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/sample_subset.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2897 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/sample_time_shift.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4732 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/sample_timezone.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4463 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/single_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2451 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/socket_receiver.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1891 2023-02-06 14:01:57.000000 scs-analysis-2.8.5/src/scs_analysis/timer.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1849 2022-08-17 09:53:36.000000 scs-analysis-2.8.5/src/scs_analysis/uds_receiver.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:48.608063 scs-analysis-2.8.5/src/scs_analysis.egg-info/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-07-25 12:39:48.000000 scs-analysis-2.8.5/src/scs_analysis.egg-info/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5984 2023-07-25 12:39:48.000000 scs-analysis-2.8.5/src/scs_analysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-07-25 12:39:48.000000 scs-analysis-2.8.5/src/scs_analysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)      247 2023-07-25 12:39:48.000000 scs-analysis-2.8.5/src/scs_analysis.egg-info/requires.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       13 2023-07-25 12:39:48.000000 scs-analysis-2.8.5/src/scs_analysis.egg-info/top_level.txt
```

### Comparing `scs-analysis-2.7.7/LICENSE` & `scs-analysis-2.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/PKG-INFO` & `scs-analysis-2.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 2.7.7
+Version: 2.8.5
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `scs-analysis-2.7.7/README.md` & `scs-analysis-2.8.5/README.md`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/setup.py` & `scs-analysis-2.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,18 +53,16 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows :: Windows 10",
         "Operating System :: POSIX",
     ],
     scripts=[
-        'src/scs_analysis/access_key.py',
         'src/scs_analysis/alert.py',
         'src/scs_analysis/alert_status.py',
-        'src/scs_analysis/aws_api_auth.py',
         'src/scs_analysis/aws_byline.py',
         'src/scs_analysis/aws_client_auth.py',
         'src/scs_analysis/aws_mqtt_client.py',
         'src/scs_analysis/aws_topic_history.py',
         'src/scs_analysis/aws_topic_publisher.py',
         'src/scs_analysis/aws_upload_interval.py',
         'src/scs_analysis/baseline.py',
@@ -95,18 +93,19 @@
         'src/scs_analysis/organisation_path_roots.py',
         'src/scs_analysis/organisation_user_paths.py',
         'src/scs_analysis/organisation_users.py',
         'src/scs_analysis/organisations.py',
         'src/scs_analysis/sample_aggregate.py',
         'src/scs_analysis/sample_average.py',
         'src/scs_analysis/sample_collator.py',
-        'src/scs_analysis/sample_concentration.py',
         'src/scs_analysis/sample_distance.py',
         'src/scs_analysis/sample_duplicates.py',
         'src/scs_analysis/sample_error.py',
+        'src/scs_analysis/sample_gas_concentration.py',
+        'src/scs_analysis/sample_gas_density.py',
         'src/scs_analysis/sample_interval.py',
         'src/scs_analysis/sample_iso_8601.py',
         'src/scs_analysis/sample_low_pass.py',
         'src/scs_analysis/sample_max.py',
         'src/scs_analysis/sample_median.py',
         'src/scs_analysis/sample_midpoint.py',
         'src/scs_analysis/sample_min.py',
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/alert.py` & `scs-analysis-2.8.5/src/scs_analysis/alert.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,65 +13,55 @@
 together with the aggregation period (usually in minutes). The minimum period is one minute.
 
 Important note: when an alert is triggered, only one email is sent to each of the specified recipients. No further
 email is sent until the parameter has returned within bounds and then, subsequently, exceeds the bounds. The end of an
 out-of-bound event is logged in the alert status history. A history of out-of-bounds events for each alert
 specification can be found using the alert_status utility.
 
-In --find mode, results can be filtered by description, topic, field or creator email address.
+In --find mode, results can be filtered by description, topic, field or email address.
 Finder matches are exact.
 
 SYNOPSIS
-alert.py [-c CREDENTIALS]  { -F | -R ID | -C | -U ID | -D ID } [-d DESCRIPTION] [-p TOPIC] [-f FIELD] [-l LOWER]
-[-u UPPER] [-n { 1 | 0 }] [-a INTERVAL UNITS] [-t INTERVAL] [-s { 1 | 0 }] [-i INDENT] [-v] [-e EMAIL_ADDR]
-[-g EMAIL_ADDR_1 .. EMAIL_ADDR_N]
+alert.py { -z | [-c CREDENTIALS]  { -F | -R ID | -C | -U ID | -D ID } [-d DESCRIPTION] [-p TOPIC] [-f FIELD]
+[-l LOWER] [-u UPPER] [-n { 0 | 1 }] [{ -r INTERVAL UNITS TIMEZONE | -t START END TIMEZONE }] [-j { 0 | 1 }]
+[-s { 0 | 1 }] [-i INDENT] [-v] [-e EMAIL_ADDR] [-g EMAIL_ADDR_1 .. EMAIL_ADDR_N]}
 
 EXAMPLES
-alert.py -vi4 -c bruno -C -d "warm" -p south-coast-science-dev/development/loc/1/climate -f val.tmp -u 30 -n 1 -a 1 M
+alert.py -vi4 -c super -C -d be2-3-nightime-test -p south-coast-science-dev/development/loc/1/climate -f val.tmp \
+-u 10 -n 1 -t 16:00 8:00 Europe/London -e bruno.beloff@southcoastscience.com -g jade.page@southcoastscience.com
 
-DOCUMENT EXAMPLE
-{
-    "id": 88,
-    "description": "warm",
-    "topic": "south-coast-science-dev/development/loc/1/climate",
-    "field": "val.tmp",
-    "lower-threshold": null,
-    "upper-threshold": 30.0,
-    "alert-on-none": false,
-    "aggregation-period": {
-        "interval": 1,
-        "units": "M"
-    },
-    "test-interval": null,
-    "json-message": false,
-    "creator-email-address": "bruno.beloff@southcoastscience.com",
-    "to": "bruno.beloff@southcoastscience.com",
-    "cc-list": [
-        "bbeloff@me.com",
-        "jadempage@outlook.com"
-    ],
-    "suspended": false
-}
+DOCUMENT EXAMPLE (recurring)
+{"id": null, "description": "my description", "topic": "my/topic",
+"field": "my.field", "lower-threshold": null,  "upper-threshold": 100.0, "alert-on-none": true,
+"aggregation-period": {"type": "recurring", "interval": 1, "units": "D", "timezone": "Europe/London"},
+"test-interval": {"type": "recurring", "interval": 1, "units": "M"}, "json-message": true,
+"creator-email-address": "bruno.beloff@southcoastscience.com", "to": "bruno.beloff@southcoastscience.com",
+"cc-list": ["bbeloff@me.com", "hhopton@me.com"], "suspended": false}
+
+DOCUMENT EXAMPLE (diurnal)
+{"id": 107, "description": "be2-3-nightime-test", "topic": "south-coast-science-dev/development/loc/1/climate",
+"field": "val.tmp", "lower-threshold": null, "upper-threshold": 10.0, "alert-on-none": true,
+"aggregation-period": {"type": "diurnal", "start": "16:00:00", "end": "08:00:00", "timezone": "Europe/London"},
+"test-interval": null, "json-message": false, "creator-email-address": "production@southcoastscience.com",
+"to": "bruno.beloff@southcoastscience.com", "cc-list": ["jade.page@southcoastscience.com"], "suspended": false}
 
 SEE ALSO
 scs_analysis/alert_status
 scs_analysis/cognito_user_credentials
 
 BUGS
-The --test-interval flag is not currently in use, and is ignored.
+The test-interval field is not currently in use, and is ignored.
 """
 
 import json
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_alert import CmdAlert
 
-from scs_core.aws.client.api_auth import APIAuth
-
 from scs_core.aws.data.alert import AlertSpecification
 
 from scs_core.aws.manager.alert_specification_manager import AlertSpecificationManager
 from scs_core.aws.manager.byline_manager import BylineManager
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
@@ -79,25 +69,28 @@
 from scs_core.client.http_exception import HTTPException, HTTPNotFoundException
 
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 from scs_core.data.path_dict import PathDict
 from scs_core.data.str import Str
 
+from scs_core.location.timezone import Timezone
+
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
-    response = None
+    credentials = None
+    auth = None
     report = None
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
         cmd = CmdAlert()
@@ -111,32 +104,26 @@
 
         logger.info(cmd)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # authentication...
 
-        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
-
-        if not credentials:
-            exit(1)
+        if not cmd.list:
+            credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
 
-        gatekeeper = CognitoLoginManager(requests)
-        auth = gatekeeper.user_login(credentials)
+            if not credentials:
+                exit(1)
 
-        if not auth.is_ok():
-            logger.error("login: %s" % auth.authentication_status.description)
-            exit(1)
+            gatekeeper = CognitoLoginManager(requests)
+            auth = gatekeeper.user_login(credentials)
 
-        # APIAuth (for BylineManager)...
-        api_auth = APIAuth.load(Host)
-
-        if api_auth is None:
-            logger.error("APIAuth is not available")
-            exit(1)
+            if not auth.is_ok():
+                logger.error("login: %s" % auth.authentication_status.description)
+                exit(1)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
         byline_manager = BylineManager(requests)
         specification_manager = AlertSpecificationManager(requests)
@@ -158,21 +145,40 @@
 
         if cmd.cc:
             for email in cmd.cc_list:
                 if email is not None and not Datum.is_email_address(email):
                     logger.error("the email address '%s' is not valid." % email)
                     exit(2)
 
+        if not cmd.is_valid_start_time():
+            logger.error("the start time is invalid.")
+            exit(2)
+
+        if not cmd.is_valid_end_time():
+            logger.error("the end time is invalid.")
+            exit(2)
+
+        if not cmd.is_valid_timezone():
+            logger.error("the timezone is invalid.")
+            exit(2)
+
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
+        if cmd.list:
+            for zone in Timezone.zones():
+                print(zone, file=sys.stderr)
+            exit(0)
+
         if cmd.find:
-            response = specification_manager.find(auth.id_token, cmd.description, cmd.topic, cmd.field, cmd.email)
-            report = sorted(response.alerts)
+            response = specification_manager.find(auth.id_token, cmd.description, cmd.topic, cmd.field, None)
+            filtered = [alert for alert in response.alerts if cmd.email in alert] if cmd.email else response.alerts
+
+            report = sorted(filtered)
 
         if cmd.retrieve:
             report = specification_manager.retrieve(auth.id_token, cmd.id)
 
         if cmd.create:
             # validate...
             if not cmd.is_complete():
@@ -194,15 +200,15 @@
 
             # create...
             to = credentials.email if cmd.email is None else cmd.email
             cc = cmd.cc_list if cmd.cc else {}
 
             alert = AlertSpecification(None, cmd.description, cmd.topic, cmd.field, cmd.lower_threshold,
                                        cmd.upper_threshold, cmd.alert_on_none, cmd.aggregation_period,
-                                       cmd.test_interval, bool(cmd.json_message), None, to, cc, bool(cmd.suspended))
+                                       None, bool(cmd.json_message), None, to, cc, bool(cmd.suspended))
 
             if not alert.has_valid_thresholds():
                 logger.error("threshold values are invalid.")
                 exit(2)
 
             if not alert.has_valid_aggregation_period():
                 logger.error("the aggregation period is invalid.")
@@ -224,22 +230,21 @@
 
             # update...
             description = alert.description if not cmd.description else cmd.description
             lower_threshold = alert.lower_threshold if cmd.lower_threshold is None else cmd.lower_threshold
             upper_threshold = alert.upper_threshold if cmd.upper_threshold is None else cmd.upper_threshold
             alert_on_none = alert.alert_on_none if cmd.alert_on_none is None else bool(cmd.alert_on_none)
             aggregation_period = alert.aggregation_period if cmd.aggregation_period is None else cmd.aggregation_period
-            test_interval = alert.test_interval if cmd.test_interval is None else cmd.test_interval
             json_message = alert.json_message if cmd.json_message is None else bool(cmd.json_message)
             suspended = alert.suspended if cmd.suspended is None else bool(cmd.suspended)
             to = alert.to if cmd.email is None else cmd.email
             cc = cmd.cc_list if cmd.cc else alert.cc_list
 
             updated = AlertSpecification(alert.id, description, alert.topic, alert.field, lower_threshold,
-                                         upper_threshold, alert_on_none, aggregation_period, test_interval,
+                                         upper_threshold, alert_on_none, aggregation_period, None,
                                          json_message, alert.creator_email_address, to, cc, suspended)
 
             if not updated.has_valid_thresholds():
                 logger.error("threshold values are invalid.")
                 exit(2)
 
             if not updated.has_valid_aggregation_period():
@@ -259,15 +264,15 @@
         # end...
 
         # report...
         if report is not None:
             print(JSONify.dumps(report, indent=cmd.indent))
 
         if cmd.find:
-            logger.info('retrieved: %s' % len(response))
+            logger.info('retrieved: %s' % len(report))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPException as ex:
         logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/alert_status.py` & `scs-analysis-2.8.5/src/scs_analysis/alert_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/aws_api_auth.py` & `scs-analysis-2.8.5/src/scs_analysis/aws_client_auth.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,81 +4,90 @@
 Created on 2 Apr 2018
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The aws_api_auth utility is used to store or read the endpoint host name and API key required by the South Coast
-Science / AWS historic data retrieval system.
+The aws_api_auth utility is used to store or read the endpoint host name, client ID and client certificate ID
+required by the South Coast Science / AWS messaging infrastructure.
+
+The certificate files - created using the AWS IoT tools - must be installed by hand.
 
 SYNOPSIS
-aws_api_auth.py [{ [-e ENDPOINT] [-a API_KEY] | -d }] [-v]
+aws_client_auth.py [{ [-e ENDPOINT] [-c CLIENT_ID] [-I CERT_ID] | -d }] [-v]
 
 EXAMPLES
-aws_api_auth.py -e aws.southcoastscience.com -a de92c5ff-b47a-4cc4-a04c-62d684d64a1f
+aws_client_auth.py -e asrft7e5j5ecz.iot.us-west-2.amazonaws.com -c bruno -i 9f08402232
 
 FILES
-~/SCS/aws/aws_api_auth.json
+~/SCS/aws/aws_client_auth.json
+
+~/SCS/aws/certs/XXX-certificate.pem.crt
+~/SCS/aws/certs/XXX-private.pem.key
+~/SCS/aws/certs/XXX-public.pem.key
+~/SCS/aws/certs/root-CA.crt
 
 DOCUMENT EXAMPLE
-{"endpoint": "aws.southcoastscience.com", "api-key": "de92c5ff-b47a-4cc4-a04c-62d684d64a1f"}
+{"endpoint": "asrft7e5j5ecz.iot.us-west-2.amazonaws.com", "client-id": "bruno", "cert-id": "9f08402232"}
 
 SEE ALSO
-scs_analysis/aws_topic_history
+scs_analysis/aws_mqtt_client
+scs_analysis/aws_mqtt_control
 """
 
 import sys
 
-from scs_core.aws.client.api_auth import APIAuth
+from scs_core.aws.client.client_auth import ClientAuth
 from scs_core.data.json import JSONify
 
 from scs_host.sys.host import Host
 
-from scs_analysis.cmd.cmd_aws_api_auth import CmdAWSAPIAuth
+from scs_analysis.cmd.cmd_aws_client_auth import CmdAWSClientAuth
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     # ----------------------------------------------------------------------------------------------------------------
     # cmd...
 
-    cmd = CmdAWSAPIAuth()
+    cmd = CmdAWSClientAuth()
 
     if not cmd.is_valid():
         cmd.print_help(sys.stderr)
         exit(2)
 
     if cmd.verbose:
-        print("aws_api_auth: %s" % cmd, file=sys.stderr)
+        print("aws_client_auth: %s" % cmd, file=sys.stderr)
         sys.stderr.flush()
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # resources...
 
-    # APIAuth...
-    auth = APIAuth.load(Host)
+    # ClientAuth...
+    auth = ClientAuth.load(Host)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # run...
 
     if cmd.set():
         if auth is None and not cmd.is_complete():
-            print("aws_api_auth: No configuration is stored - you must therefore set all fields.", file=sys.stderr)
+            print("aws_client_auth: No configuration is stored - you must therefore set all fields.", file=sys.stderr)
             cmd.print_help(sys.stderr)
             exit(2)
 
         endpoint = cmd.endpoint if cmd.endpoint else auth.endpoint
-        api_key = cmd.api_key if cmd.api_key else auth.api_key
+        client_id = cmd.client_id if cmd.client_id else auth.client_id
+        cert_id = cmd.cert_id if cmd.cert_id else auth.cert_id
 
-        auth = APIAuth(endpoint, api_key)
+        auth = ClientAuth(endpoint, client_id, cert_id)
         auth.save(Host)
 
     if cmd.delete:
         auth.delete(Host)
         auth = None
 
     if auth:
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/aws_byline.py` & `scs-analysis-2.8.5/src/scs_analysis/aws_byline.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,45 +12,51 @@
 or device. The user may specify a topic path (find all devices that have published to the given topic), or a device tag
 (find all topics which the given device has published to), but not both. A further option --all reports all bylines.
 
 Output is in the form of zero or more JSON documents, indicating the device, topic and localised date / time for each
 latest sense event.
 
 SYNOPSIS
-Usage: aws_byline.py { -d DEVICE | -t TOPIC [-l] | -a } [-x EXCLUDED] [-m] [-i INDENT] [-v]
+aws_byline.py [-c CREDENTIALS] { -d DEVICE | -t TOPIC [-l] | -a } [-x EXCLUDED] [-s] [-m] [-i INDENT] [-v]
 
 EXAMPLES
 aws_byline.py -t south-coast-science-demo -v -x /control
 
 DOCUMENT EXAMPLE - OUTPUT
 {"device": "scs-bgx-401", "topic": "south-coast-science-demo/brighton/loc/1/climate",
 "lastSeenTime": "2020-10-23T08:52:20Z", "last_write": "2020-10-23T08:52:20Z",
 "message": "{\"val\": {\"hmd\": 68.4, \"tmp\": 19.8, \"bar\": null}, \"rec\": \"2020-10-23T08:52:20Z\",
 \"tag\": \"scs-bgx-401\"}"}
 
 SEE ALSO
 scs_analysis/aws_topic_history
+scs_analysis/cognito_user_credentials
 """
 
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_aws_byline import CmdAWSByline
 from scs_analysis.handler.batch_download_reporter import BatchDownloadReporter
 
 from scs_core.aws.manager.byline_manager import BylineManager
 
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
+from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
+
 from scs_core.client.http_exception import HTTPException
 from scs_core.client.network import Network
 from scs_core.client.resource_unavailable_exception import ResourceUnavailableException
 
 from scs_core.data.json import JSONify
 
 from scs_core.sys.logging import Logging
 
+from scs_host.sys.host import Host
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     group = None
 
@@ -66,14 +72,30 @@
     Logging.config('aws_byline', verbose=cmd.verbose)
     logger = Logging.getLogger()
 
     logger.info(cmd)
 
     try:
         # ------------------------------------------------------------------------------------------------------------
+        # authentication...
+
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
+
+        if not credentials:
+            exit(1)
+
+        gatekeeper = CognitoLoginManager(requests)
+        auth = gatekeeper.user_login(credentials)
+
+        if not auth.is_ok():
+            logger.error("login: %s" % auth.authentication_status.description)
+            exit(1)
+
+
+        # ------------------------------------------------------------------------------------------------------------
         # resources...
 
         # reporter...
         reporter = BatchDownloadReporter()
 
         # BylineManager...
         manager = BylineManager(requests, reporter=reporter)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/aws_mqtt_client.py` & `scs-analysis-2.8.5/src/scs_analysis/aws_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/aws_topic_history.py` & `scs-analysis-2.8.5/src/scs_analysis/aws_topic_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,61 +26,59 @@
 no data is returned.
 
 Equivalent to cURL:
 curl "https://aws.southcoastscience.com/topicMessages?topic=south-coast-science-dev/production-test/loc/1/gases
 &startTime=2018-12-13T07:03:59.712Z&endTime=2018-12-13T15:10:59.712Z"
 
 SYNOPSIS
-aws_topic_history.py { -l | -a LATEST_AT | -t { [[DD-]HH:]MM[:SS] | :SS } | -s START [-e END] }
-{ -c HH:MM:SS [-m] [-x] | [-w] [-f] } [-r] [{ -v | -d }] TOPIC
+aws_topic_history.py [-c CREDENTIALS] { -l | -a LATEST_AT [-b BACK-OFF] | -t { [[DD-]HH:]MM[:SS] | :SS } |
+-s START [-e END] } { -p HH:MM:SS [-m] [-x] | [-w] [-f] } [-r] [{ -v | -d }] TOPIC
 
 EXAMPLES
 aws_topic_history.py south-coast-science-dev/production-test/loc/1/gases -t 1 -v -w
 
 DOCUMENT EXAMPLE - OUTPUT
 {"device": "scs-bbe-401", "topic": "south-coast-science-demo/brighton/loc/1/climate", "upload": "2019-01-11T12:15:36Z",
 "payload": {"val": {"hmd": 68.4, "tmp": 12.3}, "rec": "2019-01-11T12:15:36Z", "tag": "scs-bgx-401"}}
 
 {"val": {"hmd": 68.4, "tmp": 12.3}, "rec": "2019-01-11T12:15:36Z", "tag": "scs-bgx-401"}
 
-FILES
-~/SCS/aws/aws_api_auth.json
-
 SEE ALSO
-scs_analysis/aws_api_auth
-scs_analysis/localised_datetime
+scs_analysis/aws_byline
+scs_analysis/cognito_user_credentials
 
 RESOURCES
 https://github.com/curl/curl
 """
 
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_aws_topic_history import CmdAWSTopicHistory
 from scs_analysis.handler.batch_download_reporter import BatchDownloadReporter
 
-from scs_core.aws.client.api_auth import APIAuth
 from scs_core.aws.manager.byline_manager import BylineManager
 from scs_core.aws.manager.lambda_message_manager import MessageManager
 
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
+from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
+
 from scs_core.client.http_exception import HTTPException
 from scs_core.client.network import Network
 from scs_core.client.resource_unavailable_exception import ResourceUnavailableException
 
 from scs_core.data.checkpoint_generator import CheckpointGenerator
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.json import JSONify
 
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
-# TODO: remove APIAuth requirement
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     agent = None
     reporter = None
     start_time = None
@@ -117,36 +115,44 @@
         cmd.print_help(sys.stderr)
         exit(2)
 
     logger.info(cmd)
 
     try:
         # ------------------------------------------------------------------------------------------------------------
-        # resources...
+        # authentication...
+
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
+
+        if not credentials:
+            exit(1)
 
-        # APIAuth...
-        api_auth = APIAuth.load(Host)
+        gatekeeper = CognitoLoginManager(requests)
+        auth = gatekeeper.user_login(credentials)
 
-        if api_auth is None:
-            logger.error("APIAuth not available.")
+        if not auth.is_ok():
+            logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
-        logger.info(api_auth)
+
+        # ------------------------------------------------------------------------------------------------------------
+        # resources...
 
         # reporter...
         reporter = BatchDownloadReporter()
 
         # BylineManager...
         byline_manager = BylineManager(requests)
 
         # MessageManager...
-        message_manager = MessageManager(api_auth, reporter=reporter)
+        message_manager = MessageManager(reporter=reporter)
 
         logger.info(message_manager)
 
+
         # ------------------------------------------------------------------------------------------------------------
         # check...
 
         if not Network.is_available():
             logger.info("waiting for network")
             Network.wait()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/aws_topic_publisher.py` & `scs-analysis-2.8.5/src/scs_analysis/aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/aws_upload_interval.py` & `scs-analysis-2.8.5/src/scs_analysis/aws_upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/baseline.py` & `scs-analysis-2.8.5/src/scs_analysis/baseline.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,30 +21,26 @@
 is restarted. How the restart happens is specified by the --uptake flag.
 
 If the --rehearse flag is used, the baseline utility shows what changes would be made, but does not make the changes.
 
 Operating parameters are specified by the baseline_conf utility, and may be overridden by the baseline utility flags.
 Any number of named baseline_conf files may be stored.
 
-The baseline utility requires access_key, aws_api_auth and aws_client_auth to be set.
-
 SYNOPSIS
-baseline.py [-a] -c NAME -f { V | E } [{ -r | -u COMMAND }] [-s START] [-e END] [-p AGGREGATION] [-m GAS MINIMUM]
-[{ -o GAS | -x GAS }] [-v] DEVICE_TAG_1 .. DEVICE_TAG_N
+Usage: baseline.py [-c CREDENTIALS] -n CONF_NAME -f { V | E } [{ -r | -u COMMAND }] [-s START] [-e END]
+[-p AGGREGATION] [-m GAS MINIMUM] [{ -o GAS | -x GAS }] [-v] DEVICE_TAG_1 .. DEVICE_TAG_N
 
 EXAMPLES
-baseline.py -ac freshfield -t scs-be2-3 -f E -r
+baseline.py -c super -n freshfield -e 07:00 -fV scs-bgb-410
 
 FILES
-~/SCS/conf/NAME_baseline_conf.json
+~/SCS/conf/baseline_conf/NAME_baseline_conf.json
 
 SEE ALSO
-scs_analysis/access_key
-scs_analysis/aws_api_auth
-scs_analysis/aws_client_auth
+scs_analysis/cognito_user_credentials
 scs_analysis/baseline_conf
 
 scs_dev/gases_sampler
 
 scs_mfr/afe_baseline
 scs_mfr/gas_baseline
 scs_mfr/scd30_baseline
@@ -54,25 +50,25 @@
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_baseline import CmdBaseline
 
 from scs_analysis.handler.batch_download_reporter import BatchDownloadReporter
 
-from scs_core.aws.client.api_auth import APIAuth
 from scs_core.aws.client.device_control_client import DeviceControlClient
 from scs_core.aws.manager.byline_manager import BylineManager
 from scs_core.aws.manager.lambda_message_manager import MessageManager
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 
 from scs_core.client.http_exception import HTTPGatewayTimeoutException
 
 from scs_core.data.datetime import LocalizedDatetime
+from scs_core.data.diurnal_period import DiurnalPeriod
 from scs_core.data.json import JSONify
 from scs_core.data.timedelta import Timedelta
 
 from scs_core.estate.baseline_conf import BaselineConf
 from scs_core.estate.configuration import Configuration
 
 from scs_core.gas.afe_baseline import AFEBaseline
@@ -107,14 +103,17 @@
     if not cmd.is_valid():
         cmd.print_help(sys.stderr)
         exit(2)
 
     Logging.config('baseline', verbose=cmd.verbose)
     logger = Logging.getLogger()
 
+    logger.info(cmd)
+
+
     try:
         # ------------------------------------------------------------------------------------------------------------
         # authentication...
 
         credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
 
         if not credentials:
@@ -123,33 +122,38 @@
         gatekeeper = CognitoLoginManager(requests)
         auth = gatekeeper.user_login(credentials)
 
         if not auth.is_ok():
             logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
-        # APIAuth (for MessageManager)...
-        api_auth = APIAuth.load(Host)
 
-        if api_auth is None:
-            logger.error("APIAuth is not available")
-            exit(1)
+        # ------------------------------------------------------------------------------------------------------------
+        # validation...
+
+        if cmd.start is not None and not DiurnalPeriod.is_valid_time(cmd.start):
+            logger.error("the start time is invalid.")
+            exit(2)
+
+        if cmd.end is not None and not DiurnalPeriod.is_valid_time(cmd.end):
+            logger.error("the end time is invalid.")
+            exit(2)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
         # reporter...
         reporter = BatchDownloadReporter()
 
         # BylineManager...
         byline_manager = BylineManager(requests, reporter=reporter)
 
         # MessageManager...
-        message_manager = MessageManager(api_auth, reporter=reporter)
+        message_manager = MessageManager(reporter=reporter)
 
         # DeviceControlClient...
         client = DeviceControlClient(requests)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/baseline_conf.py` & `scs-analysis-2.8.5/src/scs_analysis/baseline_conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,42 +12,44 @@
 
 Note that if the start time is a later hour than the end time, then the start time is interpreted as that hour
 on the previous day.
 
 Any number of separate baseline_conf files may be stored. The --list flag lists those that are available.
 
 SYNOPSIS
-baseline_conf.py [-a] { -z | -l | -c NAME [-t TIMEZONE_NAME] [-s START] [-e END] [-p AGGREGATION]
+baseline_conf.py [-a] { -z | -l | -n FROM TO | -c NAME [-s START] [-e END] [-p AGGREGATION] [-t TIMEZONE]
 [-g GAS MINIMUM] [-r GAS] } [-i INDENT] [-v]
 
 EXAMPLES
-./baseline_conf.py -c freshfield -t Europe/London -s 23 -e 8 -a 5 -g NO2 10
+./baseline_conf.py -c freshfield -s 23:00 -e 08:00 -a 5 -t Europe/London -g NO2 10
 
 DOCUMENT EXAMPLE
-{"timezone": "Europe/London", "start-hour": 17, "end-hour": 8, "aggregation-period": {"interval": 5, "units": "M"},
-"gas-minimums": {"CO": 200, "CO2": 420, "H2S": 5, "NO": 10, "NO2": 10, "SO2": 5}}
+{"sample-period": {"type": "diurnal", "start": "23:00:00", "end": "08:00:00", "timezone": "Europe/London"},
+"aggregation-period": {"type": "recurring", "interval": 5, "units": "M", "timezone": "Europe/London"},
+"minimums": {"CO": 300, "CO2": 420, "H2S": 5, "NO": 10, "NO2": 10, "Ox": 50, "SO2": 5, "VOC": 250}}
 
 FILES
-~/SCS/conf/NAME_baseline_conf.json
+~/SCS/conf/baseline_conf/NAME_baseline_conf.json
 
 SEE ALSO
 scs_analysis/baseline
 scs_dev/gases_sampler
 """
 
 import sys
 
 from scs_analysis.cmd.cmd_baseline_conf import CmdBaselineConf
 
 from scs_core.aws.client.access_key import AccessKey
 from scs_core.aws.client.client import Client
 from scs_core.aws.manager.s3_manager import S3PersistenceManager
 
+from scs_core.data.diurnal_period import DiurnalPeriod
 from scs_core.data.json import JSONify
-from scs_core.data.recurring_period import RecurringMinutes
+from scs_core.data.recurring_period import RecurringMinutes, RecurringPeriod
 
 from scs_core.estate.baseline_conf import BaselineConf
 
 from scs_core.location.timezone import Timezone
 
 from scs_core.sys.logging import Logging
 
@@ -98,15 +100,15 @@
             persistence_manager = S3PersistenceManager(client, resource_client)
 
         else:
             persistence_manager = Host
 
         # GasModelConf...
         if not cmd.duplicate():
-            conf = BaselineConf.load(persistence_manager, name=cmd.conf_name)
+            conf = BaselineConf.load(persistence_manager, name=cmd.conf_name, skeleton=True)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         if cmd.zones:
             for zone in Timezone.zones():
@@ -133,44 +135,57 @@
                 logger.error("no configuration is stored - you must therefore set all fields.")
                 exit(2)
 
             if cmd.timezone and not Timezone.is_valid(cmd.timezone):
                 logger.error("unrecognised timezone name: %s." % cmd.timezone)
                 exit(2)
 
-            if cmd.aggregation_period and cmd.aggregation_period not in RecurringMinutes.valid_intervals():
+            if cmd.interval and cmd.interval not in RecurringMinutes.valid_intervals():
                 logger.error("aggregation period must be one of: %s." % str(RecurringMinutes.valid_intervals()))
                 exit(2)
 
-            timezone = conf.timezone if cmd.timezone is None else cmd.timezone
-            start_hour = conf.start_hour if cmd.start_hour is None else cmd.start_hour
-            end_hour = conf.end_hour if cmd.end_hour is None else cmd.end_hour
-            aggregation_period = conf.aggregation_period if cmd.aggregation_period is None else \
-                RecurringMinutes(cmd.aggregation_period)
+            if cmd.start is not None and not DiurnalPeriod.is_valid_time(cmd.start):
+                logger.error("the start time is invalid.")
+                exit(2)
+
+            if cmd.end is not None and not DiurnalPeriod.is_valid_time(cmd.end):
+                logger.error("the end time is invalid.")
+                exit(2)
+
+            start_time_str = str(conf.sample_period.start_time) if cmd.start is None else cmd.start
+            end_time_str = str(conf.sample_period.end_time) if cmd.end is None else cmd.end
+            timezone_str = str(conf.timezone) if cmd.timezone is None else cmd.timezone
 
-            if start_hour == end_hour:
+            sample_period = DiurnalPeriod.construct(start_time_str, end_time_str, timezone_str)
+
+            interval = conf.aggregation_period.interval if cmd.interval is None else cmd.interval
+
+            aggregation_period = RecurringPeriod.construct(interval, 'M', timezone_str)
+
+            if sample_period.start_time == sample_period.end_time:
                 logger.error("the start and end hours may not be the same.")
                 exit(2)
 
             minimums = {} if conf is None else conf.minimums
 
-            conf = BaselineConf(cmd.conf_name, timezone, start_hour, end_hour, aggregation_period, minimums)
+            conf = BaselineConf(cmd.conf_name, sample_period, aggregation_period, minimums)
 
             if cmd.set_gas_name:
                 if cmd.set_gas_name not in BaselineConf.supported_gases():
                     logger.error("the gas '%s' is not supported." % cmd.set_gas_name)
                     exit(2)
 
                 conf.set_minimum(cmd.set_gas_name, cmd.set_gas_minimum)
 
             if cmd.remove_gas:
                 conf.remove_minimum(cmd.remove_gas)
 
             conf.save(persistence_manager)
 
+
         # ------------------------------------------------------------------------------------------------------------
         # end...
 
         if conf:
             print(JSONify.dumps(conf, indent=cmd.indent))
 
     except KeyboardInterrupt:
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/chart/chart.py` & `scs-analysis-2.8.5/src/scs_analysis/chart/chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/chart/histo_chart.py` & `scs-analysis-2.8.5/src/scs_analysis/chart/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/chart/multi_chart.py` & `scs-analysis-2.8.5/src/scs_analysis/chart/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/chart/single_chart.py` & `scs-analysis-2.8.5/src/scs_analysis/chart/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_access_key.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_monitor_auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 """
-Created on 17 Oct 2020
+Created on 20 Apr 2021
 
-@author: Jade Page (jade.page@southcoastscience.com)
+@author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdAccessKey(object):
+class CmdMonitorAuth(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [{ -s | -d }] [-v]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [{ -s | -d }] [-v]", version=version())
 
-        # commands..
+        # operations..
         self.__parser.add_option("--set", "-s", action="store_true", dest="set", default=False,
-                                 help="set the key")
+                                 help="set the authentication interactively")
 
         self.__parser.add_option("--delete", "-d", action="store_true", dest="delete", default=False,
-                                 help="delete the key")
+                                 help="delete the authentication")
 
-        # reporting flag..
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
         if self.set and self.delete:
             return False
 
         return True
 
-
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def set(self):
         return self.__opts.set
 
 
@@ -61,9 +62,9 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdAccessKey:{set:%s, delete:%s, verbose:%s}" % \
+        return "CmdMonitorAuth:{set:%s, delete:%s, verbose:%s}" % \
                (self.set, self.delete, self.verbose)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_alert.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_alert.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,40 +2,50 @@
 Created on 29 Jun 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
+from scs_core.data.diurnal_period import DiurnalPeriod
 from scs_core.data.recurring_period import RecurringPeriod
 
+from scs_core.location.timezone import Timezone
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdAlert(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS]  { -F | -R ID | -C | -U ID | -D ID } "
+        self.__parser = optparse.OptionParser(usage="%prog { -z | [-c CREDENTIALS]  "
+                                                    "{ -F | -R ID | -C | -U ID | -D ID } "
                                                     "[-d DESCRIPTION] [-p TOPIC] [-f FIELD] [-l LOWER] [-u UPPER] "
-                                                    "[-n { 1 | 0 }] [-a INTERVAL UNITS] [-t INTERVAL] [-j { 1 | 0 }] "
-                                                    "[-s { 1 | 0 }] [-i INDENT] [-v] "
-                                                    "[-e EMAIL_ADDR] [-g EMAIL_ADDR_1 .. EMAIL_ADDR_N]",
-                                              version="%prog 1.0")
+                                                    "[-n { 0 | 1 }] "
+                                                    "[{ -r INTERVAL UNITS TIMEZONE | -t START END TIMEZONE }] "
+                                                    "[-j { 0 | 1 }] [-s { 0 | 1 }] [-i INDENT] [-v] "
+                                                    "[-e EMAIL_ADDR] [-g EMAIL_ADDR_1 .. EMAIL_ADDR_N]}",
+                                              version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
+        self.__parser.add_option("--zones", "-z", action="store_true", dest="list", default=False,
+                                 help="list the available timezone names to stderr")
+
         self.__parser.add_option("--find", "-F", action="store_true", dest="find", default=False,
-                                 help="find alerts for given TOPIC (and FIELD) or creator email")
+                                 help="find alerts for given description, topic, field or email")
 
         self.__parser.add_option("--retrieve", "-R", type="int", action="store", dest="retrieve_id",
                                  help="retrieve alert with given ID")
 
         self.__parser.add_option("--create", "-C", action="store_true", dest="create", default=False,
                                  help="create alert")
 
@@ -60,48 +70,51 @@
 
         self.__parser.add_option("--upper-threshold", "-u", type="float", action="store", dest="upper_threshold",
                                  help="upper threshold")
 
         self.__parser.add_option("--alert-on-none", "-n", type="int", action="store", dest="alert_on_none",
                                  default=False, help="alert on none (default false)")
 
-        self.__parser.add_option("--aggregation-period", "-a", type="string", nargs=2, action="store",
-                                 dest="aggregation_period", help="aggregation interval and units { D | H | M }")
+        self.__parser.add_option("--recurring-period", "-r", type="string", nargs=3, action="store",
+                                 dest="recurring_period", help="aggregation interval and units { D | H | M }")
 
-        self.__parser.add_option("--test-interval", "-t", type="string", action="store", dest="test_interval",
-                                 help="test interval (NOT IN USE)")
+        self.__parser.add_option("--timed-period", "-t", type="string", nargs=3, action="store",
+                                 dest="timed_period", help="aggregation start and end")
 
         self.__parser.add_option("--json-message", "-j", type="int", action="store", dest="json_message",
                                  default=None, help="message body is JSON (default false)")
 
         self.__parser.add_option("--suspended", "-s", type="int", action="store", dest="suspended",
                                  default=None, help="suspended (default false)")
 
         # email...
         self.__parser.add_option("--email", "-e", type="string", action="store", dest="email",
-                                 help="email To address or creator address")
+                                 help="email To address (any on find)")
 
         self.__parser.add_option("--cc-list", "-g", action="store_true", dest="cc", default=False,
                                  help="email CC list")
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
         count = 0
 
+        if self.list:
+            count += 1
+
         if self.find:
             count += 1
 
         if self.retrieve:
             count += 1
 
         if self.create:
@@ -112,20 +125,14 @@
 
         if self.delete:
             count += 1
 
         if count != 1:
             return False
 
-        if self.__opts.aggregation_period is not None:
-            try:
-                int(self.__opts.aggregation_period[0])
-            except ValueError:
-                return False
-
         if self.alert_on_none is not None and self.alert_on_none != 0 and self.alert_on_none != 1:
             return False
 
         if self.json_message is not None and self.json_message != 0 and self.json_message != 1:
             return False
 
         if self.suspended is not None and self.suspended != 0 and self.suspended != 1:
@@ -143,14 +150,38 @@
 
         if self.lower_threshold is None and self.upper_threshold is None and not self.alert_on_none:
             return False
 
         return True
 
 
+    def is_valid_start_time(self):
+        if self.__opts.timed_period is None:
+            return True
+
+        return DiurnalPeriod.is_valid_time(self.__opts.timed_period[0])
+
+
+    def is_valid_end_time(self):
+        if self.__opts.timed_period is None:
+            return True
+
+        return DiurnalPeriod.is_valid_time(self.__opts.timed_period[1])
+
+
+    def is_valid_timezone(self):
+        if self.__opts.recurring_period is not None:
+            return Timezone.is_valid(self.__opts.recurring_period[2])
+
+        if self.__opts.timed_period is not None:
+            return Timezone.is_valid(self.__opts.timed_period[2])
+
+        return True
+
+
     # ----------------------------------------------------------------------------------------------------------------
     # properties: identity...
 
     @property
     def credentials_name(self):
         return self.__opts.credentials_name
 
@@ -169,14 +200,19 @@
         return None
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # properties: operations...
 
     @property
+    def list(self):
+        return self.__opts.list
+
+
+    @property
     def find(self):
         return self.__opts.find
 
 
     @property
     def retrieve(self):
         return self.__opts.retrieve_id is not None
@@ -228,21 +264,27 @@
     @property
     def alert_on_none(self):
         return self.__opts.alert_on_none
 
 
     @property
     def aggregation_period(self):
-        period = self.__opts.aggregation_period
-        return None if period is None else RecurringPeriod.construct(period[0], period[1])
+        return self.timed_period if self.recurring_period is None else self.recurring_period
+
+
+    @property
+    def recurring_period(self):
+        period = self.__opts.recurring_period
+        return None if period is None else RecurringPeriod.construct(period[0], period[1], period[2])
 
 
     @property
-    def test_interval(self):
-        return self.__opts.test_interval
+    def timed_period(self):
+        period = self.__opts.timed_period
+        return None if period is None else DiurnalPeriod.construct(period[0], period[1], period[2])
 
 
     @property
     def json_message(self):
         return self.__opts.json_message
 
 
@@ -285,15 +327,15 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdAlert:{credentials_name:%s, find:%s, retrieve:%s, create:%s, update:%s, " \
-               "delete:%s, topic:%s, field:%s, lower_threshold:%s, upper_threshold:%s, " \
-               "alert_on_none:%s, aggregation_period:%s, test_interval:%s, json_message:%s, suspended:%s, " \
-               "email:%s, cc:%s, cc_list:%s, indent:%s, verbose:%s}" % \
-               (self.credentials_name, self.find, self.__opts.retrieve_id, self.create, self.__opts.update_id,
-                self.__opts.delete_id, self.topic, self.field, self.lower_threshold, self.upper_threshold,
-                self.alert_on_none, self.aggregation_period, self.test_interval, self.json_message, self.suspended,
-                self.email, self.cc, self.cc_list, self.indent, self.verbose)
+        return "CmdAlert:{list:%s, credentials_name:%s, find:%s, retrieve:%s, create:%s, " \
+               "update:%s, delete:%s, topic:%s, field:%s, lower_threshold:%s, " \
+               "upper_threshold:%s, alert_on_none:%s, recurring_period:%s, timed_period:%s, " \
+               " json_message:%s, suspended:%s, email:%s, cc:%s, cc_list:%s, indent:%s, verbose:%s}" % \
+               (self.list, self.credentials_name, self.find, self.__opts.retrieve_id, self.create,
+                self.__opts.update_id, self.__opts.delete_id, self.topic, self.field, self.lower_threshold,
+                self.upper_threshold, self.alert_on_none, self.__opts.recurring_period, self.__opts.timed_period,
+                self.json_message, self.suspended, self.email, self.cc, self.cc_list, self.indent, self.verbose)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_alert_status.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_alert_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Created on 29 Jun 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
 from scs_core.aws.manager.alert_status_manager import AlertStatusFindRequest
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdAlertStatus(object):
     """unix command line handler"""
@@ -21,16 +22,15 @@
     def __init__(self):
         """
         Constructor
         """
         causes = ' | '.join(self.__CAUSES)
 
         self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -F { -l | -d [-a CAUSE] } | -D } "
-                                                    "[-i INDENT] [-v] ID",
-                                              version="%prog 1.0")
+                                                    "[-i INDENT] [-v] ID", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--find", "-F", action="store_true", dest="find", default=False,
@@ -46,15 +46,15 @@
         self.__parser.add_option("--history", "-d", action="store_true", dest="history", default=False,
                                  help="find history of status reports")
 
         self.__parser.add_option("--cause", "-a", type="string", action="store", dest="cause",
                                  help="filter history by cause { %s }" % causes)
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_api_auth.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_aws_client_auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,36 +7,42 @@
 
 example document:
 {"org-id": "south-coast-science-test-user", "api-key": "9fdfb841-3433-45b8-b223-3f5a283ceb8e"}
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdAWSAPIAuth(object):
+class CmdAWSClientAuth(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [{ [-e ENDPOINT] [-a API_KEY] | -d }] [-v]",
-                                              version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [{ [-e ENDPOINT] [-c CLIENT_ID] [-I CERT_ID] | -d }] [-v]",
+                                              version=version())
+
+        # fields...
+        self.__parser.add_option("--endpoint", "-e", type="string", action="store", dest="endpoint",
+                                 help="set broker endpoint")
 
-        # set...
-        self.__parser.add_option("--endpoint", "-e", type="string", nargs=1, action="store", dest="endpoint",
-                                 help="set API endpoint")
+        self.__parser.add_option("--client", "-c", type="string", action="store", dest="client_id",
+                                 help="set client ID")
 
-        self.__parser.add_option("--api-key", "-a", type="string", nargs=1, action="store", dest="api_key",
-                                 help="set API key")
+        self.__parser.add_option("--cert", "-i", type="string", action="store", dest="cert_id",
+                                 help="set certificate ID")
 
+        # delete...
         self.__parser.add_option("--delete", "-d", action="store_true", dest="delete", default=False,
-                                 help="delete the API configuration")
+                                 help="delete the client authentication")
 
         # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
@@ -47,34 +53,42 @@
         if self.set() and self.delete:
             return False
 
         return True
 
 
     def is_complete(self):
-        if self.endpoint is None or self.api_key is None:
+        if self.endpoint is None or self.client_id is None or self.cert_id is None:
             return False
 
         return True
 
 
     def set(self):
-        return self.endpoint is not None or self.api_key is not None
+        if self.endpoint is None and self.client_id is None and self.cert_id is None:
+            return False
+
+        return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def endpoint(self):
         return self.__opts.endpoint
 
 
     @property
-    def api_key(self):
-        return self.__opts.api_key
+    def client_id(self):
+        return self.__opts.client_id
+
+
+    @property
+    def cert_id(self):
+        return self.__opts.cert_id
 
 
     @property
     def delete(self):
         return self.__opts.delete
 
 
@@ -86,9 +100,9 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdAWSAPIAuth:{endpoint:%s, api_key:%s, delete:%s, verbose:%s}" % \
-               (self.endpoint, self.api_key, self.delete, self.verbose)
+        return "CmdAWSClientAuth:{endpoint:%s, client_id:%s, cert_id:%s, delete:%s, verbose:%s}" % \
+               (self.endpoint, self.client_id, self.cert_id, self.delete, self.verbose)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_byline.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_device_controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,112 +1,101 @@
 """
-Created on 25 Dec 2018
+Created on 17 Apr 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdAWSByline(object):
-    """unix command line handler"""
+class CmdDeviceController(object):
+    """unix message line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog { -d DEVICE | -t TOPIC [-l] | -a } [-x EXCLUDED] [-m] "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
-
-        # search types...
-        self.__parser.add_option("--device", "-d", type="string", nargs=1, action="store", dest="device",
-                                 help="report bylines for DEVICE")
-
-        self.__parser.add_option("--topic", "-t", type="string", nargs=1, action="store", dest="topic",
-                                 help="report bylines for TOPIC")
-
-        self.__parser.add_option("--all", "-a", action="store_true", dest="all", default=False,
-                                 help="report all bylines")
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] -t DEVICE_TAG "
+                                                    "[-m CMD_TOKENS [{ [-w] [-i INDENT] | -s }]] [-v]",
+                                              version=version())
+
+        # identity...
+        self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
+                                 help="the stored credentials to be presented")
+
+        # target...
+        self.__parser.add_option("--device-tag", "-t", type="string", action="store", dest="device_tag",
+                                 help="the device tag")
+
+        # mode...
+        self.__parser.add_option("--message", "-m", type="string", action="store", dest="message",
+                                 help="send the given command line string")
 
         # output...
-        self.__parser.add_option("--excluded", "-x", type="string", nargs=1, action="store", dest="excluded",
-                                 help="exclude topics ending with EXCLUDED")
-
-        self.__parser.add_option("--latest", "-l", action="store_true", dest="latest", default=False,
-                                 help="only report the most recent byline")
+        self.__parser.add_option("--wrapper", "-w", action="store_true", dest="wrapper", default=False,
+                                 help="report message wrapper")
 
-        self.__parser.add_option("--include-messages", "-m", action="store_true", dest="include_messages",
-                                 default=False, help="report the message with each byline")
+        self.__parser.add_option("--std", "-s", action="store_true", dest="std", default=False,
+                                 help="write to stderr and stdout")
 
-        self.__parser.add_option("--indent", "-i", action="store", dest="indent", type=int,
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        count = 0
-
-        if bool(self.device):
-            count += 1
-
-        if bool(self.topic):
-            count += 1
-
-        if self.all:
-            count += 1
+        if self.message is not None and len(self.message) < 1:
+            return False
 
-        if count != 1:
+        if self.std and (self.indent is not None or self.wrapper):
             return False
 
-        if self.latest and not bool(self.topic):
+        if (self.wrapper or self.indent or self.std) and not self.message:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def device(self):
-        return self.__opts.device
-
-
-    @property
-    def topic(self):
-        return self.__opts.topic
+    def credentials_name(self):
+        return self.__opts.credentials_name
 
 
     @property
-    def latest(self):
-        return self.__opts.latest
+    def device_tag(self):
+        return self.__opts.device_tag
 
 
     @property
-    def all(self):
-        return self.__opts.all
+    def message(self):
+        return self.__opts.message
 
 
     @property
-    def excluded(self):
-        return self.__opts.excluded
+    def wrapper(self):
+        return self.__opts.wrapper
 
 
     @property
-    def include_messages(self):
-        return self.__opts.include_messages
+    def std(self):
+        return self.__opts.std
 
 
     @property
     def indent(self):
         return self.__opts.indent
 
 
@@ -118,11 +107,11 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdAWSByline:{device:%s, topic:%s, latest:%s, all:%s, excluded:%s, include_messages:%s, " \
+        return "CmdDeviceController:{credentials_name:%s, device_tag:%s, message:%s, wrapper:%s, std:%s, " \
                "indent:%s, verbose:%s}" % \
-               (self.device, self.topic, self.latest, self.all, self.excluded, self.include_messages,
+               (self.credentials_name, self.device_tag, self.message, self.wrapper, self.std,
                 self.indent, self.verbose)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_client_auth.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_tally.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,104 +1,78 @@
 """
-Created on 2 Apr 2018
+Created on 22 Aug 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
-
-example document:
-{"org-id": "south-coast-science-test-user", "api-key": "9fdfb841-3433-45b8-b223-3f5a283ceb8e"}
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdAWSClientAuth(object):
+class CmdSampleTally(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [{ [-e ENDPOINT] [-c CLIENT_ID] [-I CERT_ID] | -d }] [-v]",
-                                              version="%prog 1.0")
-
-        # optional...
-        self.__parser.add_option("--endpoint", "-e", type="string", nargs=1, action="store", dest="endpoint",
-                                 help="set broker endpoint")
+        self.__parser = optparse.OptionParser(usage="%prog [-t TALLY] [-p PRECISION] [-v] [PATH]", version=version())
 
-        self.__parser.add_option("--client", "-c", type="string", nargs=1, action="store", dest="client_id",
-                                 help="set client ID")
-
-        self.__parser.add_option("--cert", "-i", type="string", nargs=1, action="store", dest="cert_id",
-                                 help="set certificate ID")
-
-        self.__parser.add_option("--delete", "-d", action="store_true", dest="delete", default=False,
-                                 help="delete the client authentication")
+        # mode...
+        self.__parser.add_option("--tally", "-t", type="int", action="store", dest="tally",
+                                 help="generate a rolling aggregate for TALLY number of data points (default all)")
+
+        # output...
+        self.__parser.add_option("--prec", "-p", type="int", action="store", default=None, dest="precision",
+                                 help="precision (default 0 decimal places)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.set() and self.delete:
-            return False
-
-        return True
-
-
-    def is_complete(self):
-        if self.endpoint is None or self.client_id is None or self.cert_id is None:
-            return False
-
-        return True
-
-
-    def set(self):
-        if self.endpoint is None and self.client_id is None and self.cert_id is None:
+        if self.tally is not None and self.tally < 1:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def endpoint(self):
-        return self.__opts.endpoint
+    def tally(self):
+        return self.__opts.tally
 
 
     @property
-    def client_id(self):
-        return self.__opts.client_id
+    def precision(self):
+        return self.__opts.precision
 
 
     @property
-    def cert_id(self):
-        return self.__opts.cert_id
-
-
-    @property
-    def delete(self):
-        return self.__opts.delete
+    def verbose(self):
+        return self.__opts.verbose
 
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdAWSClientAuth:{endpoint:%s, client_id:%s, cert_id:%s, delete:%s, verbose:%s}" % \
-               (self.endpoint, self.client_id, self.cert_id, self.delete, self.verbose)
+        return "CmdSampleTally:{tally:%s, precision:%s, verbose:%s, path:%s}" % \
+                    (self.tally, self.precision, self.verbose, self.path)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_topic_history.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_aws_topic_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,54 +5,60 @@
 
 source repo: scs_analysis
 """
 
 import logging
 import optparse
 
+from scs_analysis import version
+
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.timedelta import Timedelta
 
 
 # TODO: add backoff limit flag
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdAWSTopicHistory(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog { -l | -a LATEST_AT [-b BACK-OFF] | "
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -l | -a LATEST_AT [-b BACK-OFF] | "
                                                     "-t { [[DD-]HH:]MM[:SS] | :SS } | -s START [-e END] } "
-                                                    "{ -c HH:MM:SS [-m] [-x] | [-w] [-f] } [-r] [{ -v | -d }] TOPIC",
-                                              version="%prog 1.0")
+                                                    "{ -p HH:MM:SS [-m] [-x] | [-w] [-f] } [-r] [{ -v | -d }] TOPIC",
+                                              version=version())
+
+        # identity...
+        self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
+                                 help="the stored credentials to be presented")
 
         # functions...
         self.__parser.add_option("--latest", "-l", action="store_true", dest="latest", default=False,
                                  help="the most recent document")
 
-        self.__parser.add_option("--latest-at", "-a", type="string", nargs=1, action="store", dest="latest_at",
+        self.__parser.add_option("--latest-at", "-a", type="string", action="store", dest="latest_at",
                                  help="the most recent document before ISO 8601 datetime")
 
-        self.__parser.add_option("--back-off", "-b", type="int", nargs=1, action="store", dest="back_off",
+        self.__parser.add_option("--back-off", "-b", type="int", action="store", dest="back_off",
                                  help="maximum look-back period (seconds)")
 
-        self.__parser.add_option("--timedelta", "-t", type="string", nargs=1, action="store", dest="timedelta",
+        self.__parser.add_option("--timedelta", "-t", type="string", action="store", dest="timedelta",
                                  help="starting days / hours / minutes / seconds ago, and ending now")
 
-        self.__parser.add_option("--start", "-s", type="string", nargs=1, action="store", dest="start",
+        self.__parser.add_option("--start", "-s", type="string", action="store", dest="start",
                                  help="ISO 8601 datetime START")
 
-        self.__parser.add_option("--end", "-e", type="string", nargs=1, action="store", dest="end",
+        self.__parser.add_option("--end", "-e", type="string", action="store", dest="end",
                                  help="ISO 8601 datetime END")
 
         # aggregation...
-        self.__parser.add_option("--checkpoint", "-c", type="string", nargs=1, action="store", dest="checkpoint",
+        self.__parser.add_option("--checkpoint", "-p", type="string", action="store", dest="checkpoint",
                                  help="a time specification as **:/05:00")
 
         self.__parser.add_option("--min-max", "-m", action="store_true", dest="min_max", default=False,
                                  help="include min and max in addition to midpoint")
 
         self.__parser.add_option("--exclude-remainder", "-x", action="store_true", dest="exclude_remainder",
                                  help="ignore documents after the last complete period")
@@ -161,14 +167,22 @@
         if self.verbose:
             return logging.INFO
 
         return logging.ERROR
 
 
     # ----------------------------------------------------------------------------------------------------------------
+    # properties: identity...
+
+    @property
+    def credentials_name(self):
+        return self.__opts.credentials_name
+
+
+    # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def latest(self):
         return self.__opts.latest
 
 
     @property
@@ -244,13 +258,13 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdAWSTopicHistory:{latest:%s, latest_at:%s, latest_at:%s, timedelta:%s, start:%s, end:%s, " \
-               "fetch_last:%s, checkpoint:%s, include_wrapper:%s, rec_only:%s, min_max:%s, " \
-               "exclude_remainder:%s, verbose:%s, debug:%s, topic:%s}" % \
-                    (self.latest, self.__opts.latest_at, self.back_off, self.__opts.timedelta, self.start, self.end,
-                     self.fetch_last, self.checkpoint, self.include_wrapper, self.rec_only, self.min_max,
-                     self.exclude_remainder, self.verbose, self.debug, self.topic)
+        return "CmdAWSTopicHistory:{credentials_name:%s, latest:%s, latest_at:%s, latest_at:%s, timedelta:%s, " \
+               "start:%s, end:%s, fetch_last:%s, checkpoint:%s, include_wrapper:%s, rec_only:%s, " \
+               "min_max:%s, exclude_remainder:%s, verbose:%s, debug:%s, topic:%s}" % \
+                    (self.credentials_name, self.latest, self.__opts.latest_at, self.back_off, self.__opts.timedelta,
+                     self.start, self.end, self.fetch_last, self.checkpoint, self.include_wrapper, self.rec_only,
+                     self.min_max, self.exclude_remainder, self.verbose, self.debug, self.topic)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_topic_publisher.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_aws_topic_publisher.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,31 +4,33 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdAWSTopicPublisher(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog -t TOPIC [-v]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog -t TOPIC [-v]", version=version())
 
-        # compulsory...
-        self.__parser.add_option("--topic", "-t", type="string", nargs=1, action="store", dest="topic",
+        # fields...
+        self.__parser.add_option("--topic", "-t", type="string", action="store", dest="topic",
                                  help="topic path")
 
-        # optional...
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_baseline.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_baseline.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 Created on 28 Jul 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
+from scs_core.data.diurnal_period import DiurnalPeriod
 from scs_core.data.recurring_period import RecurringMinutes
+
 from scs_core.estate.baseline_conf import BaselineConf
+
 from scs_core.gas.minimum import Minimum
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdBaseline(object):
     """unix command line handler"""
@@ -27,53 +32,53 @@
         """
         cmds = ' | '.join(self.__UPTAKE_CMDS)
 
         self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] -n CONF_NAME -f { V | E } "
                                                     "[{ -r | -u COMMAND }] "
                                                     "[-s START] [-e END] [-p AGGREGATION] [-m GAS MINIMUM] "
                                                     "[{ -o GAS | -x GAS }] [-v] DEVICE_TAG_1 .. DEVICE_TAG_N",
-                                              version="%prog 1.0")
+                                              version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # target...
-        self.__parser.add_option("--conf-name", "-n", type="string", nargs=1, action="store", dest="conf_name",
+        self.__parser.add_option("--conf-name", "-n", type="string", action="store", dest="conf_name",
                                  help="the name of the baseline configuration")
 
         # function...
-        self.__parser.add_option("--fields", "-f", type="string", nargs=1, action="store", dest="fields",
+        self.__parser.add_option("--fields", "-f", type="string", action="store", dest="fields",
                                  help="baseline Val or Exg fields")
 
         self.__parser.add_option("--rehearse", "-r", action="store_true", dest="rehearse", default=False,
                                  help="show what actions should be performed")
 
-        self.__parser.add_option("--uptake", "-u", type="string", nargs=1, action="store", dest="uptake",
+        self.__parser.add_option("--uptake", "-u", type="string", action="store", dest="uptake",
                                  default=self.__DEFAULT_UPTAKE_CMD,
-                                 help="{ %s }, default '%s'" % (cmds, self.__DEFAULT_UPTAKE_CMD))
+                                 help="{ %s } default '%s'" % (cmds, self.__DEFAULT_UPTAKE_CMD))
 
         # fields...
-        self.__parser.add_option("--start-hour", "-s", type="int", nargs=1, action="store", dest="start_hour",
-                                 help="override the configuration's start hour")
+        self.__parser.add_option("--start", "-s", type="string", action="store", dest="start",
+                                 help="override the configuration's start time")
 
-        self.__parser.add_option("--end-hour", "-e", type="int", nargs=1, action="store", dest="end_hour",
-                                 help="override the configuration's end hour")
+        self.__parser.add_option("--end", "-e", type="string", action="store", dest="end",
+                                 help="override the configuration's end time")
 
-        self.__parser.add_option("--aggregation-period", "-p", type="int", nargs=1, action="store",
-                                 dest="aggregation_period", help="override the configuration's aggregation period")
+        self.__parser.add_option("--aggregation-period", "-p", type="int", action="store",
+                                 dest="interval", help="override the configuration's aggregation period")
 
         self.__parser.add_option("--minimum", "-m", type="string", nargs=2, action="store", dest="minimum",
                                  help="override configuration's minimum for GAS")
 
         # exclusions...
-        self.__parser.add_option("--only-gas", "-o", type="string", nargs=1, action="store", dest="only_gas",
+        self.__parser.add_option("--only-gas", "-o", type="string", action="store", dest="only_gas",
                                  help="baseline only GAS")
 
-        self.__parser.add_option("--exclude-gas", "-x", type="string", nargs=1, action="store", dest="exclude_gas",
+        self.__parser.add_option("--exclude-gas", "-x", type="string", action="store", dest="exclude_gas",
                                  help="exclude GAS")
 
         # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
@@ -99,22 +104,24 @@
         if self.only_gas is not None and self.exclude_gas is not None:
             return False
 
         return True
 
 
     def override(self, conf: BaselineConf):
-        start_hour = conf.start_hour if self.start_hour is None else self.start_hour
-        end_hour = conf.end_hour if self.end_hour is None else self.end_hour
-        aggregation_period = conf.aggregation_period if self.aggregation_period is None else \
-            RecurringMinutes(self.aggregation_period)
+        start_str = str(conf.sample_period.start_time) if self.start is None else self.start
+        end_str = str(conf.sample_period.end_time) if self.end is None else self.end
+        sample_period = DiurnalPeriod.construct(start_str, end_str, str(conf.timezone))
+
+        aggregation_period = conf.aggregation_period if self.start is None else \
+            RecurringMinutes(self.start, conf.timezone)
 
         minimums = {self.only_gas: conf.minimum(self.only_gas)} if self.only_gas else conf.minimums
 
-        conf = BaselineConf(conf.name, conf.timezone, start_hour, end_hour, aggregation_period, minimums)
+        conf = BaselineConf(conf.name, sample_period, aggregation_period, minimums)
 
         if self.minimum_gas is not None:
             conf.set_minimum(self.minimum_gas, self.minimum_value)
 
         if self.exclude_gas is not None:
             conf.remove_minimum(self.exclude_gas)
 
@@ -149,26 +156,26 @@
 
     @property
     def uptake(self):
         return self.__opts.uptake
 
 
     @property
-    def start_hour(self):
-        return self.__opts.start_hour
+    def start(self):
+        return self.__opts.start
 
 
     @property
-    def end_hour(self):
-        return self.__opts.end_hour
+    def end(self):
+        return self.__opts.end
 
 
     @property
-    def aggregation_period(self):
-        return self.__opts.aggregation_period
+    def interval(self):
+        return self.__opts.interval
 
 
     @property
     def minimum_gas(self):
         return None if self.__opts.minimum is None else self.__opts.minimum[0]
 
 
@@ -200,13 +207,13 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdBaseline:{credentials_name:%s, conf_name:%s, fields:%s, rehearse:%s, uptake:%s, start_hour:%s, " \
-               "end_hour:%s, aggregation_period:%s, minimum:%s, only_gas:%s, exclude_gas:%s, " \
+        return "CmdBaseline:{credentials_name:%s, conf_name:%s, fields:%s, rehearse:%s, uptake:%s, start:%s, " \
+               "end:%s, aggregation_period:%s, minimum:%s, only_gas:%s, exclude_gas:%s, " \
                "verbose:%s, device_tags:%s}" % \
-               (self.credentials_name, self.conf_name, self.fields, self.rehearse, self.uptake, self.start_hour,
-                self.end_hour, self.aggregation_period, self.__opts.minimum, self.only_gas, self.exclude_gas,
+               (self.credentials_name, self.conf_name, self.fields, self.rehearse, self.uptake, self.start,
+                self.end, self.interval, self.__opts.minimum, self.only_gas, self.exclude_gas,
                 self.verbose, self.device_tags)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_baseline_conf.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_baseline_conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,68 +2,71 @@
 Created on 31 Jul 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdBaselineConf(object):
     """
     unix command line handler
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self):
-        self.__parser = optparse.OptionParser(usage="%prog [-a] { -z | -l | -n FROM TO | -c NAME [-t TIMEZONE_NAME] "
-                                                    "[-s START] [-e END] [-p AGGREGATION] [-g GAS MINIMUM] [-r GAS] } "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-a] { -z | -l | -d FROM TO | -n NAME "
+                                                    "[-s START] [-e END] [-p AGGREGATION] [-t TIMEZONE] "
+                                                    "[-g GAS MINIMUM] [-r GAS] } "
+                                                    "[-i INDENT] [-v]", version=version())
 
         # source...
         self.__parser.add_option("--aws", "-a", action="store_true", dest="aws", default=False,
                                  help="Use AWS S3 instead of local storage for configuration")
 
         # helpers...
         self.__parser.add_option("--zones", "-z", action="store_true", dest="zones", default=False,
                                  help="list the available timezone names to stderr")
 
         self.__parser.add_option("--list", "-l", action="store_true", dest="list", default=False,
                                  help="list the available baseline configurations")
 
         # identity...
-        self.__parser.add_option("--duplicate", "-n", type="string", nargs=2, action="store", dest="duplicate",
+        self.__parser.add_option("--duplicate", "-d", type="string", nargs=2, action="store", dest="duplicate",
                                  help="create a new configuration based on FROM")
 
-        self.__parser.add_option("--conf-name", "-c", type="string", nargs=1, action="store", dest="conf_name",
+        self.__parser.add_option("--conf-name", "-n", type="string", action="store", dest="conf_name",
                                  help="the name of the baseline configuration")
 
         # fields...
-        self.__parser.add_option("--timezone", "-t", type="string", nargs=1, action="store", dest="timezone",
-                                 help="set the timezone for the tests")
+        self.__parser.add_option("--start", "-s", type="string", action="store", dest="start",
+                                 help="start of test period")
 
-        self.__parser.add_option("--start-hour", "-s", type="int", nargs=1, action="store", dest="start_hour",
-                                 help="test starts at the beginning of start hour")
+        self.__parser.add_option("--end", "-e", type="string", action="store", dest="end",
+                                 help="end of test period")
 
-        self.__parser.add_option("--end-hour", "-e", type="int", nargs=1, action="store", dest="end_hour",
-                                 help="test ends at the beginning of end hour")
+        self.__parser.add_option("--aggregation-period", "-p", type="int", action="store",
+                                 dest="interval", help="aggregation in minutes")
 
-        self.__parser.add_option("--aggregation-period", "-p", type="int", nargs=1, action="store",
-                                 dest="aggregation_period", help="aggregation in minutes")
+        self.__parser.add_option("--timezone", "-t", type="string", action="store", dest="timezone",
+                                 help="set the timezone for the tests")
 
         self.__parser.add_option("--set-gas", "-g", type="string", nargs=2, action="store", dest="set_gas",
                                  help="set minimum for GAS")
 
-        self.__parser.add_option("--remove-gas", "-r", type="string", nargs=1, action="store", dest="remove_gas",
+        self.__parser.add_option("--remove-gas", "-r", type="string", action="store", dest="remove_gas",
                                  help="remove GAS from minimums")
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
@@ -93,28 +96,28 @@
         except ValueError:
             return False
 
         return True
 
 
     def is_complete(self):
-        if self.timezone is None or self.start_hour is None or self.end_hour is None or \
-                self.aggregation_period is None:
+        if self.start is None or self.end is None or self.timezone is None or \
+                self.interval is None:
             return False
 
         return True
 
 
     def duplicate(self):
         return self.__opts.duplicate is not None
 
 
     def set(self):
-        return self.timezone is not None or self.start_hour is not None or self.end_hour is not None or \
-               self.aggregation_period is not None or self.__opts.set_gas is not None or self.remove_gas is not None
+        return self.start is not None or self.end is not None or self.interval is not None or \
+            self.timezone is not None or self.__opts.set_gas is not None or self.remove_gas is not None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def aws(self):
         return self.__opts.aws
@@ -142,31 +145,31 @@
 
     @property
     def conf_name(self):
         return self.__opts.conf_name
 
 
     @property
-    def timezone(self):
-        return self.__opts.timezone
+    def start(self):
+        return self.__opts.start
 
 
     @property
-    def start_hour(self):
-        return self.__opts.start_hour
+    def end(self):
+        return self.__opts.end
 
 
     @property
-    def end_hour(self):
-        return self.__opts.end_hour
+    def interval(self):
+        return self.__opts.interval
 
 
     @property
-    def aggregation_period(self):
-        return self.__opts.aggregation_period
+    def timezone(self):
+        return self.__opts.timezone
 
 
     @property
     def set_gas_name(self):
         return None if self.__opts.set_gas is None else self.__opts.set_gas[0]
 
 
@@ -193,11 +196,11 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdBaselineConf:{aws:%s, zones:%s, list:%s, list:%s, conf_name:%s, timezone:%s, start_hour:%s, " \
-               "end_hour:%s, aggregation_period:%s, set_gas:%s, remove_gas:%s, indent:%s, verbose:%s}" % \
-               (self.aws, self.zones, self.list, self.__opts.duplicate, self.conf_name, self.timezone, self.start_hour,
-                self.end_hour, self.aggregation_period, self.__opts.set_gas, self.remove_gas, self.indent, self.verbose)
+        return "CmdBaselineConf:{aws:%s, zones:%s, list:%s, list:%s, conf_name:%s, start:%s, end:%s, " \
+               "interval:%s, timezone:%s, set_gas:%s, remove_gas:%s, indent:%s, verbose:%s}" % \
+               (self.aws, self.zones, self.list, self.__opts.duplicate, self.conf_name, self.start, self.end,
+                self.interval, self.timezone, self.__opts.set_gas, self.remove_gas, self.indent, self.verbose)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_devices.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_cognito_devices.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Created on 24 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdCognitoDevices(object):
     """unix command line handler"""
 
     def __init__(self):
@@ -17,42 +19,42 @@
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] "
                                                     "{ -F [{ -t TAG | -n INVOICE }] [-m] "
                                                     "| -U TAG INVOICE "
                                                     "| -D TAG } "
                                                     "[-i INDENT] [-v]",
-                                              version="%prog 1.0")
+                                              version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
                                  help="list the devices visible to me")
 
         self.__parser.add_option("--Update", "-U", type="string", action="store", nargs=2, dest="update",
                                  help="update the device")
 
-        self.__parser.add_option("--Delete", "-D", type="string", action="store", nargs=1, dest="delete",
+        self.__parser.add_option("--Delete", "-D", type="string", action="store", dest="delete",
                                  help="delete the device (superuser only)")
 
         # filters...
         self.__parser.add_option("--tag", "-t", type="string", action="store", dest="tag",
                                  help="filter by device tag")
 
-        self.__parser.add_option("--invoice", "-n", type="string", action="store", dest="invoice_name",
+        self.__parser.add_option("--invoice", "-n", type="string", action="store", dest="invoice_number",
                                  help="filter by invoice")
 
         # output...
         self.__parser.add_option("--memberships", "-m", action="store_true", dest="memberships", default=False,
                                  help="show device's organisation memberships")
 
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
@@ -73,15 +75,15 @@
 
         if count != 1:
             return False
 
         if self.memberships and not self.find:
             return False
 
-        if self.tag and self.invoice_name:
+        if self.tag and self.invoice_number:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
@@ -117,16 +119,16 @@
 
     @property
     def tag(self):
         return self.__opts.tag
 
 
     @property
-    def invoice_name(self):
-        return self.__opts.invoice_name
+    def invoice_number(self):
+        return self.__opts.invoice_number
 
 
     @property
     def memberships(self):
         return self.__opts.memberships
 
 
@@ -146,8 +148,8 @@
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
         return "CmdCognitoDevices:{credentials_name:%s, find:%s, update:%s, delete:%s, " \
                "tag:%s, invoice:%s, memberships:%s, indent:%s, verbose:%s}" % \
                (self.credentials_name, self.find, self.update, self.delete,
-                self.tag, self.invoice_name, self.memberships, self.indent, self.verbose)
+                self.tag, self.invoice_number, self.memberships, self.indent, self.verbose)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_email.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_cognito_email.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 Created on 22 Nov 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdCognitoEmail(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog { -e | -c | -s | -r } EMAIL",
-                                              version="%prog 1.0")
+                                              version=version())
 
-        # functions...
+        # operations...
         self.__parser.add_option("--send-email", "-e", action="store_true", dest="send_email",
                                  help="send access email")
 
         self.__parser.add_option("--confirm", "-c", action="store_true", dest="confirm",
                                  help="confirm account (using confirmation code)")
 
         self.__parser.add_option("--set-password", "-s", action="store_true", dest="set_password",
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_user_credentials.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_cognito_user_credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 Created on 22 Nov 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdCognitoUserCredentials(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [{ -l | [-c CREDENTIALS] [{ -s | -p | -t | -d }] }] [-v]",
-                                              version="%prog 1.0")
+                                              version=version())
 
         # helpers...
         self.__parser.add_option("--list", "-l", action="store_true", dest="list", default=False,
                                  help="list the available credentials")
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_user_identity.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_cognito_user_identity.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 Created on 24 Nov 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdCognitoUserIdentity(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -C | -R | -U } [-i INDENT] [-v]",
-                                              version="%prog 1.0")
+                                              version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Create", "-C", action="store_true", dest="create", default=False,
@@ -30,15 +32,15 @@
         self.__parser.add_option("--Retrieve", "-R", action="store_true", dest="retrieve", default=False,
                                  help="retrieve my identity")
 
         self.__parser.add_option("--Update", "-U", action="store_true", dest="update", default=False,
                                  help="update my identity")
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_users.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_cognito_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Created on 24 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
 from scs_core.aws.security.cognito_user import CognitoUserIdentity
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdCognitoUsers(object):
     """unix command line handler"""
@@ -18,21 +19,21 @@
         """
         Constructor
         """
         confirmations = ' | '.join(CognitoUserIdentity.status_codes())
 
         self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] "
                                                     "{ -F [{ -e EMAIL_ADDR | -l ORG_LABEL | -o CONFIRMATION | "
-                                                    "-s { 1 | 0 } } }] [-m] "
+                                                    "-s { 0 | 1 } } }] [-m] "
                                                     "| -C -g GIVEN_NAME -f FAMILY_NAME -e EMAIL_ADDR "
                                                     "| -U EMAIL_ADDR [-g GIVEN_NAME] [-f FAMILY_NAME] [-e EMAIL_ADDR] "
-                                                    "[-s { 1 | 0 }] "
+                                                    "[-s { 0 | 1 }] "
                                                     "| -D EMAIL_ADDR } "
                                                     "[-i INDENT] [-v]",
-                                              version="%prog 1.0")
+                                              version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
@@ -61,21 +62,21 @@
                                  help="the organisation label")
 
         self.__parser.add_option("--confirmation-status", "-o", type="string", action="store",
                                  dest="confirmation_status",
                                  help="filter list by confirmation status { %s }" % confirmations)
 
         self.__parser.add_option("--enabled-status", "-s", type="int", action="store", dest="enabled",
-                                 help="filter list by enabled status { 1 | 0 }")
+                                 help="filter list by enabled status { 0 | 1 }")
 
         # output...
         self.__parser.add_option("--memberships", "-m", action="store_true", dest="memberships", default=False,
                                  help="show user's organisation memberships")
 
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_configuration_csv.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_configuration_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 Created on 7 Jul 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 from scs_core.aws.manager.configuration_finder import ConfigurationRequest
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdConfigurationCSV(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -n | -s | -l OUTPUT_CSV | "
                                                     "{ -d | -f } [-o OUTPUT_CSV_DIR] } [-t DEVICE_TAG [-x]] "
-                                                    "[-v] [NODE_1..NODE_N]", version="%prog 1.0")
+                                                    "[-v] [NODE_1..NODE_N]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # help...
         self.__parser.add_option("--node-names", "-n", action="store_true", dest="node_names", default=False,
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_configuration_monitor.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_configuration_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 Created on 20 Apr 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
 from scs_core.aws.manager.configuration_finder import ConfigurationRequest
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdConfigurationMonitor(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [-t TAG [-x]] { -l | -f | -d | -o } "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+                                                    "[-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # filters...
         self.__parser.add_option("--tag-filter", "-t", type="string", action="store", dest="tag_filter",
@@ -42,15 +43,15 @@
         self.__parser.add_option("--diff-history", "-d", action="store_true", dest="diff", default=False,
                                  help="report configuration differences")
 
         self.__parser.add_option("--tags-only", "-o", action="store_true", dest="tags_only", default=False,
                                  help="report device tags only")
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_configuration_monitor_check.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_configuration_monitor_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 Created on 20 Apr 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
-from scs_core.aws.manager.configuration_check_finder import ConfigurationCheckRequest
+from scs_analysis import version
 
+from scs_core.aws.manager.configuration_check_finder import ConfigurationCheckRequest
 from scs_core.estate.configuration_check import ConfigurationCheck
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdConfigurationMonitorCheck(object):
     """unix command line handler"""
@@ -19,15 +20,15 @@
     def __init__(self):
         """
         Constructor
         """
         codes = ' | '.join(ConfigurationCheck.result_codes())
 
         self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -f TAG | [-t TAG [-x]] [-o] } "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+                                                    "[-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--force", "-f", type="string", action="store", dest="force",
@@ -36,22 +37,22 @@
         # filters...
         self.__parser.add_option("--tag-filter", "-t", type="string", action="store", dest="tag_filter",
                                  help="the (partial) tag of the device(s)")
 
         self.__parser.add_option("--exactly", "-x", action="store_true", dest="exact_match", default=False,
                                  help="exact match for tag")
 
-        self.__parser.add_option("--result", "-r", type="string", nargs=1, action="store", dest="result_code",
+        self.__parser.add_option("--result", "-r", type="string", action="store", dest="result_code",
                                  help="match the result { %s }" % codes)
 
         # output...
         self.__parser.add_option("--tags-only", "-o", action="store_true", dest="tags_only", default=False,
                                  help="report device tags only")
 
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_collation_summary.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_csv_collation_summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 source repo: scs_analysis
 """
 
 import optparse
 
 from glob import glob
 
+from scs_analysis import version
 from scs_core.data.model_delta import ModelDelta
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdCollationSummary(object):
     """unix command line handler"""
@@ -22,24 +23,24 @@
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog  -f FILE_PREFIX -i IND_PATH "
                                                     "[-p IND_PRECISION DEP_PRECISION] [-v] DEP_PATH_1 .. DEP_PATH_N",
-                                              version="%prog 1.0")
+                                              version=version())
 
-        # compulsory...
-        self.__parser.add_option("--file-prefix", "-f", type="string", nargs=1, action="store", dest="file_prefix",
+        # input...
+        self.__parser.add_option("--file-prefix", "-f", type="string", action="store", dest="file_prefix",
                                  help="file prefix for collated CSVs")
 
-        self.__parser.add_option("--ind-path", "-i", type="string", nargs=1, action="store", dest="ind_path",
+        self.__parser.add_option("--ind-path", "-i", type="string", action="store", dest="ind_path",
                                  help="path to independent variable")
 
-        # optional...
+        # output...
         self.__parser.add_option("--prec", "-p", type="int", nargs=2, action="store", dest="precisions",
                                  help="precision for independent and dependent variables (default 1, 3 decimals)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_collator.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_csv_collator.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,39 +4,41 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdCSVCollator(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog -l LOWER_BOUND -u UPPER_BOUND -d DELTA [-f FILE_PREFIX] "
-                                                    "[-v] PATH", version="%prog 1.0")
+                                                    "[-v] PATH", version=version())
 
-        # compulsory...
-        self.__parser.add_option("--lower", "-l", type="float", nargs=1, action="store", dest="lower",
+        # input...
+        self.__parser.add_option("--lower", "-l", type="float", action="store", dest="lower",
                                  help="lower bound of dataset")
 
-        self.__parser.add_option("--upper", "-u", type="float", nargs=1, action="store", dest="upper",
+        self.__parser.add_option("--upper", "-u", type="float", action="store", dest="upper",
                                  help="upper bound of dataset")
 
-        self.__parser.add_option("--delta", "-d", type="float", nargs=1, action="store", dest="delta",
+        self.__parser.add_option("--delta", "-d", type="float", action="store", dest="delta",
                                  help="width of bin")
 
-        # optional...
-        self.__parser.add_option("--file-prefix", "-f", type="string", nargs=1, action="store", dest="file_prefix",
+        # output...
+        self.__parser.add_option("--file-prefix", "-f", type="string", action="store", dest="file_prefix",
                                  help="file prefix for collated CSVs")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_join.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_csv_join.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,41 +4,44 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdCSVJoin(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-t TYPE] [-i] [-v] -l PREFIX PK FILENAME "
-                                                    "-r PREFIX PK FILENAME", version="%prog 1.0")
+                                                    "-r PREFIX PK FILENAME", version=version())
 
-        # compulsory...
+        # input...
         self.__parser.add_option("--left", "-l", type="string", nargs=3, action="store", dest="left",
                                  help="output path prefix, primary key and filename for left-hand set")
 
         self.__parser.add_option("--right", "-r", type="string", nargs=3, action="store", dest="right",
                                  help="output path prefix, primary key and filename for right-hand set")
 
-        # optional...
-        self.__parser.add_option("--type", "-t", type="string", nargs=1, action="store", dest="type", default='INNER',
+        # mode...
+        self.__parser.add_option("--type", "-t", type="string", action="store", dest="type", default='INNER',
                                  help="{ 'INNER' | 'LEFT' | 'RIGHT' | 'FULL' } (default 'INNER')")
 
         self.__parser.add_option("--iso8601", "-i", action="store_true", dest="iso8601", default=False,
                                  help="interpret the primary key as an ISO 8601 datetime")
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_reader.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_csv_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,37 +4,40 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdCSVReader(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-s] [-n] [-l LIMIT] [-a] [-v] [FILENAME_1 .. FILENAME_N]",
-                                              version="%prog 1.0")
+                                              version=version())
 
-        # optional...
+        # mode...
         self.__parser.add_option("--string", "-s", action="store_true", dest="string", default=False,
                                  help="interpret all values as strings")
 
         self.__parser.add_option("--nullify", "-n", action="store_true", dest="nullify", default=False,
                                  help="convert empty or \"NULL\" strings to nulls")
 
-        self.__parser.add_option("--limit", "-l", type="int", nargs=1, action="store", dest="limit",
+        self.__parser.add_option("--limit", "-l", type="int", action="store", dest="limit",
                                  help="output a maximum of LIMIT rows")
 
+        # output...
         self.__parser.add_option("--array", "-a", action="store_true", dest="array", default=False,
                                  help="output JSON documents as array instead of a sequence")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_segmentor.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_csv_segmentor.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,38 +4,39 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
 from scs_core.data.timedelta import Timedelta
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdCSVSegmentor(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog -m { [DD-]HH:MM[:SS] | :SS } [-i ISO] [-f FILE_PREFIX] "
-                                                    "[-v]", version="%prog 1.0")
+                                                    "[-v]", version=version())
 
-        # compulsory...
-        self.__parser.add_option("--max-interval", "-m", type="string", nargs=1, action="store", dest="max_interval",
+        # input...
+        self.__parser.add_option("--max-interval", "-m", type="string", action="store", dest="max_interval",
                                  help="maximum permitted interval")
 
-        # optional...
-        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
+        self.__parser.add_option("--iso-path", "-i", type="string", action="store", default="rec", dest="iso",
                                  help="path for ISO 8601 datetime field (default 'rec')")
 
-        self.__parser.add_option("--file-prefix", "-f", type="string", nargs=1, action="store", dest="file_prefix",
+        # output...
+        self.__parser.add_option("--file-prefix", "-f", type="string", action="store", dest="file_prefix",
                                  help="file prefix for contiguous CSVs")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_writer.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_csv_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdCSVWriter(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [{ -a | -x | -s }] [-q] [-e] [-v] [FILENAME]",
-                                              version="%prog 1.0")
+                                              version=version())
 
-        # functions...
+        # mode...
         self.__parser.add_option("--append", "-a", action="store_true", dest="append", default=False,
                                  help="append rows to existing file")
 
         self.__parser.add_option("--exclude-header", "-x", action="store_true", dest="exclude_header", default=False,
                                  help="do not write the header row to stdout")
 
         self.__parser.add_option("--header-scan", "-s", action="store_true", dest="header_scan", default=False,
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_device_controller.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_multi_chart.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,115 +1,113 @@
 """
-Created on 17 Apr 2023
+Created on 13 Oct 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdDeviceController(object):
-    """unix message line handler"""
+class CmdMultiChart(object):
+    """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] -t DEVICE_TAG "
-                                                    "[-m CMD_TOKENS [{ [-w] [-i INDENT] | -s }]] [-v]",
-                                              version="%prog 1.0")
-
-        # identity...
-        self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
-                                 help="the stored credentials to be presented")
-
-        # target...
-        self.__parser.add_option("--device-tag", "-t", type="string", action="store", dest="device_tag",
-                                 help="the device tag")
+        self.__parser = optparse.OptionParser(usage="%prog [-b] [-x POINTS] [-y MIN MAX] [-e] [-t TITLE] [-v] "
+                                                    "PATH_1 .. PATH_N", version=version())
 
         # mode...
-        self.__parser.add_option("--message", "-m", type="string", nargs=1, action="store", dest="message",
-                                 help="send the given command line string")
+        self.__parser.add_option("--batch", "-b", action="store_true", dest="batch_mode", default=False,
+                                 help="wait for all data before displaying chart")
 
-        # output...
-        self.__parser.add_option("--wrapper", "-w", action="store_true", dest="wrapper", default=False,
-                                 help="report message wrapper")
+        self.__parser.add_option("--x", "-x", type="int", action="store", default=600, dest="x",
+                                 help="number of x points (default 600)")
+
+        self.__parser.add_option("--y", "-y", type="float", nargs=2, action="store", default=(-10.0, 10.0), dest="y",
+                                 help="set y-axis to min / max (default -10, 10)")
 
-        self.__parser.add_option("--std", "-s", action="store_true", dest="std", default=False,
-                                 help="write to stderr and stdout")
+        self.__parser.add_option("--skip-malformed", "-s", action="store_true", dest="skip_malformed", default=False,
+                                 help="ignore rows with missing path values")
 
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
-                                 help="pretty-print the output with INDENT")
+        # output...
+        self.__parser.add_option("--title", "-t", type="string", action="store", dest="title",
+                                 help="chart title")
+
+        self.__parser.add_option("--echo", "-e", action="store_true", dest="echo", default=False,
+                                 help="echo stdin to stdout")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.message is not None and len(self.message) < 1:
-            return False
-
-        if self.std and (self.indent is not None or self.wrapper):
-            return False
-
-        if (self.wrapper or self.indent or self.std) and not self.message:
+        if len(self.paths) == 0:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def credentials_name(self):
-        return self.__opts.credentials_name
+    def batch_mode(self):
+        return self.__opts.batch_mode
 
 
     @property
-    def device_tag(self):
-        return self.__opts.device_tag
+    def x(self):
+        return self.__opts.x
 
 
     @property
-    def message(self):
-        return self.__opts.message
+    def y(self):
+        return self.__opts.y
 
 
     @property
-    def wrapper(self):
-        return self.__opts.wrapper
+    def echo(self):
+        return self.__opts.echo
 
 
     @property
-    def std(self):
-        return self.__opts.std
+    def skip_malformed(self):
+        return self.__opts.skip_malformed
 
 
     @property
-    def indent(self):
-        return self.__opts.indent
+    def title(self):
+        return self.__opts.title
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
+    @property
+    def paths(self):
+        return self.__args
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdDeviceController:{credentials_name:%s, device_tag:%s, message:%s, wrapper:%s, std:%s, " \
-               "indent:%s, verbose:%s}" % \
-               (self.credentials_name, self.device_tag, self.message, self.wrapper, self.std,
-                self.indent, self.verbose)
+        return "CmdMultiChart:{batch_mode:%s, x:%d, y:%s, echo:%s, skip_malformed:%s, title:%s, " \
+               "verbose:%s, paths:%s}" % \
+                    (self.batch_mode, self.x, self.y, self.echo, self.skip_malformed, self.title,
+                     self.verbose, self.paths)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_device_monitor.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_device_monitor.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,57 +2,66 @@
 Created on 28 Jun 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdDeviceMonitor(object):
     """unix command line handler"""
 
     # --------------------------------------------------------------------------------------------------------------------
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] "
                                                     "{ -F [{ -e EMAIL_ADDR | -t DEVICE_TAG } [-x]] | "
-                                                    "-A EMAIL_ADDR DEVICE_TAG | -D EMAIL_ADDR [-t DEVICE_TAG] } "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+                                                    "-A EMAIL_ADDR DEVICE_TAG | -S DEVICE_TAG { 0 | 1 } | "
+                                                    "-D EMAIL_ADDR [{ -t DEVICE_TAG | -f }] } "
+                                                    "[-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--find", "-F", action="store_true", dest="find", default=False,
                                  help="find monitoring (for email address or device)")
 
         self.__parser.add_option("--add", "-A", type="string", nargs=2, action="store", dest="add",
                                  help="add email address to device")
 
+        self.__parser.add_option("--suspend", "-S", type="string", nargs=2, action="store", dest="suspend",
+                                 help="suspend monitoring of the device")
+
         self.__parser.add_option("--delete", "-D", type="string", action="store", dest="delete",
                                  help="delete email address (from device or throughout)")
 
+        # self.__parser.add_option("--force", "-f", type="string", action="store", dest="force",
+        #                          help="force deletion from multiple devices")
+
         # filters...
         self.__parser.add_option("--email", "-e", type="string", action="store", dest="email",
                                  help="email address")
 
         self.__parser.add_option("--device-tag", "-t", type="string", action="store", dest="device_tag",
                                  help="device tag")
 
         self.__parser.add_option("--exactly", "-x", action="store_true", dest="exact_match", default=False,
                                  help="exact match for tag")
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
@@ -64,20 +73,26 @@
 
         if self.find:
             count += 1
 
         if self.add:
             count += 1
 
+        if self.suspend:
+            count += 1
+
         if self.delete:
             count += 1
 
         if count != 1:
             return False
 
+        if self.suspend and self.__opts.suspend[1] not in [None, '0', '1']:
+            return False
+
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # properties: identity...
 
     @property
@@ -93,14 +108,25 @@
         return self.__opts.find
 
 
     @property
     def add(self):
         return bool(self.__opts.add)
 
+
+    @property
+    def suspend(self):
+        return bool(self.__opts.suspend)
+
+
+    @property
+    def is_suspended(self):
+        return bool(int(self.__opts.suspend[1])) if self.suspend else None
+
+
     @property
     def delete(self):
         return bool(self.__opts.delete)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # properties: filters...
@@ -117,14 +143,17 @@
 
 
     @property
     def device_tag(self):
         if self.add:
             return self.__opts.add[1]
 
+        if self.suspend:
+            return self.__opts.suspend[0]
+
         return self.__opts.device_tag
 
 
     @property
     def exact_match(self):
         return self.__opts.exact_match
 
@@ -145,11 +174,11 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdDeviceMonitor:{credentials_name:%s, find:%s, add:%s, delete:%s, " \
+        return "CmdDeviceMonitor:{credentials_name:%s, find:%s, add:%s, suspend:%s, delete:%s, " \
                "email:%s, device_tag:%s, exact_match:%s, indent:%s, verbose:%s}" % \
-               (self.credentials_name, self.__opts.find, self.__opts.add, self.__opts.delete,
+               (self.credentials_name, self.__opts.find, self.__opts.add, self.__opts.suspend, self.__opts.delete,
                 self.__opts.email, self.__opts.device_tag, self.exact_match, self.indent, self.verbose)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_device_monitor_status.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_device_monitor_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 Created on 28 Jun 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdDeviceMonitorStatus(object):
     """unix command line handler"""
 
     # --------------------------------------------------------------------------------------------------------------------
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [-t DEVICE_TAG [-x]] "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+                                                    "[-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # filters...
         self.__parser.add_option("--tag-filter", "-t", type="string", action="store", dest="tag_filter",
                                  help="the (partial) tag of the device(s)")
 
         self.__parser.add_option("--exactly", "-x", action="store_true", dest="exact_match", default=False,
                                  help="exact match for tag")
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_histo_chart.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_histo_chart.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,52 +4,55 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdHistoChart(object):
     """
     unix command line handler
     """
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-b] [-x MIN MAX] [-c BIN_COUNT] [-p PRECISION] "
-                                                    "[-o FILENAME] [-e] [-t TITLE] [-v] PATH", version="%prog 1.0")
+                                                    "[-o FILENAME] [-e] [-t TITLE] [-v] PATH", version=version())
 
-        # optional...
+        # mode...
         self.__parser.add_option("--batch", "-b", action="store_true", dest="batch_mode", default=False,
                                  help="wait for all data before displaying chart")
 
         self.__parser.add_option("--x", "-x", type="float", nargs=2, action="store", default=(-1.0, 1.0), dest="x",
                                  help="set x-axis to min / max (default -1, 1)")
 
-        self.__parser.add_option("--bincount", "-c", type="int", nargs=1, action="store", default=200, dest="bin_count",
+        self.__parser.add_option("--bincount", "-c", type="int", action="store", default=200, dest="bin_count",
                                  help="number of bins (default 200)")
 
-        self.__parser.add_option("--precision", "-p", type="int", nargs=1, action="store", default=3, dest="precision",
-                                 help="precision of reported deltas (default 3)")
-
         self.__parser.add_option("--skip-malformed", "-s", action="store_true", dest="skip_malformed", default=False,
                                  help="ignore rows with missing path values")
 
-        self.__parser.add_option("--output", "-o", type="string", nargs=1, action="store", dest="outfile",
+        # output...
+        self.__parser.add_option("--precision", "-p", type="int", action="store", default=3, dest="precision",
+                                 help="precision of reported deltas (default 3)")
+
+        self.__parser.add_option("--output", "-o", type="string", action="store", dest="outfile",
                                  help="output histogram to CSV file")
 
         self.__parser.add_option("--echo", "-e", action="store_true", dest="echo", default=False,
                                  help="echo stdin to stdout")
 
-        self.__parser.add_option("--title", "-t", type="string", nargs=1, action="store", dest="title",
+        self.__parser.add_option("--title", "-t", type="string", action="store", dest="title",
                                  help="chart title")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_localised_datetime.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_localised_datetime.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,43 +4,47 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdLocalizedDatetime(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog { [-o HOURS] [-m MINUTES] [-s SECONDS] [-t TIMEZONE_NAME] | "
-                                                    "-z }", version="%prog 1.0")
+                                                    "-z }", version=version())
 
-        # optional...
-        self.__parser.add_option("--hours", "-o", type="int", nargs=1, default=0, action="store", dest="hours",
+        # fields...
+        self.__parser.add_option("--hours", "-o", type="int", default=0, action="store", dest="hours",
                                  help="offset from now in hours")
 
-        self.__parser.add_option("--minutes", "-m", type="int", nargs=1, default=0, action="store", dest="minutes",
+        self.__parser.add_option("--minutes", "-m", type="int", default=0, action="store", dest="minutes",
                                  help="offset from now in minutes")
 
-        self.__parser.add_option("--seconds", "-s", type="int", nargs=1, default=0, action="store", dest="seconds",
+        self.__parser.add_option("--seconds", "-s", type="int", default=0, action="store", dest="seconds",
                                  help="offset from now in seconds")
 
-        self.__parser.add_option("--timezone", "-t", type="string", nargs=1, action="store", dest="zone",
+        self.__parser.add_option("--timezone", "-t", type="string", action="store", dest="zone",
                                  help="present the time in the given zone")
 
+        # helper...
         self.__parser.add_option("--zones", "-z", action="store_true", dest="list", default=False,
                                  help="list the available timezone names to stderr")
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_monitor_auth.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_socket_receiver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,51 @@
 """
-Created on 20 Apr 2021
+Created on 13 Jul 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
+
+source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdMonitorAuth(object):
+class CmdSocketReceiver(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [{ -s | -d }] [-v]", version="%prog 1.0")
-
-        # commands..
-        self.__parser.add_option("--set", "-s", action="store_true", dest="set", default=False,
-                                 help="set the authentication interactively")
+        self.__parser = optparse.OptionParser(usage="%prog [-p PORT] [-v]", version=version())
 
-        self.__parser.add_option("--delete", "-d", action="store_true", dest="delete", default=False,
-                                 help="delete the authentication")
+        # input...
+        self.__parser.add_option("--port", "-p", type="int", action="store", default=2000, dest="port",
+                                 help="socket port (default 2000)")
 
-        # reporting flag..
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def is_valid(self):
-        if self.set and self.delete:
-            return False
-
-        return True
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @property
-    def set(self):
-        return self.__opts.set
-
-
     @property
-    def delete(self):
-        return self.__opts.delete
+    def port(self):
+        return self.__opts.port
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def print_help(self, file):
-        self.__parser.print_help(file)
-
-
     def __str__(self, *args, **kwargs):
-        return "CmdMonitorAuth:{set:%s, delete:%s, verbose:%s}" % \
-               (self.set, self.delete, self.verbose)
+        return "CmdSocketReceiver:{port:%d, verbose:%s}" % (self.port, self.verbose)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_mqtt_client.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_mqtt_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Created on 23 Mar 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
 from scs_core.data.str import Str
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdMQTTClient(object):
     """unix command line handler"""
@@ -17,32 +18,33 @@
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-p UDS_PUB] "
                                                     "[-s] { -c { C | G | P | S | X } (UDS_SUB_1) | "
                                                     "[SUB_TOPIC_1 (UDS_SUB_1) .. SUB_TOPIC_N (UDS_SUB_N)] } "
-                                                    "[-n] [-t] [-e] [-v]", version="%prog 1.0")
+                                                    "[-n] [-t] [-e] [-v]", version=version())
 
-        # optional...
-        self.__parser.add_option("--pub", "-p", type="string", nargs=1, action="store", dest="uds_pub",
+        # operations..
+        self.__parser.add_option("--pub", "-p", type="string", action="store", dest="uds_pub",
                                  default=None, help="read publications from UDS instead of stdin")
 
         self.__parser.add_option("--sub", "-s", action="store_true", dest="uds_sub",
                                  help="write subscriptions to UDS instead of stdout")
 
-        self.__parser.add_option("--channel", "-c", type="string", nargs=1, action="store", dest="channel",
+        self.__parser.add_option("--channel", "-c", type="string", action="store", dest="channel",
                                  help="subscribe to channel")
 
         self.__parser.add_option("--no-wrapper", "-n", action="store_true", dest="no_wrapper", default=False,
                                  help="discard topic wrapper")
 
         self.__parser.add_option("--timed", "-t", action="store_true", dest="timed", default=False,
                                  help="add a field for received datetime")
 
+        # output...
         self.__parser.add_option("--echo", "-e", action="store_true", dest="echo", default=False,
                                  help="echo input to stdout (if not writing subscriptions to stdout)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_multi_chart.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_single_chart.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,72 +1,83 @@
 """
-Created on 13 Oct 2016
+Created on 11 Jul 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdMultiChart(object):
+class CmdSingleChart(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-b] [-x POINTS] [-y MIN MAX] [-e] [-t TITLE] [-v] "
-                                                    "PATH_1 .. PATH_N", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-b] [-r] [-x POINTS] [-y MIN MAX] [-e] [-t TITLE] [-v] "
+                                                    "[PATH]", version=version())
 
-        # optional...
+        # mode...
         self.__parser.add_option("--batch", "-b", action="store_true", dest="batch_mode", default=False,
                                  help="wait for all data before displaying chart")
 
-        self.__parser.add_option("--x", "-x", type="int", nargs=1, action="store", default=600, dest="x",
+        self.__parser.add_option("--relative", "-r", action="store_true", dest="relative", default=False,
+                                 help="display relative values (first value is 0)")
+
+        self.__parser.add_option("--x", "-x", type="int", action="store", default=600, dest="x",
                                  help="number of x points (default 600)")
 
         self.__parser.add_option("--y", "-y", type="float", nargs=2, action="store", default=(-10.0, 10.0), dest="y",
                                  help="set y-axis to min / max (default -10, 10)")
 
-        self.__parser.add_option("--echo", "-e", action="store_true", dest="echo", default=False,
-                                 help="echo stdin to stdout")
-
         self.__parser.add_option("--skip-malformed", "-s", action="store_true", dest="skip_malformed", default=False,
                                  help="ignore rows with missing path values")
 
-        self.__parser.add_option("--title", "-t", type="string", nargs=1, action="store", dest="title",
+        # output...
+        self.__parser.add_option("--title", "-t", type="string", action="store", dest="title",
                                  help="chart title")
 
+        self.__parser.add_option("--echo", "-e", action="store_true", dest="echo", default=False,
+                                 help="echo stdin to stdout")
+
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if len(self.paths) == 0:
+        if self.path is None:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def batch_mode(self):
         return self.__opts.batch_mode
 
 
     @property
+    def relative(self):
+        return self.__opts.relative
+
+
+    @property
     def x(self):
         return self.__opts.x
 
 
     @property
     def y(self):
         return self.__opts.y
@@ -89,22 +100,22 @@
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     @property
-    def paths(self):
-        return self.__args
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdMultiChart:{batch_mode:%s, x:%d, y:%s, echo:%s, skip_malformed:%s, title:%s, " \
-               "verbose:%s, paths:%s}" % \
-                    (self.batch_mode, self.x, self.y, self.echo, self.skip_malformed, self.title,
-                     self.verbose, self.paths)
+        return "CmdSingleChart:{batch_mode:%s, relative:%s, x:%d, y:%s, echo:%s, skip_malformed:%s, title:%s, " \
+               "verbose:%s, path:%s}" % \
+                    (self.batch_mode, self.relative, self.x, self.y, self.echo, self.skip_malformed, self.title,
+                     self.verbose, self.path)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_node.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,44 +4,45 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
 from scs_core.data.path_dict import PathDict
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdNode(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-x] [-a] [-s] [-f FILE] [-i INDENT] [-v] "
-                                                    "[SUB_PATH_1 .. SUB_PATH_N]", version="%prog 1.0")
+                                                    "[SUB_PATH_1 .. SUB_PATH_N]", version=version())
 
-        # optional...
+        # mode...
         self.__parser.add_option("--exclude", "-x", action="store_true", dest="exclude", default=False,
                                  help="include all sub-paths except the named one(s)")
 
         self.__parser.add_option("--array", "-a", action="store_true", dest="array", default=False,
                                  help="output the sequence of input JSON documents as array")
 
         self.__parser.add_option("--sequence", "-s", action="store_true", dest="sequence", default=False,
                                  help="output the contents of the input array node(s) as a sequence")
 
-        self.__parser.add_option("--file", "-f", type="string", nargs=1, action="store", dest="filename",
+        self.__parser.add_option("--file", "-f", type="string", action="store", dest="filename",
                                  help="read from FILE instead of stdin")
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_devices.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_organisation_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 Created on 19 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdOrganisationDevices(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -F { -l ORG_LABEL | -t DEVICE_TAG } | "
                                                     "-C -l ORG_LABEL -t DEVICE_TAG -p PATH_ROOT GROUP LOCATION"
-                                                    " -d DEPLOYMENT_LABEL | "
-                                                    "-D -t DEVICE_TAG } "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+                                                    " -d DEPLOYMENT_LABEL | -D -t DEVICE_TAG } "
+                                                    "[-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
@@ -46,15 +47,15 @@
         self.__parser.add_option("--project", "-p", type="string", nargs=3, action="store", dest="project",
                                  help="path root, group and location number")
 
         self.__parser.add_option("--deployment-label", "-d", type="string", action="store", dest="deployment_label",
                                  help="the device's deployment label")
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_path_roots.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_organisation_path_roots.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 Created on 18 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdOrganisationPathRoots(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F [-l ORG_LABEL] | "
                                                     "-C -l ORG_LABEL -r PATH_ROOT | "
                                                     "-D -l ORG_LABEL -r PATH_ROOT } "
-                                                    "[-m] [-i INDENT] [-v]", version="%prog 1.0")
+                                                    "[-m] [-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
@@ -42,15 +44,15 @@
         self.__parser.add_option("--path-root", "-r", type="string", action="store", dest="path_root",
                                  help="the organisation path root")
 
         # output...
         self.__parser.add_option("--memberships", "-m", action="store_true", dest="memberships", default=False,
                                  help="show path root's user path memberships")
 
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_user_paths.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_organisation_user_paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 Created on 18 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdOrganisationUserPaths(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F { -e EMAIL | -r PATH_ROOT } | "
                                                     "-C -e EMAIL -r PATH_ROOT -x PATH_EXTENSION | "
                                                     "-D -e EMAIL -r PATH_ROOT -x PATH_EXTENSION } "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+                                                    "[-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
@@ -42,15 +44,15 @@
         self.__parser.add_option("--path-root", "-r", type="string", action="store", dest="path_root",
                                  help="the organisation path root")
 
         self.__parser.add_option("--path-extension", "-x", type="string", action="store", dest="path_extension",
                                  help="the organisation path root")
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_users.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_organisation_users.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 Created on 18 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdOrganisationUsers(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F [{ -e EMAIL | -l ORG_LABEL }] | "
                                                     "-R -e EMAIL -l ORG_LABEL | "
-                                                    "-C -e EMAIL -l ORG_LABEL -o { 1 | 0 } -d { 1 | 0 } | "
-                                                    "-U -e EMAIL -l ORG_LABEL [-o { 1 | 0 }] [-d { 1 | 0 }] "
-                                                    "[-s { 1 | 0 }] | "
+                                                    "-C -e EMAIL -l ORG_LABEL -o { 0 | 1 } -d { 0 | 1 } | "
+                                                    "-U -e EMAIL -l ORG_LABEL [-o { 0 | 1 }] [-d { 0 | 1 }] "
+                                                    "[-s { 0 | 1 }] | "
                                                     "-D -e EMAIL -l ORG_LABEL } "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+                                                    "[-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
@@ -57,15 +59,15 @@
         self.__parser.add_option("--device-admin", "-d", type="int", action="store", dest="device_admin",
                                  help="the device administrator status")
 
         self.__parser.add_option("--suspended", "-s", type="int", action="store", dest="suspended",
                                  help="the suspended status")
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisations.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_organisations.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 Created on 10 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdOrganisations(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F | "
                                                     "-C -l LABEL -n LONG_NAME -u URL -o OWNER_EMAIL | "
                                                     "-U LABEL [-l LABEL] [-n LONG_NAME] [-u URL] [-o OWNER_EMAIL] | "
                                                     "-D LABEL } "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+                                                    "[-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
@@ -49,15 +51,15 @@
         self.__parser.add_option("--url", "-u", type="string", action="store", dest="url",
                                  help="the organisation URL")
 
         self.__parser.add_option("--owner", "-o", type="string", action="store", dest="owner",
                                  help="the organisation owner email")
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+        self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_aggregate.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_aggregate.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,46 +4,48 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
 from scs_core.data.timedelta import Timedelta
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleAggregate(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog -c HH:MM:SS [-m] [-i ISO] [-r { [DD-]HH:MM[:SS] | :SS }] "
-                                                    "[-x] [-v] [PATH_1 .. PATH_N]", version="%prog 1.0")
+                                                    "[-x] [-v] [PATH_1 .. PATH_N]", version=version())
 
-        # compulsory...
-        self.__parser.add_option("--checkpoint", "-c", type="string", nargs=1, action="store", dest="checkpoint",
+        # operation...
+        self.__parser.add_option("--checkpoint", "-c", type="string", action="store", dest="checkpoint",
                                  help="a time specification i.e. **:/05:00")
 
-        # optional...
+        # mode...
         self.__parser.add_option("--min-max", "-m", action="store_true", dest="min_max", default=False,
                                  help="report min and max in addition to midpoint")
 
-        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
+        self.__parser.add_option("--iso-path", "-i", type="string", action="store", default="rec", dest="iso",
                                  help="path for ISO 8601 datetime field (default 'rec')")
 
-        self.__parser.add_option("--rule", "-r", type="string", nargs=1, action="store", dest="rule",
+        self.__parser.add_option("--rule", "-r", type="string", action="store", dest="rule",
                                  help="apply 75% rule with sampling INTERVAL")
 
         self.__parser.add_option("--exclude-remainder", "-x", action="store_true", dest="exclude_remainder",
                                  help="ignore data points after the last complete period")
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_collator.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_collator.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,50 +4,53 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleCollator(object):
     """unix command line handler"""
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog -x IND_PATH [-n NAME] -y DEP_PATH "
                                                     "[-l LOWER_BOUND] -u UPPER_BOUND -d DELTA [-v]",
-                                              version="%prog 1.0")
+                                              version=version())
 
         # compulsory...
-        self.__parser.add_option("--ind-path", "-x", type="string", nargs=1, action="store", dest="ind_path",
+        self.__parser.add_option("--ind-path", "-x", type="string", action="store", dest="ind_path",
                                  help="path to independent variable")
 
-        self.__parser.add_option("--name", "-n", type="string", nargs=1, action="store", dest="name",
+        self.__parser.add_option("--name", "-n", type="string", action="store", dest="name",
                                  help="name of the independent variable")
 
-        self.__parser.add_option("--dep-path", "-y", type="string", nargs=1, action="store", dest="dep_path",
+        self.__parser.add_option("--dep-path", "-y", type="string", action="store", dest="dep_path",
                                  help="path to dependent variable")
 
-        self.__parser.add_option("--upper", "-u", type="int", nargs=1, action="store", dest="upper",
+        self.__parser.add_option("--upper", "-u", type="int", action="store", dest="upper",
                                  help="upper bound of dataset")
 
-        self.__parser.add_option("--delta", "-d", type="int", nargs=1, action="store", dest="delta",
+        self.__parser.add_option("--delta", "-d", type="int", action="store", dest="delta",
                                  help="width of column domain")
 
         # optional...
-        self.__parser.add_option("--lower", "-l", type="int", nargs=1, action="store", dest="lower", default=0,
+        self.__parser.add_option("--lower", "-l", type="int", action="store", dest="lower", default=0,
                                  help="lower bound of dataset (default 0)")
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_concentration.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_gas_concentration.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,34 +4,36 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
 from scs_core.gas.gas import Gas
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleConcentration(object):
+class CmdSampleGasConcentration(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-v] GAS DENSITY_PATH T_PATH [{P_PATH | -p PRESSURE}]",
-                                              version="%prog 1.0")
+                                              version=version())
 
-        # optional...
-        self.__parser.add_option("--pressure", "-p", type="float", nargs=1, action="store", dest="pressure",
+        # mode...
+        self.__parser.add_option("--pressure", "-p", type="float", action="store", dest="pressure",
                                  default=Gas.STP_PRESSURE, help="assume constant atmospheric pressure in kPA "
-                                                                "(default 101.3)")
+                                                                "(default %s)" % Gas.STP_PRESSURE)
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
@@ -81,9 +83,9 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleConcentration:{pressure:%s, verbose:%s, gas:%s, density_path:%s, t_path:%s, p_path:%s}" % \
+        return "CmdSampleGasConcentration:{pressure:%s, verbose:%s, gas:%s, density_path:%s, t_path:%s, p_path:%s}" % \
                (self.pressure, self.verbose, self.gas, self.density_path, self.t_path, self.p_path)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_distance.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_distance.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,38 +4,41 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleDistance(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog -p LAT LNG [-i ISO] [-q QUALITY] [-v] GPS_PATH",
-                                              version="%prog 1.0")
+                                              version=version())
 
         # compulsory...
         self.__parser.add_option("--position", "-p", type="float", nargs=2, action="store", dest="position",
                                  help="position (in degrees)")
 
         # optional...
-        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
+        self.__parser.add_option("--iso-path", "-i", type="string", action="store", default="rec", dest="iso",
                                  help="path for ISO 8601 datetime output (default 'rec')")
 
-        self.__parser.add_option("--quality", "-q", type="int", nargs=1, action="store", dest="quality",
+        self.__parser.add_option("--quality", "-q", type="int", action="store", dest="quality",
                                  help="minimum acceptable GPS quality")
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_duplicates.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_duplicates.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,33 +4,36 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleDuplicates(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [{ -x | -c }] [-v] [PATH]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [{ -x | -c }] [-v] [PATH]", version=version())
 
-        # optional...
+        # mode...
         self.__parser.add_option("--exclude", "-x", action="store_true", dest="exclude", default=False,
                                  help="output non-duplicate documents only")
 
         self.__parser.add_option("--counts", "-c", action="store_true", dest="counts", default=False,
                                  help="only list the count of matching documents")
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_error.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_error.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,38 +4,40 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleError(object):
     """
     unix command line handler
     """
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog { -l | -s } [-p PRECISION] [-v] "
-                                                    "REFERENCE_PATH REPORTED_PATH ERROR_PATH", version="%prog 1.0")
+                                                    "REFERENCE_PATH REPORTED_PATH ERROR_PATH", version=version())
 
-        # compulsory...
+        # mode...
         self.__parser.add_option("--linear", "-l", action="store_true", dest="linear", default=False,
                                  help="error is REPORTED - REFERENCE")
 
         self.__parser.add_option("--scaling", "-s", action="store_true", dest="scaling", default=False,
                                  help="error is REPORTED / REFERENCE")
 
-        # optional...
-        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=3, dest="precision",
+        # output...
+        self.__parser.add_option("--prec", "-p", type="int", action="store", default=3, dest="precision",
                                  help="precision (default 3 decimal places)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_filter.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleFilter(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-p PRECISION] [-v] [PATH]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-p PRECISION] [-v] [PATH]", version=version())
 
-        # optional...
-        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=None, dest="precision",
+        # output...
+        self.__parser.add_option("--prec", "-p", type="int", action="store", default=None, dest="precision",
                                  help="precision (default 0 decimal places)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_interval.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_interval.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleInterval(object):
     """
     unix command line handler
     """
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-p PRECISION] [-v] [PATH]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-p PRECISION] [-v] [PATH]", version=version())
 
-        # optional...
-        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=3, dest="precision",
+        # output...
+        self.__parser.add_option("--prec", "-p", type="int", action="store", default=3, dest="precision",
                                  help="precision (default 3 decimal places)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_iso_8601.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_iso_8601.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,51 +4,56 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleISO8601(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog { -z | { -o | -f DATE_FORMAT } "
                                                     "[-t TIMEZONE_NAME [-u]] [-i ISO_PATH] "
                                                     "{ DATETIME_PATH | DATE_PATH TIME_PATH } } [-s] [-v]",
-                                              version="%prog 1.0")
+                                              version=version())
 
-        # optional...
+        # helper...
         self.__parser.add_option("--zones", "-z", action="store_true", dest="zones", default=False,
                                  help="list the available timezone names to stderr")
 
+        # formats...
         self.__parser.add_option("--oad", "-o", action="store_true", dest="oad", default=False,
                                  help="datetime format is OLE Automation date")
 
-        self.__parser.add_option("--format", "-f", type="string", nargs=1, action="store", dest="format",
+        self.__parser.add_option("--format", "-f", type="string", action="store", dest="format",
                                  help="specifies format of input date string, e.g. YYYY-MM-DD")
 
-        self.__parser.add_option("--timezone", "-t", type="string", nargs=1, action="store",
+        self.__parser.add_option("--timezone", "-t", type="string", action="store",
                                  dest="timezone", help="source timezone (default 'UTC')")
 
         self.__parser.add_option("--utc", "-u", action="store_true", dest="utc", default=False,
                                  help="shift timezone to UTC")
 
-        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
+        self.__parser.add_option("--iso-path", "-i", type="string", action="store", default="rec", dest="iso",
                                  help="path for ISO 8601 datetime output (default 'rec')")
 
+        # mode...
         self.__parser.add_option("--skip-malformed", "-s", action="store_true", dest="skip_malformed", default=False,
                                  help="ignore rows with malformed datetimes")
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_low_pass.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_low_pass.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,38 +4,40 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdLowPass(object):
     """
     unix command line handler
     """
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog -d DELTA_T -c CUT_OFF [-p PRECISION] [-v] [PATH]",
-                                              version="%prog 1.0")
+                                              version=version())
 
         # compulsory...
-        self.__parser.add_option("--delta", "-d", type="float", nargs=1, action="store", dest="delta",
+        self.__parser.add_option("--delta", "-d", type="float", action="store", dest="delta",
                                  help="sampling time interval")
 
-        self.__parser.add_option("--cut-off", "-c", type="float", nargs=1, action="store", dest="cut_off",
+        self.__parser.add_option("--cut-off", "-c", type="float", action="store", dest="cut_off",
                                  help="cut-off frequency")
 
-        # optional...
-        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=None, dest="precision",
+        # output...
+        self.__parser.add_option("--prec", "-p", type="int", action="store", default=None, dest="precision",
                                  help="precision (default 0 decimal places)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_median.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_median.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,34 +4,37 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleMedian(object):
     """
     unix command line handler
     """
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-w SIZE] [-p PRECISION] [-v] [PATH]",
-                                              version="%prog 1.0")
+                                              version=version())
 
         # optional...
-        self.__parser.add_option("--window", "-w", type="int", nargs=1, action="store", dest="window", default=3,
+        self.__parser.add_option("--window", "-w", type="int", action="store", dest="window", default=3,
                                  help="window size (must be an odd number, default 3)")
 
-        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=None, dest="precision",
+        # output...
+        self.__parser.add_option("--prec", "-p", type="int", action="store", default=None, dest="precision",
                                  help="precision (default 0 decimal places)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_nullify.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_nullify.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,41 +4,44 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleNullify(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog -t TARGET_PATH -s SOURCE_PATH [-l LOWER] [-u UPPER]"
-                                                    " [-v]", version="%prog 1.0")
+                                                    " [-v]", version=version())
 
-        # compulsory...
-        self.__parser.add_option("--target", "-t", type="string", nargs=1, action="store", dest="target",
+        # input...
+        self.__parser.add_option("--target", "-t", type="string", action="store", dest="target",
                                  help="field to be nullified")
 
-        self.__parser.add_option("--source", "-s", type="string", nargs=1, action="store", dest="source",
+        self.__parser.add_option("--source", "-s", type="string", action="store", dest="source",
                                  help="field providing the test value")
 
-        # optional...
-        self.__parser.add_option("--lower", "-l", type="float", nargs=1, action="store", dest="lower",
+        # operation...
+        self.__parser.add_option("--lower", "-l", type="float", action="store", dest="lower",
                                  help="lower bound")
 
-        self.__parser.add_option("--upper", "-u", type="float", nargs=1, action="store", dest="upper",
+        self.__parser.add_option("--upper", "-u", type="float", action="store", dest="upper",
                                  help="upper bound")
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_paths.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_uds.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,60 @@
 """
-Created on 18 Sep 2021
+Created on 25 Apr 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-source repo: scs_exegesis
+source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSamplePaths(object):
+class CmdUDS(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-v]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-v] UDS_SUB", version=version())
 
         # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
+    def is_valid(self):
+        if self.path is None:
+            return False
+
+        return True
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    @property
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
+
+
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSamplePaths:{verbose:%s}" % self.verbose
+        return "CmdUDS:{verbose:%s}" % self.verbose
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_record.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_record.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleRecord(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-v] [PATH]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-v] [PATH]", version=version())
 
-        # optional...
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_slope.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_slope.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,47 +4,49 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
 from scs_core.data.timedelta import Timedelta
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleSlope(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog -n NAME [-i ISO] [-t TALLY] [-m [DD-]HH:MM[:SS]] [-x] "
-                                                    "[-p PRECISION] [-v] PATH", version="%prog 1.0")
+                                                    "[-p PRECISION] [-v] PATH", version=version())
 
-        # compulsory...
-        self.__parser.add_option("--name", "-n", type="string", nargs=1, action="store", dest="name",
+        # identity...
+        self.__parser.add_option("--name", "-n", type="string", action="store", dest="name",
                                  help="slope field name (i.e. '1min')")
 
-        # optional...
-        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
+        # mode...
+        self.__parser.add_option("--iso-path", "-i", type="string", action="store", default="rec", dest="iso",
                                  help="path for ISO 8601 datetime field (default 'rec')")
 
-        self.__parser.add_option("--tally", "-t", type="int", nargs=1, action="store", default=2, dest="tally",
+        self.__parser.add_option("--tally", "-t", type="int", action="store", default=2, dest="tally",
                                  help="compute for rolling TALLY number of data points (default 2)")
 
-        self.__parser.add_option("--max-interval", "-m", type="string", nargs=1, action="store", dest="max_interval",
+        self.__parser.add_option("--max-interval", "-m", type="string", action="store", dest="max_interval",
                                  help="restart regression on long intervals")
 
         self.__parser.add_option("--exclude-incomplete", "-x", action="store_true", dest="exclude_incomplete",
                                  default=False, help="exclude incomplete tallies")
 
-        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=6, dest="precision",
+        # output...
+        self.__parser.add_option("--prec", "-p", type="int", action="store", default=6, dest="precision",
                                  help="precision (default 6 decimal places)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_sort.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_sort.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleSort(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-v] SORT_PATH_1 .. SORT_PATH_N", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-v] SORT_PATH_1 .. SORT_PATH_N", version=version())
 
         # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_stats.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,36 +4,38 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleStats(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-t TAG] [-i] [-p PRECISION] [-a] [-r] [-v] "
-                                                    "PATH1 [PATH2 .. PATHN]", version="%prog 1.0")
+                                                    "PATH1 [PATH2 .. PATHN]", version=version())
 
         # input...
-        self.__parser.add_option("--tag", "-t", type="string", nargs=1, action="store", default='tag', dest="tag",
+        self.__parser.add_option("--tag", "-t", type="string", action="store", default='tag', dest="tag",
                                  help="name of the tag field (default 'tag')")
 
         # output...
         self.__parser.add_option("--include-tag", "-i", action="store_true", dest="include_tag", default=False,
                                  help="include the device tag")
 
-        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=6, dest="precision",
+        self.__parser.add_option("--prec", "-p", type="int", action="store", default=6, dest="precision",
                                  help="precision (default 6 decimal places)")
 
         self.__parser.add_option("--analytic", "-a", action="store_true", dest="analytic", default=False,
                                  help="analytic output")
 
         self.__parser.add_option("--rows", "-r", action="store_true", dest="rows", default=False,
                                  help="output results for each path on a separate row")
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_subset.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_subset.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,51 +4,53 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.datum import Datum
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleSubset(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog { -i | -n | -s } { [-e EQUAL] | [-l LOWER] [-u UPPER] } "
-                                                    "[-t] [-x] [-v] PATH", version="%prog 1.0")
+                                                    "[-t] [-x] [-v] PATH", version=version())
 
         # casting...
         self.__parser.add_option("--iso8601", "-i", action="store_true", dest="iso8601", default=False,
                                  help="interpret the value as an ISO 8601 datetime")
 
         self.__parser.add_option("--numeric", "-n", action="store_true", dest="numeric", default=False,
                                  help="interpret the value as a number")
 
         self.__parser.add_option("--string", "-s", action="store_true", dest="string", default=False,
                                  help="interpret the value as a string")
 
         self.__parser.add_option("--strict", "-t", action="store_true", dest="strict", default=False,
                                  help="halt on type errors")
 
-        # function...
-        self.__parser.add_option("--equal", "-e", type="string", nargs=1, action="store", dest="equal",
+        # operation...
+        self.__parser.add_option("--equal", "-e", type="string", action="store", dest="equal",
                                  help="equal to")
 
-        self.__parser.add_option("--lower", "-l", type="string", nargs=1, action="store", dest="lower",
+        self.__parser.add_option("--lower", "-l", type="string", action="store", dest="lower",
                                  help="lower bound")
 
-        self.__parser.add_option("--upper", "-u", type="string", nargs=1, action="store", dest="upper",
+        self.__parser.add_option("--upper", "-u", type="string", action="store", dest="upper",
                                  help="upper bound")
 
         # output...
         self.__parser.add_option("--exclusions", "-x", action="store_true", dest="exclusions", default=False,
                                  help="output exclusions instead of inclusions")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_tally.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_gas_density.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,71 @@
 """
-Created on 22 Aug 2017
+Created on 17 Jul 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleTally(object):
-    """unix command line handler"""
+class CmdSampleGasDensity(object):
+    """
+    unix command line handler
+    """
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-t TALLY] [-p PRECISION] [-v] [PATH]", version="%prog 1.0")
-
-        # optional...
-        self.__parser.add_option("--tally", "-t", type="int", nargs=1, action="store", dest="tally",
-                                 help="generate a rolling aggregate for TALLY number of data points (default all)")
+        self.__parser = optparse.OptionParser(usage="%prog [-p PRECISION] [-v] PATH", version=version())
 
-        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=None, dest="precision",
-                                 help="precision (default 0 decimal places)")
+        # output...
+        self.__parser.add_option("--prec", "-p", type="int", action="store", default=1, dest="precision",
+                                 help="precision (default 1 decimal place)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.tally is not None and self.tally < 1:
+        if len(self.__args) != 1:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def tally(self):
-        return self.__opts.tally
-
-
-    @property
     def precision(self):
         return self.__opts.precision
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     @property
     def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
+        return None if self.__args is None else self.__args[0]
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleTally:{tally:%s, precision:%s, verbose:%s, path:%s}" % \
-                    (self.tally, self.precision, self.verbose, self.path)
+        return "CmdSampleGasDensity:{precision:%s, verbose:%s, path:%s}" % \
+               (self.precision, self.verbose, self.path)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_time_shift.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_time_shift.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
 from scs_core.data.timedelta import Timedelta
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleTimeShift(object):
     """
@@ -19,17 +20,17 @@
     """
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog -t { + | - } [[DD-]HH:]MM[:SS] [-v] [PATH]",
-                                              version="%prog 1.0")
+                                              version=version())
 
-        # functions...
+        # operation...
         self.__parser.add_option("--timedelta", "-t", type="string", nargs=2, action="store", dest="timedelta",
                                  help="sign and offset in days / hours / minutes / seconds")
 
         # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_timezone.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_timezone.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,33 +4,37 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CmdSampleTimezone(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog { -z | [-i ISO_PATH] TIMEZONE_NAME }", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog { -z | [-i ISO_PATH] TIMEZONE_NAME }", version=version())
 
-        # optional...
+        # helper...
         self.__parser.add_option("--zones", "-z", action="store_true", dest="zones", default=False,
                                  help="list the available timezone names to stderr")
 
-        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
+        # input...
+        self.__parser.add_option("--iso-path", "-i", type="string", action="store", default="rec", dest="iso",
                                  help="path for ISO 8601 datetime output (default 'rec')")
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_single_chart.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_aws_byline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,118 +1,151 @@
 """
-Created on 11 Jul 2016
+Created on 25 Dec 2018
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSingleChart(object):
+class CmdAWSByline(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-b] [-r] [-x POINTS] [-y MIN MAX] [-e] [-t TITLE] [-v] "
-                                                    "[PATH]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -d DEVICE | -t TOPIC [-l] | -a } "
+                                                    "[-x EXCLUDED] [-s] [-m] [-i INDENT] [-v]", version=version())
+
+        # identity...
+        self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
+                                 help="the stored credentials to be presented")
+
+        # search types...
+        self.__parser.add_option("--device", "-d", type="string", action="store", dest="device",
+                                 help="report bylines for DEVICE")
 
-        # optional...
-        self.__parser.add_option("--batch", "-b", action="store_true", dest="batch_mode", default=False,
-                                 help="wait for all data before displaying chart")
+        self.__parser.add_option("--topic", "-t", type="string", action="store", dest="topic",
+                                 help="report bylines for TOPIC")
 
-        self.__parser.add_option("--relative", "-r", action="store_true", dest="relative", default=False,
-                                 help="display relative values (first value is 0)")
+        self.__parser.add_option("--all", "-a", action="store_true", dest="all", default=False,
+                                 help="report all bylines")
 
-        self.__parser.add_option("--x", "-x", type="int", nargs=1, action="store", default=600, dest="x",
-                                 help="number of x points (default 600)")
+        # filters...
+        self.__parser.add_option("--excluded", "-x", type="string", action="store", dest="excluded",
+                                 help="exclude topics ending with EXCLUDED")
 
-        self.__parser.add_option("--y", "-y", type="float", nargs=2, action="store", default=(-10.0, 10.0), dest="y",
-                                 help="set y-axis to min / max (default -10, 10)")
+        self.__parser.add_option("--strict", "-s", action="store_true", dest="strict", default=False,
+                                 help="only report devices with valid tags")
 
-        self.__parser.add_option("--echo", "-e", action="store_true", dest="echo", default=False,
-                                 help="echo stdin to stdout")
+        # output...
+        self.__parser.add_option("--latest", "-l", action="store_true", dest="latest", default=False,
+                                 help="only report the most recent byline")
 
-        self.__parser.add_option("--skip-malformed", "-s", action="store_true", dest="skip_malformed", default=False,
-                                 help="ignore rows with missing path values")
+        self.__parser.add_option("--include-messages", "-m", action="store_true", dest="include_messages",
+                                 default=False, help="report the message with each byline")
 
-        self.__parser.add_option("--title", "-t", type="string", nargs=1, action="store", dest="title",
-                                 help="chart title")
+        self.__parser.add_option("--indent", "-i", action="store", dest="indent", type=int,
+                                 help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.path is None:
+        count = 0
+
+        if bool(self.device):
+            count += 1
+
+        if bool(self.topic):
+            count += 1
+
+        if self.all:
+            count += 1
+
+        if count != 1:
+            return False
+
+        if self.latest and not bool(self.topic):
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
+    # properties: identity...
 
     @property
-    def batch_mode(self):
-        return self.__opts.batch_mode
+    def credentials_name(self):
+        return self.__opts.credentials_name
 
 
+    # ----------------------------------------------------------------------------------------------------------------
+
     @property
-    def relative(self):
-        return self.__opts.relative
+    def device(self):
+        return self.__opts.device
 
 
     @property
-    def x(self):
-        return self.__opts.x
+    def topic(self):
+        return self.__opts.topic
 
 
     @property
-    def y(self):
-        return self.__opts.y
+    def latest(self):
+        return self.__opts.latest
 
 
     @property
-    def echo(self):
-        return self.__opts.echo
+    def all(self):
+        return self.__opts.all
 
 
     @property
-    def skip_malformed(self):
-        return self.__opts.skip_malformed
+    def excluded(self):
+        return self.__opts.excluded
 
 
     @property
-    def title(self):
-        return self.__opts.title
+    def strict(self):
+        return self.__opts.strict
 
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def include_messages(self):
+        return self.__opts.include_messages
 
 
     @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
+    def indent(self):
+        return self.__opts.indent
+
+
+    @property
+    def verbose(self):
+        return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSingleChart:{batch_mode:%s, relative:%s, x:%d, y:%s, echo:%s, skip_malformed:%s, title:%s, " \
-               "verbose:%s, path:%s}" % \
-                    (self.batch_mode, self.relative, self.x, self.y, self.echo, self.skip_malformed, self.title,
-                     self.verbose, self.path)
+        return "CmdAWSByline:{credentials_name:%s, device:%s, topic:%s, latest:%s, all:%s, excluded:%s, strict:%s, " \
+               "include_messages:%s, indent:%s, verbose:%s}" % \
+               (self.credentials_name, self.device, self.topic, self.latest, self.all, self.excluded, self.strict,
+                self.include_messages, self.indent, self.verbose)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_uds.py` & `scs-analysis-2.8.5/src/scs_analysis/cmd/cmd_sample_paths.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,46 @@
 """
-Created on 25 Apr 2017
+Created on 18 Sep 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-source repo: scs_analysis
+source repo: scs_exegesis
 """
 
 import optparse
 
+from scs_analysis import version
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdUDS(object):
+class CmdSamplePaths(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-v] UDS_SUB", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-v]", version=version())
 
-        # optional...
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def is_valid(self):
-        if self.path is None:
-            return False
-
-        return True
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
-
-
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdUDS:{verbose:%s}" % self.verbose
+        return "CmdSamplePaths:{verbose:%s}" % self.verbose
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cognito_devices.py` & `scs-analysis-2.8.5/src/scs_analysis/cognito_devices.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,31 +5,32 @@
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
 The cognito_devices utility is used to create, update and retrieve AWS Cognito identities. This utility can only be used
-by organisation administrators and superusers.
+by customer organisation administrators, SCS administrators and superusers.
 
 If the --Create function is used, an email is sent to the new user. The verification link in the email must be
-excercised in order for the account to gain a CONFIRMED status.
+excercised using the cognito_email utility in order for the account to gain a CONFIRMED status.
 
 SYNOPSIS
 cognito_devices.py  [-c CREDENTIALS] { -F [{ -t TAG | -n INVOICE }] [-m] | -U TAG INVOICE | -D TAG } [-i INDENT] [-v]
 
 EXAMPLES
 cognito_devices.py -vi4 -c super -F -m
 
 DOCUMENT EXAMPLE
 {"username": "scs-bgx-401", "invoice": "INV-000123",
 "created": "2023-06-23T10:32:52+01:00", "last-updated": "2023-06-23T10:32:52+01:00"}
 
 SEE ALSO
 scs_analysis/cognito_credentials
+scs_analysis/cognito_email
 scs_analysis/cognito_users
 scs_analysis/organisation_devices
 
 RESOURCES
 https://docs.aws.amazon.com/cognito/latest/developerguide/signing-up-users-in-your-app.html
 https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-policies.html
 """
@@ -57,16 +58,14 @@
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
-    credentials = None
-    finder = None
     report = None
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
         cmd = CmdCognitoDevices()
@@ -112,16 +111,16 @@
         if cmd.find:
             if cmd.tag is not None:
                 report = sorted(finder.find_by_tag(auth.id_token, cmd.tag))   # TODO: Internal Server Error on null tag
 
             else:
                 report = sorted(finder.find_all(auth.id_token))
 
-            if cmd.invoice_name is not None:
-                report = [device for device in report if device.invoice_number == cmd.invoice_name]
+            if cmd.invoice_number is not None:
+                report = [device for device in report if device.invoice_number == cmd.invoice_number]
 
             if cmd.memberships:
                 org_devices = org_manager.find_devices(auth.id_token)
                 report = CognitoMembership.merge(report, org_devices)
 
         if cmd.update:
             # find...
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cognito_email.py` & `scs-analysis-2.8.5/src/scs_analysis/cognito_email.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cognito_user_credentials.py` & `scs-analysis-2.8.5/src/scs_analysis/cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cognito_user_identity.py` & `scs-analysis-2.8.5/src/scs_analysis/cognito_user_identity.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 SYNOPSIS
 cognito_user_identity.py [-c CREDENTIALS] | -C | -R | -U } [-i INDENT] [-v]
 
 EXAMPLES
 ./cognito_user_identity.py -R
 
 DOCUMENT EXAMPLE
-{"username""8", "creation-date""2021-11-24T12:51:12Z", "confirmation-status""CONFIRMED", "enabled": true,
-"email""bruno.beloff@southcoastscience.com", "given-name""Bruno", "family-name""Beloff", "is-super": true}
+{"username": "506cd055-1978-4984-9f17-2fad77797fa1", "email": "bruno.beloff@southcoastscience.com",
+"given-name": "Bruno", "family-name": "Beloff", "confirmation-status": "CONFIRMED", "enabled": true,
+"email-verified": true, "is-super": false, "is-tester": false, "is-financial": false,
+"created": "2023-04-20T11:45:21Z", "last-updated": "2023-06-26T14:39:17Z"}
 
 SEE ALSO
 scs_analysis/cognito_credentials
 
 RESOURCES
 https://docs.aws.amazon.com/cognito/latest/developerguide/signing-up-users-in-your-app.html
 https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-policies.html
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/cognito_users.py` & `scs-analysis-2.8.5/src/scs_analysis/cognito_users.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 The cognito_users utility is used to create, update and retrieve AWS Cognito identities. This utility can only be used
 by organisation administrators and superusers.
 
 If the --Create function is used, an email is sent to the new user. The verification link in the email must be
 excercised in order for the account to gain a CONFIRMED status.
 
 SYNOPSIS
-cognito_users.py  [-c CREDENTIALS] { -F [{ -e EMAIL_ADDR | -l ORG_LABEL | -c CONFIRMATION | -s { 1 | 0 } } }] | \
+cognito_users.py  [-c CREDENTIALS] { -F [{ -e EMAIL_ADDR | -l ORG_LABEL | -c CONFIRMATION | -s { 0 | 1 } } }] | \
 -C | -U -e EMAIL_ADDR | -D -e EMAIL_ADDR } [-i INDENT] [-v]
 
 EXAMPLES
 cognito_users.py -Fe bruno.beloff@southcoastscience.com
 
 DOCUMENT EXAMPLE
 {"username": "506cd055-1978-4984-9f17-2fad77797fa1", "email": "bruno.beloff@southcoastscience.com",
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/configuration_csv.py` & `scs-analysis-2.8.5/src/scs_analysis/configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/configuration_monitor.py` & `scs-analysis-2.8.5/src/scs_analysis/configuration_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/configuration_monitor_check.py` & `scs-analysis-2.8.5/src/scs_analysis/configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/csv_collation_summary.py` & `scs-analysis-2.8.5/src/scs_analysis/csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/csv_collator.py` & `scs-analysis-2.8.5/src/scs_analysis/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/csv_join.py` & `scs-analysis-2.8.5/src/scs_analysis/csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/csv_reader.py` & `scs-analysis-2.8.5/src/scs_analysis/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/csv_segmentor.py` & `scs-analysis-2.8.5/src/scs_analysis/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/csv_writer.py` & `scs-analysis-2.8.5/src/scs_analysis/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/device_controller.py` & `scs-analysis-2.8.5/src/scs_analysis/device_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,18 @@
 EXAMPLES
 device_controller.py -c super -t scs-be2-3 -m "vcal_baseline -i4" -s
 
 SEE ALSO
 scs_analysis/cognito_credentials
 
 BUGS
-Interactive history features may be unavailable in macOS.
+On macOS, interactive history features require full disk access for the Terminal app:
+
+PermissionError: [Errno 1] Operation not permitted after macOS Catalina Update
+https://stackoverflow.com/questions/58479686/permissionerror-errno-1-operation-not-permitted-after-macos-catalina-update
 """
 
 import json
 import os
 import sys
 
 import requests
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/device_monitor.py` & `scs-analysis-2.8.5/src/scs_analysis/device_monitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 DESCRIPTION
 The device monitor periodically checks on the availability and health of every air quality monitoring device. The
 device_monitor utility is used to manage the email addresses associated with individual devices.
 
 SYNOPSIS
 device_monitor.py [-c CREDENTIALS] { -F [{ -e EMAIL_ADDR | -t DEVICE_TAG } [-x]] | -A EMAIL_ADDR DEVICE_TAG |
--D EMAIL_ADDR [-t DEVICE_TAG] } [-i INDENT] [-v]
+-S DEVICE_TAG { 0 | 1 } | -D EMAIL_ADDR [-t DEVICE_TAG] } [-i INDENT] [-v]
 
 EXAMPLES
 device_monitor.py -c super -Ft scs-opc-109
 
 DOCUMENT EXAMPLE
-{"scs-opc-109": ["somebody@somewhere.com", "somebody@somewhere-else.com"], ...}
+{"device-tag": "scs-ph1-43", "recipients": ["someone@somewhere.com"], "suspended": false}
 
 SEE ALSO
 scs_analysis/cognito_user_credentials
 scs_analysis/device_monitor_status
 """
 
 import requests
@@ -31,47 +31,46 @@
 
 from scs_core.aws.manager.device_monitor_specification_manager import DeviceMonitorSpecificationManager
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_device import CognitoDeviceCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 
-from scs_core.client.http_exception import HTTPException
+from scs_core.client.http_exception import HTTPException, HTTPNotFoundException
 
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
-    logger = None
     response = None
     report = None
 
-    try:
-        # ------------------------------------------------------------------------------------------------------------
-        # cmd...
+    # ------------------------------------------------------------------------------------------------------------
+    # cmd...
 
-        cmd = CmdDeviceMonitor()
+    cmd = CmdDeviceMonitor()
 
-        if not cmd.is_valid():
-            cmd.print_help(sys.stderr)
-            exit(2)
+    if not cmd.is_valid():
+        cmd.print_help(sys.stderr)
+        exit(2)
 
-        Logging.config('device_monitor', verbose=cmd.verbose)
-        logger = Logging.getLogger()
+    Logging.config('device_monitor', verbose=cmd.verbose)
+    logger = Logging.getLogger()
 
-        logger.info(cmd)
+    logger.info(cmd)
 
+    try:
         # ------------------------------------------------------------------------------------------------------------
         # authentication...
 
         credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
 
         if not credentials:
             exit(1)
@@ -105,18 +104,21 @@
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         if cmd.find:
             report = manager.find(auth.id_token, email_address=cmd.email, device_tag=cmd.device_tag,
                                   exact=cmd.exact_match)
 
-        if cmd.add:
+        elif cmd.add:
             report = manager.add(auth.id_token, cmd.email, cmd.device_tag)
 
-        if cmd.delete:
+        elif cmd.suspend:
+            report = manager.set_suspended(auth.id_token, cmd.device_tag, bool(cmd.is_suspended))
+
+        elif cmd.delete:
             report = manager.remove(auth.id_token, cmd.email, device_tag=cmd.device_tag)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # end...
 
         # report...
@@ -125,10 +127,14 @@
 
         if cmd.find:
             logger.info('retrieved: %s' % len(report))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
+    except HTTPNotFoundException:
+        logger.error("device '%s' not found." % cmd.device_tag)
+        exit(1)
+
     except HTTPException as ex:
         logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/device_monitor_status.py` & `scs-analysis-2.8.5/src/scs_analysis/device_monitor_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/handler/aws_mqtt_publisher.py` & `scs-analysis-2.8.5/src/scs_analysis/handler/aws_mqtt_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/handler/aws_mqtt_subscription_handler.py` & `scs-analysis-2.8.5/src/scs_analysis/handler/aws_mqtt_subscription_handler.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/handler/batch_download_reporter.py` & `scs-analysis-2.8.5/src/scs_analysis/handler/batch_download_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/handler/configuration_csv_generator.py` & `scs-analysis-2.8.5/src/scs_analysis/handler/configuration_csv_generator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/handler/csv_collator.py` & `scs-analysis-2.8.5/src/scs_analysis/handler/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/handler/csv_segmentor.py` & `scs-analysis-2.8.5/src/scs_analysis/handler/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/handler/mqtt_reporter.py` & `scs-analysis-2.8.5/src/scs_analysis/handler/mqtt_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/handler/sample_midpoint.py` & `scs-analysis-2.8.5/src/scs_analysis/handler/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/handler/sample_regression.py` & `scs-analysis-2.8.5/src/scs_analysis/handler/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/histo_chart.py` & `scs-analysis-2.8.5/src/scs_analysis/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/localised_datetime.py` & `scs-analysis-2.8.5/src/scs_analysis/localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/monitor_auth.py` & `scs-analysis-2.8.5/src/scs_analysis/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/multi_chart.py` & `scs-analysis-2.8.5/src/scs_analysis/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/node.py` & `scs-analysis-2.8.5/src/scs_analysis/node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/organisation_devices.py` & `scs-analysis-2.8.5/src/scs_analysis/organisation_devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 import sys
 
 from scs_analysis.cmd.cmd_organisation_devices import CmdOrganisationDevices
 
 from scs_core.aws.config.project import Project
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
+from scs_core.aws.security.cognito_device import CognitoDeviceCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 
 from scs_core.aws.security.organisation import Organisation, OrganisationPathRoot, OrganisationDevice
 from scs_core.aws.security.organisation_manager import OrganisationManager
 
 from scs_core.client.http_exception import HTTPException
 
@@ -78,15 +79,15 @@
 
         logger.info(cmd)
 
         if cmd.org_label is not None and not Organisation.is_valid_label(cmd.org_label):
             logger.error("the organisation label '%s' is not valid." % cmd.org_label)
             exit(2)
 
-        if cmd.device_tag is not None and not OrganisationDevice.is_valid_tag(cmd.device_tag):
+        if cmd.device_tag is not None and not CognitoDeviceCredentials.is_valid_tag(cmd.device_tag):
             logger.error("the device tag '%s' is not valid." % cmd.device_tag)
             exit(2)
 
         if cmd.project_organisation is not None and \
                 not OrganisationPathRoot.is_valid_path_root(cmd.project_organisation):
             logger.error("the path root '%s' is not valid." % cmd.project_organisation)
             exit(2)
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/organisation_path_roots.py` & `scs-analysis-2.8.5/src/scs_analysis/organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/organisation_user_paths.py` & `scs-analysis-2.8.5/src/scs_analysis/organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/organisation_users.py` & `scs-analysis-2.8.5/src/scs_analysis/organisation_users.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 DESCRIPTION
 The organisation_users utility is used to
 
 SYNOPSIS
 organisation_users.py  [-c CREDENTIALS] { -F { -e EMAIL | -l ORG_LABEL } | \
 -R -e EMAIL -l ORG_LABEL | \
--C -e EMAIL -l ORG_LABEL -o { 1 | 0 } -d { 1 | 0 } | \
--U -e EMAIL -l ORG_LABEL [-o { 1 | 0 }] [-d { 1 | 0 }] [-s { 1 | 0 }] | \
+-C -e EMAIL -l ORG_LABEL -o { 0 | 1 } -d { 0 | 1 } | \
+-U -e EMAIL -l ORG_LABEL [-o { 0 | 1 }] [-d { 0 | 1 }] [-s { 0 | 1 }] | \
 -D -e EMAIL -l ORG_LABEL } \
 [-i INDENT] [-v]
 
 EXAMPLES
 organisation_users.py -F -l NARA
 
 DOCUMENT EXAMPLE
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/organisations.py` & `scs-analysis-2.8.5/src/scs_analysis/organisations.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_aggregate.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_average.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_average.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_collator.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_concentration.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_gas_concentration.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 Created on 15 Feb 2019
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The sample_concentration utility is used to inject a gas concentration value, based on a given density (microgrammes
+The sample_gas_concentration utility is used to inject a gas concentration value, based on a given density (microgrammes
 per cubic metre), temperature and pressure. The reported value is in parts per billion.
 
 Density and temperature must be supplied from the input JSON document. Atmospheric pressure may be supplied from the
 input JSON document. Alternatively, a pressure estimate may be supplied on the command line. In both cases, pressure
 should be indicated in kilopascals (kPa). If no pressure value is supplied, the standard pressure of 101.3 kPa is used.
 
 The path for the node in the output document indicating concentration is based on the path for the node in the
 input document indicating density. For example, if the input path is SUB-PATH.dns, the output path is SUB-PATH.cnc. If
 a SUB-PATH.cnc field exists in the input document, it is overwritten.
 
 SYNOPSIS
-sample_concentration.py [-v] GAS DENSITY_PATH T_PATH [{P_PATH | -p PRESSURE}]
+sample_gas_concentration.py [-v] GAS DENSITY_PATH T_PATH [{P_PATH | -p PRESSURE}]
 
 EXAMPLES
-csv_reader.py joined_2019-02.csv | sample_concentration.py -v NO2 ref.val.NO2.dns praxis.val.sht.tmp
+csv_reader.py joined_2019-02.csv | sample_gas_concentration.py -v NO2 ref.val.NO2.dns praxis.val.sht.tmp
 
 DOCUMENT EXAMPLE - INPUT
 {"rec": "2019-02-12T13:00:00Z", "praxis": {"val":
 {"NO2": {"weV": 0.300059, "cnc": 23.4, "aeV": 0.302339, "weC": -0.002793},
 "sht": {"hmd": 67.6, "tmp": 13.1}}}, "ref": {"val": {"NO2": {"units": "ugm-3", "dns": 51}}}}
 
 DOCUMENT EXAMPLE - OUTPUT
@@ -37,21 +37,23 @@
 
 RESOURCES
 http://www.apis.ac.uk/unit-conversion
 """
 
 import sys
 
-from scs_analysis.cmd.cmd_sample_concentration import CmdSampleConcentration
+from scs_analysis.cmd.cmd_sample_gas_concentration import CmdSampleGasConcentration
 
 from scs_core.data.json import JSONify
 from scs_core.data.path_dict import PathDict
 
 from scs_core.gas.gas import Gas
 
+from scs_core.sys.logging import Logging
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     density = None
     t = None
@@ -59,29 +61,36 @@
 
     document_count = 0
     processed_count = 0
 
     # ----------------------------------------------------------------------------------------------------------------
     # cmd...
 
-    cmd = CmdSampleConcentration()
+    cmd = CmdSampleGasConcentration()
 
     if not cmd.is_valid():
         cmd.print_help(sys.stderr)
         exit(2)
 
-    if not Gas.is_valid_name(cmd.gas):
-        print("sample_concentration: the gas '%s' is not recognised." % cmd.gas, file=sys.stderr)
-        exit(1)
+    Logging.config('sample_gas_concentration', verbose=cmd.verbose)
+    logger = Logging.getLogger()
+
+    logger.info(cmd)
 
-    if cmd.verbose:
-        print("sample_concentration: %s" % cmd, file=sys.stderr)
 
     try:
         # ------------------------------------------------------------------------------------------------------------
+        # validation...
+
+        if not Gas.is_valid_name(cmd.gas):
+            logger.error("the gas '%s' is not recognised." % cmd.gas)
+            exit(1)
+
+
+        # ------------------------------------------------------------------------------------------------------------
         # resources...
 
         density_nodes = cmd.density_path.split('.')
         concentration_path = '.'.join(density_nodes[:-1] + ['cnc'])
 
 
         # ------------------------------------------------------------------------------------------------------------
@@ -107,34 +116,34 @@
 
             if density_node == '' or t_node == '':
                 continue
 
             try:
                 density = float(density_node)
             except ValueError:
-                print("sample_concentration: invalid value for density in %s" % jstr, file=sys.stderr)
+                logger.error("invalid value for density in %s" % jstr)
                 exit(1)
 
             try:
                 t = float(t_node)
             except ValueError:
-                print("sample_concentration: invalid value for t in %s" % jstr, file=sys.stderr)
+                logger.error("invalid value for t in %s" % jstr)
                 exit(1)
 
             # p...
             if cmd.p_path:
                 p_node = datum.node(cmd.p_path)
 
                 if p_node == '':
                     continue
 
                 try:
                     p = float(p_node)
                 except ValueError:
-                    print("sample_concentration: invalid value for p in %s" % jstr, file=sys.stderr)
+                    logger.error("invalid value for p in %s" % jstr)
                     exit(1)
 
             else:
                 p = cmd.pressure
 
             # compute...
             cnc = round(Gas.concentration(cmd.gas, density, t, p), 1)
@@ -161,14 +170,12 @@
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except KeyError as ex:
-        print("sample_concentration: %s" % repr(ex), file=sys.stderr)
+        logger.error(repr(ex))
         exit(1)
 
     finally:
-        if cmd.verbose:
-            print("sample_concentration: documents: %d processed: %d" % (document_count, processed_count),
-                  file=sys.stderr)
+        logger.info("sample_gas_concentration: documents: %d processed: %d" % (document_count, processed_count))
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_distance.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_duplicates.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_error.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_interval.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_iso_8601.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_low_pass.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_max.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_max.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_median.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_median.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_midpoint.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_min.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_min.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_noise.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_noise.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_nullify.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_paths.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_regression.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_slope.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_sort.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_stats.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_subset.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_time_shift.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/sample_timezone.py` & `scs-analysis-2.8.5/src/scs_analysis/sample_timezone.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/single_chart.py` & `scs-analysis-2.8.5/src/scs_analysis/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/socket_receiver.py` & `scs-analysis-2.8.5/src/scs_analysis/socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/timer.py` & `scs-analysis-2.8.5/src/scs_analysis/timer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis/uds_receiver.py` & `scs-analysis-2.8.5/src/scs_analysis/uds_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.7/src/scs_analysis.egg-info/PKG-INFO` & `scs-analysis-2.8.5/src/scs_analysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 2.7.7
+Version: 2.8.5
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `scs-analysis-2.7.7/src/scs_analysis.egg-info/SOURCES.txt` & `scs-analysis-2.8.5/src/scs_analysis.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 README.rst
 requirements.txt
 setup.py
 src/scs_analysis/__init__.py
-src/scs_analysis/access_key.py
 src/scs_analysis/alert.py
 src/scs_analysis/alert_status.py
-src/scs_analysis/aws_api_auth.py
 src/scs_analysis/aws_byline.py
 src/scs_analysis/aws_client_auth.py
 src/scs_analysis/aws_mqtt_client.py
 src/scs_analysis/aws_topic_history.py
 src/scs_analysis/aws_topic_publisher.py
 src/scs_analysis/aws_upload_interval.py
 src/scs_analysis/baseline.py
@@ -43,18 +41,19 @@
 src/scs_analysis/organisation_path_roots.py
 src/scs_analysis/organisation_user_paths.py
 src/scs_analysis/organisation_users.py
 src/scs_analysis/organisations.py
 src/scs_analysis/sample_aggregate.py
 src/scs_analysis/sample_average.py
 src/scs_analysis/sample_collator.py
-src/scs_analysis/sample_concentration.py
 src/scs_analysis/sample_distance.py
 src/scs_analysis/sample_duplicates.py
 src/scs_analysis/sample_error.py
+src/scs_analysis/sample_gas_concentration.py
+src/scs_analysis/sample_gas_density.py
 src/scs_analysis/sample_interval.py
 src/scs_analysis/sample_iso_8601.py
 src/scs_analysis/sample_low_pass.py
 src/scs_analysis/sample_max.py
 src/scs_analysis/sample_median.py
 src/scs_analysis/sample_midpoint.py
 src/scs_analysis/sample_min.py
@@ -79,18 +78,16 @@
 src/scs_analysis.egg-info/top_level.txt
 src/scs_analysis/chart/__init__.py
 src/scs_analysis/chart/chart.py
 src/scs_analysis/chart/histo_chart.py
 src/scs_analysis/chart/multi_chart.py
 src/scs_analysis/chart/single_chart.py
 src/scs_analysis/cmd/__init__.py
-src/scs_analysis/cmd/cmd_access_key.py
 src/scs_analysis/cmd/cmd_alert.py
 src/scs_analysis/cmd/cmd_alert_status.py
-src/scs_analysis/cmd/cmd_aws_api_auth.py
 src/scs_analysis/cmd/cmd_aws_byline.py
 src/scs_analysis/cmd/cmd_aws_client_auth.py
 src/scs_analysis/cmd/cmd_aws_topic_history.py
 src/scs_analysis/cmd/cmd_aws_topic_publisher.py
 src/scs_analysis/cmd/cmd_baseline.py
 src/scs_analysis/cmd/cmd_baseline_conf.py
 src/scs_analysis/cmd/cmd_cognito_devices.py
@@ -119,19 +116,20 @@
 src/scs_analysis/cmd/cmd_organisation_devices.py
 src/scs_analysis/cmd/cmd_organisation_path_roots.py
 src/scs_analysis/cmd/cmd_organisation_user_paths.py
 src/scs_analysis/cmd/cmd_organisation_users.py
 src/scs_analysis/cmd/cmd_organisations.py
 src/scs_analysis/cmd/cmd_sample_aggregate.py
 src/scs_analysis/cmd/cmd_sample_collator.py
-src/scs_analysis/cmd/cmd_sample_concentration.py
 src/scs_analysis/cmd/cmd_sample_distance.py
 src/scs_analysis/cmd/cmd_sample_duplicates.py
 src/scs_analysis/cmd/cmd_sample_error.py
 src/scs_analysis/cmd/cmd_sample_filter.py
+src/scs_analysis/cmd/cmd_sample_gas_concentration.py
+src/scs_analysis/cmd/cmd_sample_gas_density.py
 src/scs_analysis/cmd/cmd_sample_interval.py
 src/scs_analysis/cmd/cmd_sample_iso_8601.py
 src/scs_analysis/cmd/cmd_sample_low_pass.py
 src/scs_analysis/cmd/cmd_sample_median.py
 src/scs_analysis/cmd/cmd_sample_nullify.py
 src/scs_analysis/cmd/cmd_sample_paths.py
 src/scs_analysis/cmd/cmd_sample_record.py
```

