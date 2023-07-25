# Comparing `tmp/satosacontrib.perun-3.8.0.tar.gz` & `tmp/satosacontrib.perun-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satosacontrib.perun-3.8.0.tar", last modified: Tue Jul 18 15:41:31 2023, max compression
+gzip compressed data, was "satosacontrib.perun-4.0.0.tar", last modified: Tue Jul 25 15:05:04 2023, max compression
```

## Comparing `satosacontrib.perun-3.8.0.tar` & `satosacontrib.perun-4.0.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:41:31.382076 satosacontrib.perun-3.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6068 2023-07-18 15:41:31.382076 satosacontrib.perun-3.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4921 2023-07-18 09:46:21.000000 satosacontrib.perun-3.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:41:31.338075 satosacontrib.perun-3.8.0/satosacontrib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:41:31.338075 satosacontrib.perun-3.8.0/satosacontrib/perun/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:41:31.338075 satosacontrib.perun-3.8.0/satosacontrib/perun/addons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/addons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1528 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/addons/extended_introspection_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:41:31.338075 satosacontrib.perun-3.8.0/satosacontrib/perun/backends/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/backends/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10129 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/backends/seznam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:41:31.354075 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/
--rw-rw-rw-   0 root         (0) root         (0)      727 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/auth_switcher_lite.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/compute_eligibility.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/context_attributes_microservice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:41:31.358075 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8313 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/additional_identifiers.py
--rw-rw-rw-   0 root         (0) root         (0)     5927 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    11822 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)    11268 2023-07-18 15:27:35.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     4831 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/perun_user.py
--rw-rw-rw-   0 root         (0) root         (0)    24791 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/sp_authorization.py
--rw-rw-rw-   0 root         (0) root         (0)    11491 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/is_banned_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3840 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2023-07-18 09:46:21.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     1594 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/persist_authorization_params_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2122 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/session_started_with_microservice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:41:31.378076 satosacontrib.perun-3.8.0/satosacontrib/perun/utils/
--rw-rw-rw-   0 root         (0) root         (0)     2042 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/utils/ConfigStore.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/utils/CurlConnector.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/utils/CurlConnectorInterface.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/utils/PerunConstants.py
--rw-rw-rw-   0 root         (0) root         (0)     6719 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/utils/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/satosacontrib/perun/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:41:31.338075 satosacontrib.perun-3.8.0/satosacontrib.perun.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6068 2023-07-18 15:41:31.000000 satosacontrib.perun-3.8.0/satosacontrib.perun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2591 2023-07-18 15:41:31.000000 satosacontrib.perun-3.8.0/satosacontrib.perun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 15:41:31.000000 satosacontrib.perun-3.8.0/satosacontrib.perun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-18 15:41:31.000000 satosacontrib.perun-3.8.0/satosacontrib.perun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-18 15:41:31.000000 satosacontrib.perun-3.8.0/satosacontrib.perun.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-18 15:41:31.382076 satosacontrib.perun-3.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-18 15:27:35.000000 satosacontrib.perun-3.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:41:31.382076 satosacontrib.perun-3.8.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10917 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/tests/test_additional_indentifiers.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/tests/test_auth_event_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     3329 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/tests/test_context_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/tests/test_is_banned.py
--rw-rw-rw-   0 root         (0) root         (0)     7500 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/tests/test_is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2535 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/tests/test_microservice_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     3981 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/tests/test_perun_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    14517 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/tests/test_perun_ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)     7106 2023-07-18 15:27:35.000000 satosacontrib.perun-3.8.0/tests/test_perun_entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     5482 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/tests/test_perun_user_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)    36568 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/tests/test_sp_authorization_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     7291 2023-07-18 09:10:38.000000 satosacontrib.perun-3.8.0/tests/test_update_ues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 15:05:04.337705 satosacontrib.perun-4.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6643 2023-07-25 15:05:04.337705 satosacontrib.perun-4.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2023-07-25 07:52:58.000000 satosacontrib.perun-4.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 15:05:04.125700 satosacontrib.perun-4.0.0/satosacontrib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 15:03:06.000000 satosacontrib.perun-4.0.0/satosacontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 15:05:04.125700 satosacontrib.perun-4.0.0/satosacontrib/perun/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 15:03:06.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 15:05:04.129700 satosacontrib.perun-4.0.0/satosacontrib/perun/addons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 15:03:06.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/addons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2023-07-24 11:19:52.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/addons/extended_introspection_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 15:05:04.129700 satosacontrib.perun-4.0.0/satosacontrib/perun/backends/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-24 11:19:52.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/backends/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10129 2023-07-24 11:19:52.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/backends/seznam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 15:05:04.133700 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5591 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-24 11:19:52.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/auth_switcher_lite.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/compute_eligibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/context_attributes_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3541 2023-07-25 07:52:58.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/forward_authorization_params_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 15:05:04.137700 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8313 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/additional_identifiers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5927 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11822 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)    11268 2023-07-24 11:19:52.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/is_banned_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     4827 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/perun_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    24787 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/sp_authorization.py
+-rw-rw-rw-   0 root         (0) root         (0)    11491 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2200 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2023-07-24 11:19:52.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/persist_authorization_params_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3881 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2122 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/session_started_with_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 15:05:04.137700 satosacontrib.perun-4.0.0/satosacontrib/perun/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     2070 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/utils/ConfigStore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4435 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/utils/CurlConnector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/utils/CurlConnectorInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/utils/PerunConstants.py
+-rw-rw-rw-   0 root         (0) root         (0)     6719 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/utils/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 15:03:06.000000 satosacontrib.perun-4.0.0/satosacontrib/perun/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 15:05:04.125700 satosacontrib.perun-4.0.0/satosacontrib.perun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6643 2023-07-25 15:05:03.000000 satosacontrib.perun-4.0.0/satosacontrib.perun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-07-25 15:05:04.000000 satosacontrib.perun-4.0.0/satosacontrib.perun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 15:05:03.000000 satosacontrib.perun-4.0.0/satosacontrib.perun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-25 15:05:03.000000 satosacontrib.perun-4.0.0/satosacontrib.perun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-25 15:05:03.000000 satosacontrib.perun-4.0.0/satosacontrib.perun.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-25 15:05:04.337705 satosacontrib.perun-4.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-25 07:52:58.000000 satosacontrib.perun-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 15:05:04.305704 satosacontrib.perun-4.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 15:03:06.000000 satosacontrib.perun-4.0.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10917 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/tests/test_additional_indentifiers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3650 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/tests/test_auth_event_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     3325 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/tests/test_context_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/tests/test_is_banned.py
+-rw-rw-rw-   0 root         (0) root         (0)     7500 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/tests/test_is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/tests/test_microservice_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/tests/test_perun_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    14517 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/tests/test_perun_ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)     7106 2023-07-24 11:19:52.000000 satosacontrib.perun-4.0.0/tests/test_perun_entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     5478 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/tests/test_perun_user_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)    36564 2023-07-25 11:54:35.000000 satosacontrib.perun-4.0.0/tests/test_sp_authorization_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     7291 2023-07-18 09:10:38.000000 satosacontrib.perun-4.0.0/tests/test_update_ues.py
```

### Comparing `satosacontrib.perun-3.8.0/LICENSE` & `satosacontrib.perun-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/PKG-INFO` & `satosacontrib.perun-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satosacontrib.perun
-Version: 3.8.0
+Version: 4.0.0
 Summary: Microservices for SATOSA authentication proxy, made by the Perun team
 Home-page: https://github.com/CESNET/satosacontrib.perun.git
 License: UNKNOWN
 Description: # satosacontrib.perun
         
         Microservices for [SATOSA](https://github.com/IdentityPython/SATOSA) authentication
         proxy, made by the Perun team.
@@ -45,14 +45,23 @@
         The microservice connects to database storing user bans and redirects banned users to configured URL.
         
         ### Persist authorization params microservice
         
         This request microservice retrieves configured parameters from GET or POST request (if available) and
         stores the values to internal context state.
         
+        ### Forward authorization params microservice
+        
+        This request microservice retrieves configured parameters from GET or POST request (if available) and
+        forwards them through a context parameter. Optionally, `default_values` can be
+        provided in the config file. These will be forwarded for configured SP and/or IdP if
+        not provided in the GET/POST request. If the parameter with preconfigured
+        default value is sent via GET/POST request anyway, the value form the request will be
+        used instead of the default.
+        
         ### Session started with microservice
         
         This Satosa microservice checks, if configured attribute's value is present
         in "session_started_with" values (retrieved by Persist authorization params microservice).
         If so, adds attribute with configured name. The value is expected to be converted
         to boolean by Attribute typing microservice.
```

### Comparing `satosacontrib.perun-3.8.0/README.md` & `satosacontrib.perun-4.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,23 @@
 The microservice connects to database storing user bans and redirects banned users to configured URL.
 
 ### Persist authorization params microservice
 
 This request microservice retrieves configured parameters from GET or POST request (if available) and
 stores the values to internal context state.
 
+### Forward authorization params microservice
+
+This request microservice retrieves configured parameters from GET or POST request (if available) and
+forwards them through a context parameter. Optionally, `default_values` can be
+provided in the config file. These will be forwarded for configured SP and/or IdP if
+not provided in the GET/POST request. If the parameter with preconfigured
+default value is sent via GET/POST request anyway, the value form the request will be
+used instead of the default.
+
 ### Session started with microservice
 
 This Satosa microservice checks, if configured attribute's value is present
 in "session_started_with" values (retrieved by Persist authorization params microservice).
 If so, adds attribute with configured name. The value is expected to be converted
 to boolean by Attribute typing microservice.
```

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/addons/extended_introspection_response.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/addons/extended_introspection_response.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/backends/seznam.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/backends/seznam.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/__init__.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 from .cardinality_single_microservice import CardinalitySingle
 from .context_attributes_microservice import ContextAttributes
 from .is_eligible_microservice import IsEligible
 from .multi_idphint_microservice import MultiIdpHinting
 from .nameid_attribute_microservice import NameIDAttribute
 from .compute_eligibility import ComputeEligibility
 
-from .is_banned_microservice import IsBanned
 from .proxystatistics_microservice import ProxyStatistics
 
 
 __all__ = [
     "CardinalitySingle",
     "ContextAttributes",
     "IsEligible",
     "MultiIdpHinting",
     "NameIDAttribute",
     "ProxyStatistics",
     "AuthEventLogging",
     "ComputeEligibility",
-    "IsBanned",
 ]
```

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,47 +31,48 @@
         self.logging_db = config["logging_db"]
         self.geolite_file_path = config["path_to_geolite2_city"]
         self.ip_address_header = config.get("ip_address_header", "REMOTE_ADDR")
         logger.info("AuthEventLogging is active")
 
     @staticmethod
     def __get_id_from_identifier(cnxn, metadata, identifier, name, table):
-        metadata.create_all(cnxn)
+        with cnxn.begin():
+            metadata.create_all(cnxn)
 
-        insert_stmt = insert(table).values(None, identifier, name)
-        if name is None or name == "":
-            insert_stmt = insert_stmt.on_conflict_do_nothing()
-        else:
-            insert_stmt = insert_stmt.on_conflict_do_update(
-                index_elements=["identifier"], set_=dict(name=name)
-            )
+            insert_stmt = insert(table).values(identifier=identifier, name=name)
+            if name is None or name == "":
+                insert_stmt = insert_stmt.on_conflict_do_nothing()
+            else:
+                insert_stmt = insert_stmt.on_conflict_do_update(
+                    index_elements=["identifier"], set_=dict(name=name)
+                )
 
-        cnxn.execute(insert_stmt)
+            cnxn.execute(insert_stmt)
 
-        result = select(getattr(table.columns, "id")).where(
-            table.columns.identifier == identifier
-        )
-        return result.scalar()
+            stmt = select(getattr(table.columns, "id")).where(
+                table.columns.identifier == identifier
+            )
+            result = cnxn.execute(stmt)
+            return result.scalar()
 
     @staticmethod
     def __get_id_from_foreign_table(cnxn, metadata, value, table):
-        metadata.create_all(cnxn)
+        with cnxn.begin():
+            metadata.create_all(cnxn)
 
-        insert_stmt = insert(table).values([None, value])
-        if value is None or value == "":
+            insert_stmt = insert(table).values(value=value)
             insert_stmt = insert_stmt.on_conflict_do_nothing()
-        else:
-            insert_stmt = insert_stmt.on_conflict_do_update(set_=dict(value=value))
 
-        cnxn.execute(insert_stmt)
+            cnxn.execute(insert_stmt)
 
-        result = select(getattr(table.columns, "id")).where(
-            table.columns.value == value
-        )
-        return result.scalar()
+            stmt = select(getattr(table.columns, "id")).where(
+                table.columns.value == value
+            )
+            result = cnxn.execute(stmt)
+            return result.scalar()
 
     def __get_location(self, ip):
         with database.Reader(self.geolite_file_path) as reader:
             response = reader.city(ip)
 
             return {"city": response.city.name, "country": response.country.name}
 
@@ -89,56 +90,55 @@
             context.KEY_AUTHN_CONTEXT_CLASS_REF
         ) or context.get_decoration(context.KEY_AUTHN_CONTEXT_CLASS_REF)
         upstream_acrs = data.auth_info["auth_class_ref"]
         user_agent_raw = context.http_headers.get("User-Agent")
         user_agent_parsed = json.dumps(str(parse(user_agent_raw)))
 
         engine = create_engine(self.logging_db)
-        cnxn = engine.connect()
-        metadata = Base.metadata
-        metadata.bind = cnxn
-        auth_event_logging = AuthEventLoggingTable().__table__
-
-        metadata.create_all(engine)
-
-        idp_id = self.__get_id_from_identifier(
-            cnxn, metadata, idp, "", LoggingIdpTable().__table__
-        )
-        sp_id = self.__get_id_from_identifier(
-            cnxn, metadata, sp, sp_name, LoggingSpTable().__table__
-        )
-        session_id_values_id = self.__get_id_from_foreign_table(
-            cnxn, metadata, session_id, SessionIdTable().__table__
-        )
-        requested_acrs_id = self.__get_id_from_foreign_table(
-            cnxn, metadata, requested_acrs, RequestedAcrsTable().__table__
-        )
-        upstream_acrs_id = self.__get_id_from_foreign_table(
-            cnxn, metadata, upstream_acrs, UpstreamAcrsTable().__table__
-        )
-        user_agent_raw_id = self.__get_id_from_foreign_table(
-            cnxn, metadata, user_agent_raw, UserAgentRawTable().__table__
-        )
-        user_agent_id = self.__get_id_from_foreign_table(
-            cnxn, metadata, user_agent_parsed, UserAgentTable().__table__
-        )
-
-        fields = {
-            "id": None,
-            "day": datetime.utcnow(),
-            "user": user,
-            "idp_id": idp_id,
-            "sp_id": sp_id,
-            "ip_address": ip_address,
-            "geolocation_city": geolocation_city,
-            "geolocation_country": geolocation_country,
-            "session_id": session_id_values_id,
-            "requested_acrs_id": requested_acrs_id,
-            "upstream_acrs_id": upstream_acrs_id,
-            "user_agent_raw_id": user_agent_raw_id,
-            "user_agent_id": user_agent_id,
-        }
+        with engine.connect() as cnxn:
+            metadata = Base.metadata
+            metadata.bind = cnxn
+            auth_event_logging = AuthEventLoggingTable().__table__
+
+            metadata.create_all(engine)
+
+            idp_id = self.__get_id_from_identifier(
+                cnxn, metadata, idp, "", LoggingIdpTable().__table__
+            )
+            sp_id = self.__get_id_from_identifier(
+                cnxn, metadata, sp, sp_name, LoggingSpTable().__table__
+            )
+            session_id_values_id = self.__get_id_from_foreign_table(
+                cnxn, metadata, session_id, SessionIdTable().__table__
+            )
+            requested_acrs_id = self.__get_id_from_foreign_table(
+                cnxn, metadata, requested_acrs, RequestedAcrsTable().__table__
+            )
+            upstream_acrs_id = self.__get_id_from_foreign_table(
+                cnxn, metadata, upstream_acrs, UpstreamAcrsTable().__table__
+            )
+            user_agent_raw_id = self.__get_id_from_foreign_table(
+                cnxn, metadata, user_agent_raw, UserAgentRawTable().__table__
+            )
+            user_agent_id = self.__get_id_from_foreign_table(
+                cnxn, metadata, user_agent_parsed, UserAgentTable().__table__
+            )
 
-        insert_stmt = insert(auth_event_logging).values(**fields)
-        cnxn.execute(insert_stmt)
+            fields = {
+                "day": datetime.utcnow(),
+                "user": user,
+                "idp_id": idp_id,
+                "sp_id": sp_id,
+                "ip_address": ip_address,
+                "geolocation_city": geolocation_city,
+                "geolocation_country": geolocation_country,
+                "session_id": session_id_values_id,
+                "requested_acrs_id": requested_acrs_id,
+                "upstream_acrs_id": upstream_acrs_id,
+                "user_agent_raw_id": user_agent_raw_id,
+                "user_agent_id": user_agent_id,
+            }
+            with cnxn.begin():
+                insert_stmt = insert(auth_event_logging).values(**fields)
+                cnxn.execute(insert_stmt)
 
         return super().process(context, data)
```

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/auth_switcher_lite.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/auth_switcher_lite.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/compute_eligibility.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/compute_eligibility.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/context_attributes_microservice.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/context_attributes_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/additional_identifiers.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/additional_identifiers.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/attributes.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/ensure_member.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/ensure_member.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/entitlement.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/entitlement.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/perun_user.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/perun_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 logger = logging.getLogger(__name__)
 
 
 class PerunUser(ResponseMicroService):
     def __init__(self, config, *args, **kwargs):
         super().__init__(*args, **kwargs)
         logger.info("PerunUser is active")
-        global_config = ConfigStore.get_global_cfg(config["global_cfg_filepath"])
+        global_config = ConfigStore.get_global_cfg(config["global_cfg_path"])
 
         self.__perun_user_id_attr = global_config["perun_user_id_attribute"]
         self.__perun_login_attribute = global_config["perun_login_attribute"]
         self.__allowed_requesters = global_config.get("allowed_requesters", {})
         self.__internal_login_attribute = config["internal_login_attribute"]
         self.__internal_extsource_attribute = config["internal_extsource_attribute"]
         self.__proxy_extsource_name = config["proxy_extsource_name"]
```

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/sp_authorization.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/sp_authorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 class SpAuthorization(ResponseMicroService):
     def __init__(self, config, *args, **kwargs):
         super().__init__(*args, **kwargs)
         logger.info(f"{SpAuthorization.__name__} is active")
         self.__DEBUG_PREFIX = self.name
         self.__endpoint = "/process"
         self.__config = config
-        self.__global_config = ConfigStore.get_global_cfg(config["global_cfg_filepath"])
+        self.__global_config = ConfigStore.get_global_cfg(config["global_cfg_path"])
         self.__signing_cfg = self.__global_config["jwk"]
         self.__allowed_requesters = self.__global_config.get("allowed_requesters", {})
 
         self.__filter_config = config["filter_config"]
 
         self.__CHECK_GROUP_MEMBERSHIP_ATTR = "check_group_membership_attr"
         self.__VO_SHORT_NAMES_ATTR = "vo_short_names_attr"
```

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/is_banned_microservice.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/idm/is_banned_microservice.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 from satosa.context import Context
 from satosa.exception import SATOSAError
 from satosa.internal import InternalData
 from satosa.micro_services.base import ResponseMicroService
 from pymongo import MongoClient
 from satosa.response import Redirect
 
+from satosacontrib.perun.utils.ConfigStore import ConfigStore
+
 logger = logging.getLogger(__name__)
 
 
 class IsBanned(ResponseMicroService):
     """
     This Satosa microservice checks, if user is banned.
     Banned users are redirected to configured URL.
     Requires perun user id to be already filled in the internal data.
     """
 
     def __init__(self, config, *args, **kwargs):
         super().__init__(*args, **kwargs)
         logger.info("IsBanned is active")
 
-        self.user_id_attr = config["user_id_attr_name"]
+        self.global_config = ConfigStore.get_global_cfg(config["global_cfg_path"])
+
+        self.user_id_attr = self.global_config["perun_user_id_attribute"]
         self.redirect_url = config["redirect_url"]
         self.connection_string = config["mongo_db"]["connection_string"]
         self.database_name = config["mongo_db"]["database_name"]
         self.collection_name = config["mongo_db"]["collection_name"]
 
     def process(self, context: Context, data: InternalData):
         """
@@ -36,15 +40,15 @@
         """
         user_id = data.attributes.get(self.user_id_attr)
         if not user_id:
             raise SATOSAError(
                 self.__class__.__name__ + f"Missing mandatory attribute "
                 f"'{self.user_id_attr}' "
                 f"in data.attributes. Hint: Did you "
-                f"configured PerunUser microservice "
+                f"configure PerunUser microservice "
                 f"before this microservice?"
             )
 
         if self.find_ban(str(user_id)) is not None:
             logger.info(f"Ban found for user {user_id}, redirecting to banned URL.")
             return Redirect(self.redirect_url)
```

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/is_eligible_microservice.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/persist_authorization_params_microservice.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/persist_authorization_params_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,29 +20,30 @@
         self.driver = config["driver"]
         self.dialect = config["dialect"]
         logger.info("ProxyStatistics are active")
 
     def _get_id_from_identifier(self, cnxn, table, entity, id_column):
         identifier = entity["id"]
         name = entity["name"]
-        insert_stmt = insert(table).values(identifier=identifier, name=name)
-        if name is None or name == "":
-            insert_stmt = insert_stmt.on_conflict_do_nothing()
-        else:
-            insert_stmt = insert_stmt.on_conflict_do_update(
-                index_elements=["identifier"], set_=dict(name=name)
+        with cnxn.begin():
+            insert_stmt = insert(table).values(identifier=identifier, name=name)
+            if name is None or name == "":
+                insert_stmt = insert_stmt.on_conflict_do_nothing()
+            else:
+                insert_stmt = insert_stmt.on_conflict_do_update(
+                    index_elements=["identifier"], set_=dict(name=name)
+                )
+            cnxn.execute(insert_stmt)
+
+            result = cnxn.execute(
+                sqlalchemy.select(getattr(table.columns, id_column)).where(
+                    table.columns.identifier == identifier
+                )
             )
-        cnxn.execute(insert_stmt)
-
-        result = cnxn.execute(
-            sqlalchemy.select(getattr(table.columns, id_column)).where(
-                table.columns.identifier == identifier
-            )
-        )
-        return result.scalar()
+            return result.scalar()
 
     def process(self, context, data):
         idp = data.auth_info["issuer"]
         sp = data.requester
         sp_name = data.requester_name[0]["text"]
         if sp_name is None:
             sp_name = ""
@@ -50,42 +51,52 @@
 
         driver = f"+{self.driver}" if self.driver else ""
         engine = sqlalchemy.create_engine(
             f"{self.dialect}{driver}://"
             + f"{self.stats_user}:{self.stats_password}@{self.hostname}:{self.port}/"
             + f"{self.stats_db}"
         )
-        cnxn = engine.connect()
-        metadata = sqlalchemy.MetaData()
-        statistics_per_user = sqlalchemy.Table(
-            "statistics_per_user", metadata, autoload=True, autoload_with=engine
-        )
-        statistics_idp = sqlalchemy.Table(
-            "statistics_idp", metadata, autoload=True, autoload_with=engine
-        )
-        statistics_sp = sqlalchemy.Table(
-            "statistics_sp", metadata, autoload=True, autoload_with=engine
-        )
-
-        entities = {"IDP": {"id": idp, "name": ""}, "SP": {"id": sp, "name": sp_name}}
-        sides = {"IDP": statistics_idp, "SP": statistics_sp}
-        side_ids = {"IDP": "idp_id", "SP": "sp_id"}
-        ids = {}
-        for side in sides:
-            table = sides[side]
-            ids[side_ids[side]] = self._get_id_from_identifier(
-                cnxn, table, entities[side], side_ids[side]
+        with engine.connect() as cnxn:
+            metadata = sqlalchemy.MetaData()
+            statistics_per_user = sqlalchemy.Table(
+                "statistics_per_user", metadata, autoload_with=cnxn
+            )
+            statistics_idp = sqlalchemy.Table(
+                "statistics_idp", metadata, autoload_with=cnxn
+            )
+            statistics_sp = sqlalchemy.Table(
+                "statistics_sp", metadata, autoload_with=cnxn
             )
 
-        fields = {"day": date.today().strftime("%Y-%m-%d"), "logins": 1, "user": user}
-        fields.update(ids)
-
-        insert_stmt = insert(statistics_per_user).values(**fields)
-        insert_stmt = insert_stmt.on_conflict_do_update(
-            index_elements=["day", "idp_id", "sp_id", "user"],
-            set_={statistics_per_user.columns.logins: insert_stmt.excluded.logins + 1},
-        )
-        cnxn.execute(insert_stmt)
+            entities = {
+                "IDP": {"id": idp, "name": ""},
+                "SP": {"id": sp, "name": sp_name},
+            }
+            sides = {"IDP": statistics_idp, "SP": statistics_sp}
+            side_ids = {"IDP": "idp_id", "SP": "sp_id"}
+            ids = {}
+            for side in sides:
+                table = sides[side]
+                ids[side_ids[side]] = self._get_id_from_identifier(
+                    cnxn, table, entities[side], side_ids[side]
+                )
+
+            fields = {
+                "day": date.today().strftime("%Y-%m-%d"),
+                "logins": 1,
+                "user": user,
+            }
+            fields.update(ids)
+            with cnxn.begin():
+                insert_stmt = insert(statistics_per_user).values(**fields)
+                insert_stmt = insert_stmt.on_conflict_do_update(
+                    index_elements=["day", "idp_id", "sp_id", "user"],
+                    set_={
+                        statistics_per_user.columns.logins: insert_stmt.excluded.logins
+                        + 1
+                    },
+                )
+                cnxn.execute(insert_stmt)
 
-        logger.info(f"User {user} used IdP {idp} to log into SP {sp}")
+            logger.info(f"User {user} used IdP {idp} to log into SP {sp}")
 
         return super().process(context, data)
```

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/micro_services/session_started_with_microservice.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/micro_services/session_started_with_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 from sqlalchemy import (
     Column,
     String,
     ForeignKey,
     Integer,
 )
-from sqlalchemy.dialects.mssql import DATETIME2
+from sqlalchemy.dialects.postgresql import TIMESTAMP
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base()
 
 
 class AuthEventLoggingTable(Base):
     __tablename__ = "auth_event_logging"
 
     id = Column(Integer, primary_key=True)
-    day = Column(DATETIME2)
+    day = Column(TIMESTAMP)
     user = Column(String)
     idp_id = Column(Integer, ForeignKey("logging_idp.id"))
-    sp_id = Column(Integer, ForeignKey("logging_sp_id.id"))
+    sp_id = Column(Integer, ForeignKey("logging_sp.id"))
     ip_address = Column(String)
     geolocation_city = Column(String)
     geolocation_country = Column(String)
     session_id = Column(Integer, ForeignKey("session_id_values.id"))
     requested_acrs_id = Column(Integer, ForeignKey("requested_acrs_values.id"))
     upstream_acrs_id = Column(Integer, ForeignKey("upstream_acrs_values.id"))
     user_agent_raw_id = Column(Integer, ForeignKey("user_agent_raw_values.id"))
     user_agent_id = Column(Integer, ForeignKey("user_agent_values.id"))
 
 
 class LoggingIdpTable(Base):
     __tablename__ = "logging_idp"
 
     id = Column(Integer, primary_key=True)
-    identifier = Column(String)
+    identifier = Column(String, unique=True)
     name = Column(String)
 
 
 class LoggingSpTable(Base):
     __tablename__ = "logging_sp"
 
     id = Column(Integer, primary_key=True)
-    identifier = Column(String)
+    identifier = Column(String, unique=True)
     name = Column(String)
 
 
 class SessionIdTable(Base):
     __tablename__ = "session_id_values"
 
     id = Column(Integer, primary_key=True)
```

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/utils/ConfigStore.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/utils/CurlConnector.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/utils/CurlConnector.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/utils/CurlConnectorInterface.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/utils/CurlConnectorInterface.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib/perun/utils/Utils.py` & `satosacontrib.perun-4.0.0/satosacontrib/perun/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/satosacontrib.perun.egg-info/PKG-INFO` & `satosacontrib.perun-4.0.0/satosacontrib.perun.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satosacontrib.perun
-Version: 3.8.0
+Version: 4.0.0
 Summary: Microservices for SATOSA authentication proxy, made by the Perun team
 Home-page: https://github.com/CESNET/satosacontrib.perun.git
 License: UNKNOWN
 Description: # satosacontrib.perun
         
         Microservices for [SATOSA](https://github.com/IdentityPython/SATOSA) authentication
         proxy, made by the Perun team.
@@ -45,14 +45,23 @@
         The microservice connects to database storing user bans and redirects banned users to configured URL.
         
         ### Persist authorization params microservice
         
         This request microservice retrieves configured parameters from GET or POST request (if available) and
         stores the values to internal context state.
         
+        ### Forward authorization params microservice
+        
+        This request microservice retrieves configured parameters from GET or POST request (if available) and
+        forwards them through a context parameter. Optionally, `default_values` can be
+        provided in the config file. These will be forwarded for configured SP and/or IdP if
+        not provided in the GET/POST request. If the parameter with preconfigured
+        default value is sent via GET/POST request anyway, the value form the request will be
+        used instead of the default.
+        
         ### Session started with microservice
         
         This Satosa microservice checks, if configured attribute's value is present
         in "session_started_with" values (retrieved by Persist authorization params microservice).
         If so, adds attribute with configured name. The value is expected to be converted
         to boolean by Attribute typing microservice.
```

### Comparing `satosacontrib.perun-3.8.0/satosacontrib.perun.egg-info/SOURCES.txt` & `satosacontrib.perun-4.0.0/satosacontrib.perun.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 satosacontrib/perun/micro_services/__init__.py
 satosacontrib/perun/micro_services/attribute_typing_microservice.py
 satosacontrib/perun/micro_services/auth_event_logging_microservice.py
 satosacontrib/perun/micro_services/auth_switcher_lite.py
 satosacontrib/perun/micro_services/cardinality_single_microservice.py
 satosacontrib/perun/micro_services/compute_eligibility.py
 satosacontrib/perun/micro_services/context_attributes_microservice.py
-satosacontrib/perun/micro_services/is_banned_microservice.py
+satosacontrib/perun/micro_services/forward_authorization_params_microservice.py
 satosacontrib/perun/micro_services/is_eligible_microservice.py
 satosacontrib/perun/micro_services/multi_idphint_microservice.py
 satosacontrib/perun/micro_services/nameid_attribute_microservice.py
 satosacontrib/perun/micro_services/persist_authorization_params_microservice.py
 satosacontrib/perun/micro_services/proxystatistics_microservice.py
 satosacontrib/perun/micro_services/session_started_with_microservice.py
 satosacontrib/perun/micro_services/idm/__init__.py
 satosacontrib/perun/micro_services/idm/additional_identifiers.py
 satosacontrib/perun/micro_services/idm/attributes.py
 satosacontrib/perun/micro_services/idm/ensure_member.py
 satosacontrib/perun/micro_services/idm/entitlement.py
+satosacontrib/perun/micro_services/idm/is_banned_microservice.py
 satosacontrib/perun/micro_services/idm/perun_user.py
 satosacontrib/perun/micro_services/idm/sp_authorization.py
 satosacontrib/perun/micro_services/idm/update_user_ext_source.py
 satosacontrib/perun/utils/AuthEventLoggingDbModels.py
 satosacontrib/perun/utils/ConfigStore.py
 satosacontrib/perun/utils/CurlConnector.py
 satosacontrib/perun/utils/CurlConnectorInterface.py
```

### Comparing `satosacontrib.perun-3.8.0/setup.py` & `satosacontrib.perun-4.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     install_requires=[
         "setuptools",
         "SATOSA~=8.1",
         "pysaml2~=7.1",
         "requests~=2.28",
         "perun.connector~=3.7",
         "PyYAML~=6.0",
-        "SQLAlchemy~=1.4",
+        "SQLAlchemy~=2.0",
         "jwcrypto~=1.3",
         "natsort~=8.4.0",
         "python-dateutil~=2.8",
         "geoip2~=4.6",
         "user_agents~=2.2",
         "pymongo~=4.3",
     ],
```

### Comparing `satosacontrib.perun-3.8.0/tests/test_additional_indentifiers.py` & `satosacontrib.perun-4.0.0/tests/test_additional_indentifiers.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/tests/test_auth_event_logging.py` & `satosacontrib.perun-4.0.0/tests/test_auth_event_logging.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import satosacontrib.perun.micro_services.auth_event_logging_microservice as ms
-from unittest.mock import patch, MagicMock
+from unittest.mock import patch, MagicMock, Mock
 from satosa.context import Context
 from satosa.internal import InternalData
 from satosa.micro_services.base import MicroService
 from satosacontrib.perun.micro_services.auth_event_logging_microservice import (
     AuthEventLogging,
 )
 from tests.test_microservice_loader import Loader
@@ -116,13 +116,18 @@
     )
     AuthEventLogging._AuthEventLogging__get_id_from_identifier = MagicMock(
         side_effect=[1, 2]
     )
     AuthEventLogging._AuthEventLogging__get_location = MagicMock(
         return_value={"city": "city", "country": "country"}
     )
-    ms.create_engine = MagicMock(return_value=TestEngine())
+    mo = Mock()
+    mc = Mock()
+    mo.__enter__ = Mock(return_value=MagicMock())
+    mo.__exit__ = Mock(return_value=None)
+    mc.connect = Mock(return_value=mo)
+    ms.create_engine = Mock(return_value=mc)
     ms.Base.metadata = MagicMock(return_value=TestMetadata())
     MicroService.process = MagicMock(return_value=None)
 
     result = MICROSERVICE.process(TEST_CONTEXT, TEST_DATA)
     assert result is None
```

### Comparing `satosacontrib.perun-3.8.0/tests/test_context_attributes.py` & `satosacontrib.perun-4.0.0/tests/test_context_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from satosa.context import Context
 from satosa.internal import InternalData
 from satosa.micro_services.base import MicroService
 
 from tests.test_microservice_loader import Loader
 
 MICROSERVICE_CONFIG = {
-    "global_cfg_filepath": "example_path",
+    "global_cfg_path": "example_path",
     "allowed_requesters": ["allowed_requester1", "allowed_requester2"],
     "target_backend_attribute": "targetbackend",
     "target_issuer_attributes": ["targetissuer"],
 }
 
 MICROSERVICE = Loader(MICROSERVICE_CONFIG, "ContextAttributes").create_mocked_instance()
```

### Comparing `satosacontrib.perun-3.8.0/tests/test_is_banned.py` & `satosacontrib.perun-4.0.0/tests/test_is_banned.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from unittest.mock import MagicMock
 import logging
 
 from satosa.micro_services.base import MicroService
 from satosa.response import Redirect
-from satosacontrib.perun.micro_services.is_banned_microservice import (
+from satosacontrib.perun.micro_services.idm.is_banned_microservice import (
     IsBanned,
 )
 from tests.test_microservice_loader import Loader, TestContext, TestData
 
 CONFIG = {
-    "user_id_attr_name": "user_id",
+    "global_cfg_path": "example_path",
     "redirect_url": "https://example.org/banned.html",
     "mongo_db": {
         "connection_string": "connection_string",
         "database_name": "database_name",
         "collection_name": "bans",
     },
 }
@@ -22,19 +22,21 @@
     "description": None,
     "facilityId": "4514",
     "id": 6,
     "userId": "1",
     "validityTo": "1680134400000",
 }
 
-MICROSERVICE = Loader(CONFIG, IsBanned.__name__).create_mocked_instance()
+MICROSERVICE = Loader(CONFIG, IsBanned.__name__).create_mocked_instance(
+    perun_micro_service=True
+)
 
 
 def test_banned_user_is_redirected(caplog):
-    data = {"user_id": 1}
+    data = {"example_user_id": 1}
     expected_header = (
         "Location",
         CONFIG["redirect_url"],
     )
     ban_found_message = "Ban found for user 1, redirecting to banned URL."
 
     IsBanned.find_ban = MagicMock(return_value=BAN)
@@ -45,15 +47,15 @@
 
         assert isinstance(result, Redirect)
         assert expected_header in result.headers
         assert ban_found_message in caplog.text
 
 
 def test_banned_user_ok(caplog):
-    data = {"user_id": 1}
+    data = {"example_user_id": 1}
     ban_not_found_log_message = "Ban not found for user 1."
 
     IsBanned.find_ban = MagicMock(return_value=None)
     MicroService.process = MagicMock(return_value=None)
 
     with caplog.at_level(logging.DEBUG):
         MICROSERVICE.process(TestContext(), TestData({}, data))
```

### Comparing `satosacontrib.perun-3.8.0/tests/test_is_eligible_microservice.py` & `satosacontrib.perun-4.0.0/tests/test_is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/tests/test_microservice_loader.py` & `satosacontrib.perun-4.0.0/tests/test_microservice_loader.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/tests/test_perun_attributes.py` & `satosacontrib.perun-4.0.0/tests/test_perun_attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/tests/test_perun_ensure_member.py` & `satosacontrib.perun-4.0.0/tests/test_perun_ensure_member.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/tests/test_perun_entitlement.py` & `satosacontrib.perun-4.0.0/tests/test_perun_entitlement.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.8.0/tests/test_perun_user_microservice.py` & `satosacontrib.perun-4.0.0/tests/test_perun_user_microservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     PerunUser,
 )  # noqa
 from satosacontrib.perun.utils.Utils import Utils
 from tests.test_microservice_loader import Loader
 from tests.test_microservice_loader import TestContext
 
 MICROSERVICE_CONFIG = {
-    "global_cfg_filepath": "example_path",
+    "global_cfg_path": "example_path",
     "internal_login_attribute": "example_internal_login",
     "internal_extsource_attribute": "example_internal_extsource",
     "proxy_extsource_name": "example_extsource_name",
     "registration_page_url": "example_url",
     "registration_result_url": "example_url",
 }
```

### Comparing `satosacontrib.perun-3.8.0/tests/test_sp_authorization_microservice.py` & `satosacontrib.perun-4.0.0/tests/test_sp_authorization_microservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     SpAuthorization,
 )
 from satosacontrib.perun.utils.PerunConstants import PerunConstants
 from satosacontrib.perun.utils.Utils import Utils
 from tests.test_microservice_loader import Loader, TestContext
 
 MICROSERVICE_CONFIG = {
-    "global_cfg_filepath": "example_path",
+    "global_cfg_path": "example_path",
     "filter_config": {
         "check_group_membership_attr": "example_attr",
         "vo_short_names_attr": "example_attr",
         "allow_registration_attr": "example_attr",
         "registrar_url": "example_url",
         "registration_link_attr": "example_attr",
         "skip_notification_sps": ["sp1", "sp2", "sp3"],
```

### Comparing `satosacontrib.perun-3.8.0/tests/test_update_ues.py` & `satosacontrib.perun-4.0.0/tests/test_update_ues.py`

 * *Files identical despite different names*

