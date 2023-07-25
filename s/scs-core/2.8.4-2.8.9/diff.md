# Comparing `tmp/scs-core-2.8.4.tar.gz` & `tmp/scs-core-2.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-core-2.8.4.tar", last modified: Fri Jun 30 08:18:12 2023, max compression
+gzip compressed data, was "scs-core-2.8.9.tar", last modified: Tue Jul 25 12:39:02 2023, max compression
```

## Comparing `scs-core-2.8.4.tar` & `scs-core-2.8.9.tar`

### file list

```diff
@@ -1,419 +1,422 @@
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.373073 scs-core-2.8.4/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:27.000000 scs-core-2.8.4/LICENSE
--rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:27.000000 scs-core-2.8.4/MANIFEST.in
--rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-06-30 08:18:12.373073 scs-core-2.8.4/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)     1404 2023-06-26 09:33:48.000000 scs-core-2.8.4/README.md
--rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:27.000000 scs-core-2.8.4/README.rst
--rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-02-06 14:01:57.000000 scs-core-2.8.4/requirements.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-30 08:18:12.373073 scs-core-2.8.4/setup.cfg
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1996 2022-08-17 09:53:27.000000 scs-core-2.8.4/setup.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.289073 scs-core-2.8.4/src/
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.293073 scs-core-2.8.4/src/scs_core/
--rw-rw-r--   0 jade      (1002) jade      (1002)      183 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.293073 scs-core-2.8.4/src/scs_core/aqcsv/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.293073 scs-core-2.8.4/src/scs_core/aqcsv/conf/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/conf/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2617 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/conf/airnow_site_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1034 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/conf/airnow_uploader_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.293073 scs-core-2.8.4/src/scs_core/aqcsv/connector/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/connector/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10203 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/aqcsv/connector/airnow_mapping_task.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6655 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/connector/datum_mapping.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5042 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/connector/source_mapping.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.297073 scs-core-2.8.4/src/scs_core/aqcsv/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3750 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/data/aqcsv_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    13723 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/data/aqcsv_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3033 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/data/aqcsv_site.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.297073 scs-core-2.8.4/src/scs_core/aqcsv/specification/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2824 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/agency.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2728 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/country.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1163 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/country_iso.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1175 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/country_numeric.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9800 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/method.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3765 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/mpc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3453 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/parameter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2855 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/qc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3732 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/qualifier.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2879 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/unit.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.297073 scs-core-2.8.4/src/scs_core/aws/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.301073 scs-core-2.8.4/src/scs_core/aws/client/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/client/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3585 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/client/access_key.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2332 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/client/api_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2113 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/client/api_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1217 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/client/client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5103 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/client/client_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1281 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/client/device_control_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3294 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/client/email_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3361 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/client/monitor_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5891 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/aws/client/mqtt_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3856 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/client/rest_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.301073 scs-core-2.8.4/src/scs_core/aws/config/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/config/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      744 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/config/aws.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4471 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/aws/config/project.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.305073 scs-core-2.8.4/src/scs_core/aws/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    16736 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/data/alert.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9274 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/data/byline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1792 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/byline_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4640 2023-04-17 09:22:53.000000 scs-core-2.8.4/src/scs_core/aws/data/dataset.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3550 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/deployment.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5315 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/data/device_monitor_email_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    13432 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/data/device_monitor_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3313 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/data/device_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4032 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/aws/data/email_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2859 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/data/http_response.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/message.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1776 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/power_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1820 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/runtime_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1795 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/status_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2884 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/upload_interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1793 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/uptime_list.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.305073 scs-core-2.8.4/src/scs_core/aws/greengrass/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1998 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/aws_deployer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3017 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/aws_deployment_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9610 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/aws_group.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    16440 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/aws_group_configuration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11557 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/aws_identity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      440 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/gg_errors.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.313073 scs-core-2.8.4/src/scs_core/aws/manager/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/manager/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8285 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/alert_specification_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/alert_status_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3950 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/byline_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/configuration_check_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3256 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/configuration_check_requester.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10816 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/configuration_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2288 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/manager/device_monitor_specification_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/manager/device_monitor_status_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10307 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/dynamo_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3551 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/manager/ec2_message_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6470 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/lambda_bylines.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    15996 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/aws/manager/lambda_message_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    18045 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/aws/manager/s3_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4295 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/manager/sagemaker_model_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7802 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/manager/sagemaker_trial_manager.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.313073 scs-core-2.8.4/src/scs_core/aws/security/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/security/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/access_key_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5114 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_client_credentials.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7717 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_device.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1498 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_device_creator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3111 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_device_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1911 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_device_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10555 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_login_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2181 2023-04-17 09:22:53.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_membership.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2314 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_password_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11627 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_user.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3227 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_user_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3871 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_user_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/device_whitelist_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1947 2023-04-17 09:22:53.000000 scs-core-2.8.4/src/scs_core/aws/security/opr_membership.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    22905 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/organisation.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9601 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/organisation_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1752 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/path_filter.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.317073 scs-core-2.8.4/src/scs_core/client/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/client/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4470 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/client/http_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7463 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/client/http_exception.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      497 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/client/http_status.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2831 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/client/network.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1415 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/client/resource_unavailable_exception.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2638 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/client/sftp_client_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.317073 scs-core-2.8.4/src/scs_core/climate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1407 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/absolute_humidity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1418 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/icp10101_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3081 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/mpl115a2_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2911 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/mpl115a2_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2290 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/pressure_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2188 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/pressure_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3156 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/sht_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1844 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/sht_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.321073 scs-core-2.8.4/src/scs_core/comms/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/comms/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3125 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/comms/mqtt_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2395 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/comms/uds_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1552 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/comms/uds_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2350 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/comms/uds_server.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1614 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/comms/uds_writer.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.321073 scs-core-2.8.4/src/scs_core/control/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/control/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4918 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/control/command.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4896 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/control/control_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3792 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/control/control_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4737 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/control/control_receipt.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.325073 scs-core-2.8.4/src/scs_core/csv/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/csv/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1979 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/csv/csv_archive.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7484 2023-04-17 09:22:53.000000 scs-core-2.8.4/src/scs_core/csv/csv_dict.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5996 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/csv/csv_log.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8594 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/csv/csv_log_cursor_queue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8574 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/csv/csv_log_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8240 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/csv/csv_logger.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3323 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/csv/csv_logger_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5347 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/csv/csv_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4503 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/csv/csv_writer.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.333073 scs-core-2.8.4/src/scs_core/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4802 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/aggregate.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2050 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/data/array_dict.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2415 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/average.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2158 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/categorical_regression.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8964 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/data/checkpoint_generator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1008 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/crc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2092 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/crypt.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    19704 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/data/datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6448 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/data/datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2634 2023-04-17 09:22:53.000000 scs-core-2.8.4/src/scs_core/data/duplicates.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3809 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/data/histogram.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1747 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5951 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/join.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    14204 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/data/json.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3274 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/lin_regress.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5364 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/linear_regression.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/low_pass_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1628 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/median_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1892 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/min_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5682 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/data/model_delta.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8334 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/data/path_dict.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1291 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/precision.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3466 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/publication.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4181 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/data/queue_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8858 2023-04-17 09:22:53.000000 scs-core-2.8.4/src/scs_core/data/recurring_period.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1265 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/regression.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4348 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/data/rtc_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2249 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/data/sample_delta.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10713 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/stats.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1280 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/str.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7391 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/timedelta.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2185 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/tokens.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7456 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/data/topic_path.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.333073 scs-core-2.8.4/src/scs_core/display/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/display/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3786 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/display/display_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.333073 scs-core-2.8.4/src/scs_core/email/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/email/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2131 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/email/email_queue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2420 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/email/email_queue_manager.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.337073 scs-core-2.8.4/src/scs_core/estate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/estate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6202 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/estate/baseline_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    33022 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/estate/configuration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4521 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/estate/configuration_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5221 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/estate/git_pull.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3621 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/estate/git_pull_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6675 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/estate/mqtt_device_poller.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2450 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/estate/mqtt_peer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6563 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/estate/package_version.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.337073 scs-core-2.8.4/src/scs_core/exegesis/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/exegesis/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.337073 scs-core-2.8.4/src/scs_core/exegesis/gas/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/exegesis/gas/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      693 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/exegesis/gas/exegete_catalogue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1345 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/exegesis/gas/exegete_collection.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.337073 scs-core-2.8.4/src/scs_core/exegesis/particulate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/exegesis/particulate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      701 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/exegesis/particulate/exegete_catalogue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1353 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/exegesis/particulate/exegete_collection.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2248 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/exegesis/particulate/text.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.337073 scs-core-2.8.4/src/scs_core/gas/
--rw-rw-r--   0 jade      (1002) jade      (1002)      292 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.341073 scs-core-2.8.4/src/scs_core/gas/a4/
--rw-rw-r--   0 jade      (1002) jade      (1002)      410 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3700 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10274 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5667 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4131 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_v1.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3932 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_vA.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_vB.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_vC.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4662 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6990 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_temp_comp.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.341073 scs-core-2.8.4/src/scs_core/gas/afe/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/afe/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1542 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/afe/afe_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3242 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/afe/pt1000_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2445 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/afe/pt1000_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3600 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/afe_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11555 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/afe_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6742 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/afe_id.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.341073 scs-core-2.8.4/src/scs_core/gas/d4/
--rw-rw-r--   0 jade      (1002) jade      (1002)      130 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/d4/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3710 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/d4/d4_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3106 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/dsi_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4204 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/gas.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.341073 scs-core-2.8.4/src/scs_core/gas/isi/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/isi/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1373 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/isi/isi_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7366 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/gas/minimum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.345073 scs-core-2.8.4/src/scs_core/gas/ndir/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/ndir/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1777 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/ndir/ndir.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2723 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/ndir/ndir_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3350 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/ndir/ndir_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3649 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/ndir/ndir_version.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3065 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/ndir/ndir_voltages.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.345073 scs-core-2.8.4/src/scs_core/gas/pid/
--rw-rw-r--   0 jade      (1002) jade      (1002)      378 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/pid/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4106 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/pid/pid.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4196 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/pid/pid_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4028 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/pid/pid_calibrated_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3730 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/pid/pid_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3694 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/pid/pid_temp_comp.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.345073 scs-core-2.8.4/src/scs_core/gas/scd30/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/scd30/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2538 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/scd30/scd30_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2804 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/scd30/scd30_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2866 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/scd30/scd30_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3556 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/sensor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6165 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/gas/sensor_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3043 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/sensor_calib.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.345073 scs-core-2.8.4/src/scs_core/gps/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gps/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4077 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gps/gps_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.345073 scs-core-2.8.4/src/scs_core/interface/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/interface/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2271 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/interface/interface_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.345073 scs-core-2.8.4/src/scs_core/led/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/led/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      870 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/led/led.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2343 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/led/led_state.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.349073 scs-core-2.8.4/src/scs_core/location/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/location/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2992 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/location/timezone.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3708 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/location/timezone_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2379 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/location/timezone_offset.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.349073 scs-core-2.8.4/src/scs_core/model/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.349073 scs-core-2.8.4/src/scs_core/model/catalogue/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/catalogue/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11042 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/model/catalogue/model_compendium.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4774 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/catalogue/model_compendium_group.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5220 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/catalogue/term.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2038 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/catalogue/training_period.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.349073 scs-core-2.8.4/src/scs_core/model/gas/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3349 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1354 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/gas_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1545 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/gas_inference_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2932 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/gas_model_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.349073 scs-core-2.8.4/src/scs_core/model/gas/s1/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/s1/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2704 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/s1/gas_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3344 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/s1/s1_gas_inference_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.353073 scs-core-2.8.4/src/scs_core/model/gas/vB/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/vB/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2702 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/vB/gas_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3120 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/vB/vb_gas_inference_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.353073 scs-core-2.8.4/src/scs_core/model/gas/vE/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/vE/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3535 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/vE/gas_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4409 2022-10-03 10:46:58.000000 scs-core-2.8.4/src/scs_core/model/gas/vE/ve_gas_inference_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1218 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/vcal_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3488 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/model/model_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.353073 scs-core-2.8.4/src/scs_core/model/pmx/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/pmx/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1549 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/pmx/pmx_inference_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1609 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/pmx/pmx_model_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.353073 scs-core-2.8.4/src/scs_core/model/pmx/s1/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/pmx/s1/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2215 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/pmx/s1/pmx_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2051 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.353073 scs-core-2.8.4/src/scs_core/monitor/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/monitor/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1558 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/monitor/monitor_error.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1557 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/monitor/monitor_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1395 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/monitor/monitor_response.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.357073 scs-core-2.8.4/src/scs_core/particulate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/particulate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4558 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/particulate/opc_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5142 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/particulate/opc_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2610 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/particulate/opc_version.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2103 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/particulate/pmx_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6405 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/particulate/sps_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.357073 scs-core-2.8.4/src/scs_core/position/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4062 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/position/gps_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.361073 scs-core-2.8.4/src/scs_core/position/nmea/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1578 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gpdatetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4215 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gpgga.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gpgll.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gpgsa.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3850 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gpgsv.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2500 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gploc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4056 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gprmc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1318 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gptime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gpvtg.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2535 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/nmea_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      782 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/nmea_sentence.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3884 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/position/position.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.361073 scs-core-2.8.4/src/scs_core/psu/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/psu/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2320 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/psu/psu.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4543 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/psu/psu_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1733 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/psu/psu_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1728 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/psu/psu_uptime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5663 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/psu/psu_version.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.361073 scs-core-2.8.4/src/scs_core/sample/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sample/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3421 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sample/climate_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    12029 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/sample/configuration_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5262 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sample/gases_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3724 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sample/particulates_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2872 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sample/pressure_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4034 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sample/sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5876 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sample/status_sample.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.365073 scs-core-2.8.4/src/scs_core/sampler/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sampler/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1263 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sampler/sampler.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.365073 scs-core-2.8.4/src/scs_core/sync/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sync/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2168 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sync/interval_timer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1681 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sync/line_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      606 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sync/runner.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6819 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/sync/schedule.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1811 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sync/synchronised_process.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1724 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sync/timed_runner.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.373073 scs-core-2.8.4/src/scs_core/sys/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1791 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/sys/command.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4443 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/disk_usage.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/disk_volume.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2399 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/eeprom_image.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2622 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/exception_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6991 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/sys/filesystem.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1994 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/ipv4_address.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1167 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/sys/logging.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1297 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sys/memory.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    17409 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/sys/modem.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5733 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/network.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5974 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/sys/node.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3851 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/persistence_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2318 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/sys/platform.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      834 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/process_comms.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4919 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/sys/ps_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3284 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/serial.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2405 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/shared_secret.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2506 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/signalled_exit.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2244 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/subprocess.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5730 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/sys/system_id.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2013 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/sys/system_temp.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6610 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/sys/tail.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1409 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/timeout.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1192 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sys/timer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1784 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/trace_entry.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5602 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/sys/uptime_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.293073 scs-core-2.8.4/src/scs_core.egg-info/
--rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-06-30 08:18:12.000000 scs-core-2.8.4/src/scs_core.egg-info/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)    13337 2023-06-30 08:18:12.000000 scs-core-2.8.4/src/scs_core.egg-info/SOURCES.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-30 08:18:12.000000 scs-core-2.8.4/src/scs_core.egg-info/dependency_links.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-06-30 08:18:12.000000 scs-core-2.8.4/src/scs_core.egg-info/requires.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        9 2023-06-30 08:18:12.000000 scs-core-2.8.4/src/scs_core.egg-info/top_level.txt
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.367947 scs-core-2.8.9/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:27.000000 scs-core-2.8.9/LICENSE
+-rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:27.000000 scs-core-2.8.9/MANIFEST.in
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-07-25 12:39:02.367947 scs-core-2.8.9/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1404 2023-06-26 09:33:48.000000 scs-core-2.8.9/README.md
+-rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:27.000000 scs-core-2.8.9/README.rst
+-rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-02-06 14:01:57.000000 scs-core-2.8.9/requirements.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-07-25 12:39:02.367947 scs-core-2.8.9/setup.cfg
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1996 2022-08-17 09:53:27.000000 scs-core-2.8.9/setup.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.335947 scs-core-2.8.9/src/
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.339947 scs-core-2.8.9/src/scs_core/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      183 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.339947 scs-core-2.8.9/src/scs_core/aqcsv/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.339947 scs-core-2.8.9/src/scs_core/aqcsv/conf/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/conf/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2617 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/conf/airnow_site_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1034 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/conf/airnow_uploader_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.343947 scs-core-2.8.9/src/scs_core/aqcsv/connector/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/connector/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10203 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/aqcsv/connector/airnow_mapping_task.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6655 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/connector/datum_mapping.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5042 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/connector/source_mapping.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.343947 scs-core-2.8.9/src/scs_core/aqcsv/data/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/data/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3750 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/data/aqcsv_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    13723 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/data/aqcsv_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3033 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/data/aqcsv_site.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.343947 scs-core-2.8.9/src/scs_core/aqcsv/specification/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/specification/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2824 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/specification/agency.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2728 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/specification/country.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1163 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/specification/country_iso.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1175 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/specification/country_numeric.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9800 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/specification/method.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3765 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/specification/mpc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3453 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/specification/parameter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2855 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/specification/qc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3732 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/specification/qualifier.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2879 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aqcsv/specification/unit.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.343947 scs-core-2.8.9/src/scs_core/aws/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.343947 scs-core-2.8.9/src/scs_core/aws/client/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/client/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3585 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/client/access_key.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2332 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/client/api_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2113 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/client/api_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1217 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/client/client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5103 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/client/client_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1281 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/client/device_control_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3294 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/client/email_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3361 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/client/monitor_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5891 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/aws/client/mqtt_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3821 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/client/rest_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.343947 scs-core-2.8.9/src/scs_core/aws/config/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/config/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      744 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/config/aws.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4471 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/aws/config/project.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.347947 scs-core-2.8.9/src/scs_core/aws/data/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/data/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    17681 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/data/alert.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9655 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/data/byline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1792 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/data/byline_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4640 2023-04-17 09:22:53.000000 scs-core-2.8.9/src/scs_core/aws/data/dataset.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3550 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/data/deployment.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5315 2023-06-30 08:17:13.000000 scs-core-2.8.9/src/scs_core/aws/data/device_monitor_email_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    13437 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/data/device_monitor_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8201 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/data/device_monitor_specification.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2859 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/data/http_response.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/data/message.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1776 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/data/power_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1820 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/data/runtime_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1795 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/data/status_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2884 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/data/upload_interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1793 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/data/uptime_list.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.347947 scs-core-2.8.9/src/scs_core/aws/greengrass/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/greengrass/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1998 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/greengrass/aws_deployer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3017 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/aws/greengrass/aws_deployment_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9610 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/greengrass/aws_group.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    16440 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/aws/greengrass/aws_group_configuration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11557 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/greengrass/aws_identity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      440 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/greengrass/gg_errors.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.347947 scs-core-2.8.9/src/scs_core/aws/manager/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/manager/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8285 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/manager/alert_specification_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/manager/alert_status_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4091 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/manager/byline_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/manager/configuration_check_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3256 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/manager/configuration_check_requester.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10816 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/manager/configuration_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2745 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/manager/device_monitor_specification_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1495 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/manager/device_monitor_status_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10307 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/manager/dynamo_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3527 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/manager/ec2_message_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6470 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/manager/lambda_bylines.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    15980 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/manager/lambda_message_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    18045 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/aws/manager/s3_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4295 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/manager/sagemaker_model_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7802 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/manager/sagemaker_trial_manager.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.347947 scs-core-2.8.9/src/scs_core/aws/security/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/aws/security/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/security/access_key_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5114 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/security/cognito_client_credentials.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7792 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/security/cognito_device.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1843 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/security/cognito_device_creator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3111 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/security/cognito_device_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2357 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/security/cognito_device_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10555 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/security/cognito_login_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2181 2023-04-17 09:22:53.000000 scs-core-2.8.9/src/scs_core/aws/security/cognito_membership.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2314 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/security/cognito_password_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11627 2023-06-30 08:17:13.000000 scs-core-2.8.9/src/scs_core/aws/security/cognito_user.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3227 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/security/cognito_user_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3871 2023-06-30 08:17:13.000000 scs-core-2.8.9/src/scs_core/aws/security/cognito_user_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/security/device_whitelist_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1947 2023-04-17 09:22:53.000000 scs-core-2.8.9/src/scs_core/aws/security/opr_membership.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    22736 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/aws/security/organisation.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9601 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/security/organisation_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1752 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/aws/security/path_filter.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.351947 scs-core-2.8.9/src/scs_core/client/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/client/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4395 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/client/http_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7463 2023-06-30 08:17:13.000000 scs-core-2.8.9/src/scs_core/client/http_exception.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      497 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/client/http_status.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2831 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/client/network.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1415 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/client/resource_unavailable_exception.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2638 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/client/sftp_client_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.351947 scs-core-2.8.9/src/scs_core/climate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/climate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1407 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/climate/absolute_humidity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1418 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/climate/icp10101_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3081 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/climate/mpl115a2_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2911 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/climate/mpl115a2_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2290 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/climate/pressure_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2188 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/climate/pressure_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3156 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/climate/sht_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1844 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/climate/sht_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.351947 scs-core-2.8.9/src/scs_core/comms/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/comms/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3125 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/comms/mqtt_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2395 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/comms/uds_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1552 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/comms/uds_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2350 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/comms/uds_server.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1614 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/comms/uds_writer.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.351947 scs-core-2.8.9/src/scs_core/control/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/control/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4918 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/control/command.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4896 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/control/control_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3792 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/control/control_handler.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4737 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/control/control_receipt.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.351947 scs-core-2.8.9/src/scs_core/csv/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/csv/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1979 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/csv/csv_archive.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7484 2023-04-17 09:22:53.000000 scs-core-2.8.9/src/scs_core/csv/csv_dict.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5996 2022-09-20 10:07:36.000000 scs-core-2.8.9/src/scs_core/csv/csv_log.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8594 2022-09-20 10:07:36.000000 scs-core-2.8.9/src/scs_core/csv/csv_log_cursor_queue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9036 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/csv/csv_log_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8240 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/csv/csv_logger.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4243 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/csv/csv_logger_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5347 2022-09-20 10:07:36.000000 scs-core-2.8.9/src/scs_core/csv/csv_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4503 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/csv/csv_writer.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.355947 scs-core-2.8.9/src/scs_core/data/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4802 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/aggregate.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2050 2023-06-30 08:17:13.000000 scs-core-2.8.9/src/scs_core/data/array_dict.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2415 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/average.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2158 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/categorical_regression.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8964 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/data/checkpoint_generator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1008 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/crc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2092 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/crypt.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    20116 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/data/datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6448 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/data/datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6560 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/data/diurnal_period.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2634 2023-04-17 09:22:53.000000 scs-core-2.8.9/src/scs_core/data/duplicates.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3809 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/data/histogram.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1747 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5951 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/join.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    14204 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/data/json.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3274 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/lin_regress.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5364 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/linear_regression.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/low_pass_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1628 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/median_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1892 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/min_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5682 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/data/model_delta.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8334 2022-09-20 10:07:36.000000 scs-core-2.8.9/src/scs_core/data/path_dict.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1904 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/data/period.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1291 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/precision.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3466 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/publication.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4181 2022-09-20 10:07:36.000000 scs-core-2.8.9/src/scs_core/data/queue_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10319 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/data/recurring_period.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1265 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/regression.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4348 2022-09-20 10:07:36.000000 scs-core-2.8.9/src/scs_core/data/rtc_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2249 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/data/sample_delta.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10713 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/stats.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1280 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/str.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8116 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/data/timedelta.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2185 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/data/tokens.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7456 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/data/topic_path.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.355947 scs-core-2.8.9/src/scs_core/display/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/display/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3786 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/display/display_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.355947 scs-core-2.8.9/src/scs_core/email/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/email/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2131 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/email/email_queue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2420 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/email/email_queue_manager.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.355947 scs-core-2.8.9/src/scs_core/estate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/estate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5414 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/estate/baseline_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6211 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/estate/baseline_conf_old.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    33022 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/estate/configuration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4521 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/estate/configuration_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5221 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/estate/git_pull.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3621 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/estate/git_pull_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6675 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/estate/mqtt_device_poller.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2450 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/estate/mqtt_peer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6563 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/estate/package_version.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.355947 scs-core-2.8.9/src/scs_core/exegesis/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/exegesis/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.355947 scs-core-2.8.9/src/scs_core/exegesis/gas/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/exegesis/gas/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      693 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/exegesis/gas/exegete_catalogue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1345 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/exegesis/gas/exegete_collection.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.355947 scs-core-2.8.9/src/scs_core/exegesis/particulate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/exegesis/particulate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      701 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/exegesis/particulate/exegete_catalogue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1353 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/exegesis/particulate/exegete_collection.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2248 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/exegesis/particulate/text.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/gas/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      292 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/gas/a4/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      410 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/a4/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3700 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/gas/a4/a4.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10274 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/gas/a4/a4_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5667 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/a4/a4_calibrated_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4131 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/a4/a4_calibrated_datum_v1.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3932 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/a4/a4_calibrated_datum_vA.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/a4/a4_calibrated_datum_vB.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/a4/a4_calibrated_datum_vC.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4662 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/a4/a4_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6990 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/a4/a4_temp_comp.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/gas/afe/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/afe/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1542 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/afe/afe_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3242 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/afe/pt1000_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2445 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/afe/pt1000_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3600 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/afe_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11550 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/gas/afe_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6742 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/afe_id.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/gas/d4/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      130 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/d4/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3710 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/d4/d4_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3106 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/gas/dsi_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4351 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/gas/gas.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/gas/isi/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/isi/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1373 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/isi/isi_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7366 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/gas/minimum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/gas/ndir/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/ndir/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1777 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/ndir/ndir.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2723 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/ndir/ndir_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3350 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/ndir/ndir_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3649 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/ndir/ndir_version.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3065 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/ndir/ndir_voltages.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/gas/pid/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      378 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/pid/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4106 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/pid/pid.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4196 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/gas/pid/pid_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4028 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/pid/pid_calibrated_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3730 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/pid/pid_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3694 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/pid/pid_temp_comp.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/gas/scd30/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/scd30/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2538 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/scd30/scd30_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2804 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/scd30/scd30_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2866 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gas/scd30/scd30_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3556 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/gas/sensor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6165 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/gas/sensor_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3043 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/gas/sensor_calib.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/gps/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gps/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4077 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/gps/gps_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/interface/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/interface/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2271 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/interface/interface_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/led/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/led/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      870 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/led/led.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2343 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/led/led_state.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/location/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/location/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2992 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/location/timezone.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3708 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/location/timezone_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2379 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/location/timezone_offset.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.359947 scs-core-2.8.9/src/scs_core/model/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.363947 scs-core-2.8.9/src/scs_core/model/catalogue/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/catalogue/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11042 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/model/catalogue/model_compendium.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4774 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/catalogue/model_compendium_group.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5220 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/catalogue/term.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2038 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/catalogue/training_period.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.363947 scs-core-2.8.9/src/scs_core/model/gas/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3349 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1354 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/gas_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1545 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/gas_inference_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2932 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/gas_model_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.363947 scs-core-2.8.9/src/scs_core/model/gas/s1/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/s1/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2704 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/s1/gas_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3344 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/s1/s1_gas_inference_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.363947 scs-core-2.8.9/src/scs_core/model/gas/vB/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/vB/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2702 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/vB/gas_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3120 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/vB/vb_gas_inference_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.363947 scs-core-2.8.9/src/scs_core/model/gas/vE/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/vE/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3535 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/vE/gas_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4409 2022-10-03 10:46:58.000000 scs-core-2.8.9/src/scs_core/model/gas/vE/ve_gas_inference_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1218 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/gas/vcal_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3488 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/model/model_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.363947 scs-core-2.8.9/src/scs_core/model/pmx/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/pmx/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1549 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/pmx/pmx_inference_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1609 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/pmx/pmx_model_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.363947 scs-core-2.8.9/src/scs_core/model/pmx/s1/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/pmx/s1/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2215 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/pmx/s1/pmx_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2051 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.363947 scs-core-2.8.9/src/scs_core/monitor/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/monitor/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1558 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/monitor/monitor_error.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1557 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/monitor/monitor_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1395 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/monitor/monitor_response.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.363947 scs-core-2.8.9/src/scs_core/particulate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/particulate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5045 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/particulate/opc_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5142 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/particulate/opc_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2610 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/particulate/opc_version.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2103 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/particulate/pmx_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6405 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/particulate/sps_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.363947 scs-core-2.8.9/src/scs_core/position/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4062 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/position/gps_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.363947 scs-core-2.8.9/src/scs_core/position/nmea/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/nmea/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1578 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/nmea/gpdatetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4215 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/nmea/gpgga.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/nmea/gpgll.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/nmea/gpgsa.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3850 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/nmea/gpgsv.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2500 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/nmea/gploc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4056 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/nmea/gprmc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1318 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/nmea/gptime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/nmea/gpvtg.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2535 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/nmea/nmea_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      782 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/position/nmea/nmea_sentence.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3884 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/position/position.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.367947 scs-core-2.8.9/src/scs_core/psu/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/psu/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2320 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/psu/psu.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4543 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/psu/psu_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1733 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/psu/psu_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1728 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/psu/psu_uptime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5663 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/psu/psu_version.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.367947 scs-core-2.8.9/src/scs_core/sample/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sample/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3421 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/sample/climate_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    12029 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/sample/configuration_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5262 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/sample/gases_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3724 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/sample/particulates_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2872 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/sample/pressure_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4034 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/sample/sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5876 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/sample/status_sample.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.367947 scs-core-2.8.9/src/scs_core/sampler/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sampler/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1263 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sampler/sampler.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.367947 scs-core-2.8.9/src/scs_core/sync/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sync/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2168 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sync/interval_timer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1681 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sync/line_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      606 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sync/runner.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6819 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/sync/schedule.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1811 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sync/synchronised_process.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1724 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sync/timed_runner.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.367947 scs-core-2.8.9/src/scs_core/sys/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2827 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/sys/command.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4443 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/disk_usage.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/disk_volume.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2399 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/eeprom_image.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2622 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/exception_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6991 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/sys/filesystem.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2381 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/sys/hostname.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1994 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/ipv4_address.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1167 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/sys/logging.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1297 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/sys/memory.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    17409 2022-09-20 10:07:36.000000 scs-core-2.8.9/src/scs_core/sys/modem.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5733 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/network.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6040 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/sys/node.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3851 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/persistence_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2318 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/sys/platform.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      834 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/process_comms.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4919 2022-09-20 10:07:36.000000 scs-core-2.8.9/src/scs_core/sys/ps_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3284 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/serial.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2405 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/shared_secret.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2506 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/signalled_exit.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2244 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/subprocess.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5882 2023-07-25 12:37:52.000000 scs-core-2.8.9/src/scs_core/sys/system_id.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2013 2023-06-26 09:33:48.000000 scs-core-2.8.9/src/scs_core/sys/system_temp.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6610 2023-03-20 10:12:25.000000 scs-core-2.8.9/src/scs_core/sys/tail.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1409 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/timeout.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1192 2023-02-06 14:01:57.000000 scs-core-2.8.9/src/scs_core/sys/timer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1784 2022-08-17 09:53:27.000000 scs-core-2.8.9/src/scs_core/sys/trace_entry.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5602 2022-09-20 10:07:36.000000 scs-core-2.8.9/src/scs_core/sys/uptime_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-07-25 12:39:02.339947 scs-core-2.8.9/src/scs_core.egg-info/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-07-25 12:39:02.000000 scs-core-2.8.9/src/scs_core.egg-info/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)    13450 2023-07-25 12:39:02.000000 scs-core-2.8.9/src/scs_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-07-25 12:39:02.000000 scs-core-2.8.9/src/scs_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-07-25 12:39:02.000000 scs-core-2.8.9/src/scs_core.egg-info/requires.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        9 2023-07-25 12:39:02.000000 scs-core-2.8.9/src/scs_core.egg-info/top_level.txt
```

### Comparing `scs-core-2.8.4/LICENSE` & `scs-core-2.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/PKG-INFO` & `scs-core-2.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-core
-Version: 2.8.4
+Version: 2.8.9
 Summary: The root of all South Coast Science environmental monitoring applications.
 Home-page: https://github.com/south-coast-science/scs_core
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scs-core-2.8.4/README.md` & `scs-core-2.8.9/README.md`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/setup.py` & `scs-core-2.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/conf/airnow_site_conf.py` & `scs-core-2.8.9/src/scs_core/aqcsv/conf/airnow_site_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/conf/airnow_uploader_conf.py` & `scs-core-2.8.9/src/scs_core/aqcsv/conf/airnow_uploader_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/connector/airnow_mapping_task.py` & `scs-core-2.8.9/src/scs_core/aqcsv/connector/airnow_mapping_task.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/connector/datum_mapping.py` & `scs-core-2.8.9/src/scs_core/aqcsv/connector/datum_mapping.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/connector/source_mapping.py` & `scs-core-2.8.9/src/scs_core/aqcsv/connector/source_mapping.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/data/aqcsv_datetime.py` & `scs-core-2.8.9/src/scs_core/aqcsv/data/aqcsv_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/data/aqcsv_record.py` & `scs-core-2.8.9/src/scs_core/aqcsv/data/aqcsv_record.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/data/aqcsv_site.py` & `scs-core-2.8.9/src/scs_core/aqcsv/data/aqcsv_site.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/specification/agency.py` & `scs-core-2.8.9/src/scs_core/aqcsv/specification/agency.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/specification/country.py` & `scs-core-2.8.9/src/scs_core/aqcsv/specification/country.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/specification/country_iso.py` & `scs-core-2.8.9/src/scs_core/aqcsv/specification/country_iso.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/specification/country_numeric.py` & `scs-core-2.8.9/src/scs_core/aqcsv/specification/country_numeric.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/specification/method.py` & `scs-core-2.8.9/src/scs_core/aqcsv/specification/method.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/specification/mpc.py` & `scs-core-2.8.9/src/scs_core/aqcsv/specification/mpc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/specification/parameter.py` & `scs-core-2.8.9/src/scs_core/aqcsv/specification/parameter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/specification/qc.py` & `scs-core-2.8.9/src/scs_core/aqcsv/specification/qc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/specification/qualifier.py` & `scs-core-2.8.9/src/scs_core/aqcsv/specification/qualifier.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aqcsv/specification/unit.py` & `scs-core-2.8.9/src/scs_core/aqcsv/specification/unit.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/client/access_key.py` & `scs-core-2.8.9/src/scs_core/aws/client/access_key.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/client/api_auth.py` & `scs-core-2.8.9/src/scs_core/aws/client/api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/client/api_client.py` & `scs-core-2.8.9/src/scs_core/aws/client/api_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/client/client.py` & `scs-core-2.8.9/src/scs_core/aws/client/client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/client/client_auth.py` & `scs-core-2.8.9/src/scs_core/aws/client/client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/client/device_control_client.py` & `scs-core-2.8.9/src/scs_core/aws/client/device_control_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/client/email_client.py` & `scs-core-2.8.9/src/scs_core/aws/client/email_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/client/monitor_auth.py` & `scs-core-2.8.9/src/scs_core/aws/client/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/client/mqtt_client.py` & `scs-core-2.8.9/src/scs_core/aws/client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/client/rest_client.py` & `scs-core-2.8.9/src/scs_core/aws/client/rest_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,31 +24,32 @@
 # --------------------------------------------------------------------------------------------------------------------
 
 class RESTClient(object):
     """
     classdocs
     """
 
+    __HOST = "aws.southcoastscience.com"
+
     __HEADER_ACCEPT = "application/json"
-    __HEADER_AUTHORIZATION = "api-key "
+    __HEADER_AUTHORIZATION = "api-key"
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, auth):
+    def __init__(self):
         """
         Constructor
         """
         self.__http_client = HTTPClient()
-        self.__auth = auth
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def connect(self):
-        self.__http_client.connect(self.__auth.endpoint)
+        self.__http_client.connect(self.__HOST)
 
 
     def close(self):
         self.__http_client.close()
 
 
     # ----------------------------------------------------------------------------------------------------------------
@@ -120,15 +121,15 @@
         return response
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def __headers(self):
-        return {"Accept": RESTClient.__HEADER_ACCEPT,
-                "Authorization": RESTClient.__HEADER_AUTHORIZATION + self.__auth.api_key}
+        return {"Accept": self.__HEADER_ACCEPT,
+                "Authorization": self.__HEADER_AUTHORIZATION}
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "RESTClient:{auth:%s}" % self.__auth
+        return "RESTClient:{host:%s}" % self.__HOST
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/config/aws.py` & `scs-core-2.8.9/src/scs_core/aws/config/aws.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/config/project.py` & `scs-core-2.8.9/src/scs_core/aws/config/project.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/alert.py` & `scs-core-2.8.9/src/scs_core/aws/data/alert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 """
 Created on 17 Jun 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-Alert example:
-{"id": 88, "description": "warm", "topic": "south-coast-science-dev/development/loc/1/climate", "field": "val.tmp",
-"lower-threshold": null, "upper-threshold": 30.0, "alert-on-none": false,
-"aggregation-period": {"interval": 1, "units": "M"}, "test-interval": null, "json-message": false,
+Alert example (recurring):
+{"id": null, "description": "my description", "topic": "my/topic",
+"field": "my.field", "lower-threshold": null,  "upper-threshold": 100.0, "alert-on-none": true,
+"aggregation-period": {"type": "recurring", "interval": 1, "units": "D", "timezone": "Europe/London"},
+"test-interval": {"type": "recurring", "interval": 1, "units": "M"}, "json-message": true,
 "creator-email-address": "bruno.beloff@southcoastscience.com", "to": "bruno.beloff@southcoastscience.com",
-"cc-list": ["bbeloff@me.com", "jadempage@outlook.com"], "suspended": false}
+"cc-list": ["bbeloff@me.com", "hhopton@me.com"], "suspended": false}
+
+Alert example (diurnal):
+{"id": 107, "description": "be2-3-nightime-test", "topic": "south-coast-science-dev/development/loc/1/climate",
+"field": "val.tmp", "lower-threshold": null, "upper-threshold": 10.0, "alert-on-none": true,
+"aggregation-period": {"type": "diurnal", "start": "16:00:00", "end": "08:00:00", "timezone": "Europe/London"},
+"test-interval": null, "json-message": false, "creator-email-address": "production@southcoastscience.com",
+"to": "bruno.beloff@southcoastscience.com", "cc-list": ["jade.page@southcoastscience.com"], "suspended": false}
 
 AlertStatus example:
 {"id": 77, "rec": "2021-09-07T11:40:00Z", "cause": "OK", "val": 589.6}
 
 https://martinstapel.com/how-to-autoincrement-in-dynamo-db-if-you-really-need-to/
 https://stackoverflow.com/questions/37072341/how-to-use-auto-increment-for-primary-key-id-in-dynamodb
 """
 
 from collections import OrderedDict
 
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.datum import Datum
+from scs_core.data.diurnal_period import DiurnalPeriod
 from scs_core.data.json import JSONable, JSONify
 from scs_core.data.recurring_period import RecurringPeriod
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class AlertStatus(JSONable):
@@ -157,15 +166,19 @@
         topic = jdict.get('topic')
         field = jdict.get('field')
 
         lower_threshold = jdict.get('lower-threshold')
         upper_threshold = jdict.get('upper-threshold')
         alert_on_none = jdict.get('alert-on-none')
 
-        aggregation_period = RecurringPeriod.construct_from_jdict(jdict.get('aggregation-period'))
+        agg_jdict = jdict.get('aggregation-period')
+
+        aggregation_period = DiurnalPeriod.construct_from_jdict(agg_jdict) \
+            if agg_jdict.get('type') == DiurnalPeriod.type() else RecurringPeriod.construct_from_jdict(agg_jdict)
+
         test_interval = RecurringPeriod.construct_from_jdict(jdict.get('test-interval'))
 
         json_message = jdict.get('json-message', False)
 
         creator_email_address = jdict.get('creator-email-address')
 
         to = jdict.get('to')
@@ -236,14 +249,18 @@
 
         if self.to > other.to:
             return False
 
         return False
 
 
+    def __contains__(self, email):
+        return email == self.creator_email_address or email == self.to or email in self.cc_list
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
         if self.topic is None or self.field is None or self.aggregation_period is None or self.to is None:
             return False
 
         if not self.has_trigger():
@@ -318,18 +335,20 @@
         #     self.aggregation_period.cron(minutes_offset)
 
 
     def timedelta(self):
         return self.aggregation_period.timedelta()
 
 
+    def start_datetime(self, origin: LocalizedDatetime):
+        return self.aggregation_period.start_datetime(origin)
+
+
     def end_datetime(self, origin: LocalizedDatetime):
         return self.aggregation_period.end_datetime(origin)
-        # return self.test_interval.end_datetime(origin) if self.test_interval else \
-        #     self.aggregation_period.end_datetime(origin)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def add_cc(self, cc):
         self.__cc_list.add(cc)
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/byline.py` & `scs-core-2.8.9/src/scs_core/aws/data/byline.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 \"tag\": \"scs-bgx-401\"}"}
 """
 
 import json
 
 from collections import OrderedDict
 
+from scs_core.aws.security.cognito_device import CognitoDeviceCredentials
+
 from scs_core.data.array_dict import ArrayDict
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.json import JSONable
 from scs_core.data.topic_path import TopicPath
 
 from scs_core.sys.logging import Logging
 
@@ -152,26 +154,31 @@
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_jdict(cls, jdict, excluded=None, skeleton=False):
+    def construct_from_jdict(cls, jdict, excluded=None, strict_tags=False, skeleton=False):
         if not jdict:
             return cls({}) if skeleton else None
 
         # bylines...
         bylines = []
 
         for byline_jdict in jdict:
             byline = Byline.construct_from_jdict(byline_jdict)
 
-            if not excluded or not byline.topic.endswith(excluded):
-                bylines.append(byline)
+            if excluded is not None and byline.topic.endswith(excluded):
+                continue
+
+            if strict_tags and not CognitoDeviceCredentials.is_valid_tag(byline.device):
+                continue
+
+            bylines.append(byline)
 
         # device_bylines...
         device_bylines = ArrayDict([(byline.device, byline) for byline in sorted(bylines)])
 
         return cls(device_bylines)
 
 
@@ -212,22 +219,22 @@
         return topic
 
 
     def latest_pub(self):
         if not self.bylines:
             return None
 
-        return max([byline.pub for byline in self.bylines if byline.pub is not None])
+        return max([byline.pub for byline in self.bylines if byline.pub is not None], default=None)
 
 
     def latest_rec(self):
         if not self.bylines:
             return None
 
-        return max([byline.rec for byline in self.bylines if byline.rec is not None])
+        return max([byline.rec for byline in self.bylines if byline.rec is not None], default=None)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         return tuple(byline.as_json() for byline in self.bylines)       # matches the structure of the API response
 
@@ -289,14 +296,18 @@
         super().__init__(device_bylines)
 
         self.__logger = Logging.getLogger()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
+    def device_byline_group(self, device):
+        return DeviceBylineGroup({device: self._device_bylines[device]})
+
+
     def bylines_for_device(self, device):
         return self._device_bylines[device]
 
 
     def topic_roots(self):
         topic_roots = set()
         for device_tag, bylines in self._device_bylines.items():
@@ -311,9 +322,9 @@
         return sorted(topic_roots)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def devices(self):
-        return tuple(self._device_bylines.keys())
+        return list(self._device_bylines.keys())
         # return self._device_bylines.keys()
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/byline_list.py` & `scs-core-2.8.9/src/scs_core/aws/data/byline_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/dataset.py` & `scs-core-2.8.9/src/scs_core/aws/data/dataset.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/deployment.py` & `scs-core-2.8.9/src/scs_core/aws/data/deployment.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/device_monitor_email_list.py` & `scs-core-2.8.9/src/scs_core/aws/data/device_monitor_email_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/device_monitor_report.py` & `scs-core-2.8.9/src/scs_core/aws/data/device_monitor_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
-        period = Timedelta.construct_from_jdict(jdict.get('since'))
+        period = Timedelta.construct_from_jdict(jdict.get('period'))
 
         return cls(period)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, period: Timedelta):
@@ -379,15 +379,15 @@
         return cls.aws_dir(), cls.__FILENAME
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict, skeleton=False):
-        if not jdict:
+        if jdict is None:
             return None
 
         device_dict = {device_tag: DeviceReport.construct_from_jdict(report_jdict)
                        for device_tag, report_jdict in jdict.items()}
 
         return cls(device_dict)
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/http_response.py` & `scs-core-2.8.9/src/scs_core/aws/data/http_response.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/message.py` & `scs-core-2.8.9/src/scs_core/aws/data/message.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/power_list.py` & `scs-core-2.8.9/src/scs_core/aws/data/power_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/runtime_record.py` & `scs-core-2.8.9/src/scs_core/aws/data/runtime_record.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/status_list.py` & `scs-core-2.8.9/src/scs_core/aws/data/status_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/upload_interval.py` & `scs-core-2.8.9/src/scs_core/aws/data/upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/data/uptime_list.py` & `scs-core-2.8.9/src/scs_core/aws/data/uptime_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/greengrass/aws_deployer.py` & `scs-core-2.8.9/src/scs_core/aws/greengrass/aws_deployer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/greengrass/aws_deployment_reporter.py` & `scs-core-2.8.9/src/scs_core/aws/greengrass/aws_deployment_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/greengrass/aws_group.py` & `scs-core-2.8.9/src/scs_core/aws/greengrass/aws_group.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/greengrass/aws_group_configuration.py` & `scs-core-2.8.9/src/scs_core/aws/greengrass/aws_group_configuration.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/greengrass/aws_identity.py` & `scs-core-2.8.9/src/scs_core/aws/greengrass/aws_identity.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/alert_specification_manager.py` & `scs-core-2.8.9/src/scs_core/aws/manager/alert_specification_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/alert_status_manager.py` & `scs-core-2.8.9/src/scs_core/aws/manager/alert_status_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/byline_manager.py` & `scs-core-2.8.9/src/scs_core/aws/manager/byline_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
             if latest_byline is None or latest_byline.rec < byline.rec:
                 latest_byline = byline
 
         return latest_byline
 
 
-    def find_bylines(self, excluded=None):
+    def find_bylines(self, excluded=None, strict_tags=False):
         params = {}
         items_jdict = []
 
         while True:
             response = self._http_client.get(self.__URL, params=params)
             jdict = response.json()
 
@@ -78,27 +78,28 @@
             if jdict.get('next') is None:
                 break
 
             next_url = urlparse(jdict.get('next'))
             params = parse_qs(next_url.query)
 
         # bylines...
-        return TopicBylineGroup.construct_from_jdict(items_jdict, excluded=excluded, skeleton=True)
+        return TopicBylineGroup.construct_from_jdict(items_jdict, excluded=excluded, strict_tags=strict_tags,
+                                                     skeleton=True)
 
 
-    def find_bylines_for_topic(self, topic, excluded=None):
+    def find_bylines_for_topic(self, topic, excluded=None, strict_tags=False):
         params = {self.__TOPIC: topic}
 
         response = self._http_client.get(self.__URL, params=params)
         self._check_response(response)
 
         jdict = response.json()
 
         # bylines...
-        return TopicBylineGroup.construct_from_jdict(jdict, excluded=excluded, skeleton=True)
+        return TopicBylineGroup.construct_from_jdict(jdict, excluded=excluded, strict_tags=strict_tags, skeleton=True)
 
 
     def find_bylines_for_device(self, device, excluded=None):
         params = {self.__DEVICE: device}
 
         response = self._http_client.get(self.__URL, params=params)
         self._check_response(response)
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/configuration_check_finder.py` & `scs-core-2.8.9/src/scs_core/aws/manager/configuration_check_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/configuration_check_requester.py` & `scs-core-2.8.9/src/scs_core/aws/manager/configuration_check_requester.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/configuration_finder.py` & `scs-core-2.8.9/src/scs_core/aws/manager/configuration_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/device_monitor_specification_manager.py` & `scs-core-2.8.9/src/scs_core/aws/manager/device_monitor_specification_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 Created on 17 Jun 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 from scs_core.aws.client.api_client import APIClient
-
-from scs_core.aws.data.device_monitor_email_list import DeviceMonitorEmailList
+from scs_core.aws.data.device_monitor_specification import DeviceMonitorSpecification, DeviceMonitorSpecificationList
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class DeviceMonitorSpecificationManager(APIClient):
     """
     classdocs
@@ -32,38 +31,50 @@
             'device_tag': device_tag,
             'exact': exact
         }
 
         response = self._http_client.get(self.__URL, headers=self._token_headers(token), json=payload)
         self._check_response(response)
 
-        return DeviceMonitorEmailList.construct_from_jdict(response.json())
+        return DeviceMonitorSpecificationList.construct_from_jdict(response.json())
 
 
     def add(self, token, email_address, device_tag):
         payload = {
             'email_address': email_address,
             'device_tag': device_tag
         }
 
         response = self._http_client.post(self.__URL, headers=self._token_headers(token), json=payload)
         self._check_response(response)
 
-        return DeviceMonitorEmailList.construct_from_jdict(response.json())
+        return DeviceMonitorSpecification.construct_from_jdict(response.json())
+
+
+    def set_suspended(self, token, device_tag, is_suspended):
+        payload = {
+            'device_tag': device_tag,
+            'is_suspended': is_suspended
+        }
+
+        response = self._http_client.patch(self.__URL, headers=self._token_headers(token), json=payload)
+        self._check_response(response)
+
+        return DeviceMonitorSpecification.construct_from_jdict(response.json())
 
 
     def remove(self, token, email_address, device_tag=None):
         payload = {
             'email_address': email_address,
             'device_tag': device_tag
         }
 
         response = self._http_client.delete(self.__URL, headers=self._token_headers(token), json=payload)
         self._check_response(response)
 
-        return DeviceMonitorEmailList.construct_from_jdict(response.json())
+        return DeviceMonitorSpecificationList.construct_from_jdict(response.json())
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
         return "DeviceMonitorSpecificationManager:{}"
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/device_monitor_status_manager.py` & `scs-core-2.8.9/src/scs_core/aws/manager/device_monitor_status_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             'device_tag': device_tag_filter,
             'exact': exact
         }
 
         response = self._http_client.get(self.__URL, headers=self._token_headers(token), json=payload)
         self._check_response(response)
 
-        return DeviceMonitorReport(response.json())
+        return DeviceMonitorReport.construct_from_jdict(response.json())
 
         # return report.device(device_tag_filter) if exact else report
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/dynamo_manager.py` & `scs-core-2.8.9/src/scs_core/aws/manager/dynamo_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/ec2_message_manager.py` & `scs-core-2.8.9/src/scs_core/aws/manager/ec2_message_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 class MessageManager(object):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, api_key, _=None):
+    def __init__(self):
         """
         Constructor
         """
-        self.__rest_client = RESTClient(api_key)
+        self.__rest_client = RESTClient()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def find_for_topic(self, topic, start_date, end_date):
         request_path = '/' + '/'.join((topic, start_date.utc().as_iso8601(), end_date.utc().as_iso8601()))
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/lambda_bylines.py` & `scs-core-2.8.9/src/scs_core/aws/manager/lambda_bylines.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/lambda_message_manager.py` & `scs-core-2.8.9/src/scs_core/aws/manager/lambda_message_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,19 @@
 
     __REQUEST_PATH = '/topicMessages'
 
     # __REQUEST_PATH = '/default/AWSAggregateTest'
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, api_key, reporter=None):
+    def __init__(self, reporter=None):
         """
         Constructor
         """
-        self.__rest_client = RESTClient(api_key)
+        self.__rest_client = RESTClient()
         self.__reporter = reporter
 
         self.__logger = Logging.getLogger()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/s3_manager.py` & `scs-core-2.8.9/src/scs_core/aws/manager/s3_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/sagemaker_model_manager.py` & `scs-core-2.8.9/src/scs_core/aws/manager/sagemaker_model_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/manager/sagemaker_trial_manager.py` & `scs-core-2.8.9/src/scs_core/aws/manager/sagemaker_trial_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/access_key_manager.py` & `scs-core-2.8.9/src/scs_core/aws/security/access_key_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/cognito_client_credentials.py` & `scs-core-2.8.9/src/scs_core/aws/security/cognito_client_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/cognito_device.py` & `scs-core-2.8.9/src/scs_core/aws/security/cognito_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,18 +59,23 @@
         return cls(system_id.message_tag(), shared_secret.key)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def is_valid_tag(cls, tag):
-        if not isinstance(tag, str):
+        try:
+            if len(tag) > 255:
+                return False
+
+            return bool(re.fullmatch(r'[a-z]+\d*-[a-z]+\d*-\d+', tag))
+
+        except TypeError:
             return False
 
-        return re.search(r'^\w+-\w+-\d+$', tag) is not None
 
 
     @classmethod
     def is_valid_password(cls, password):
         if not isinstance(password, str):
             return False
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/cognito_device_creator.py` & `scs-core-2.8.9/src/scs_core/aws/security/cognito_device_creator.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Created on 24 Apr 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 Enables a device to register itself as a CognitoDevice
 """
 
+import json
+
 from scs_core.aws.client.api_client import APIClient
 from scs_core.aws.security.cognito_device import CognitoDeviceIdentity
 
 from scs_core.data.json import JSONify
 
 
 # --------------------------------------------------------------------------------------------------------------------
@@ -26,14 +28,24 @@
 
     def __init__(self, http_client):
         super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
+    def may_create(self, device_tag):
+        payload = {"DeviceTag": device_tag}
+
+        response = self._http_client.get(self.__URL, headers=self._auth_headers(self.__AUTH),
+                                         data=JSONify.dumps(payload))
+        self._check_response(response)
+
+        return json.loads(response.json())
+
+
     def create(self, identity: CognitoDeviceIdentity):
         response = self._http_client.post(self.__URL, headers=self._auth_headers(self.__AUTH),
                                           data=JSONify.dumps(identity))
         self._check_response(response)
 
         return CognitoDeviceIdentity.construct_from_jdict(response.json())
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/cognito_device_finder.py` & `scs-core-2.8.9/src/scs_core/aws/security/cognito_device_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/cognito_device_manager.py` & `scs-core-2.8.9/src/scs_core/aws/security/cognito_device_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,29 +23,39 @@
 
     def __init__(self, http_client):
         super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
+    def update_self(self, token, credentials):
+        url = '/'.join((self.__URL, 'self'))
+
+        response = self._http_client.patch(url, headers=self._token_headers(token), data=JSONify.dumps(credentials))
+        self._check_response(response)
+
+        return CognitoDeviceIdentity.construct_from_jdict(response.json())
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
     def create(self, token, identity):
         response = self._http_client.post(self.__URL, headers=self._token_headers(token), data=JSONify.dumps(identity))
         self._check_response(response)
 
         return CognitoDeviceIdentity.construct_from_jdict(response.json())
 
 
     def update(self, token, identity):
         response = self._http_client.patch(self.__URL, headers=self._token_headers(token), data=JSONify.dumps(identity))
         self._check_response(response)
 
         return CognitoDeviceIdentity.construct_from_jdict(response.json())
 
 
-
     def delete(self, token, device_tag):
         payload = {"DeviceTag": device_tag}
 
         response = self._http_client.delete(self.__URL, headers=self._token_headers(token), data=JSONify.dumps(payload))
         self._check_response(response)
 
         # TODO: delete device from organisations?
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/cognito_login_manager.py` & `scs-core-2.8.9/src/scs_core/aws/security/cognito_login_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/cognito_membership.py` & `scs-core-2.8.9/src/scs_core/aws/security/cognito_membership.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/cognito_password_manager.py` & `scs-core-2.8.9/src/scs_core/aws/security/cognito_password_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/cognito_user.py` & `scs-core-2.8.9/src/scs_core/aws/security/cognito_user.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/cognito_user_finder.py` & `scs-core-2.8.9/src/scs_core/aws/security/cognito_user_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/cognito_user_manager.py` & `scs-core-2.8.9/src/scs_core/aws/security/cognito_user_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/device_whitelist_manager.py` & `scs-core-2.8.9/src/scs_core/aws/security/device_whitelist_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/opr_membership.py` & `scs-core-2.8.9/src/scs_core/aws/security/opr_membership.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/organisation.py` & `scs-core-2.8.9/src/scs_core/aws/security/organisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 "DeploymentLabel": "Preston Circus"}
 """
 
 import re
 
 from collections import OrderedDict
 
+from scs_core.aws.security.cognito_device import CognitoDeviceCredentials
+
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONable
 from scs_core.data.timedelta import Timedelta
 
 
 # --------------------------------------------------------------------------------------------------------------------
@@ -580,26 +582,14 @@
     def deployment_interval(cls):
         return cls.__DEPLOYMENT_INTERVAL
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def is_valid_tag(cls, device_tag):
-        try:
-            if len(device_tag) > 255:
-                return False
-
-            return bool(re.fullmatch(r'[a-z]+[0-9]*-[a-z]+[0-9]*-[0-9]+', device_tag))
-
-        except TypeError:
-            return False
-
-
-    @classmethod
     def is_valid_deployment_label(cls, deployment_label):
         try:
             return 1 < len(deployment_label) < 256
 
         except TypeError:
             return False
 
@@ -681,16 +671,17 @@
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
         if self.device_tag is None or self.org_id is None:
             return False
 
-        return self.is_valid_tag(self.device_tag) and self.is_valid_deployment_label(self.deployment_label) and \
-            self.is_valid_path(self.device_path) and self.is_valid_path(self.location_path)
+        return CognitoDeviceCredentials.is_valid_tag(self.device_tag) and \
+            self.is_valid_deployment_label(self.deployment_label) and self.is_valid_path(self.device_path) and \
+            self.is_valid_path(self.location_path)
 
 
     def has_unix_era_start(self):
         return self.start_datetime == LocalizedDatetime.unix_era_start()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/organisation_manager.py` & `scs-core-2.8.9/src/scs_core/aws/security/organisation_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/aws/security/path_filter.py` & `scs-core-2.8.9/src/scs_core/aws/security/path_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/client/http_client.py` & `scs-core-2.8.9/src/scs_core/client/http_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Created on 9 Nov 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import ssl
-# import sys
 
 import http.client
 
 import urllib.parse
 
 from socket import gaierror, timeout as timeout_error
 
@@ -36,15 +35,15 @@
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def connect(self, host, secure=True, verified=True, timeout=None):
         # print("connect: host: {}, timeout: {}".format(host, timeout), file=sys.stderr)
 
-        self.__host = host                                          # PersistenceManager
+        self.__host = host
 
         if secure:
             # noinspection PyProtectedMember,PyUnresolvedReferences
             context = None if verified else ssl._create_unverified_context()
 
             if timeout is not None:
                 self.__conn = http.client.HTTPSConnection(host, context=context, timeout=timeout)
```

### Comparing `scs-core-2.8.4/src/scs_core/client/http_exception.py` & `scs-core-2.8.9/src/scs_core/client/http_exception.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/client/network.py` & `scs-core-2.8.9/src/scs_core/client/network.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/client/resource_unavailable_exception.py` & `scs-core-2.8.9/src/scs_core/client/resource_unavailable_exception.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/client/sftp_client_conf.py` & `scs-core-2.8.9/src/scs_core/client/sftp_client_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/climate/absolute_humidity.py` & `scs-core-2.8.9/src/scs_core/climate/absolute_humidity.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/climate/icp10101_datum.py` & `scs-core-2.8.9/src/scs_core/climate/icp10101_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/climate/mpl115a2_calib.py` & `scs-core-2.8.9/src/scs_core/climate/mpl115a2_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/climate/mpl115a2_datum.py` & `scs-core-2.8.9/src/scs_core/climate/mpl115a2_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/climate/pressure_conf.py` & `scs-core-2.8.9/src/scs_core/climate/pressure_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/climate/pressure_datum.py` & `scs-core-2.8.9/src/scs_core/climate/pressure_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/climate/sht_conf.py` & `scs-core-2.8.9/src/scs_core/climate/sht_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/climate/sht_datum.py` & `scs-core-2.8.9/src/scs_core/climate/sht_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/comms/mqtt_conf.py` & `scs-core-2.8.9/src/scs_core/comms/mqtt_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/comms/uds_client.py` & `scs-core-2.8.9/src/scs_core/comms/uds_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/comms/uds_reader.py` & `scs-core-2.8.9/src/scs_core/comms/uds_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/comms/uds_server.py` & `scs-core-2.8.9/src/scs_core/comms/uds_server.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/comms/uds_writer.py` & `scs-core-2.8.9/src/scs_core/comms/uds_writer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/control/command.py` & `scs-core-2.8.9/src/scs_core/control/command.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/control/control_datum.py` & `scs-core-2.8.9/src/scs_core/control/control_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/control/control_handler.py` & `scs-core-2.8.9/src/scs_core/control/control_handler.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/control/control_receipt.py` & `scs-core-2.8.9/src/scs_core/control/control_receipt.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/csv/csv_archive.py` & `scs-core-2.8.9/src/scs_core/csv/csv_archive.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/csv/csv_dict.py` & `scs-core-2.8.9/src/scs_core/csv/csv_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/csv/csv_log.py` & `scs-core-2.8.9/src/scs_core/csv/csv_log.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/csv/csv_log_cursor_queue.py` & `scs-core-2.8.9/src/scs_core/csv/csv_log_cursor_queue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/csv/csv_log_reader.py` & `scs-core-2.8.9/src/scs_core/csv/csv_log_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 import sys
 import time
 
 from collections import OrderedDict
 from multiprocessing import Manager
 
 from requests.exceptions import ConnectionError                                             # raised by requests
+
 from scs_core.client.resource_unavailable_exception import ResourceUnavailableException     # raised by HTTPClient
 
 from scs_core.csv.csv_log_cursor_queue import CSVLogCursorQueue, CSVLogCursor
 from scs_core.csv.csv_reader import CSVReader
 
+from scs_core.data.datetime import LocalizedDatetime
+
 from scs_core.sync.synchronised_process import SynchronisedProcess
 
 from scs_core.sys.logging import Logging
 from scs_core.sys.tail import Tail
 
 
 # --------------------------------------------------------------------------------------------------------------------
@@ -72,15 +75,15 @@
     def run(self, halt_on_empty_queue=False):
         # self.__logger.info('CSVLogReader: running')
 
         try:
             # build queue...
             timeline_start, cursors = self.__queue_builder.find_cursors()       # waits indefinitely for network
 
-            self.__logger.info("timeline_start: %s" % timeline_start)
+            self.__logger.info("timeline_start: %s" % timeline_start.as_iso8601())
 
             with self._lock:
                 queue = CSVLogCursorQueue.construct_from_jdict(OrderedDict(self._value))
                 for cursor in cursors:
                     queue.include(cursor)
                 queue.as_list(self._value)
 
@@ -201,19 +204,22 @@
     """
 
     __BYLINE_WAIT_TIME = 20.0                   # seconds
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, topic_name, topic_path, byline_manager, system_id, conf):
-        self.__topic_name = topic_name
-        self.__topic_path = topic_path
-        self.__byline_manager = byline_manager
-        self.__system_id = system_id
-        self.__conf = conf
+        """
+        Constructor
+        """
+        self.__topic_name = topic_name                                      # string
+        self.__topic_path = topic_path                                      # string
+        self.__byline_manager = byline_manager                              # BylineManager
+        self.__system_id = system_id                                        # SystemID
+        self.__conf = conf                                                  # CSVLoggerConf
 
         self.__logger = Logging.getLogger()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def find_cursors(self):
@@ -224,19 +230,21 @@
                                                                             self.__topic_path)
                 break
             except (ConnectionError, ResourceUnavailableException) as ex:
                 self.__logger.info(repr(ex))
                 time.sleep(self.__BYLINE_WAIT_TIME)
 
         rec = None if byline is None else byline.rec
-        timeline_start = None if rec is None else rec.utc_datetime
+        byline_start = None if rec is None else rec.utc_datetime
+
+        timeline_start = self.__conf.retrospection_start(LocalizedDatetime(byline_start))
 
         # CSVLog...
         read_log = self.__conf.csv_log(self.__topic_name, tag=self.__system_id.message_tag(),
-                                       timeline_start=timeline_start)
+                                       timeline_start=timeline_start.datetime)
 
         return timeline_start, CSVLogCursorQueue.find_cursors_for_log(read_log, 'rec')  # may raise FileNotFoundError
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self):
```

### Comparing `scs-core-2.8.4/src/scs_core/csv/csv_logger.py` & `scs-core-2.8.9/src/scs_core/csv/csv_logger.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/csv/csv_logger_conf.py` & `scs-core-2.8.9/src/scs_core/gas/ndir/ndir_datum.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,110 +1,118 @@
 """
-Created on 13 Apr 2018
+Created on 20 Jun 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-example JSON:
-{"root-path": "/home/pi/SCS/logs", "delete-oldest": true, "write-interval": 0}
+Alphasense A4 IRC-AT non-dispersive infra-red detector
 """
 
 from collections import OrderedDict
+from numbers import Number
 
-from scs_core.csv.csv_log import CSVLog
-from scs_core.data.json import PersistentJSONable
-from scs_core.sys.filesystem import FilesystemReport
+from scs_core.data.datum import Datum
+from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CSVLoggerConf(PersistentJSONable):
+class NDIRDatum(JSONable):
     """
     classdocs
     """
 
-    __FILENAME = "csv_logger_conf.json"
-
-    @classmethod
-    def persistence_location(cls):
-        return cls.conf_dir(), cls.__FILENAME
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_jdict(cls, jdict, skeleton=False):
+    def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
-        root_path = jdict.get('root-path')
-        delete_oldest = jdict.get('delete-oldest')
-        write_interval = jdict.get('write-interval')
+        temp = jdict.get('tmp')
+        cnc = jdict.get('cnc-raw')
+        cnc_igl = jdict.get('cnc')
 
-        return CSVLoggerConf(root_path, delete_oldest, write_interval)
+        return NDIRDatum(temp, cnc, cnc_igl)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, root_path, delete_oldest, write_interval):
+    def __init__(self, temp, cnc, cnc_igl):
         """
         Constructor
         """
-        super().__init__()
-
-        self.__root_path = root_path                            # string
-        self.__delete_oldest = bool(delete_oldest)              # bool
-        self.__write_interval = int(write_interval)             # int
+        self.__temp = Datum.float(temp, 1)              # temperature                               °C
+        self.__cnc = Datum.float(cnc, 1)                # concentration                             ppm
+        self.__cnc_igl = Datum.float(cnc_igl, 1)        # concentration (ideal gas law corrected)   ppm
 
 
     def __eq__(self, other):
         try:
-            return self.root_path == other.root_path and self.delete_oldest == other.delete_oldest and \
-                   self.write_interval == other.write_interval
+            return self.temp == other.temp and self.cnc == other.cnc and self.cnc_igl == other.cnc_igl
 
-        except (TypeError, AttributeError):
+        except AttributeError:
             return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
+    # Support for averaging...
+
+    def __add__(self, other):
+        if not isinstance(other, self.__class__):
+            raise TypeError(other)
 
-    def csv_log(self, topic_subject, tag=None, timeline_start=None):
-        return CSVLog(self.root_path, topic_subject, tag=tag, timeline_start=timeline_start)
+        temp = self.temp + other.temp
+        cnc = self.cnc + other.cnc
+        cnc_igl = self.cnc_igl + other.cnc_igl
 
+        return NDIRDatum(temp, cnc, cnc_igl)
 
-    def filesystem_report(self):
-        return FilesystemReport.construct(self.root_path)
+
+    def __truediv__(self, other):
+        if not isinstance(other, Number):
+            raise TypeError(other)
+
+        temp = self.temp / other
+        cnc = None if self.cnc is None else self.cnc / other
+        cnc_igl = None if self.cnc_igl is None else self.cnc_igl / other
+
+        return NDIRDatum(temp, cnc, cnc_igl)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
-        jdict['root-path'] = self.root_path
-        jdict['delete-oldest'] = self.delete_oldest
-        jdict['write-interval'] = self.write_interval
+        jdict['tmp'] = self.temp
+        jdict['cnc-raw'] = self.cnc
+        jdict['cnc'] = self.cnc_igl
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def root_path(self):
-        return self.__root_path
+    def temp(self):
+        return self.__temp
+
+
+    @property
+    def cnc(self):
+        return self.__cnc
 
 
     @property
-    def delete_oldest(self):
-        return self.__delete_oldest
+    def co2(self):              # a synonym of cnc for compatibility with GasesSample and SCD30Datum
+        return self.cnc_igl
 
 
     @property
-    def write_interval(self):
-        return self.__write_interval
+    def cnc_igl(self):
+        return self.__cnc_igl
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "CSVLoggerConf:{root_path:%s, delete_oldest:%s, write_interval:%s}" %  \
-               (self.root_path, self.delete_oldest, self.write_interval)
+        return "NDIRDatum:{temp:%s, cnc:%s, cnc_igl:%s}" % (self.temp, self.cnc, self.cnc_igl)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scs-core-2.8.4/src/scs_core/csv/csv_reader.py` & `scs-core-2.8.9/src/scs_core/csv/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/csv/csv_writer.py` & `scs-core-2.8.9/src/scs_core/csv/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/aggregate.py` & `scs-core-2.8.9/src/scs_core/data/aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/array_dict.py` & `scs-core-2.8.9/src/scs_core/data/array_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/average.py` & `scs-core-2.8.9/src/scs_core/data/average.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/categorical_regression.py` & `scs-core-2.8.9/src/scs_core/data/categorical_regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/checkpoint_generator.py` & `scs-core-2.8.9/src/scs_core/data/checkpoint_generator.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/crc.py` & `scs-core-2.8.9/src/scs_core/data/crc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/crypt.py` & `scs-core-2.8.9/src/scs_core/data/crypt.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/datetime.py` & `scs-core-2.8.9/src/scs_core/data/datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 http://code.activestate.com/recipes/496683-converting-ole-datetime-values-into-python-datetim/
 """
 
 import pytz
 import re
 import tzlocal
 
-from datetime import datetime, timedelta, timezone
+from datetime import date, datetime, timedelta, timezone
 
 from scs_core.data.json import JSONable
 from scs_core.data.timedelta import Timedelta
 
 
 # TODO: object should carry a flag indicating presence of millis - for "preserve millis" mode?
 # --------------------------------------------------------------------------------------------------------------------
@@ -69,17 +69,17 @@
 
     @classmethod
     def unix_era_start(cls):
         return cls.construct_from_iso8601(cls.UNIX_ERA_START)
 
 
     @classmethod
-    def construct_from_date(cls, date):
+    def construct_from_date(cls, d):
         zone = tzlocal.get_localzone()
-        localized = zone.localize(datetime(date.year, month=date.month, day=date.day))
+        localized = zone.localize(datetime(d.year, month=d.month, day=d.day))
 
         return LocalizedDatetime(localized)
 
 
     @classmethod
     def construct_from_timestamp(cls, t, tz=None):
         zone = tzlocal.get_localzone() if tz is None else tz
@@ -102,17 +102,17 @@
         # numeric timezone offset...
         return cls.__construct_from_iso8601_numeric(datetime_str)
 
 
     @classmethod
     def construct_from_date_time(cls, date_parser, date_str, time_str, tz=None):
         # date...
-        date = date_parser.datetime(date_str)
+        d = date_parser.datetime(date_str)
 
-        if date is None:
+        if d is None:
             return None
 
         # time (rightmost time in string)...
         match = re.match(r'(\d{1,2}):(\d{2})(:(\d{2}))? *([APap][Mm])? *$', time_str)       # e.g. 24:00:00
 
         if match is None:
             return None
@@ -126,15 +126,15 @@
         if fields[4] == 'pm' or fields[4] == 'PM':
             hours_delta += 12
 
         # zone...
         zone = pytz.timezone('Etc/UTC') if tz is None else tz
 
         # construct...
-        start = LocalizedDatetime(zone.localize(date))
+        start = LocalizedDatetime(zone.localize(d))
 
         corrected = start.timedelta(seconds=seconds_delta, minutes=minutes_delta, hours=hours_delta)
 
         return corrected
 
 
     @classmethod
@@ -173,21 +173,21 @@
         localized = datetime(year, month=month, day=day, hour=hour, minute=minute, second=second, tzinfo=zone)
 
         return LocalizedDatetime(localized)
 
 
     @classmethod
     def construct_from_oad(cls, oad, tz=None):
-        date = cls.OLE_TIME_ZERO + timedelta(days=float(oad))
+        d = cls.OLE_TIME_ZERO + timedelta(days=float(oad))
 
         # zone...
         zone = pytz.timezone('Etc/UTC') if tz is None else tz
 
         # construct...
-        return LocalizedDatetime(zone.localize(date))
+        return LocalizedDatetime(zone.localize(d))
 
 
     @classmethod
     def construct_from_jdict(cls, jdict):               # TODO: deprecated
         return cls.construct_from_iso8601(jdict)
 
 
@@ -384,56 +384,60 @@
     def timedelta(self, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
         td = timedelta(days=days, seconds=seconds, microseconds=microseconds, milliseconds=milliseconds,
                        minutes=minutes, hours=hours, weeks=weeks)
 
         return LocalizedDatetime(self.__datetime + td)
 
 
+    def dst(self):
+        return Timedelta.construct(self.__datetime.dst())
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         return self.as_iso8601()
 
 
     def as_iso8601(self, include_millis=False):
         """
         example: 2016-08-13T00:38:05.210+01:00
         """
-        date = self.__datetime.strftime("%Y-%m-%d")
-        time = self.__datetime.strftime("%H:%M:%S")
+        d = self.__datetime.strftime("%Y-%m-%d")
+        t = self.__datetime.strftime("%H:%M:%S")
 
         # millis...
         if include_millis:
             micros = float(self.__datetime.strftime("%f"))
             millis = ".%03d" % (micros // 1000)
 
         else:
             millis = ""
 
         # time zone...
         zone = self.__datetime.strftime("%z")
 
         # Z format...
         if float(zone[1:]) == 0.0:
-            return "%sT%s%sZ" % (date, time, millis)
+            return "%sT%s%sZ" % (d, t, millis)
 
         # numeric format...
         zone_hours = zone[:3]
         zone_mins = zone[3:]
 
-        return "%sT%s%s%s:%s" % (date, time, millis, zone_hours, zone_mins)
+        return "%sT%s%s%s:%s" % (d, t, millis, zone_hours, zone_mins)
 
 
     def as_time(self):
-        time = self.__datetime.strftime("%H:%M:%S")
+        t = self.__datetime.strftime("%H:%M:%S")
 
         micros = float(self.__datetime.strftime("%f"))
         millis = "%03d" % (micros // 1000)
 
-        return "%s.%s" % (time, millis)
+        return "%s.%s" % (t, millis)
 
 
     def timestamp(self):
         return self.__datetime.timestamp()
 
 
     # ----------------------------------------------------------------------------------------------------------------
@@ -459,14 +463,31 @@
 
     def __str__(self, *args, **kwargs):
         return "LocalizedDatetime:{datetime:%s}" % self.datetime
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
+class Date(object):
+    """
+    classdocs
+    """
+
+    @classmethod
+    def is_valid_iso_format(cls, date_str):
+        try:
+            date.fromisoformat(date_str)
+            return True
+
+        except (TypeError, ValueError):
+            return False
+
+
+# --------------------------------------------------------------------------------------------------------------------
+
 class DateParser(object):
     """
     classdocs
     """
 
     __FORMATS = {
         'DD-MM-YYYY': ('%d-%m-%Y', False),
```

### Comparing `scs-core-2.8.4/src/scs_core/data/datum.py` & `scs-core-2.8.9/src/scs_core/data/datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/duplicates.py` & `scs-core-2.8.9/src/scs_core/data/duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/histogram.py` & `scs-core-2.8.9/src/scs_core/data/histogram.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/interval.py` & `scs-core-2.8.9/src/scs_core/data/interval.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/join.py` & `scs-core-2.8.9/src/scs_core/data/join.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/json.py` & `scs-core-2.8.9/src/scs_core/data/json.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/lin_regress.py` & `scs-core-2.8.9/src/scs_core/data/lin_regress.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/linear_regression.py` & `scs-core-2.8.9/src/scs_core/data/linear_regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/low_pass_filter.py` & `scs-core-2.8.9/src/scs_core/data/low_pass_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/median_filter.py` & `scs-core-2.8.9/src/scs_core/data/median_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/min_list.py` & `scs-core-2.8.9/src/scs_core/data/min_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/model_delta.py` & `scs-core-2.8.9/src/scs_core/data/model_delta.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/path_dict.py` & `scs-core-2.8.9/src/scs_core/data/path_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/precision.py` & `scs-core-2.8.9/src/scs_core/data/precision.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/publication.py` & `scs-core-2.8.9/src/scs_core/data/publication.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/queue_report.py` & `scs-core-2.8.9/src/scs_core/data/queue_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/recurring_period.py` & `scs-core-2.8.9/src/scs_core/data/recurring_period.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,125 +1,139 @@
 """
 Created on 7 Jul 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/ScheduledEvents.html
+https://en.wikipedia.org/wiki/Cron
 
 document example:
-{"interval": 1, "units": "D"}
+{"type": "recurring", "interval": 1, "units": "D", "timezone": "Europe/London"}
 """
 
 import pytz
 
 from abc import abstractmethod
 from collections import OrderedDict
 from datetime import datetime
 
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.json import JSONable
+from scs_core.data.period import Period
 from scs_core.data.timedelta import Timedelta
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class RecurringPeriod(JSONable):
+class RecurringPeriod(Period, JSONable):
     """
     classdocs
     """
     _UTC = pytz.timezone('Etc/UTC')
 
+    __TYPE = 'recurring'
+
+    @classmethod
+    def type(cls):
+        return cls.__TYPE
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     @abstractmethod
     def valid_intervals(cls):
         pass
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_jdict(cls, jdict):
+    def construct_from_jdict(cls, jdict, timezone=None):
         if not jdict:
             return None
 
         interval = jdict.get('interval')
         units = jdict.get('units')
+        timezone_str = jdict.get('timezone', timezone)
 
-        return cls.construct(interval, units)
+        return cls.construct(interval, units, timezone_str)
 
 
     @classmethod
-    def construct(cls, interval, units):
+    def construct(cls, interval, units, timezone_str):
+        timezone = pytz.timezone(timezone_str)
+
         if units == 'D':
-            return RecurringDay(interval)
+            return RecurringDay(interval, timezone)
 
         if units == 'H':
-            return RecurringHours(interval)
+            return RecurringHours(interval, timezone)
 
         if units == 'M':
-            return RecurringMinutes(interval)
+            return RecurringMinutes(interval, timezone)
 
         raise ValueError(units)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, interval):
+    def __init__(self, interval, timezone: pytz.timezone):
         """
         Constructor
         """
+        Period.__init__(self, timezone)
+
         self.__interval = int(interval)                     # int
 
 
     @abstractmethod
     def __lt__(self, other):
         pass
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @abstractmethod
-    def is_valid(self):
-        pass
+    def _cron_minutes(self, minutes_offset):
+        utc_now = LocalizedDatetime.now().utc()
+        local_now = utc_now.localize(self.timezone)
+        cron_minutes = (abs(local_now.datetime.minute - utc_now.datetime.minute) + minutes_offset) % 60
 
+        return cron_minutes
 
-    @abstractmethod
-    def checkpoint(self):
-        pass
 
+    # ----------------------------------------------------------------------------------------------------------------
 
     @abstractmethod
-    def cron(self, minutes_offset):
+    def timedelta(self):
         pass
 
 
-    @abstractmethod
-    def aws_cron(self, minutes_offset):
-        pass
+    # ----------------------------------------------------------------------------------------------------------------
 
+    def has_expiring_dst(self):
+        return False
 
-    @abstractmethod
-    def timedelta(self):
-        pass
 
+    # ----------------------------------------------------------------------------------------------------------------
 
-    @abstractmethod
-    def end_datetime(self, origin: LocalizedDatetime):
-        pass
+    def start_datetime(self, point: LocalizedDatetime):
+        return self.end_datetime(point) - self.timedelta()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
+        jdict['type'] = self.type()
+
         jdict['interval'] = self.interval
         jdict['units'] = self.units
+        jdict['timezone'] = str(self.timezone)
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
@@ -142,15 +156,15 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def __repr__(self):
         return ' '.join((str(self.interval), self.repr_units))
 
 
     def __str__(self, *args, **kwargs):
-        return self.__class__.__name__ + ":{interval:%s}" %  self.interval
+        return self.__class__.__name__ + ":{interval:%s, timezone:%s}" %  (self.interval, self.timezone)
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class RecurringDay(RecurringPeriod):
     """
     classdocs
@@ -159,19 +173,19 @@
     @classmethod
     def valid_intervals(cls):
         return 1,
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, interval):
+    def __init__(self, interval, timezone: pytz.timezone):
         """
         Constructor
         """
-        super().__init__(interval)
+        super().__init__(interval, timezone)
 
 
     def __lt__(self, other):
         if isinstance(other, RecurringHours) or isinstance(other, RecurringMinutes):
             return False
 
         return self.interval < other.interval
@@ -184,19 +198,19 @@
 
 
     def checkpoint(self):
         return '00:00:00'
 
 
     def cron(self, minutes_offset):
-        return '%d 0 * * *' % minutes_offset
+        return '%d 0 * * *' % self._cron_minutes(minutes_offset)
 
 
     def aws_cron(self, minutes_offset):
-        return 'cron(%d 0 * * ? *)' % minutes_offset
+        return 'cron(%d 0 * * ? *)' % self._cron_minutes(minutes_offset)
 
 
     def timedelta(self):
         return Timedelta(days=self.interval)
 
 
     def end_datetime(self, origin: LocalizedDatetime):
@@ -229,19 +243,19 @@
     @classmethod
     def valid_intervals(cls):
         return cls.__DIVISORS
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, interval):
+    def __init__(self, interval, timezone: pytz.timezone):
         """
         Constructor
         """
-        super().__init__(interval)
+        super().__init__(interval, timezone)
 
 
     def __lt__(self, other):
         if isinstance(other, RecurringDay):
             return True
 
         if isinstance(other, RecurringMinutes):
@@ -256,20 +270,25 @@
         return self.interval in self.__DIVISORS
 
 
     def checkpoint(self):
         return '/%d:00:00' % self.interval
 
 
+    # ----------------------------------------------------------------------------------------------------------------
+
     def cron(self, minutes_offset):
-        return '%d */%d * * *' % (minutes_offset, self.interval)
+        return '%d */%d * * *' % (self._cron_minutes(minutes_offset), self.interval)
 
 
     def aws_cron(self, minutes_offset):
-        return 'cron(%d 0/%d * * ? *)' % (minutes_offset, self.interval)
+        return 'cron(%d 0/%d * * ? *)' % (self._cron_minutes(minutes_offset), self.interval)
+
+
+    # ----------------------------------------------------------------------------------------------------------------
 
 
     def timedelta(self):
         return Timedelta(hours=self.interval)
 
 
     def end_datetime(self, origin: LocalizedDatetime):
@@ -303,19 +322,19 @@
     @classmethod
     def valid_intervals(cls):
         return cls.__DIVISORS
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, interval):
+    def __init__(self, interval, timezone: pytz.timezone):
         """
         Constructor
         """
-        super().__init__(interval)
+        super().__init__(interval, timezone)
 
 
     def __lt__(self, other):
         if isinstance(other, RecurringDay) or isinstance(other, RecurringHours):
             return True
 
         return self.interval < other.interval
```

### Comparing `scs-core-2.8.4/src/scs_core/data/regression.py` & `scs-core-2.8.9/src/scs_core/data/regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/rtc_datetime.py` & `scs-core-2.8.9/src/scs_core/data/rtc_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/sample_delta.py` & `scs-core-2.8.9/src/scs_core/data/sample_delta.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/stats.py` & `scs-core-2.8.9/src/scs_core/data/stats.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/str.py` & `scs-core-2.8.9/src/scs_core/data/str.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/timedelta.py` & `scs-core-2.8.9/src/scs_core/data/timedelta.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,14 +137,34 @@
                 print(ExceptionReport.construct(ex), file=sys.stderr)
                 return None
 
             return cls(days=days, hours=hours, minutes=minutes)
 
 
     @classmethod
+    def construct_from_dst_report(cls, report):
+        if report is None:
+            return None
+
+        # CPU time...
+        match = re.match(r'(\d+):(\d+):(\d+)', report)
+
+        if match is None:
+            return None
+
+        fields = match.groups()
+
+        hours = int(fields[0])
+        minutes = int(fields[1])
+        seconds = int(fields[2])
+
+        return Timedelta(hours=hours, minutes=minutes, seconds=seconds)
+
+
+    @classmethod
     def construct_from_jdict(cls, jdict):
         if jdict is None:
             return None
 
         match = re.match(r'(\d+)-(\d{2}):(\d{2}):(\d{2})(.(\d{3}))?', jdict)
 
         if match is None:
@@ -196,14 +216,24 @@
         return self.delta <= other.delta
 
 
     def __lt__(self, other):
         return self.delta < other.delta
 
 
+    def __add__(self, other):
+        seconds = self.total_seconds() + other.total_seconds()
+        return Timedelta(seconds=seconds)
+
+
+    def __sub__(self, other):
+        seconds = self.total_seconds() - other.total_seconds()
+        return Timedelta(seconds=seconds)
+
+
     def __truediv__(self, other):
         seconds = self.total_seconds() / other
         return Timedelta(seconds=seconds)
 
 
     def __mul__(self, other):
         seconds = self.total_seconds() * other
```

### Comparing `scs-core-2.8.4/src/scs_core/data/tokens.py` & `scs-core-2.8.9/src/scs_core/data/tokens.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/data/topic_path.py` & `scs-core-2.8.9/src/scs_core/data/topic_path.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/display/display_conf.py` & `scs-core-2.8.9/src/scs_core/display/display_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/email/email_queue.py` & `scs-core-2.8.9/src/scs_core/email/email_queue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/email/email_queue_manager.py` & `scs-core-2.8.9/src/scs_core/email/email_queue_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/estate/baseline_conf.py` & `scs-core-2.8.9/src/scs_core/estate/baseline_conf_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def construct_from_jdict(cls, jdict, name=None, skeleton=False):
         if not jdict:
             return None
 
         timezone = jdict.get('timezone')
         start_hour = jdict.get('start-hour')
         end_hour = jdict.get('end-hour')
-        aggregation_period = RecurringPeriod.construct_from_jdict(jdict.get('aggregation-period'))
+        aggregation_period = RecurringPeriod.construct_from_jdict(jdict.get('aggregation-period'), timezone=timezone)
         minimums = jdict.get('minimums')
 
         return cls(name, timezone, start_hour, end_hour, aggregation_period, minimums)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
@@ -176,15 +176,15 @@
 
     def as_json(self):
         jdict = OrderedDict()
 
         jdict['timezone'] = self.timezone
         jdict['start-hour'] = self.start_hour
         jdict['end-hour'] = self.end_hour
-        jdict['aggregation-period'] = self.aggregation_period.as_json()
+        jdict['aggregation-period'] = self.aggregation_period
         jdict['minimums'] = self.minimums
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-core-2.8.4/src/scs_core/estate/configuration.py` & `scs-core-2.8.9/src/scs_core/estate/configuration.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/estate/configuration_check.py` & `scs-core-2.8.9/src/scs_core/estate/configuration_check.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/estate/git_pull.py` & `scs-core-2.8.9/src/scs_core/estate/git_pull.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/estate/git_pull_check.py` & `scs-core-2.8.9/src/scs_core/estate/git_pull_check.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/estate/mqtt_device_poller.py` & `scs-core-2.8.9/src/scs_core/estate/mqtt_device_poller.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/estate/mqtt_peer.py` & `scs-core-2.8.9/src/scs_core/estate/mqtt_peer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/estate/package_version.py` & `scs-core-2.8.9/src/scs_core/estate/package_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/exegesis/gas/exegete_catalogue.py` & `scs-core-2.8.9/src/scs_core/exegesis/gas/exegete_catalogue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/exegesis/gas/exegete_collection.py` & `scs-core-2.8.9/src/scs_core/exegesis/gas/exegete_collection.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/exegesis/particulate/exegete_catalogue.py` & `scs-core-2.8.9/src/scs_core/exegesis/particulate/exegete_catalogue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/exegesis/particulate/exegete_collection.py` & `scs-core-2.8.9/src/scs_core/exegesis/particulate/exegete_collection.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/exegesis/particulate/text.py` & `scs-core-2.8.9/src/scs_core/exegesis/particulate/text.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/a4/a4.py` & `scs-core-2.8.9/src/scs_core/gas/a4/a4.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/a4/a4_calib.py` & `scs-core-2.8.9/src/scs_core/gas/a4/a4_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum.py` & `scs-core-2.8.9/src/scs_core/gas/a4/a4_calibrated_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_v1.py` & `scs-core-2.8.9/src/scs_core/gas/a4/a4_calibrated_datum_v1.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_vA.py` & `scs-core-2.8.9/src/scs_core/gas/a4/a4_calibrated_datum_vA.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_vB.py` & `scs-core-2.8.9/src/scs_core/gas/a4/a4_calibrated_datum_vB.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_vC.py` & `scs-core-2.8.9/src/scs_core/gas/a4/a4_calibrated_datum_vC.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/a4/a4_datum.py` & `scs-core-2.8.9/src/scs_core/gas/a4/a4_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/a4/a4_temp_comp.py` & `scs-core-2.8.9/src/scs_core/gas/a4/a4_temp_comp.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/afe/afe_datum.py` & `scs-core-2.8.9/src/scs_core/gas/afe/afe_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/afe/pt1000_calib.py` & `scs-core-2.8.9/src/scs_core/gas/afe/pt1000_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/afe/pt1000_datum.py` & `scs-core-2.8.9/src/scs_core/gas/afe/pt1000_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/afe_baseline.py` & `scs-core-2.8.9/src/scs_core/gas/afe_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/afe_calib.py` & `scs-core-2.8.9/src/scs_core/gas/afe_calib.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def download(cls, serial_number, parse=True):
         http_client = HTTPClient()
-        http_client.connect(AFECalib.ALPHASENSE_HOST)
+        http_client.connect(cls.ALPHASENSE_HOST)
 
         try:
             path = AFECalib.ALPHASENSE_PATH + serial_number
             response = http_client.get(path, None, AFECalib.ALPHASENSE_HEADER)
 
             logger = Logging.getLogger()
             logger.debug("afe response: %s" % response)
```

### Comparing `scs-core-2.8.4/src/scs_core/gas/afe_id.py` & `scs-core-2.8.9/src/scs_core/gas/afe_id.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/d4/d4_datum.py` & `scs-core-2.8.9/src/scs_core/gas/d4/d4_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/dsi_calib.py` & `scs-core-2.8.9/src/scs_core/gas/dsi_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/gas.py` & `scs-core-2.8.9/src/scs_core/gas/gas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Created on 13 Feb 2018
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
+Conversion Factors Between ppb and μg m-3 and ppm and mgm-3 (EC, not WHO)
+
 http://www.apis.ac.uk/unit-conversion
 https://keisan.casio.com/exec/system/1224579725
 """
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
@@ -23,29 +25,30 @@
     GRAVITY =                9.80665                            # m/s2
     MOLAR_MASS_OF_AIR =     28.9644                             # g/mol
     GAS_CONSTANT =           8.3144598                          # J/(mol*K)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    __NAMES = {'CO', 'CO2', 'NO', 'NO2', 'O3', 'SO2'}
+    __NAMES = {'CO', 'CO2', 'NO', 'NO2', 'O3', 'Ox', 'SO2'}
 
     @classmethod
     def is_valid_name(cls, name):
         return name in cls.__NAMES
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     __MOLAR_DENSITY_STP = {
                 'CO':   1.1642,
                 'CO2':  1.9600,
                 'NO':   1.3402,
                 'NO2':  1.9125,
                 'O3':   1.9957,
+                'Ox':   1.9957,
                 'SO2':  2.6609
     }
 
     @classmethod
     def __molar_density_stp(cls, gas):
         if gas not in cls.__MOLAR_DENSITY_STP:
             raise ValueError("Gas: unrecognised name: %s" % gas)
@@ -55,14 +58,15 @@
 
     __MOLAR_MASS = {
                 'CO':   28.0100,
                 'CO2':  44.0100,
                 'NO':   30.0100,
                 'NO2':  46.0055,
                 'O3':   48.0000,
+                'Ox':   48.0000,
                 'SO2':  64.0660
     }
 
     @classmethod
     def __molar_mass(cls, gas):
         if gas not in cls.__MOLAR_MASS:
             raise ValueError("Gas: unrecognised name: %s" % gas)
```

### Comparing `scs-core-2.8.4/src/scs_core/gas/isi/isi_datum.py` & `scs-core-2.8.9/src/scs_core/gas/isi/isi_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/minimum.py` & `scs-core-2.8.9/src/scs_core/gas/minimum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/ndir/ndir.py` & `scs-core-2.8.9/src/scs_core/gas/ndir/ndir.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/ndir/ndir_conf.py` & `scs-core-2.8.9/src/scs_core/gas/ndir/ndir_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/ndir/ndir_datum.py` & `scs-core-2.8.9/src/scs_core/gas/ndir/ndir_version.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,118 +1,138 @@
 """
-Created on 20 Jun 2017
+Created on 2 Jan 2018
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-Alphasense A4 IRC-AT non-dispersive infra-red detector
+document example:
+version: {"id": "SCS NDIR Type 001", "tag": "001.001.001"}
 """
 
 from collections import OrderedDict
-from numbers import Number
 
-from scs_core.data.datum import Datum
 from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class NDIRDatum(JSONable):
+class NDIRVersion(JSONable):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
-        temp = jdict.get('tmp')
-        cnc = jdict.get('cnc-raw')
-        cnc_igl = jdict.get('cnc')
+        id = jdict.get('id')
+        tag = NDIRTag.construct_from_jdict(jdict.get('tag'))
 
-        return NDIRDatum(temp, cnc, cnc_igl)
+        return NDIRVersion(id, tag)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, temp, cnc, cnc_igl):
+    def __init__(self, id, tag):
         """
         Constructor
         """
-        self.__temp = Datum.float(temp, 1)              # temperature                               °C
-        self.__cnc = Datum.float(cnc, 1)                # concentration                             ppm
-        self.__cnc_igl = Datum.float(cnc_igl, 1)        # concentration (ideal gas law corrected)   ppm
+        self.__id = id                                  # string
+        self.__tag = tag                                # NDIRTag
 
 
-    def __eq__(self, other):
-        try:
-            return self.temp == other.temp and self.cnc == other.cnc and self.cnc_igl == other.cnc_igl
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def as_json(self):
+        jdict = OrderedDict()
 
-        except AttributeError:
-            return False
+        jdict['id'] = self.id
+        jdict['tag'] = self.tag
+
+        return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
-    # Support for averaging...
 
-    def __add__(self, other):
-        if not isinstance(other, self.__class__):
-            raise TypeError(other)
+    @property
+    def id(self):
+        return self.__id
 
-        temp = self.temp + other.temp
-        cnc = self.cnc + other.cnc
-        cnc_igl = self.cnc_igl + other.cnc_igl
 
-        return NDIRDatum(temp, cnc, cnc_igl)
+    @property
+    def tag(self):
+        return self.__tag
 
 
-    def __truediv__(self, other):
-        if not isinstance(other, Number):
-            raise TypeError(other)
+    # ----------------------------------------------------------------------------------------------------------------
 
-        temp = self.temp / other
-        cnc = None if self.cnc is None else self.cnc / other
-        cnc_igl = None if self.cnc_igl is None else self.cnc_igl / other
+    def __str__(self, *args, **kwargs):
+        return "NDIRVersion:{id:%s, tag:%s}" % (self.id, self.tag)
 
-        return NDIRDatum(temp, cnc, cnc_igl)
 
+# --------------------------------------------------------------------------------------------------------------------
+
+class NDIRTag(JSONable):
+    """
+    classdocs
+    """
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
-        jdict = OrderedDict()
+    @classmethod
+    def construct_from_jdict(cls, jdict):
+        if not jdict:
+            return None
 
-        jdict['tmp'] = self.temp
-        jdict['cnc-raw'] = self.cnc
-        jdict['cnc'] = self.cnc_igl
+        items = jdict.split('.')
 
-        return jdict
+        try:
+            device = int(items[0])
+            api = int(items[1])
+            patch = int(items[2])
+
+        except ValueError:
+            return None
+
+        return NDIRTag(device, api, patch)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @property
-    def temp(self):
-        return self.__temp
+    def __init__(self, device, api, patch):
+        """
+        Constructor
+        """
+        self.__device = device                  # int
+        self.__api = api                        # int
+        self.__patch = patch                    # int
+
+
+    # ----------------------------------------------------------------------------------------------------------------
 
+    def as_json(self):
+        return '.'.join((str(self.device), str(self.api), str(self.patch)))
+
+
+    # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def cnc(self):
-        return self.__cnc
+    def device(self):
+        return self.__device
 
 
     @property
-    def co2(self):              # a synonym of cnc for compatibility with GasesSample and SCD30Datum
-        return self.cnc_igl
+    def api(self):
+        return self.__api
 
 
     @property
-    def cnc_igl(self):
-        return self.__cnc_igl
+    def patch(self):
+        return self.__patch
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "NDIRDatum:{temp:%s, cnc:%s, cnc_igl:%s}" % (self.temp, self.cnc, self.cnc_igl)
+        return "NDIRTag:{device:%s, api:%s, patch:%s}" % (self.device, self.api, self.patch)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scs-core-2.8.4/src/scs_core/gas/ndir/ndir_version.py` & `scs-core-2.8.9/src/scs_core/gas/pid/pid_datum.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,135 @@
 """
-Created on 2 Jan 2018
+Created on 19 Sep 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
-
-document example:
-version: {"id": "SCS NDIR Type 001", "tag": "001.001.001"}
 """
 
 from collections import OrderedDict
 
+from scs_core.data.datum import Datum
 from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class NDIRVersion(JSONable):
+class PIDDatum(JSONable):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
-        id = jdict.get('id')
-        tag = NDIRTag.construct_from_jdict(jdict.get('tag'))
+        we_v = jdict.get('weV')
 
-        return NDIRVersion(id, tag)
+        we_c = jdict.get('weC')
+        cnc = jdict.get('cnc')
 
+        return cls(we_v, we_c, cnc)
 
-    # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, id, tag):
-        """
-        Constructor
-        """
-        self.__id = id                                  # string
-        self.__tag = tag                                # NDIRTag
+    @classmethod
+    def construct(cls, calib, baseline, tc, temp, we_v):
+        if calib is None or tc is None:
+            return PIDDatum(we_v)
 
+        # weC...
+        we_c = cls.__we_c(calib, tc, temp, we_v)
 
-    # ----------------------------------------------------------------------------------------------------------------
+        if we_c is None:
+            return PIDDatum(we_v)
 
-    def as_json(self):
-        jdict = OrderedDict()
+        # cnc...
+        cnc = cls.__cnc(calib, we_c)
 
-        jdict['id'] = self.id
-        jdict['tag'] = self.tag
+        baselined_cnc = cnc + baseline.offset               # a positive offset causes the value to be raised
 
-        return jdict
+        return cls(we_v, we_c, baselined_cnc)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @property
-    def id(self):
-        return self.__id
-
-
-    @property
-    def tag(self):
-        return self.__tag
-
+    @classmethod
+    def __we_c(cls, calib, tc, temp, we_v):
+        """
+        Compute weC from sensor temperature compensation of weV
+        """
+        offset_v = calib.pid_elc_mv / 1000.0
 
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def __str__(self, *args, **kwargs):
-        return "NDIRVersion:{id:%s, tag:%s}" % (self.id, self.tag)
+        response_v = we_v - offset_v                    # remove electronic zero
+        response_c = tc.correct(temp, response_v)       # correct the response component
 
+        if response_c is None:
+            return None
 
-# --------------------------------------------------------------------------------------------------------------------
+        we_c = response_c + offset_v                    # replace electronic zero
 
-class NDIRTag(JSONable):
-    """
-    classdocs
-    """
+        return we_c
 
-    # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_jdict(cls, jdict):
-        if not jdict:
+    def __cnc(cls, calib, we_c):
+        """
+        Compute cnc from weC
+        """
+        if we_c is None:
             return None
 
-        items = jdict.split('.')
-
-        try:
-            device = int(items[0])
-            api = int(items[1])
-            patch = int(items[2])
+        offset_v = calib.pid_elc_mv / 1000.0
 
-        except ValueError:
-            return None
+        response_c = we_c - offset_v                    # remove electronic zero
+        cnc = response_c / calib.pid_sens_v_ppb         # units are Volts / ppb
 
-        return NDIRTag(device, api, patch)
+        return cnc
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, device, api, patch):
+    def __init__(self, we_v, we_c=None, cnc=None):
         """
         Constructor
         """
-        self.__device = device                  # int
-        self.__api = api                        # int
-        self.__patch = patch                    # int
+        self.__we_v = Datum.float(we_v, 5)              # uncorrected working electrode output      Volts
+
+        self.__we_c = Datum.float(we_c, 5)              # corrected working electrode voltage       Volts
+        self.__cnc = Datum.float(cnc, 1)                # gas concentration                         ppb
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
-        return '.'.join((str(self.device), str(self.api), str(self.patch)))
+        jdict = OrderedDict()
+
+        jdict['weV'] = self.we_v
+
+        jdict['weC'] = self.we_c                        # may be None
+        jdict['cnc'] = self.cnc                         # may be None
+
+        return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def device(self):
-        return self.__device
+    def we_v(self):
+        return self.__we_v
 
 
     @property
-    def api(self):
-        return self.__api
+    def we_c(self):
+        return self.__we_c
 
 
     @property
-    def patch(self):
-        return self.__patch
+    def cnc(self):
+        return self.__cnc
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "NDIRTag:{device:%s, api:%s, patch:%s}" % (self.device, self.api, self.patch)
+        return "PIDDatum:{we_v:%0.6f, we_c:%s, cnc:%s}" % (self.we_v, self.we_c, self.cnc)
```

### Comparing `scs-core-2.8.4/src/scs_core/gas/ndir/ndir_voltages.py` & `scs-core-2.8.9/src/scs_core/gas/ndir/ndir_voltages.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/pid/pid.py` & `scs-core-2.8.9/src/scs_core/gas/pid/pid.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/pid/pid_calib.py` & `scs-core-2.8.9/src/scs_core/gas/pid/pid_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/pid/pid_calibrated_datum.py` & `scs-core-2.8.9/src/scs_core/gas/pid/pid_calibrated_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/pid/pid_datum.py` & `scs-core-2.8.9/src/scs_core/position/gps_datum.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,153 @@
 """
-Created on 19 Sep 2016
+Created on 10 Jan 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
+
+https://www.nmea.org
+https://en.wikipedia.org/wiki/NMEA_0183
+
+reference coordinate systems:
+https://en.wikipedia.org/wiki/World_Geodetic_System#WGS84
+https://en.wikipedia.org/wiki/PZ-90
 """
 
 from collections import OrderedDict
+from numbers import Number
 
 from scs_core.data.datum import Datum
-from scs_core.data.json import JSONable
+from scs_core.data.json import JSONReport
+
+from scs_core.position.position import Position
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class PIDDatum(JSONable):
+class GPSDatum(JSONReport):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_jdict(cls, jdict):
+    def construct_from_jdict(cls, jdict, skeleton=False):
         if not jdict:
-            return None
+            return cls.null_datum()
 
-        we_v = jdict.get('weV')
+        pos = Position.construct_from_jdict(jdict.get('pos'))
+        elv = jdict.get('elv')
 
-        we_c = jdict.get('weC')
-        cnc = jdict.get('cnc')
+        quality = jdict.get('qual')
 
-        return cls(we_v, we_c, cnc)
+        return cls(pos, elv, quality)
 
 
     @classmethod
-    def construct(cls, calib, baseline, tc, temp, we_v):
-        if calib is None or tc is None:
-            return PIDDatum(we_v)
+    def construct_from_gga(cls, gga):
+        if gga is None:
+            return None
 
-        # weC...
-        we_c = cls.__we_c(calib, tc, temp, we_v)
+        pos = Position.construct_from_gga(gga)
+        elv = None if gga.alt is None else round(gga.alt)
 
-        if we_c is None:
-            return PIDDatum(we_v)
+        quality = gga.quality
 
-        # cnc...
-        cnc = cls.__cnc(calib, we_c)
+        return cls(pos, elv, quality)
 
-        baselined_cnc = cnc + baseline.offset               # a positive offset causes the value to be raised
 
-        return cls(we_v, we_c, baselined_cnc)
+    @classmethod
+    def null_datum(cls):
+        return cls(Position(None, None), None, None)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @classmethod
-    def __we_c(cls, calib, tc, temp, we_v):
+    def __init__(self, pos, elv, quality):
         """
-        Compute weC from sensor temperature compensation of weV
+        Constructor
         """
-        offset_v = calib.pid_elc_mv / 1000.0
+        self.__pos = pos                            # Position
+        self.__elv = Datum.float(elv, 1)            # metres above mean sea level
 
-        response_v = we_v - offset_v                    # remove electronic zero
-        response_c = tc.correct(temp, response_v)       # correct the response component
+        self.__quality = quality                    # number or None
 
-        if response_c is None:
-            return None
 
-        we_c = response_c + offset_v                    # replace electronic zero
+    # ----------------------------------------------------------------------------------------------------------------
+    # Support for averaging...
 
-        return we_c
+    def __add__(self, other):
+        if not isinstance(other, self.__class__):
+            raise TypeError(other)
 
+        pos = self.pos + other.pos
+        elv = self.elv + other.elv
 
-    @classmethod
-    def __cnc(cls, calib, we_c):
-        """
-        Compute cnc from weC
-        """
-        if we_c is None:
-            return None
+        quality = self.quality + other.quality
+
+        return GPSDatum(pos, elv, quality)
 
-        offset_v = calib.pid_elc_mv / 1000.0
 
-        response_c = we_c - offset_v                    # remove electronic zero
-        cnc = response_c / calib.pid_sens_v_ppb         # units are Volts / ppb
+    def __truediv__(self, other):
+        if not isinstance(other, Number):
+            raise TypeError(other)
 
-        return cnc
+        pos = self.pos / other
+        elv = self.elv / other
+
+        quality = self.quality / other
+
+        return GPSDatum(pos, elv, quality)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, we_v, we_c=None, cnc=None):
-        """
-        Constructor
-        """
-        self.__we_v = Datum.float(we_v, 5)              # uncorrected working electrode output      Volts
+    def distance(self, other_pos, minimum_acceptable_quality=None):
+        if self.pos is None:
+            return None
 
-        self.__we_c = Datum.float(we_c, 5)              # corrected working electrode voltage       Volts
-        self.__cnc = Datum.float(cnc, 1)                # gas concentration                         ppb
+        if minimum_acceptable_quality is not None:
+            if self.quality is None or round(self.quality) < minimum_acceptable_quality:
+                return None
+
+        return self.pos.distance(other_pos)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
-        jdict['weV'] = self.we_v
+        jdict['pos'] = self.pos
+        jdict['elv'] = None if self.elv is None else round(self.elv, 1)
 
-        jdict['weC'] = self.we_c                        # may be None
-        jdict['cnc'] = self.cnc                         # may be None
+        jdict['qual'] = None if self.quality is None else round(self.quality, 1)
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def we_v(self):
-        return self.__we_v
+    def pos(self):
+        return self.__pos
 
 
     @property
-    def we_c(self):
-        return self.__we_c
+    def elv(self):
+        return self.__elv
 
 
     @property
-    def cnc(self):
-        return self.__cnc
+    def quality(self):
+        return self.__quality
+
+
+    @quality.setter
+    def quality(self, quality):
+        self.__quality = quality
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "PIDDatum:{we_v:%0.6f, we_c:%s, cnc:%s}" % (self.we_v, self.we_c, self.cnc)
+        return "GPSDatum:{pos:%s, elv:%s, quality:%s}" % (self.pos, self.elv, self.quality)
```

### Comparing `scs-core-2.8.4/src/scs_core/gas/pid/pid_temp_comp.py` & `scs-core-2.8.9/src/scs_core/gas/pid/pid_temp_comp.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/scd30/scd30_baseline.py` & `scs-core-2.8.9/src/scs_core/gas/scd30/scd30_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/scd30/scd30_conf.py` & `scs-core-2.8.9/src/scs_core/gas/scd30/scd30_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/scd30/scd30_datum.py` & `scs-core-2.8.9/src/scs_core/gas/scd30/scd30_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/sensor.py` & `scs-core-2.8.9/src/scs_core/gas/sensor.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/sensor_baseline.py` & `scs-core-2.8.9/src/scs_core/gas/sensor_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gas/sensor_calib.py` & `scs-core-2.8.9/src/scs_core/gas/sensor_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/gps/gps_conf.py` & `scs-core-2.8.9/src/scs_core/gps/gps_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/interface/interface_conf.py` & `scs-core-2.8.9/src/scs_core/interface/interface_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/led/led.py` & `scs-core-2.8.9/src/scs_core/led/led.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/led/led_state.py` & `scs-core-2.8.9/src/scs_core/led/led_state.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/location/timezone.py` & `scs-core-2.8.9/src/scs_core/location/timezone.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/location/timezone_conf.py` & `scs-core-2.8.9/src/scs_core/location/timezone_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/location/timezone_offset.py` & `scs-core-2.8.9/src/scs_core/location/timezone_offset.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/catalogue/model_compendium.py` & `scs-core-2.8.9/src/scs_core/model/catalogue/model_compendium.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/catalogue/model_compendium_group.py` & `scs-core-2.8.9/src/scs_core/model/catalogue/model_compendium_group.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/catalogue/term.py` & `scs-core-2.8.9/src/scs_core/model/catalogue/term.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/catalogue/training_period.py` & `scs-core-2.8.9/src/scs_core/model/catalogue/training_period.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/gas/baseline.py` & `scs-core-2.8.9/src/scs_core/model/gas/baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/gas/gas_baseline.py` & `scs-core-2.8.9/src/scs_core/model/gas/gas_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/gas/gas_inference_client.py` & `scs-core-2.8.9/src/scs_core/model/gas/gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/gas/gas_model_conf.py` & `scs-core-2.8.9/src/scs_core/model/gas/gas_model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/gas/s1/gas_request.py` & `scs-core-2.8.9/src/scs_core/model/gas/s1/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/gas/s1/s1_gas_inference_client.py` & `scs-core-2.8.9/src/scs_core/model/gas/s1/s1_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/gas/vB/gas_request.py` & `scs-core-2.8.9/src/scs_core/model/gas/vB/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/gas/vB/vb_gas_inference_client.py` & `scs-core-2.8.9/src/scs_core/model/gas/vB/vb_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/gas/vE/gas_request.py` & `scs-core-2.8.9/src/scs_core/model/gas/vE/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/gas/vE/ve_gas_inference_client.py` & `scs-core-2.8.9/src/scs_core/model/gas/vE/ve_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/gas/vcal_baseline.py` & `scs-core-2.8.9/src/scs_core/model/gas/vcal_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/model_conf.py` & `scs-core-2.8.9/src/scs_core/model/model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/pmx/pmx_inference_client.py` & `scs-core-2.8.9/src/scs_core/model/pmx/pmx_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/pmx/pmx_model_conf.py` & `scs-core-2.8.9/src/scs_core/model/pmx/pmx_model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/pmx/s1/pmx_request.py` & `scs-core-2.8.9/src/scs_core/model/pmx/s1/pmx_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py` & `scs-core-2.8.9/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/monitor/monitor_error.py` & `scs-core-2.8.9/src/scs_core/monitor/monitor_error.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/monitor/monitor_request.py` & `scs-core-2.8.9/src/scs_core/monitor/monitor_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/monitor/monitor_response.py` & `scs-core-2.8.9/src/scs_core/monitor/monitor_response.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/particulate/opc_conf.py` & `scs-core-2.8.9/src/scs_core/particulate/opc_conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 Created on 11 Jul 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 settings for OPCMonitor
 
 example JSON:
-{"model": "N3", "sample-period": 10, "restart-on-zeroes": true, "power-saving": false}
+{"model": "N3", "sample-period": 10, "restart-on-zeroes": true, "power-saving": false,
+"custom-dev-path": "/dev/spi/by-connector/H3"}
 """
 
 from collections import OrderedDict
 
 from scs_core.data.json import MultiPersistentJSONable
 
 
@@ -31,15 +32,15 @@
 
 
     @classmethod
     def load(cls, manager, name=None, encryption_key=None, skeleton=False):
         conf = super().load(manager, name=name, encryption_key=encryption_key, skeleton=skeleton)
 
         if conf:
-            conf.__dev_path = manager.opc_spi_dev_path()
+            conf.__default_dev_path = manager.opc_spi_dev_path()
 
         return conf
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
@@ -48,40 +49,41 @@
             return None
 
         model = jdict.get('model')
         sample_period = jdict.get('sample-period')
         restart_on_zeroes = jdict.get('restart-on-zeroes', True)
         power_saving = jdict.get('power-saving')
 
-        dev_path = jdict.get('dev_path')
+        custom_dev_path = jdict.get('custom-dev-path')
 
-        return cls(model, sample_period, restart_on_zeroes, power_saving, dev_path, name=name)
+        return cls(model, sample_period, restart_on_zeroes, power_saving, custom_dev_path, name=name)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, model, sample_period, restart_on_zeroes, power_saving, dev_path, name=None):
+    def __init__(self, model, sample_period, restart_on_zeroes, power_saving, custom_dev_path, name=None):
         """
         Constructor
         """
         super().__init__(name)
 
         self.__model = model                                        # string
         self.__sample_period = int(sample_period)                   # int
         self.__restart_on_zeroes = bool(restart_on_zeroes)          # bool
         self.__power_saving = bool(power_saving)                    # bool
 
-        self.__dev_path = dev_path                                  # string
+        self.__default_dev_path = None                              # string
+        self.__custom_dev_path = custom_dev_path                    # string
 
 
     def __eq__(self, other):                            # ignore name
         try:
             return self.model == other.model and self.sample_period == other.sample_period and \
                    self.restart_on_zeroes == other.restart_on_zeroes and self.power_saving == other.power_saving and \
-                   self.dev_path == other.dev_path
+                   self.custom_dev_path == other.custom_dev_path
 
         except (TypeError, AttributeError):
             return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
@@ -120,33 +122,43 @@
     @property
     def restart_on_zeroes(self):
         return self.__restart_on_zeroes
 
 
     @property
     def dev_path(self):
-        return self.__dev_path
+        return self.default_dev_path if self.custom_dev_path is None else self.custom_dev_path
+
+
+    @property
+    def default_dev_path(self):
+        return self.__default_dev_path
+
+
+    @property
+    def custom_dev_path(self):
+        return self.__custom_dev_path
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
         jdict['model'] = self.model
         jdict['sample-period'] = self.sample_period
         jdict['restart-on-zeroes'] = self.restart_on_zeroes
         jdict['power-saving'] = self.power_saving
 
-        if self.__dev_path is not None:
-            jdict['dev_path'] = self.dev_path
+        if self.custom_dev_path is not None:
+            jdict['custom-dev-path'] = self.custom_dev_path
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
         return "OPCConf(core):{name:%s, model:%s, sample_period:%s, restart_on_zeroes:%s, power_saving:%s, " \
-               "dev_path:%s}" %  \
+               "default_dev_path:%s, custom_dev_path:%s}" %  \
                (self.name, self.model, self.sample_period, self.restart_on_zeroes, self.power_saving,
-                self.dev_path)
+                self.default_dev_path, self.custom_dev_path)
```

### Comparing `scs-core-2.8.4/src/scs_core/particulate/opc_datum.py` & `scs-core-2.8.9/src/scs_core/particulate/opc_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/particulate/opc_version.py` & `scs-core-2.8.9/src/scs_core/particulate/opc_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/particulate/pmx_datum.py` & `scs-core-2.8.9/src/scs_core/particulate/pmx_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/particulate/sps_datum.py` & `scs-core-2.8.9/src/scs_core/particulate/sps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/position/gps_datum.py` & `scs-core-2.8.9/src/scs_core/psu/psu_conf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,153 +1,149 @@
 """
-Created on 10 Jan 2017
+Created on 21 Jun 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-https://www.nmea.org
-https://en.wikipedia.org/wiki/NMEA_0183
+specifies which PSU is present, if any
 
-reference coordinate systems:
-https://en.wikipedia.org/wiki/World_Geodetic_System#WGS84
-https://en.wikipedia.org/wiki/PZ-90
+example JSON:
+{"model": "MobileV2", "batt-model": "PackV1", "ignore-threshold": true, "reporting-interval": 10,
+"report-file": "/tmp/southcoastscience/psu_status_report.json"}
 """
 
 from collections import OrderedDict
-from numbers import Number
 
-from scs_core.data.datum import Datum
-from scs_core.data.json import JSONReport
-
-from scs_core.position.position import Position
+from scs_core.data.json import PersistentJSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class GPSDatum(JSONReport):
+class PSUConf(PersistentJSONable):
     """
     classdocs
     """
 
-    # ----------------------------------------------------------------------------------------------------------------
+    __DEFAULT_REPORTING_INTERVAL = 10               # seconds
 
-    @classmethod
-    def construct_from_jdict(cls, jdict, skeleton=False):
-        if not jdict:
-            return cls.null_datum()
+    __FILENAME = "psu_conf.json"
 
-        pos = Position.construct_from_jdict(jdict.get('pos'))
-        elv = jdict.get('elv')
-
-        quality = jdict.get('qual')
+    @classmethod
+    def persistence_location(cls):
+        return cls.conf_dir(), cls.__FILENAME
 
-        return cls(pos, elv, quality)
 
+    # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_gga(cls, gga):
-        if gga is None:
+    def construct_from_jdict(cls, jdict, skeleton=False):
+        if not jdict:
             return None
 
-        pos = Position.construct_from_gga(gga)
-        elv = None if gga.alt is None else round(gga.alt)
-
-        quality = gga.quality
+        psu_model = jdict.get('model')
+        batt_model = jdict.get('batt-model')
+        ignore_threshold = jdict.get('ignore-threshold', False)
 
-        return cls(pos, elv, quality)
+        reporting_interval = jdict.get('reporting-interval', cls.__DEFAULT_REPORTING_INTERVAL)
+        report_file = jdict.get('report-file')
 
-
-    @classmethod
-    def null_datum(cls):
-        return cls(Position(None, None), None, None)
+        return cls(psu_model, batt_model, ignore_threshold, reporting_interval, report_file)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, pos, elv, quality):
+    def __init__(self, psu_model, batt_model, ignore_threshold, reporting_interval, report_file):
         """
         Constructor
         """
-        self.__pos = pos                            # Position
-        self.__elv = Datum.float(elv, 1)            # metres above mean sea level
-
-        self.__quality = quality                    # number or None
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-    # Support for averaging...
+        super().__init__()
 
-    def __add__(self, other):
-        if not isinstance(other, self.__class__):
-            raise TypeError(other)
+        self.__psu_model = psu_model                                        # string
+        self.__batt_model = batt_model                                      # string
+        self.__ignore_threshold = ignore_threshold                          # bool
 
-        pos = self.pos + other.pos
-        elv = self.elv + other.elv
+        self.__reporting_interval = int(reporting_interval)                 # int
+        self.__report_file = report_file                                    # string
 
-        quality = self.quality + other.quality
 
-        return GPSDatum(pos, elv, quality)
+    def __eq__(self, other):
+        try:
+            return self.psu_model == other.psu_model and \
+                   self.batt_model == other.batt_model and \
+                   self.ignore_threshold == other.ignore_threshold and \
+                   self.reporting_interval == other.reporting_interval and \
+                   self.report_file == other.report_file
 
+        except (TypeError, AttributeError):
+            return False
 
-    def __truediv__(self, other):
-        if not isinstance(other, Number):
-            raise TypeError(other)
 
-        pos = self.pos / other
-        elv = self.elv / other
+    # ----------------------------------------------------------------------------------------------------------------
 
-        quality = self.quality / other
+    # noinspection PyMethodMayBeStatic,PyUnusedLocal
+    def psu(self, host, interface_model):
+        return None
 
-        return GPSDatum(pos, elv, quality)
 
+    # noinspection PyMethodMayBeStatic,PyUnusedLocal
+    def psu_monitor(self, host, interface_model, ignore_standby):
+        return None
 
-    # ----------------------------------------------------------------------------------------------------------------
 
-    def distance(self, other_pos, minimum_acceptable_quality=None):
-        if self.pos is None:
-            return None
+    # noinspection PyMethodMayBeStatic
+    def psu_class(self):
+        return None
 
-        if minimum_acceptable_quality is not None:
-            if self.quality is None or round(self.quality) < minimum_acceptable_quality:
-                return None
 
-        return self.pos.distance(other_pos)
+    # noinspection PyMethodMayBeStatic
+    def psu_report_class(self):
+        return None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
-        jdict = OrderedDict()
+    @property
+    def psu_model(self):
+        return self.__psu_model
 
-        jdict['pos'] = self.pos
-        jdict['elv'] = None if self.elv is None else round(self.elv, 1)
 
-        jdict['qual'] = None if self.quality is None else round(self.quality, 1)
+    @property
+    def batt_model(self):
+        return self.__batt_model
 
-        return jdict
 
+    @property
+    def ignore_threshold(self):
+        return self.__ignore_threshold
 
-    # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def pos(self):
-        return self.__pos
+    def report_file(self):
+        return self.__report_file
 
 
     @property
-    def elv(self):
-        return self.__elv
+    def reporting_interval(self):
+        return self.__reporting_interval
 
 
-    @property
-    def quality(self):
-        return self.__quality
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def as_json(self):
+        jdict = OrderedDict()
 
+        jdict['model'] = self.__psu_model
+        jdict['batt-model'] = self.__batt_model
+        jdict['ignore-threshold'] = self.__ignore_threshold
 
-    @quality.setter
-    def quality(self, quality):
-        self.__quality = quality
+        jdict['reporting-interval'] = self.__reporting_interval
+        jdict['report-file'] = self.__report_file
+
+        return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "GPSDatum:{pos:%s, elv:%s, quality:%s}" % (self.pos, self.elv, self.quality)
+        return "PSUConf(core):{psu_model:%s, batt_model:%s, ignore_threshold:%s, reporting_interval:%s, " \
+               "report_file:%s}" % \
+               (self.psu_model, self.batt_model, self.ignore_threshold, self.reporting_interval,
+                self.report_file)
```

### Comparing `scs-core-2.8.4/src/scs_core/position/nmea/gpdatetime.py` & `scs-core-2.8.9/src/scs_core/position/nmea/gpdatetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/position/nmea/gpgga.py` & `scs-core-2.8.9/src/scs_core/position/nmea/gpgga.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/position/nmea/gpgll.py` & `scs-core-2.8.9/src/scs_core/position/nmea/gpgll.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/position/nmea/gpgsa.py` & `scs-core-2.8.9/src/scs_core/position/nmea/gpgsa.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/position/nmea/gpgsv.py` & `scs-core-2.8.9/src/scs_core/position/nmea/gpgsv.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/position/nmea/gploc.py` & `scs-core-2.8.9/src/scs_core/position/nmea/gploc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/position/nmea/gprmc.py` & `scs-core-2.8.9/src/scs_core/position/nmea/gprmc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/position/nmea/gptime.py` & `scs-core-2.8.9/src/scs_core/position/nmea/gptime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/position/nmea/gpvtg.py` & `scs-core-2.8.9/src/scs_core/position/nmea/gpvtg.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/position/nmea/nmea_report.py` & `scs-core-2.8.9/src/scs_core/position/nmea/nmea_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/position/nmea/nmea_sentence.py` & `scs-core-2.8.9/src/scs_core/position/nmea/nmea_sentence.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/position/position.py` & `scs-core-2.8.9/src/scs_core/position/position.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/psu/psu.py` & `scs-core-2.8.9/src/scs_core/psu/psu.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/psu/psu_report.py` & `scs-core-2.8.9/src/scs_core/psu/psu_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/psu/psu_uptime.py` & `scs-core-2.8.9/src/scs_core/psu/psu_uptime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/psu/psu_version.py` & `scs-core-2.8.9/src/scs_core/psu/psu_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sample/climate_sample.py` & `scs-core-2.8.9/src/scs_core/sample/climate_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sample/configuration_sample.py` & `scs-core-2.8.9/src/scs_core/sample/configuration_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sample/gases_sample.py` & `scs-core-2.8.9/src/scs_core/sample/gases_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sample/particulates_sample.py` & `scs-core-2.8.9/src/scs_core/sample/particulates_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sample/pressure_sample.py` & `scs-core-2.8.9/src/scs_core/sample/pressure_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sample/sample.py` & `scs-core-2.8.9/src/scs_core/sample/sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sample/status_sample.py` & `scs-core-2.8.9/src/scs_core/sample/status_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sampler/sampler.py` & `scs-core-2.8.9/src/scs_core/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sync/interval_timer.py` & `scs-core-2.8.9/src/scs_core/sync/interval_timer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sync/line_reader.py` & `scs-core-2.8.9/src/scs_core/sync/line_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sync/runner.py` & `scs-core-2.8.9/src/scs_core/sync/runner.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sync/schedule.py` & `scs-core-2.8.9/src/scs_core/sync/schedule.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sync/synchronised_process.py` & `scs-core-2.8.9/src/scs_core/sync/synchronised_process.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sync/timed_runner.py` & `scs-core-2.8.9/src/scs_core/sync/timed_runner.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/command.py` & `scs-core-2.8.9/src/scs_core/sys/command.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,62 +6,86 @@
 https://pymotw.com/2/subprocess/
 """
 
 import sys
 
 from subprocess import Popen, PIPE
 
+from scs_core.sys.logging import Logging
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class Command(object):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, verbose):
         """
         Constructor
         """
-        self.__verbose = verbose                    # bool
+        self.__verbose = verbose                            # bool
+        self.__logger = Logging.getLogger()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def o(self, cmd_args, wait=False):
-        p = Popen(self.__cmd(cmd_args), stdout=PIPE)
+    def s(self, cmd_args, wait=True, no_verbose=False, abort_on_fail=True):
+        tokens = self.__cmd(cmd_args, no_verbose=no_verbose)
+        p = Popen(' '.join(tokens), shell=True)
 
-        if wait:
-            p.wait()
+        return self.__process(p, wait=wait, abort_on_fail=abort_on_fail)
 
-        return p
 
+    def o(self, cmd_args, wait=False, abort_on_fail=True):
+        tokens = self.__cmd(cmd_args)
+        p = Popen(tokens, stdout=PIPE)
 
-    def io(self, p, cmd_args, wait=False):
-        p = Popen(self.__cmd(cmd_args), stdin=p.stdout, stdout=PIPE)
+        return self.__process(p, wait=wait, abort_on_fail=abort_on_fail)
 
-        if wait:
-            p.wait()
 
-        return p
+    def io(self, p, cmd_args, wait=False, abort_on_fail=True):
+        tokens = self.__cmd(cmd_args)
+        p = Popen(tokens, stdin=p.stdout, stdout=PIPE)
+
+        return self.__process(p, wait=wait, abort_on_fail=abort_on_fail)
+
+
+    def i(self, p, cmd_args, wait=False, abort_on_fail=True):
+        tokens = self.__cmd(cmd_args)
+        p = Popen(tokens, stdin=p.stdout, stdout=sys.stderr)
 
+        return self.__process(p, wait=wait, abort_on_fail=abort_on_fail)
 
-    def i(self, p, cmd_args, wait=True):
-        p = Popen(self.__cmd(cmd_args), stdin=p.stdout, stdout=sys.stderr)
 
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def __cmd(self, cmd_args, no_verbose=False):
+        tokens = [str(cmd_arg) for cmd_arg in cmd_args if cmd_arg is not None]
+
+        if self.__verbose and not no_verbose:
+            tokens = tokens[:1] + ['-v'] + tokens[1:]
+
+        self.__logger.info(' '.join(tokens))
+
+        return tokens
+
+
+    def __process(self, p, wait=False, abort_on_fail=True):
         if wait:
             p.wait()
 
+        if abort_on_fail and p.returncode != 0:
+            self.__logger.error('ABORTED.')
+            exit(p.returncode)
 
-    def __cmd(self, cmd_args):
-        strs = [str(cmd_arg) for cmd_arg in cmd_args if cmd_arg is not None]
-
-        return strs[:1] + ['-v'] + strs[1:] if self.__verbose else strs
+        return p
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def verbose(self):
         return self.__verbose
```

### Comparing `scs-core-2.8.4/src/scs_core/sys/disk_usage.py` & `scs-core-2.8.9/src/scs_core/sys/disk_usage.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/disk_volume.py` & `scs-core-2.8.9/src/scs_core/sys/disk_volume.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/eeprom_image.py` & `scs-core-2.8.9/src/scs_core/sys/eeprom_image.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/exception_report.py` & `scs-core-2.8.9/src/scs_core/sys/exception_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/filesystem.py` & `scs-core-2.8.9/src/scs_core/sys/filesystem.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/ipv4_address.py` & `scs-core-2.8.9/src/scs_core/sys/ipv4_address.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/logging.py` & `scs-core-2.8.9/src/scs_core/sys/logging.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/memory.py` & `scs-core-2.8.9/src/scs_core/sys/memory.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/modem.py` & `scs-core-2.8.9/src/scs_core/sys/modem.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/network.py` & `scs-core-2.8.9/src/scs_core/sys/network.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/node.py` & `scs-core-2.8.9/src/scs_core/sys/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,14 +136,19 @@
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
     # identity...
 
+    @abstractmethod
+    def hostname_prefix(self):
+        pass
+
+
     @classmethod
     def numeric_component_of_name(cls):
         hostname = socket.gethostname()
         pieces = hostname.split('-')
 
         if len(pieces) != 3:
             raise ValueError(hostname)
```

### Comparing `scs-core-2.8.4/src/scs_core/sys/persistence_manager.py` & `scs-core-2.8.9/src/scs_core/sys/persistence_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/platform.py` & `scs-core-2.8.9/src/scs_core/sys/platform.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/process_comms.py` & `scs-core-2.8.9/src/scs_core/sys/process_comms.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/ps_datum.py` & `scs-core-2.8.9/src/scs_core/sys/ps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/serial.py` & `scs-core-2.8.9/src/scs_core/sys/serial.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/shared_secret.py` & `scs-core-2.8.9/src/scs_core/sys/shared_secret.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/signalled_exit.py` & `scs-core-2.8.9/src/scs_core/sys/signalled_exit.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/subprocess.py` & `scs-core-2.8.9/src/scs_core/sys/subprocess.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/system_id.py` & `scs-core-2.8.9/src/scs_core/sys/system_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -161,12 +161,17 @@
 
 
     @property
     def system_serial_number(self):
         return self.__system_serial_number
 
 
+    @system_serial_number.setter
+    def system_serial_number(self, system_serial_number):
+        self.__system_serial_number = system_serial_number
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
         return "SystemID:{vendor_id:%s, model_id:%s, model_name:%s, configuration:%s, system_serial_number:%s}" % \
                (self.vendor_id, self.model_id, self.model_name, self.configuration, self.system_serial_number)
```

### Comparing `scs-core-2.8.4/src/scs_core/sys/system_temp.py` & `scs-core-2.8.9/src/scs_core/sys/system_temp.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/tail.py` & `scs-core-2.8.9/src/scs_core/sys/tail.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/timeout.py` & `scs-core-2.8.9/src/scs_core/sys/timeout.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/timer.py` & `scs-core-2.8.9/src/scs_core/sys/timer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/trace_entry.py` & `scs-core-2.8.9/src/scs_core/sys/trace_entry.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core/sys/uptime_datum.py` & `scs-core-2.8.9/src/scs_core/sys/uptime_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.4/src/scs_core.egg-info/PKG-INFO` & `scs-core-2.8.9/src/scs_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-core
-Version: 2.8.4
+Version: 2.8.9
 Summary: The root of all South Coast Science environmental monitoring applications.
 Home-page: https://github.com/south-coast-science/scs_core
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scs-core-2.8.4/src/scs_core.egg-info/SOURCES.txt` & `scs-core-2.8.9/src/scs_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,15 @@
 src/scs_core/aws/data/alert.py
 src/scs_core/aws/data/byline.py
 src/scs_core/aws/data/byline_list.py
 src/scs_core/aws/data/dataset.py
 src/scs_core/aws/data/deployment.py
 src/scs_core/aws/data/device_monitor_email_list.py
 src/scs_core/aws/data/device_monitor_report.py
-src/scs_core/aws/data/device_report.py
-src/scs_core/aws/data/email_list.py
+src/scs_core/aws/data/device_monitor_specification.py
 src/scs_core/aws/data/http_response.py
 src/scs_core/aws/data/message.py
 src/scs_core/aws/data/power_list.py
 src/scs_core/aws/data/runtime_record.py
 src/scs_core/aws/data/status_list.py
 src/scs_core/aws/data/upload_interval.py
 src/scs_core/aws/data/uptime_list.py
@@ -149,26 +148,28 @@
 src/scs_core/data/average.py
 src/scs_core/data/categorical_regression.py
 src/scs_core/data/checkpoint_generator.py
 src/scs_core/data/crc.py
 src/scs_core/data/crypt.py
 src/scs_core/data/datetime.py
 src/scs_core/data/datum.py
+src/scs_core/data/diurnal_period.py
 src/scs_core/data/duplicates.py
 src/scs_core/data/histogram.py
 src/scs_core/data/interval.py
 src/scs_core/data/join.py
 src/scs_core/data/json.py
 src/scs_core/data/lin_regress.py
 src/scs_core/data/linear_regression.py
 src/scs_core/data/low_pass_filter.py
 src/scs_core/data/median_filter.py
 src/scs_core/data/min_list.py
 src/scs_core/data/model_delta.py
 src/scs_core/data/path_dict.py
+src/scs_core/data/period.py
 src/scs_core/data/precision.py
 src/scs_core/data/publication.py
 src/scs_core/data/queue_report.py
 src/scs_core/data/recurring_period.py
 src/scs_core/data/regression.py
 src/scs_core/data/rtc_datetime.py
 src/scs_core/data/sample_delta.py
@@ -180,14 +181,15 @@
 src/scs_core/display/__init__.py
 src/scs_core/display/display_conf.py
 src/scs_core/email/__init__.py
 src/scs_core/email/email_queue.py
 src/scs_core/email/email_queue_manager.py
 src/scs_core/estate/__init__.py
 src/scs_core/estate/baseline_conf.py
+src/scs_core/estate/baseline_conf_old.py
 src/scs_core/estate/configuration.py
 src/scs_core/estate/configuration_check.py
 src/scs_core/estate/git_pull.py
 src/scs_core/estate/git_pull_check.py
 src/scs_core/estate/mqtt_device_poller.py
 src/scs_core/estate/mqtt_peer.py
 src/scs_core/estate/package_version.py
@@ -333,14 +335,15 @@
 src/scs_core/sys/__init__.py
 src/scs_core/sys/command.py
 src/scs_core/sys/disk_usage.py
 src/scs_core/sys/disk_volume.py
 src/scs_core/sys/eeprom_image.py
 src/scs_core/sys/exception_report.py
 src/scs_core/sys/filesystem.py
+src/scs_core/sys/hostname.py
 src/scs_core/sys/ipv4_address.py
 src/scs_core/sys/logging.py
 src/scs_core/sys/memory.py
 src/scs_core/sys/modem.py
 src/scs_core/sys/network.py
 src/scs_core/sys/node.py
 src/scs_core/sys/persistence_manager.py
```

