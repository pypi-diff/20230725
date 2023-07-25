# Comparing `tmp/msticpy-2.5.3.tar.gz` & `tmp/msticpy-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msticpy-2.5.3.tar", last modified: Sat Jun 24 21:51:48 2023, max compression
+gzip compressed data, was "msticpy-2.6.0.tar", last modified: Tue Jul 25 01:04:56 2023, max compression
```

## Comparing `msticpy-2.5.3.tar` & `msticpy-2.6.0.tar`

### file list

```diff
@@ -1,418 +1,419 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.914789 msticpy-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-24 21:51:36.000000 msticpy-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-24 21:51:36.000000 msticpy-2.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)   487752 2023-06-24 21:51:36.000000 msticpy-2.5.3/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-06-24 21:51:48.914789 msticpy-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15960 2023-06-24 21:51:36.000000 msticpy-2.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.866788 msticpy-2.5.3/msticpy/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.870788 msticpy-2.5.3/msticpy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.870788 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/anomalous.py
--rw-r--r--   0 runner    (1001) docker     (123)    29469 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/sessionize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.870788 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/cmds_only.py
--rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py
--rw-r--r--   0 runner    (1001) docker     (123)    21586 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/cluster_auditd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/code_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/eventcluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/observationlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/polling_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/syslog_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/analysis/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.870788 msticpy-2.5.3/msticpy/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/azure_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/azure_auth_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/cloud_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/cred_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/keyring_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/keyvault_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/keyvault_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/msal_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/auth/secret_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.874788 msticpy-2.5.3/msticpy/common/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/azure_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/check_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19073 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/pkg_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/provider_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/proxy_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/timespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.874788 msticpy-2.5.3/msticpy/common/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/utility/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/utility/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/utility/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/utility/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/common/wsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.878788 msticpy-2.5.3/msticpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_azure_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_data_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_keyvault.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_msticpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_other_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_simple_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_ti_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/ce_user_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/comp_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/compound_ctrls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/file_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/mp_config_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/mp_config_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/config/mp_config_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.878788 msticpy-2.5.3/msticpy/context/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.878788 msticpy-2.5.3/msticpy/context/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_dynamic_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    25652 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_dynamic_summary_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_incidents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_ti.py
--rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_watchlists.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/azure/sentinel_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/contextlookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.882789 msticpy-2.5.3/msticpy/context/contextproviders/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/contextproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/contextproviders/context_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/contextproviders/http_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/contextproviders/servicenow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/domain_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/geoip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/http_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    25638 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/ip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/lookup_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/preprocess_observable.py
--rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tilookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.882789 msticpy-2.5.3/msticpy/context/tiproviders/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/alienvault_otx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/azure_sent_byoti.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/greynoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/ibm_xforce.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/intsights.py
--rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/kql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/mblookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/open_page_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/pulsedive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/result_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/riskiq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/ti_http_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/ti_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/tor_exit_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/tiproviders/virustotal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.882789 msticpy-2.5.3/msticpy/context/vtlookupv3/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/vtlookupv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/vtlookupv3/vtfile_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/vtlookupv3/vtlookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32429 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/context/vtlookupv3/vtlookupv3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.886788 msticpy-2.5.3/msticpy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.886788 msticpy-2.5.3/msticpy/data/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/azure/azure_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/azure/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/azure_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/azure_sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.886788 msticpy-2.5.3/msticpy/data/core/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20161 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/data_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/data_query_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/param_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_defns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_provider_connections_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_provider_utils_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/core/query_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/data_obfus.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/data_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.890789 msticpy-2.5.3/msticpy/data/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33479 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/azure_kusto_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    23645 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/azure_monitor_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/cybereason_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/driver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/elastic_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    23399 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/kql_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/kusto_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/local_data_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/local_osquery_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/mdatp_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    29511 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/mordor_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/odata_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/resource_graph_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/security_graph_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/sentinel_query_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/splunk_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/drivers/sumologic_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.862788 msticpy-2.5.3/msticpy/data/queries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.890789 msticpy-2.5.3/msticpy/data/queries/cybereason/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/cybereason/cybereason_connections.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/cybereason/cybereason_hosts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/cybereason/cybereason_processes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.890789 msticpy-2.5.3/msticpy/data/queries/localdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/localdata/local_data.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.890789 msticpy-2.5.3/msticpy/data/queries/m365d/
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_alerts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    29648 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_hunting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_network.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_process.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_user.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.890789 msticpy-2.5.3/msticpy/data/queries/mde/
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_alerts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_hunting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_network.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_process.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_user.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.890789 msticpy-2.5.3/msticpy/data/queries/msgraph/
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/msgraph/graph_alerts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/data/queries/mssentinel/
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_alert.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_azure.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_net.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_o365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/data/queries/resourcegraph/
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/resourcegraph/sentinel_resources.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/data/queries/splunk/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/splunk/splunk_alert_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/splunk/splunk_authentication_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/splunk/splunk_queries.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/data/queries/sumologic/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/queries/sumologic/sumologic_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/query_container.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/query_defns.py
--rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/sql_to_kql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/data/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/storage/azure_blob_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/data/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/uploaders/loganalytics_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/uploaders/splunk_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/data/uploaders/uploader_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.894789 msticpy-2.5.3/msticpy/datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.898789 msticpy-2.5.3/msticpy/datamodel/entities/
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/azure_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/cloud_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/cloud_logon_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/entity_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/entity_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/file_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/geo_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/graph_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/host_logon_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/iot_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/mail_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/mail_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/malware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/network_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/registry_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/registry_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/submission_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/threat_intelligence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/unknown_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/entities/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/pivot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.898789 msticpy-2.5.3/msticpy/datamodel/soc/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/soc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/soc/incident.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/datamodel/soc/sentinel_alert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.902789 msticpy-2.5.3/msticpy/init/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/azure_ml_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    19979 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/azure_synapse_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/mp_pandas_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/mp_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    31388 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/nbinit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/nbmagics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.902789 msticpy-2.5.3/msticpy/init/pivot_core/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_magic_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_core/pivot_register_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.902789 msticpy-2.5.3/msticpy/init/pivot_init/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_init/pivot_data_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_init/pivot_ti_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/pivot_init/vt_pivot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/init/user_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/msticpyconfig.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.906789 msticpy-2.5.3/msticpy/nbtools/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/data_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/entityschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/morph_charts.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/nbdisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/nbwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/observationlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/process_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/security_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/security_alert_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18315 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/security_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/security_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/ti_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/timeline_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/timeline_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbtools/wsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.906789 msticpy-2.5.3/msticpy/nbwidgets/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/get_environment_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/get_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/lookback.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/option_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/query_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/select_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/select_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/nbwidgets/select_subset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.906789 msticpy-2.5.3/msticpy/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   104245 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/resources/WinSecurityEvent.json
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/resources/cmd_line_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/resources/mp_pivot_reg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/resources/mpconfig_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/resources/obfuscation_cols.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.910789 msticpy-2.5.3/msticpy/sectools/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/auditdextract.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/base64unpack.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/domain_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/eventcluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/geoip.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/iocextract.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/ip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/proc_tree_build_mde.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/proc_tree_build_winlx.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/proc_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/proc_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/proc_tree_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/sectools_magics.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/syslog_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/tilookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.910789 msticpy-2.5.3/msticpy/sectools/tiproviders/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/tiproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/tiproviders/ti_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/vtlookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.910789 msticpy-2.5.3/msticpy/sectools/vtlookupv3/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/vtlookupv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/vtlookupv3/vtfile_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/vtlookupv3/vtlookupv3.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/sectools/vtlookupv3/vtobject_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.910789 msticpy-2.5.3/msticpy/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/auditdextract.py
--rw-r--r--   0 runner    (1001) docker     (123)    30712 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/base64unpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    26354 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/iocextract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/proc_tree_build_mde.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/proc_tree_build_winlx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/proc_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/proc_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/transform/process_tree_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.914789 msticpy-2.5.3/msticpy/vis/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/code_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/data_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/data_viewer_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/entity_graph_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/figure_dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)    33234 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/matrix_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/mordor_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/morph_charts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/mp_pandas_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/nbdisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/network_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/process_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/query_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/ti_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/timeline_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/timeline_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/timeline_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/timeline_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-24 21:51:36.000000 msticpy-2.5.3/msticpy/vis/vtobject_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:51:48.866788 msticpy-2.5.3/msticpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-06-24 21:51:48.000000 msticpy-2.5.3/msticpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-06-24 21:51:48.000000 msticpy-2.5.3/msticpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:51:48.000000 msticpy-2.5.3/msticpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:51:48.000000 msticpy-2.5.3/msticpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-24 21:51:48.000000 msticpy-2.5.3/msticpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-24 21:51:48.000000 msticpy-2.5.3/msticpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-24 21:51:36.000000 msticpy-2.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-24 21:51:36.000000 msticpy-2.5.3/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-24 21:51:36.000000 msticpy-2.5.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-24 21:51:36.000000 msticpy-2.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-24 21:51:48.914789 msticpy-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-24 21:51:36.000000 msticpy-2.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.175965 msticpy-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-25 01:04:41.000000 msticpy-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-25 01:04:41.000000 msticpy-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)   487752 2023-07-25 01:04:41.000000 msticpy-2.6.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-07-25 01:04:56.175965 msticpy-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15960 2023-07-25 01:04:41.000000 msticpy-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.131965 msticpy-2.6.0/msticpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.131965 msticpy-2.6.0/msticpy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.135965 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/anomalous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29469 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/sessionize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.135965 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/cmds_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21586 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/cluster_auditd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/code_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/eventcluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/observationlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/outliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/polling_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/syslog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.135965 msticpy-2.6.0/msticpy/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/azure_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/azure_auth_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/cloud_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/cred_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/keyring_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/keyvault_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/keyvault_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/msal_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/secret_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.135965 msticpy-2.6.0/msticpy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/azure_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/check_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19073 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/pkg_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/provider_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/proxy_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/timespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.139965 msticpy-2.6.0/msticpy/common/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/utility/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/utility/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/utility/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/utility/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/wsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.139965 msticpy-2.6.0/msticpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_azure_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_data_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_keyvault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_msticpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_other_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_simple_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_ti_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_user_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/comp_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/compound_ctrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/file_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/mp_config_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/mp_config_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/mp_config_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.139965 msticpy-2.6.0/msticpy/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.143965 msticpy-2.6.0/msticpy/context/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_dynamic_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25652 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_dynamic_summary_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_incidents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_ti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_watchlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/contextlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.143965 msticpy-2.6.0/msticpy/context/contextproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/contextproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/contextproviders/context_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/contextproviders/http_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/contextproviders/servicenow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/domain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25638 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/ip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/lookup_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/preprocess_observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tilookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.147965 msticpy-2.6.0/msticpy/context/tiproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/alienvault_otx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/azure_sent_byoti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/greynoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/ibm_xforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/intsights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/kql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/mblookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/open_page_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/pulsedive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/result_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/riskiq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/ti_http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/ti_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/tor_exit_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/virustotal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.147965 msticpy-2.6.0/msticpy/context/vtlookupv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/vtlookupv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/vtlookupv3/vtfile_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/vtlookupv3/vtlookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32775 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/vtlookupv3/vtlookupv3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.147965 msticpy-2.6.0/msticpy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.147965 msticpy-2.6.0/msticpy/data/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/azure/azure_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/azure/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/azure_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/azure_sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.147965 msticpy-2.6.0/msticpy/data/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18111 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/data_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/data_query_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/param_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_defns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_provider_connections_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_provider_utils_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/data_obfus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/data_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.151965 msticpy-2.6.0/msticpy/data/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37132 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/azure_kusto_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25511 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/azure_monitor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/cybereason_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/driver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/elastic_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23399 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/kql_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/kusto_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/local_data_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/local_osquery_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/local_velociraptor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/mdatp_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29511 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/mordor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/odata_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/resource_graph_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/security_graph_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/sentinel_query_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/splunk_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/sumologic_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.127965 msticpy-2.6.0/msticpy/data/queries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.151965 msticpy-2.6.0/msticpy/data/queries/cybereason/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/cybereason/cybereason_connections.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/cybereason/cybereason_hosts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/cybereason/cybereason_processes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.151965 msticpy-2.6.0/msticpy/data/queries/localdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/localdata/local_data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.151965 msticpy-2.6.0/msticpy/data/queries/m365d/
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_alerts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    29655 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_hunting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_process.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_user.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/queries/mde/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_alerts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    29249 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_hunting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_process.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_user.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/queries/msgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/msgraph/graph_alerts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/queries/mssentinel/
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_alert.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_azure.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_net.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_o365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/queries/resourcegraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/resourcegraph/sentinel_resources.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/queries/splunk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/splunk/splunk_alert_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/splunk/splunk_authentication_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/splunk/splunk_queries.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/queries/sumologic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/sumologic/sumologic_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/query_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/query_defns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/sql_to_kql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/storage/azure_blob_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/uploaders/loganalytics_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/uploaders/splunk_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/uploaders/uploader_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.159965 msticpy-2.6.0/msticpy/datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.159965 msticpy-2.6.0/msticpy/datamodel/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/azure_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/cloud_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/cloud_logon_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/entity_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/entity_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/file_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/graph_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/host_logon_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/iot_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/mail_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/mail_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/malware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/network_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/registry_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/registry_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/submission_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/threat_intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/unknown_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/pivot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.163965 msticpy-2.6.0/msticpy/datamodel/soc/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/soc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/soc/incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/soc/sentinel_alert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.163965 msticpy-2.6.0/msticpy/init/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/azure_ml_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19979 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/azure_synapse_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/mp_pandas_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/mp_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31530 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/nbinit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/nbmagics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.163965 msticpy-2.6.0/msticpy/init/pivot_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_magic_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_register_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.163965 msticpy-2.6.0/msticpy/init/pivot_init/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_init/pivot_data_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_init/pivot_ti_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_init/vt_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/user_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/msticpyconfig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.167965 msticpy-2.6.0/msticpy/nbtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/entityschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/morph_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/nbdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/nbwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/observationlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/process_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/security_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/security_alert_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18315 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/security_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/security_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/ti_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/timeline_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/timeline_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/wsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.167965 msticpy-2.6.0/msticpy/nbwidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/get_environment_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/get_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/lookback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/option_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/query_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/select_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/select_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/select_subset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.167965 msticpy-2.6.0/msticpy/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   104245 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/resources/WinSecurityEvent.json
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/resources/cmd_line_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/resources/mp_pivot_reg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/resources/mpconfig_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/resources/obfuscation_cols.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.171965 msticpy-2.6.0/msticpy/sectools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/auditdextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/base64unpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/domain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/eventcluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/iocextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/ip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/proc_tree_build_mde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/proc_tree_build_winlx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/proc_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/proc_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/proc_tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/sectools_magics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/syslog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/tilookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.171965 msticpy-2.6.0/msticpy/sectools/tiproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/tiproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/tiproviders/ti_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/vtlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.171965 msticpy-2.6.0/msticpy/sectools/vtlookupv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/vtlookupv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/vtlookupv3/vtfile_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/vtlookupv3/vtlookupv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/vtlookupv3/vtobject_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.175965 msticpy-2.6.0/msticpy/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/auditdextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30712 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/base64unpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26354 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/iocextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/proc_tree_build_mde.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/proc_tree_build_winlx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/proc_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/proc_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/process_tree_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.175965 msticpy-2.6.0/msticpy/vis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/code_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/data_viewer_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/entity_graph_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/figure_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33234 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/matrix_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/mordor_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/morph_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/mp_pandas_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/nbdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/network_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/process_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/query_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/ti_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/timeline_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/timeline_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/timeline_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/timeline_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/vtobject_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.131965 msticpy-2.6.0/msticpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-07-25 01:04:56.000000 msticpy-2.6.0/msticpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-07-25 01:04:56.000000 msticpy-2.6.0/msticpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:04:56.000000 msticpy-2.6.0/msticpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:04:55.000000 msticpy-2.6.0/msticpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-25 01:04:56.000000 msticpy-2.6.0/msticpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 01:04:56.000000 msticpy-2.6.0/msticpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-25 01:04:42.000000 msticpy-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-25 01:04:42.000000 msticpy-2.6.0/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-25 01:04:42.000000 msticpy-2.6.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-25 01:04:42.000000 msticpy-2.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-25 01:04:56.179965 msticpy-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-25 01:04:42.000000 msticpy-2.6.0/setup.py
```

### Comparing `msticpy-2.5.3/LICENSE` & `msticpy-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/NOTICE.txt` & `msticpy-2.6.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/PKG-INFO` & `msticpy-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msticpy
-Version: 2.5.3
+Version: 2.6.0
 Summary: MSTIC Security Tools
 Home-page: https://github.com/microsoft/msticpy
 Author: Ian Hellen
 Author-email: ianhelle@microsoft.com
 Maintainer: Pete Bryan
 Maintainer-email: peter.bryan@microsoft.com
 License: MIT License
```

### Comparing `msticpy-2.5.3/README.md` & `msticpy-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/__init__.py` & `msticpy-2.6.0/msticpy/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/__init__.py` & `msticpy-2.6.0/msticpy/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/anomalous.py` & `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/anomalous.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/model.py` & `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/model.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/sessionize.py` & `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/sessionize.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/cmds_only.py` & `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/cmds_only.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py` & `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py` & `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/data_structures.py` & `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py` & `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/anomalous_sequence/utils/probabilities.py` & `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/probabilities.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/cluster_auditd.py` & `msticpy-2.6.0/msticpy/analysis/cluster_auditd.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/code_cleanup.py` & `msticpy-2.6.0/msticpy/analysis/code_cleanup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/eventcluster.py` & `msticpy-2.6.0/msticpy/analysis/eventcluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/observationlist.py` & `msticpy-2.6.0/msticpy/analysis/observationlist.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/outliers.py` & `msticpy-2.6.0/msticpy/analysis/outliers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/polling_detection.py` & `msticpy-2.6.0/msticpy/analysis/polling_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,14 @@
 
     Attributes
     ----------
     data: DataFrame
         Dataframe containing the data to be analysed. Must contain a
         column of edges and a column of timestamps
 
-    Methods
-    -------
-    detect_polling(timestamps, process_start, process_end, interval)
-        Detect strong periodic frequencies
-
     """
 
     def __init__(self, data: pd.DataFrame, copy: bool = False) -> None:
         """
         Create periodogram polling detector.
 
         Parameters
```

### Comparing `msticpy-2.5.3/msticpy/analysis/syslog_utils.py` & `msticpy-2.6.0/msticpy/analysis/syslog_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/analysis/timeseries.py` & `msticpy-2.6.0/msticpy/analysis/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/auth/__init__.py` & `msticpy-2.6.0/msticpy/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/auth/azure_auth.py` & `msticpy-2.6.0/msticpy/auth/azure_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/auth/azure_auth_core.py` & `msticpy-2.6.0/msticpy/auth/azure_auth_core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/auth/cloud_mappings.py` & `msticpy-2.6.0/msticpy/auth/cloud_mappings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/auth/cred_wrapper.py` & `msticpy-2.6.0/msticpy/auth/cred_wrapper.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/auth/keyring_client.py` & `msticpy-2.6.0/msticpy/auth/keyring_client.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/auth/keyvault_client.py` & `msticpy-2.6.0/msticpy/auth/keyvault_client.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/auth/keyvault_settings.py` & `msticpy-2.6.0/msticpy/auth/keyvault_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/auth/msal_auth.py` & `msticpy-2.6.0/msticpy/auth/msal_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/auth/secret_settings.py` & `msticpy-2.6.0/msticpy/auth/secret_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/__init__.py` & `msticpy-2.6.0/msticpy/common/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/azure_auth.py` & `msticpy-2.6.0/msticpy/common/azure_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/check_version.py` & `msticpy-2.6.0/msticpy/common/check_version.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/data_types.py` & `msticpy-2.6.0/msticpy/common/data_types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/data_utils.py` & `msticpy-2.6.0/msticpy/common/data_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/exceptions.py` & `msticpy-2.6.0/msticpy/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/pkg_config.py` & `msticpy-2.6.0/msticpy/common/pkg_config.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/provider_settings.py` & `msticpy-2.6.0/msticpy/common/provider_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/proxy_settings.py` & `msticpy-2.6.0/msticpy/common/proxy_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/settings.py` & `msticpy-2.6.0/msticpy/common/settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/timespan.py` & `msticpy-2.6.0/msticpy/common/timespan.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/utility/__init__.py` & `msticpy-2.6.0/msticpy/common/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/utility/format.py` & `msticpy-2.6.0/msticpy/common/utility/format.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/utility/ipython.py` & `msticpy-2.6.0/msticpy/common/utility/ipython.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/utility/package.py` & `msticpy-2.6.0/msticpy/common/utility/package.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/utility/types.py` & `msticpy-2.6.0/msticpy/common/utility/types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/common/wsconfig.py` & `msticpy-2.6.0/msticpy/common/wsconfig.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/__init__.py` & `msticpy-2.6.0/msticpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/ce_azure.py` & `msticpy-2.6.0/msticpy/config/ce_azure.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/ce_azure_sentinel.py` & `msticpy-2.6.0/msticpy/config/ce_azure_sentinel.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/ce_common.py` & `msticpy-2.6.0/msticpy/config/ce_common.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/ce_data_providers.py` & `msticpy-2.6.0/msticpy/config/ce_data_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/ce_keyvault.py` & `msticpy-2.6.0/msticpy/config/ce_keyvault.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/ce_msticpy.py` & `msticpy-2.6.0/msticpy/config/ce_msticpy.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/ce_other_providers.py` & `msticpy-2.6.0/msticpy/config/ce_other_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/ce_provider_base.py` & `msticpy-2.6.0/msticpy/config/ce_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/ce_simple_settings.py` & `msticpy-2.6.0/msticpy/config/ce_simple_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/ce_ti_providers.py` & `msticpy-2.6.0/msticpy/config/ce_ti_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/ce_user_defaults.py` & `msticpy-2.6.0/msticpy/config/ce_user_defaults.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/comp_edit.py` & `msticpy-2.6.0/msticpy/config/comp_edit.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/compound_ctrls.py` & `msticpy-2.6.0/msticpy/config/compound_ctrls.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/file_browser.py` & `msticpy-2.6.0/msticpy/config/file_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/mp_config_control.py` & `msticpy-2.6.0/msticpy/config/mp_config_control.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/mp_config_edit.py` & `msticpy-2.6.0/msticpy/config/mp_config_edit.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/config/mp_config_file.py` & `msticpy-2.6.0/msticpy/config/mp_config_file.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/__init__.py` & `msticpy-2.6.0/msticpy/context/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/azure/azure_data.py` & `msticpy-2.6.0/msticpy/context/azure/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/azure/sentinel_analytics.py` & `msticpy-2.6.0/msticpy/context/azure/sentinel_analytics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/azure/sentinel_bookmarks.py` & `msticpy-2.6.0/msticpy/context/azure/sentinel_bookmarks.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/azure/sentinel_core.py` & `msticpy-2.6.0/msticpy/context/azure/sentinel_core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/azure/sentinel_dynamic_summary.py` & `msticpy-2.6.0/msticpy/context/azure/sentinel_dynamic_summary.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/azure/sentinel_dynamic_summary_types.py` & `msticpy-2.6.0/msticpy/context/azure/sentinel_dynamic_summary_types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/azure/sentinel_incidents.py` & `msticpy-2.6.0/msticpy/context/azure/sentinel_incidents.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/azure/sentinel_search.py` & `msticpy-2.6.0/msticpy/context/azure/sentinel_search.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/azure/sentinel_ti.py` & `msticpy-2.6.0/msticpy/context/azure/sentinel_ti.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/azure/sentinel_utils.py` & `msticpy-2.6.0/msticpy/context/azure/sentinel_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/azure/sentinel_watchlists.py` & `msticpy-2.6.0/msticpy/context/azure/sentinel_watchlists.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/azure/sentinel_workspaces.py` & `msticpy-2.6.0/msticpy/context/azure/sentinel_workspaces.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/contextlookup.py` & `msticpy-2.6.0/msticpy/context/contextlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/contextproviders/context_provider_base.py` & `msticpy-2.6.0/msticpy/context/contextproviders/context_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/contextproviders/http_context_provider.py` & `msticpy-2.6.0/msticpy/context/contextproviders/http_context_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/contextproviders/servicenow.py` & `msticpy-2.6.0/msticpy/context/contextproviders/servicenow.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/domain_utils.py` & `msticpy-2.6.0/msticpy/context/domain_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/geoip.py` & `msticpy-2.6.0/msticpy/context/geoip.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/http_provider.py` & `msticpy-2.6.0/msticpy/context/http_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/ip_utils.py` & `msticpy-2.6.0/msticpy/context/ip_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/lookup.py` & `msticpy-2.6.0/msticpy/context/lookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/lookup_result.py` & `msticpy-2.6.0/msticpy/context/lookup_result.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/preprocess_observable.py` & `msticpy-2.6.0/msticpy/context/preprocess_observable.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/provider_base.py` & `msticpy-2.6.0/msticpy/context/provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tilookup.py` & `msticpy-2.6.0/msticpy/context/tilookup.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         ioc_query_type: Optional[str] = None,
         providers: Optional[List[str]] = None,
         default_providers: Optional[List[str]] = None,
         prov_scope: str = "primary",
         **kwargs,
     ) -> pd.DataFrame:
         """
-        Lookup single IoC in active providers.
+        Lookup Threat Intelligence reports for a single IoC in active providers.
 
         Parameters
         ----------
         ioc : str
             IoC observable
         observable : str
             alias for `ioc`
@@ -84,14 +84,27 @@
         Returns
         -------
         pd.DataFrame
             The result returned as a tuple(bool, list):
             bool indicates whether a TI record was found in any provider
             list has an entry for each provider result
 
+        See Also
+        --------
+        lookup_iocs : Lookup Threat Intelligence reports for a collection of IoCs.
+
+        Notes
+        -----
+        Queries active Threat Intelligence (TI) providers for a single
+        indicator of compromise (IoC). It returns results as a pandas
+        DataFrame. `ioc_type` can be used to specify the type (ipv4,
+        ipv6, dns, url, file_hash). If this is not supplied the
+        type is inferred using regular expressions.
+        By default, providers are queried asynchronously, in parallel.
+
         """
         ioc = ioc or kwargs.pop("observable", None)
         if ioc is None:
             raise ValueError("No value supplied for 'ioc' parameter")
         return self.lookup_item(
             item=ioc,
             item_type=ioc_type,
@@ -110,15 +123,15 @@
         ioc_query_type: str = None,
         providers: List[str] = None,
         default_providers: Optional[List[str]] = None,
         prov_scope: str = "primary",
         **kwargs,
     ) -> pd.DataFrame:
         """
-        Lookup a collection of IoCs.
+        Lookup Threat Intelligence reports for a collection of IoCs in active providers.
 
         Parameters
         ----------
         data : Union[pd.DataFrame, Mapping[str, str], Iterable[str]]
             Data input in one of three formats:
             1. Pandas dataframe (you must supply the column name in
             `ioc_col` parameter)
@@ -142,14 +155,29 @@
             Additional arguments passed to the underlying provider(s)
 
         Returns
         -------
         pd.DataFrame
             DataFrame of results
 
+        See Also
+        --------
+        lookup_ioc : Lookup Threat Intelligence reports for a single IoC.
+
+        Notes
+        -----
+        `lookup_iocs` queries active Threat Intelligence (TI) providers for
+        threat reports. It can accept input as a Python iterable or
+        a pandas dataframe. In the latter case, you also need to supply
+        the `ioc_col` parameter to indicate which column the IoC value can
+        be found. The `ioc_type_col` parameter is optional and can be used
+        to manually specify the IoC type for each row. If this is not supplied
+        the ioc types are inferred using regular expressions.
+        The results are returned as a pandas DataFrame.
+
         """
         return _make_sync(
             self._lookup_iocs_async(
                 data=data,
                 ioc_col=ioc_col,
                 ioc_type_col=ioc_type_col,
                 ioc_query_type=ioc_query_type,
```

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/__init__.py` & `msticpy-2.6.0/msticpy/context/tiproviders/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/alienvault_otx.py` & `msticpy-2.6.0/msticpy/context/tiproviders/alienvault_otx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/azure_sent_byoti.py` & `msticpy-2.6.0/msticpy/context/tiproviders/azure_sent_byoti.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/greynoise.py` & `msticpy-2.6.0/msticpy/context/tiproviders/greynoise.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/ibm_xforce.py` & `msticpy-2.6.0/msticpy/context/tiproviders/ibm_xforce.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/intsights.py` & `msticpy-2.6.0/msticpy/context/tiproviders/intsights.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/kql_base.py` & `msticpy-2.6.0/msticpy/context/tiproviders/kql_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/mblookup.py` & `msticpy-2.6.0/msticpy/context/tiproviders/mblookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/open_page_rank.py` & `msticpy-2.6.0/msticpy/context/tiproviders/open_page_rank.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/pulsedive.py` & `msticpy-2.6.0/msticpy/context/tiproviders/pulsedive.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/result_severity.py` & `msticpy-2.6.0/msticpy/context/tiproviders/result_severity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/riskiq.py` & `msticpy-2.6.0/msticpy/context/tiproviders/riskiq.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/ti_http_provider.py` & `msticpy-2.6.0/msticpy/context/tiproviders/ti_http_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/ti_provider_base.py` & `msticpy-2.6.0/msticpy/context/tiproviders/ti_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/tor_exit_nodes.py` & `msticpy-2.6.0/msticpy/context/tiproviders/tor_exit_nodes.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/tiproviders/virustotal.py` & `msticpy-2.6.0/msticpy/context/tiproviders/virustotal.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/vtlookupv3/__init__.py` & `msticpy-2.6.0/msticpy/context/vtlookupv3/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/vtlookupv3/vtfile_behavior.py` & `msticpy-2.6.0/msticpy/context/vtlookupv3/vtfile_behavior.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/vtlookupv3/vtlookup.py` & `msticpy-2.6.0/msticpy/context/vtlookupv3/vtlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/context/vtlookupv3/vtlookupv3.py` & `msticpy-2.6.0/msticpy/context/vtlookupv3/vtlookupv3.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 
     # pylint: disable=too-many-locals
     async def _lookup_ioc_relationships_async(
         self,
         observable: str,
         vt_type: str,
         relationship: str,
-        limit: int = None,
+        limit: Optional[int] = None,
         all_props: bool = False,
         full_objects: bool = False,
     ):
         """
         Look up and single IoC observable relationships.
 
         Parameters
@@ -502,16 +502,17 @@
         return result_df
 
     def lookup_ioc_relationships(
         self,
         observable: str,
         vt_type: str,
         relationship: str,
-        limit: int = None,
+        limit: Optional[int] = None,
         all_props: bool = False,
+        full_objects: bool = False,
     ) -> pd.DataFrame:
         """
         Look up single IoC observable relationship links.
 
         Parameters
         ----------
         observable: str
@@ -520,14 +521,16 @@
             The VT entity type
         relationship: str
             Desired relationship
         limit: int
             Relations limit
         all_props : bool, optional
             If True, return all properties, by default False
+        full_objects : bool, optional
+            If True, return the full object rather than just ID links.
 
         Returns
         -------
             Relationship Pandas DataFrame with the relationships of the entity
 
         Notes
         -----
@@ -539,22 +542,31 @@
         --------
         lookup_ioc_related : return the full related objects.
 
         """
         try:
             return _make_sync(
                 self._lookup_ioc_relationships_async(
-                    observable, vt_type, relationship, limit, all_props=all_props
+                    observable,
+                    vt_type,
+                    relationship,
+                    limit,
+                    all_props=all_props,
+                    full_objects=full_objects,
                 )
             )
         finally:
             self._vt_client.close()
 
     def lookup_ioc_related(
-        self, observable: str, vt_type: str, relationship: str, limit: int = None
+        self,
+        observable: str,
+        vt_type: str,
+        relationship: str,
+        limit: Optional[int] = None,
     ) -> pd.DataFrame:
         """
         Look single IoC observable related items.
 
         Parameters
         ----------
         observable: str
@@ -671,15 +683,15 @@
 
     def lookup_iocs_relationships(
         self,
         observables_df: pd.DataFrame,
         relationship: str,
         observable_column: str = ColumnNames.TARGET.value,
         observable_type_column: str = ColumnNames.TARGET_TYPE.value,
-        limit: int = None,
+        limit: Optional[int] = None,
         all_props: bool = False,
     ) -> pd.DataFrame:
         """
         Look up and single IoC observable relationships.
 
         Parameters
         ----------
```

### Comparing `msticpy-2.5.3/msticpy/data/__init__.py` & `msticpy-2.6.0/msticpy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/azure/__init__.py` & `msticpy-2.6.0/msticpy/data/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/azure/azure_blob_storage.py` & `msticpy-2.6.0/msticpy/data/azure/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/azure/azure_data.py` & `msticpy-2.6.0/msticpy/data/azure/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/azure_blob_storage.py` & `msticpy-2.6.0/msticpy/data/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/azure_data.py` & `msticpy-2.6.0/msticpy/data/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/azure_sentinel.py` & `msticpy-2.6.0/msticpy/data/azure_sentinel.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/core/data_providers.py` & `msticpy-2.6.0/msticpy/data/core/data_providers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Data provider loader."""
-from datetime import datetime
+import logging
 from functools import partial
-from itertools import tee
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import pandas as pd
-from tqdm.auto import tqdm
 
 from ..._version import VERSION
 from ...common.pkg_config import get_config
 from ...common.utility import export, valid_pyname
 from ...nbwidgets import QueryTime
 from .. import drivers
 from ..drivers.driver_base import DriverBase, DriverProps
 from .param_extractor import extract_query_params
 from .query_container import QueryContainer
 from .query_defns import DataEnvironment
 from .query_provider_connections_mixin import QueryProviderConnectionsMixin
 from .query_provider_utils_mixin import QueryProviderUtilsMixin
-from .query_source import QuerySource
 from .query_store import QueryStore
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 _HELP_FLAGS = ("help", "?")
 _DEBUG_FLAGS = ("print", "debug_query", "print_query")
 _COMPATIBLE_DRIVER_MAPPINGS = {
     "mssentinel": ["m365d"],
     "mde": ["m365d"],
-    "mssentinel_new": ["mssentinel"],
+    "mssentinel_new": ["mssentinel", "m365d"],
     "kusto_new": ["kusto"],
 }
 
+logger = logging.getLogger(__name__)
+
 
 # These are mixin classes that do not have an __init__ method
 # pylint: disable=super-init-not-called
 @export
 class QueryProvider(QueryProviderConnectionsMixin, QueryProviderUtilsMixin):
     """
     Container for query store and query execution provider.
@@ -110,33 +109,39 @@
         else:
             self.driver_class = driver.__class__
         # allow the driver to override the data environment used for selecting queries
         self.environment_name = (
             driver.get_driver_property(DriverProps.EFFECTIVE_ENV)
             or self.environment_name
         )
+        logger.info("Using data environment %s", self.environment_name)
+        logger.info("Driver class: %s", self.driver_class.__name__)
 
         self._additional_connections: Dict[str, DriverBase] = {}
         self._query_provider = driver
         # replace the connect method docstring with that from
         # the driver's connect method
         self.__class__.connect.__doc__ = driver.connect.__doc__
         self.all_queries = QueryContainer()
 
         # Add any query files
         data_env_queries: Dict[str, QueryStore] = {}
+        self._query_paths = query_paths
         if driver.use_query_paths:
+            logger.info("Using query paths %s", query_paths)
             data_env_queries.update(
                 self._read_queries_from_paths(query_paths=query_paths)
             )
         self.query_store = data_env_queries.get(
             self.environment_name, QueryStore(self.environment_name)
         )
+        logger.info("Adding query functions to provider")
         self._add_query_functions()
         self._query_time = QueryTime(units="day")
+        logger.info("Initialization complete.")
 
     def _check_environment(
         self, data_environment
     ) -> Tuple[Union[str, DataEnvironment], str]:
         """Check environment against known names."""
         if isinstance(data_environment, str):
             data_env = DataEnvironment.parse(data_environment)
@@ -175,14 +180,15 @@
 
         Parameters
         ----------
         connection_str : str
             Connection string for the data source
 
         """
+        logger.info("Calling connect on driver")
         self._query_provider.connect(connection_str=connection_str, **kwargs)
 
         # If the driver has any attributes to expose via the provider
         # add those here.
         for attr_name, attr in self._query_provider.public_attribs.items():
             setattr(self, attr_name, attr)
 
@@ -190,22 +196,24 @@
         # if the driver supports dynamic filtering of queries,
         # filter the query store based on connect-time parameters
         if self._query_provider.filter_queries_on_connect:
             self.query_store.apply_query_filter(self._query_provider.query_usable)
             refresh_query_funcs = True
         # Add any built-in or dynamically retrieved queries from driver
         if self._query_provider.has_driver_queries:
+            logger.info("Adding driver queries to provider")
             driver_queries = self._query_provider.driver_queries
             self._add_driver_queries(queries=driver_queries)
             refresh_query_funcs = True
 
         if refresh_query_funcs:
             self._add_query_functions()
 
         # Since we're now connected, add Pivot functions
+        logger.info("Adding query pivot functions")
         self._add_pivots(lambda: self._query_time.timespan)
 
     def exec_query(self, query: str, **kwargs) -> Union[pd.DataFrame, Any]:
         """
         Execute simple query string.
 
         Parameters
@@ -226,20 +234,21 @@
         Union[pd.DataFrame, Any]
             Query results - a DataFrame if successful
             or a KqlResult if unsuccessful.
 
         """
         query_options = kwargs.pop("query_options", {}) or kwargs
         query_source = kwargs.pop("query_source", None)
-        result = self._query_provider.query(
-            query, query_source=query_source, **query_options
-        )
+
+        logger.info("Executing query '%s...'", query[:40])
         if not self._additional_connections:
-            return result
-        return self._exec_additional_connections(query, result, **kwargs)
+            return self._query_provider.query(
+                query, query_source=query_source, **query_options
+            )
+        return self._exec_additional_connections(query, **kwargs)
 
     @property
     def query_time(self):
         """Return the default QueryTime control for queries."""
         return self._query_time
 
     def _execute_query(self, *args, **kwargs) -> Union[pd.DataFrame, Any]:
@@ -261,42 +270,48 @@
             query_path=family, query_name=query_name
         )
         if _help_flag(*args):
             query_source.help()
             return None
 
         params, missing = extract_query_params(query_source, *args, **kwargs)
+        logger.info("Parameters for query: %s", params)
         query_options = {
             "default_time_params": self._check_for_time_params(params, missing)
         }
         if missing:
             query_source.help()
             raise ValueError(f"No values found for these parameters: {missing}")
 
-        split_by = kwargs.pop("split_query_by", None)
+        split_by = kwargs.pop("split_query_by", kwargs.pop("split_by", None))
         if split_by:
+            logger.info("Split query selected - interval - %s", split_by)
             split_result = self._exec_split_query(
                 split_by=split_by,
                 query_source=query_source,
                 query_params=params,
+                debug=_debug_flag(*args, **kwargs),
                 args=args,
                 **kwargs,
             )
             if split_result is not None:
                 return split_result
             # if split queries could not be created, fall back to default
         query_str = query_source.create_query(
             formatters=self._query_provider.formatters, **params
         )
         # This looks for any of the "print query" debug args in args or kwargs
         if _debug_flag(*args, **kwargs):
             return query_str
 
         # Handle any query options passed and run the query
-        query_options.update(_get_query_options(params, kwargs))
+        query_options.update(self._get_query_options(params, kwargs))
+        logger.info(
+            "Running query '%s...' with params: %s", query_str[:40], query_options
+        )
         return self.exec_query(query_str, query_source=query_source, **query_options)
 
     def _check_for_time_params(self, params, missing) -> bool:
         """Fall back on builtin query time if no time parameters were supplied."""
         defaults_added = False
         if "start" in missing:
             missing.remove("start")
@@ -338,14 +353,15 @@
                     all_query_paths.append(custom_qry_path)
         if query_paths:
             for param_path in query_paths:
                 param_qry_path = _resolve_path(param_path)
                 if param_qry_path:
                     all_query_paths.append(param_qry_path)
         if all_query_paths:
+            logger.info("Reading queries from %s", all_query_paths)
             return QueryStore.import_files(
                 source_path=all_query_paths,
                 recursive=True,
                 driver_query_filter=self._query_provider.query_attach_spec,
             )
         # if no queries - just return an empty store
         return {self.environment_name: QueryStore(self.environment_name)}
@@ -391,88 +407,31 @@
                 description=query["description"],
             )
         # For now, just add all of the functions again (with any connect-time acquired
         # queries) - we could be more efficient than this but unless there are 1000s of
         # queries it should not be noticeable.
         self._add_query_functions()
 
-    def _exec_split_query(
-        self,
-        split_by: str,
-        query_source: QuerySource,
-        query_params: Dict[str, Any],
-        args,
-        **kwargs,
-    ) -> Union[pd.DataFrame, str, None]:
-        start = query_params.pop("start", None)
-        end = query_params.pop("end", None)
-        if not (start or end):
-            print(
-                "Cannot split a query that does not have 'start' and 'end' parameters"
-            )
-            return None
-        try:
-            split_delta = pd.Timedelta(split_by)
-        except ValueError:
-            split_delta = pd.Timedelta("1D")
-
-        ranges = _calc_split_ranges(start, end, split_delta)
-
-        split_queries = [
-            query_source.create_query(
-                formatters=self._query_provider.formatters,
-                start=q_start,
-                end=q_end,
-                **query_params,
-            )
-            for q_start, q_end in ranges
-        ]
-        # This looks for any of the "print query" debug args in args or kwargs
-        if _debug_flag(*args, **kwargs):
-            return "\n\n".join(split_queries)
-
-        # Retrieve any query options passed (other than query params)
-        # and send to query function.
-        query_options = _get_query_options(query_params, kwargs)
-        query_dfs = [
-            self.exec_query(query_str, query_source=query_source, **query_options)
-            for query_str in tqdm(split_queries, unit="sub-queries", desc="Running")
-        ]
-
-        return pd.concat(query_dfs)
-
-
-def _calc_split_ranges(start: datetime, end: datetime, split_delta: pd.Timedelta):
-    """Return a list of time ranges split by `split_delta`."""
-    # Use pandas date_range and split the result into 2 iterables
-    s_ranges, e_ranges = tee(pd.date_range(start, end, freq=split_delta))
-    next(e_ranges, None)  # skip to the next item in the 2nd iterable
-    # Zip them together to get a list of (start, end) tuples of ranges
-    # Note: we subtract 1 nanosecond from the 'end' value of each range so
-    # to avoid getting duplicated records at the boundaries of the ranges.
-    # Some providers don't have nanosecond granularity so we might
-    # get duplicates in these cases
-    ranges = [
-        (s_time, e_time - pd.Timedelta("1ns"))
-        for s_time, e_time in zip(s_ranges, e_ranges)
-    ]
-
-    # Since the generated time ranges are based on deltas from 'start'
-    # we need to adjust the end time on the final range.
-    # If the difference between the calculated last range end and
-    # the query 'end' that the user requested is small (< 10% of a delta),
-    # we just replace the last "end" time with our query end time.
-    if (ranges[-1][1] - end) < (split_delta / 10):
-        ranges[-1] = ranges[-1][0], end
-    else:
-        # otherwise append a new range starting after the last range
-        # in ranges and ending in 'end"
-        # note - we need to add back our subtracted 1 nanosecond
-        ranges.append((ranges[-1][0] + pd.Timedelta("1ns"), end))
-    return ranges
+    @staticmethod
+    def _get_query_options(
+        params: Dict[str, Any], kwargs: Dict[str, Any]
+    ) -> Dict[str, Any]:
+        # sourcery skip: inline-immediately-returned-variable, use-or-for-fallback
+        """Return any kwargs not already in params."""
+        query_options = kwargs.pop("query_options", {})
+        if not query_options:
+            # Any kwargs left over we send to the query provider driver
+            query_options = {
+                key: val for key, val in kwargs.items() if key not in params
+            }
+        query_options["time_span"] = {
+            "start": params.get("start"),
+            "end": params.get("end"),
+        }
+        return query_options
 
 
 def _resolve_package_path(config_path: str) -> Path:
     """Resolve path relative to current package."""
     return (
         Path(config_path)
         if Path(config_path).is_absolute()
@@ -496,23 +455,7 @@
 
 
 def _debug_flag(*args, **kwargs) -> bool:
     """Return True if debug/print args passed."""
     return any(db_arg for db_arg in _DEBUG_FLAGS if db_arg in args) or any(
         db_arg for db_arg in _DEBUG_FLAGS if kwargs.get(db_arg, False)
     )
-
-
-def _get_query_options(
-    params: Dict[str, Any], kwargs: Dict[str, Any]
-) -> Dict[str, Any]:
-    # sourcery skip: inline-immediately-returned-variable, use-or-for-fallback
-    """Return any kwargs not already in params."""
-    query_options = kwargs.pop("query_options", {})
-    if not query_options:
-        # Any kwargs left over we send to the query provider driver
-        query_options = {key: val for key, val in kwargs.items() if key not in params}
-    query_options["time_span"] = {
-        "start": params.get("start"),
-        "end": params.get("end"),
-    }
-    return query_options
```

### Comparing `msticpy-2.5.3/msticpy/data/core/data_query_reader.py` & `msticpy-2.6.0/msticpy/data/core/data_query_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/core/param_extractor.py` & `msticpy-2.6.0/msticpy/data/core/param_extractor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/core/query_container.py` & `msticpy-2.6.0/msticpy/data/core/query_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/core/query_defns.py` & `msticpy-2.6.0/msticpy/data/core/query_defns.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     """
 
     Unknown = 0
     MSSentinel = 1
     AzureSentinel = 1  # alias of LogAnalytics
     LogAnalytics = 1
     Kusto = 2
+    AzureDataExplorer = 2  # alias of Kusto
     AzureSecurityCenter = 3
     MSGraph = 4
     SecurityGraph = 4
     MDE = 5
     MDATP = 5  # alias of MDE
     LocalData = 6
     Splunk = 7
@@ -102,16 +103,19 @@
     Mordor = 8
     ResourceGraph = 9
     Sumologic = 10
     M365D = 11
     Cybereason = 12
     Elastic = 14
     OSQueryLogs = 15
+    OSQuery = 15
     MSSentinel_New = 16
     Kusto_New = 17
+    VelociraptorLogs = 18
+    Velociraptor = 18
 
     @classmethod
     def parse(cls, value: Union[str, int]) -> "DataEnvironment":
         """
         Convert string or int to enum.
 
         Parameters
```

### Comparing `msticpy-2.5.3/msticpy/data/core/query_provider_utils_mixin.py` & `msticpy-2.6.0/msticpy/data/core/query_provider_utils_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,19 @@
         Returns
         -------
         List[str]
             List of current data environments
 
         """
         # pylint: disable=not-an-iterable
-        return [env for env in DataEnvironment.__members__ if env != "Unknown"]
+        return [
+            de
+            for de in dir(DataEnvironment)
+            if de != "Unknown" and not de.startswith("_")
+        ]
         # pylint: enable=not-an-iterable
 
     def list_queries(self, substring: Optional[str] = None) -> List[str]:
         """
         Return list of family.query in the store.
 
         Parameters
```

### Comparing `msticpy-2.5.3/msticpy/data/core/query_source.py` & `msticpy-2.6.0/msticpy/data/core/query_source.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/core/query_store.py` & `msticpy-2.6.0/msticpy/data/core/query_store.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/core/query_template.py` & `msticpy-2.6.0/msticpy/data/core/query_template.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/data_obfus.py` & `msticpy-2.6.0/msticpy/data/data_obfus.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/data_providers.py` & `msticpy-2.6.0/msticpy/data/data_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/drivers/__init__.py` & `msticpy-2.6.0/msticpy/data/drivers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     DataEnvironment.Sumologic: ("sumologic_driver", "SumologicDriver"),
     DataEnvironment.ResourceGraph: ("resource_graph_driver", "ResourceGraphDriver"),
     DataEnvironment.M365D: ("mdatp_driver", "MDATPDriver"),
     DataEnvironment.Cybereason: ("cybereason_driver", "CybereasonDriver"),
     DataEnvironment.Elastic: ("elastic_driver", "ElasticDriver"),
     DataEnvironment.MSSentinel_New: ("azure_monitor_driver", "AzureMonitorDriver"),
     DataEnvironment.Kusto_New: ("azure_kusto_driver", "AzureKustoDriver"),
+    DataEnvironment.VelociraptorLogs: (
+        "local_velociraptor_driver",
+        "VelociraptorLogDriver",
+    ),
 }
 
 CUSTOM_PROVIDERS: Dict[str, type] = {}
 
 
 @singledispatch
 def import_driver(data_environment) -> type:
```

### Comparing `msticpy-2.5.3/msticpy/data/drivers/azure_kusto_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/azure_kusto_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Kusto Driver subclass."""
+import base64
 import dataclasses
 import json
 import logging
 from datetime import timedelta
 from functools import partial
 from typing import Any, Dict, List, NamedTuple, Optional, Tuple, Union
 
 import pandas as pd
 from azure.kusto.data import (
     ClientRequestProperties,
     KustoClient,
     KustoConnectionStringBuilder,
 )
+from cryptography.hazmat.primitives import hashes, serialization
+from cryptography.hazmat.primitives.serialization import pkcs12
 
 from ..._version import VERSION
 from ...auth.azure_auth import az_connect, get_default_resource_name
 from ...auth.cloud_mappings import AzureCloudConfig
 from ...common.exceptions import (
     MsticpyDataQueryError,
     MsticpyMissingDependencyError,
@@ -30,14 +33,15 @@
 from ...common.provider_settings import ProviderArgs, get_protected_setting
 from ...common.settings import get_config, get_http_proxies
 from ...common.utility import export
 from ..core.query_defns import DataEnvironment
 from ..core.query_source import QuerySource
 from .driver_base import DriverBase, DriverProps
 
+# pylint: disable=ungrouped-imports
 try:
     from azure.kusto.data.exceptions import KustoApiError, KustoServiceError
     from azure.kusto.data.helpers import dataframe_from_result_table
     from azure.kusto.data.response import KustoResponseDataSet
 except ImportError as imp_err:
     raise MsticpyMissingDependencyError(
         "Cannot use this feature without Azure Kusto client installed",
@@ -74,14 +78,15 @@
         TENANT_ID = "TenantId"
         INTEG_AUTH = "IntegratedAuth"
         DEFAULTS = "ClusterDefaults"
         CLIENT_ID = "ClientId"
         CLIENT_SEC = "ClientSecret"
         ARGS = "Args"
         CLUSTER_GROUPS = "ClusterGroups"
+        CERTIFICATE = "Certificate"
 
     # pylint: disable=no-member
     @property
     def default_db(self):
         """Return default database for this cluster."""
         return self.args.get("Database", self.args.get("DefaultDatabase"))
 
@@ -158,26 +163,30 @@
         super().__init__(**kwargs)
         if kwargs.get("debug", False):
             logger.setLevel(logging.DEBUG)
         self.environment = kwargs.get("data_environment", DataEnvironment.Kusto)
         self._strict_query_match = kwargs.get("strict_query_match", False)
         self._kusto_settings: Dict[str, Dict[str, KustoConfig]] = _get_kusto_settings()
         self._default_database: Optional[str] = None
-        self.current_connection: Optional[str] = connection_str
+        self._current_connection: Optional[str] = connection_str
         self._current_config: Optional[KustoConfig] = None
         self.client: Optional[KustoClient] = None
         self._az_auth_types: Optional[List[str]] = None
         self._az_tenant_id: Optional[str] = None
         self._def_timeout = min(kwargs.pop("timeout", _DEFAULT_TIMEOUT), _MAX_TIMEOUT)
         self._def_proxies = kwargs.get("proxies", get_http_proxies())
 
         self.add_query_filter("data_environments", "Kusto")
         self.set_driver_property(DriverProps.PUBLIC_ATTRS, self._set_public_attribs())
         self.set_driver_property(DriverProps.FILTER_ON_CONNECT, True)
         self.set_driver_property(DriverProps.EFFECTIVE_ENV, DataEnvironment.Kusto.name)
+        self.set_driver_property(DriverProps.SUPPORTS_THREADING, value=True)
+        self.set_driver_property(
+            DriverProps.MAX_PARALLEL, value=kwargs.get("max_threads", 4)
+        )
         self._loaded = True
 
     def _set_public_attribs(self):
         """Expose subset of attributes via query_provider."""
         return {
             "get_database_names": self.get_database_names,
             "get_database_schema": self.get_database_schema,
@@ -186,26 +195,34 @@
             "cluster_name": self.cluster_name,
             "cluster_config_name": self.cluster_config_name,
             "set_cluster": self.set_cluster,
             "set_database": self.set_database,
         }
 
     @property
+    def current_connection(self) -> Optional[str]:
+        """Return current connection string or URI."""
+        if self._current_connection:
+            return self._current_connection
+        return self.cluster_uri
+
+    @current_connection.setter
+    def current_connection(self, value: str):
+        """Set current connection string or URI."""
+        self._current_connection = value
+
+    @property
     def cluster_uri(self) -> str:
         """Return current cluster URI."""
-        if not self._current_config:
-            return ""
-        return self._current_config.cluster
+        return "" if not self._current_config else self._current_config.cluster
 
     @property
     def cluster_name(self) -> str:
         """Return current cluster URI."""
-        if not self._current_config:
-            return ""
-        return self._current_config.name
+        return self._current_config.name if self._current_config else ""
 
     @property
     def cluster_config_name(self) -> str:
         """Return current cluster URI."""
         if isinstance(self._current_config, KustoConfig):
             return self._current_config.alias
         return "not defined"
@@ -298,30 +315,35 @@
         else:
             self._az_auth_types = az_auth_types
         self._az_tenant_id = kwargs.pop(
             "tenant_id", kwargs.pop("mp_az_tenant_id", None)
         )
 
         cluster = kwargs.pop("cluster", None)
+        self.current_connection = connection_str or self.current_connection
         if not connection_str and not cluster:
             raise MsticpyParameterError(
                 "Must specify either a connection string or a cluster name",
                 parameter=["connection_str", "cluster"],
             )
 
         if cluster:
             self._current_config = self._lookup_cluster_settings(cluster)
+            if not self._az_tenant_id:
+                self._az_tenant_id = self._current_config.tenant_id
             logger.info(
-                "Using cluster id: %s, retrieved %s",
+                "Using cluster id: %s, retrieved url %s to build connection string",
                 cluster,
                 self.cluster_uri,
             )
             kusto_cs = self._get_connection_string_for_cluster(self._current_config)
+            self.current_connection = cluster
         else:
             logger.info("Using connection string %s", connection_str)
+            self.current_connection = connection_str
             kusto_cs = connection_str
 
         self.client = KustoClient(kusto_cs)
         proxies = kwargs.get("proxies", self._def_proxies)
         proxy_url = proxies.get("https") if proxies else None
         if proxy_url:
             logger.info(
@@ -534,44 +556,98 @@
         }
 
     def _get_connection_string_for_cluster(
         self, cluster_config: KustoConfig
     ) -> KustoConnectionStringBuilder:
         """Return full cluster URI and credential for cluster name or URI."""
         auth_params = self._get_auth_params_from_config(cluster_config)
+        connect_auth_types = self._az_auth_types or AzureCloudConfig().auth_methods
         if auth_params.method == "clientsecret":
-            connect_auth_types = self._az_auth_types or AzureCloudConfig().auth_methods
+            logger.info("Client secret specified in config - using client secret authn")
             if "clientsecret" not in connect_auth_types:
-                connect_auth_types.append("clientsecret")
+                connect_auth_types.insert(0, "clientsecret")
             credential = az_connect(
                 auth_types=connect_auth_types, **(auth_params.params)
             )
+        elif auth_params.method == "certificate":
+            logger.info("Certificate specified in config - using certificate authn")
+            connect_auth_types.insert(0, "certificate")
+            credential = az_connect(
+                auth_types=self._az_auth_types, **(auth_params.params)
+            )
+            return self._create_kusto_cert_connection_str(auth_params)
         else:
+            logger.info("Using integrated authn")
             credential = az_connect(
                 auth_types=self._az_auth_types, **(auth_params.params)
             )
         logger.info("Credentials obtained %s", type(credential.modern).__name__)
         token = credential.modern.get_token(get_default_resource_name(auth_params.uri))
         logger.info("Token obtained for %s", auth_params.uri)
         return KustoConnectionStringBuilder.with_aad_user_token_authentication(
             connection_string=auth_params.uri,
             user_token=token.token,
         )
 
+    def _create_kql_cert_connection_str(
+        self, auth_params: AuthParams
+    ) -> KustoConnectionStringBuilder:
+        logger.info("Creating KQL connection string for certificate authentication")
+        if not self._az_tenant_id:
+            raise ValueError(
+                "Azure tenant ID must be set in config or connect parameter",
+                "to use certificate authentication",
+            )
+        cert_bytes = base64.b64decode(auth_params.params["certificate"])
+        (
+            private_key,
+            certificate,
+            _,
+        ) = pkcs12.load_key_and_certificates(data=cert_bytes, password=None)
+        if private_key is None or certificate is None:
+            raise ValueError(
+                f"Could not load certificate for cluster {self.cluster_uri}"
+            )
+        private_cert = private_key.private_bytes(
+            encoding=serialization.Encoding.PEM,
+            format=serialization.PrivateFormat.TraditionalOpenSSL,
+            encryption_algorithm=serialization.NoEncryption(),
+        )
+        public_cert = certificate.public_bytes(encoding=serialization.Encoding.PEM)
+        thumbprint = certificate.fingerprint(hashes.SHA1())
+        return KustoConnectionStringBuilder.with_aad_application_certificate_sni_authentication(
+            connection_string=self.cluster_uri,
+            aad_app_id=auth_params.params["client_id"],
+            private_certificate=private_cert.decode("utf-8"),
+            public_certificate=public_cert.decode("utf-8"),
+            thumbprint=thumbprint.hex().upper(),
+            authority_id=self._az_tenant_id,
+        )
+
     def _get_auth_params_from_config(self, cluster_config: KustoConfig) -> AuthParams:
         """Get authentication parameters for cluster from KustoConfig values."""
         method = "integrated"
         auth_params_dict = {}
         if KFields.CLIENT_SEC in cluster_config and KFields.CLIENT_ID in cluster_config:
             method = "clientsecret"
             auth_params_dict["client_id"] = cluster_config.ClientId
             auth_params_dict["client_secret"] = cluster_config.ClientSecret
             logger.info(
                 "Using client secret authentication because client_secret in config"
             )
+        elif (
+            KFields.CERTIFICATE in cluster_config
+            and KFields.CLIENT_ID in cluster_config
+        ):
+            method = "certificate"
+            auth_params_dict["client_id"] = cluster_config.ClientId
+            auth_params_dict["certificate"] = cluster_config.Certificate
+            logger.info(
+                "Using client secret authentication because client_secret in config"
+            )
         elif KFields.INTEG_AUTH in cluster_config:
             logger.info("Using integrated auth.")
         auth_params_dict["tenant_id"] = cluster_config.tenant_id
         return AuthParams(method, auth_params_dict, cluster_config.cluster)
 
     def _lookup_cluster_settings(self, cluster: str) -> KustoConfig:
         """Return cluster URI from config if cluster name is passed."""
```

### Comparing `msticpy-2.5.3/msticpy/data/drivers/azure_monitor_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/azure_monitor_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,24 +129,29 @@
         self._def_timeout = kwargs.get(
             "timeout", kwargs.get("server_timeout", self._DEFAULT_TIMEOUT)
         )
         self._def_proxies = kwargs.get("proxies", get_http_proxies())
         self._query_client: Optional[LogsQueryClient] = None
         self._az_tenant_id: Optional[str] = None
         self._ws_config: Optional[WorkspaceConfig] = None
+        self._ws_name: Optional[str] = None
         self._workspace_id: Optional[str] = None
         self._workspace_ids: List[str] = []
         self._def_connection_str: Optional[str] = connection_str
         self._connect_auth_types: Optional[List[str]] = None
         self.add_query_filter(
             "data_environments", ("MSSentinel", "LogAnalytics", "AzureSentinel")
         )
         self.set_driver_property(
             DriverProps.EFFECTIVE_ENV, DataEnvironment.MSSentinel.name
         )
+        self.set_driver_property(DriverProps.SUPPORTS_THREADING, value=True)
+        self.set_driver_property(
+            DriverProps.MAX_PARALLEL, value=kwargs.get("max_threads", 4)
+        )
         logger.info(
             "AzureMonitorDriver loaded. connect_str  %s, kwargs: %s",
             connection_str,
             kwargs,
         )
 
     @property
@@ -156,14 +161,37 @@
             AzureCloudConfig().cloud, _LOGANALYTICS_URL_BY_CLOUD["global"]
         )
         # post v1.1.0 of azure-monitor-query, the API version requires a 'v1' suffix
         if parse_version(az_monitor_version) > parse_version("1.1.0"):
             return f"{base_url}v1"
         return base_url
 
+    @property
+    def current_connection(self) -> str:
+        """Return the current connection name."""
+        connection = self._ws_name
+        if (
+            not connection
+            and self._ws_config
+            and WorkspaceConfig.CONF_WS_NAME_KEY in self._ws_config
+        ):
+            connection = self._ws_config[WorkspaceConfig.CONF_WS_NAME_KEY]
+        return (
+            connection
+            or self._def_connection_str
+            or self._workspace_id
+            or next(iter(self._workspace_ids), "")
+            or "AzureMonitor"
+        )
+
+    @current_connection.setter
+    def current_connection(self, value: str):
+        """Allow attrib to be set but ignore."""
+        del value
+
     def connect(self, connection_str: Optional[str] = None, **kwargs):
         """
         Connect to data source.
 
         Parameters
         ----------
         connection_str : Union[str, WorkspaceConfig, None]
@@ -299,21 +327,29 @@
         if not self._connected or self._query_client is None:
             raise MsticpyNotConnectedError(
                 "Please run connect() to connect to the workspace",
                 "before running a query.",
                 title="Workspace not connected.",
                 help_uri=_HELP_URL,
             )
-        logger.info("Query to run %s", query)
         time_span_value = self._get_time_span_value(**kwargs)
-
         server_timeout = kwargs.pop("timeout", self._def_timeout)
 
         workspace_id = next(iter(self._workspace_ids), None) or self._workspace_id
         additional_workspaces = self._workspace_ids[1:] if self._workspace_ids else None
+        logger.info("Query to run %s", query)
+        logger.info(
+            "Workspaces %s", ",".join(self._workspace_ids) or self._workspace_id
+        )
+        logger.info(
+            "Time span %s - %s",
+            str(time_span_value[0]) if time_span_value else "none",
+            str(time_span_value[1]) if time_span_value else "none",
+        )
+        logger.info("Timeout %s", server_timeout)
         try:
             result = self._query_client.query_workspace(
                 workspace_id=workspace_id,  # type: ignore[arg-type]
                 query=query,
                 timespan=time_span_value,  # type: ignore[arg-type]
                 server_timeout=server_timeout,
                 additional_workspaces=additional_workspaces,
@@ -409,14 +445,15 @@
                 "The workspace config or connection string did not have"
                 "the required parameters to connect to a workspace.",
                 "At least a workspace ID and tenant ID are required.",
                 title="No connection details",
                 help_uri=_HELP_URL,
             )
         self._ws_config = ws_config
+        self._ws_name = workspace_name or ws_config.workspace_id
         if not self._az_tenant_id and WorkspaceConfig.CONF_TENANT_ID_KEY in ws_config:
             self._az_tenant_id = ws_config[WorkspaceConfig.CONF_TENANT_ID_KEY]
         self._workspace_id = ws_config[WorkspaceConfig.CONF_WS_ID_KEY]
 
     def _get_workspaces_by_id(self, workspace_ids):
         if not self._az_tenant_id:
             raise MsticpyKqlConnectionError(
@@ -460,15 +497,27 @@
             time_span_value = None
             logger.info("No time parameters supplied.")
         else:
             time_span = TimeSpan(
                 start=time_params["start"],
                 end=time_params["end"],
             )
-            time_span_value = time_span.start, time_span.end
+            # Azure Monitor API expects datetime objects, so
+            # convert to datetimes if we have pd.Timestamps
+            t_start = (
+                time_span.start.to_pydatetime(warn=False)
+                if isinstance(time_span.start, pd.Timestamp)
+                else time_span.start
+            )
+            t_end = (
+                time_span.end.to_pydatetime(warn=False)
+                if isinstance(time_span.end, pd.Timestamp)
+                else time_span.end
+            )
+            time_span_value = t_start, t_end
             logger.info("Time parameters set %s", str(time_span))
         return time_span_value
 
     def _check_table_exists(self, query_source):
         """Check that query table is in the workspace schema."""
         if not self.schema:
             return
```

### Comparing `msticpy-2.5.3/msticpy/data/drivers/cybereason_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/cybereason_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/drivers/driver_base.py` & `msticpy-2.6.0/msticpy/data/drivers/driver_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,23 +84,26 @@
         # self.formatters: Dict[str, Callable] = {}
         # self.use_query_paths = True
         # self.has_driver_queries = False
         self._previous_connection = False
         self.data_environment = kwargs.get("data_environment")
         self._query_filter: Dict[str, Set[str]] = defaultdict(set)
         self._instance: Optional[str] = None
+
         self.properties = DriverProps.defaults()
         self.set_driver_property(
             name=DriverProps.EFFECTIVE_ENV,
             value=(
                 self.data_environment.name
                 if isinstance(self.data_environment, DataEnvironment)
                 else self.data_environment or ""
             ),
         )
+        self.set_driver_property(DriverProps.SUPPORTS_THREADING, False)
+        self.set_driver_property(DriverProps.MAX_PARALLEL, kwargs.get("max_threads", 4))
 
     def __getattr__(self, attrib):
         """Return item from the properties dictionary as an attribute."""
         if attrib in self.properties:
             return self.properties[attrib]
         raise AttributeError(f"{self.__class__.__name__} has no attribute '{attrib}'")
```

### Comparing `msticpy-2.5.3/msticpy/data/drivers/elastic_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/elastic_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/drivers/kql_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/kql_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/drivers/kusto_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/kusto_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/drivers/local_data_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/local_data_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/drivers/local_osquery_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/local_osquery_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/drivers/mdatp_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/mdatp_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """MDATP OData Driver class."""
-from typing import Any, Union
+from typing import Any, Optional, Union
 
 import pandas as pd
 
 from ..._version import VERSION
 from ...auth.azure_auth import AzureCloudConfig
 from ...auth.cloud_mappings import get_defender_endpoint, get_m365d_endpoint
 from ...common.data_utils import ensure_df_datetimes
@@ -23,15 +23,17 @@
 @export
 class MDATPDriver(OData):
     """KqlDriver class to retreive date from MS Defender APIs."""
 
     CONFIG_NAME = "MicrosoftDefender"
     _ALT_CONFIG_NAMES = ["MDATPApp"]
 
-    def __init__(self, connection_str: str = None, instance: str = "Default", **kwargs):
+    def __init__(
+        self, connection_str: Optional[str] = None, instance: str = "Default", **kwargs
+    ):
         """
         Instantiate MSDefenderDriver and optionally connect.
 
         Parameters
         ----------
         connection_str : str, optional
             Connection string
@@ -70,30 +72,30 @@
             ]
 
         if connection_str:
             self.current_connection = connection_str
             self.connect(connection_str)
 
     def query(
-        self, query: str, query_source: QuerySource = None, **kwargs
+        self, query: str, query_source: Optional[QuerySource] = None, **kwargs
     ) -> Union[pd.DataFrame, Any]:
         """
         Execute query string and return DataFrame of results.
 
         Parameters
         ----------
         query : str
             The query to execute
         query_source : QuerySource
             The query definition object
 
         Returns
         -------
         Union[pd.DataFrame, results.ResultSet]
-            A DataFrame (if successfull) or
+            A DataFrame (if successful) or
             the underlying provider result if an error.
 
         """
         del query_source, kwargs
         data, response = self.query_with_results(
             query, body=True, api_end=self.api_suffix
         )
```

### Comparing `msticpy-2.5.3/msticpy/data/drivers/mordor_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/mordor_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/drivers/odata_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/odata_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from ..._version import VERSION
 from ...auth.msal_auth import MSALDelegatedAuth
 from ...common.exceptions import MsticpyConnectionError, MsticpyUserConfigError
 from ...common.pkg_config import get_config
 from ...common.provider_settings import get_provider_settings
 from ...common.utility import mp_ua_header
-from .driver_base import DriverBase, QuerySource
+from .driver_base import DriverBase, DriverProps, QuerySource
 
 __version__ = VERSION
 __author__ = "Pete Bryan"
 
 _HELP_URI = (
     "https://msticpy.readthedocs.io/en/latest/data_acquisition"
     "/DataProviders.html#connecting-to-an-odata-source"
@@ -62,14 +62,19 @@
         self._loaded = True
         self.aad_token = None
         self._debug = kwargs.get("debug", False)
         self.token_type = "AAD"  # nosec
         self.scopes = None
         self.msal_auth = None
 
+        self.set_driver_property(DriverProps.SUPPORTS_THREADING, value=True)
+        self.set_driver_property(
+            DriverProps.MAX_PARALLEL, value=kwargs.get("max_threads", 4)
+        )
+
     @abc.abstractmethod
     def query(
         self, query: str, query_source: QuerySource = None, **kwargs
     ) -> Union[pd.DataFrame, Any]:
         """
         Execute query string and return DataFrame of results.
```

### Comparing `msticpy-2.5.3/msticpy/data/drivers/resource_graph_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/resource_graph_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/drivers/security_graph_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/security_graph_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Security Graph OData Driver class."""
-from typing import Any, Union
+from typing import Any, Optional, Union
 
 import pandas as pd
 
 from ..._version import VERSION
 from ...auth.azure_auth_core import AzureCloudConfig
 from ...common.utility import export
 from .odata_driver import OData, QuerySource
@@ -20,15 +20,15 @@
 @export
 class SecurityGraphDriver(OData):
     """Driver to query security graph."""
 
     CONFIG_NAME = "MicrosoftGraph"
     _ALT_CONFIG_NAMES = ["SecurityGraphApp"]
 
-    def __init__(self, connection_str: str = None, **kwargs):
+    def __init__(self, connection_str: Optional[str] = None, **kwargs):
         """
         Instantiate MSGraph driver and optionally connect.
 
         Parameters
         ----------
         connection_str : str, optional
             Connection string
@@ -50,28 +50,28 @@
         self.api_ver = kwargs.get("api_ver", "v1.0")
 
         if connection_str:
             self.current_connection = connection_str
             self.connect(connection_str)
 
     def query(
-        self, query: str, query_source: QuerySource = None, **kwargs
+        self, query: str, query_source: Optional[QuerySource] = None, **kwargs
     ) -> Union[pd.DataFrame, Any]:
         """
         Execute query string and return DataFrame of results.
 
         Parameters
         ----------
         query : str
             The query to execute
         query_source : QuerySource
             The query definition object
 
         Returns
         -------
         Union[pd.DataFrame, results.ResultSet]
-            A DataFrame (if successfull) or
+            A DataFrame (if successful) or
             the underlying provider result if an error.
 
         """
         del query_source, kwargs
         return self.query_with_results(query, body=False)[0]
```

### Comparing `msticpy-2.5.3/msticpy/data/drivers/sentinel_query_reader.py` & `msticpy-2.6.0/msticpy/data/drivers/sentinel_query_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/drivers/splunk_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/splunk_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/drivers/sumologic_driver.py` & `msticpy-2.6.0/msticpy/data/drivers/sumologic_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/cybereason/cybereason_connections.yaml` & `msticpy-2.6.0/msticpy/data/queries/cybereason/cybereason_connections.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/cybereason/cybereason_hosts.yaml` & `msticpy-2.6.0/msticpy/data/queries/cybereason/cybereason_hosts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/cybereason/cybereason_processes.yaml` & `msticpy-2.6.0/msticpy/data/queries/cybereason/cybereason_processes.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/localdata/local_data.yaml` & `msticpy-2.6.0/msticpy/data/queries/localdata/local_data.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_alerts.yaml` & `msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_file.yaml` & `msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_process.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 metadata:
   version: 1
-  description: MDATP Queries
+  description: M365D Process Queries
   data_environments: [MDATP, MDE, M365D, LogAnalytics]
-  data_families: [MDATP, MDE]
-  tags: ["file"]
+  data_families: [M365D]
+  tags: ["process"]
 defaults:
   metadata:
-    data_source: "file_events"
+    data_source: "process_events"
   parameters:
     table:
       description: Table name
       type: str
       default: "DeviceProcessEvents"
     start:
       description: Query start time
@@ -23,52 +23,64 @@
       type: str
       default: ""
     time_column:
       description: The name of the column detailing the time the event was generated.
       type: str
       default: "Timestamp"
 sources:
-  list_files:
-    description: Lists all file events by filename
+  list_host_processes:
+    description: Return all process creations for a host for the specified time range
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
-        | where FileName has "{file_name}"
+        | where DeviceName has "{host_name}"
         {add_query_items}'
       uri: None
     parameters:
-      file_name:
-        description: Name of file
+      host_name:
+        description: Name of host
         type: str
-  file_path:
-    description: Lists all file events from files in a certain path
+  process_creations:
+    description: Return all processes with matching name or hash (all hosts)
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
-        | where FolderPath contains "{path}"
+        | where FileName contains "{process_identifier}" or SHA1 has "{process_identifier}" or SHA256 has "{process_identifier}" or MD5 has "{process_identifier}"
         {add_query_items}'
     parameters:
-      path:
-        description: Full or partial path to search in
+      process_identifier:
+        description: Identifier for the process, filename, or hash
         type: str
-  list_filehash:
-    description: Lists all file events by hash
+  process_paths:
+    description: Return all processes with a matching path (part path) (all hosts)
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
-        | where SHA1 == "{file_hash}" or SHA256 == "{file_hash}" or MD5 == "{file_hash}"
+        | where FileName contains "{file_path}"
+        {add_query_items}'
+    parameters:
+      file_path:
+        description: full or partial path
+        type: str
+  process_cmd_line:
+    description: Lists all processes with a command line containing a string (all hosts)
+    metadata:
+    args:
+      query: '
+        {table}
+        | where {time_column} >= datetime({start})
+        | where {time_column} <= datetime({end})
+        | where ProcessCommandLine contains "{cmd_line}"
         {add_query_items}'
-      uri: None
     parameters:
-      file_hash:
-        description: Hash of file
+      cmd_line:
+        description: Command line artifact to search for
         type: str
-        aliases: hash
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_hunting.yaml` & `msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_hunting.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 metadata:
   version: 1
   description: MDATP Queries
   data_environments: [MDATP, MDE, M365D, LogAnalytics]
-  data_families: [MDATPHunting, MDE]
+  data_families: [MDEHunting, M365DHunting]
   tags: ['user']
 defaults:
   metadata:
     data_source: 'hunting_queries'
   parameters:
       start:
         description: Query start time
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_network.yaml` & `msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_network.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 metadata:
   version: 1
-  description: MDE Queries
+  description: M365D Network Queries
   data_environments: [MDATP, MDE, M365D, LogAnalytics]
-  data_families: [MDATP, MDE]
+  data_families: [M365D]
   tags: ["network"]
 defaults:
   metadata:
     data_source: "network_events"
   parameters:
     table:
       description: Table name
@@ -35,15 +35,15 @@
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
         {add_query_items}"
       uri: None
     parameters:
   host_connections:
-    description: Lists connections by for a specified hostname
+    description: Returns connections by for a specified hostname
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
         | where DeviceName has "{host_name}"
@@ -51,43 +51,43 @@
     parameters:
       host_name:
         description: Name of host
         type: str
         aliases:
           - hostname
   ip_connections:
-    description: Lists network connections associated with a specified remote IP
+    description: Returns network connections associated with a specified remote IP
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
         | where RemoteIP has "{ip_address}" or LocalIP has "{ip_address}"
         {add_query_items}'
     parameters:
       ip_address:
         description: Remote IP Address
         type: str
   url_connections:
-    description: Lists connections associated with a specified URL
+    description: Returns connections associated with a specified URL
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
         | where RemoteUrl has "{url}"
         {add_query_items}'
     parameters:
       url:
         description: Remote URL
         type: str
   protocol_connections:
-    description: Lists connections associated with a specified protocol
+    description: Returns connections associated with a specified protocol (port number)
     metadata:
     args:
       query: "
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
         | where RemotePort == {protocol}
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_process.yaml` & `msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_file.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 metadata:
   version: 1
-  description: MDATP Queries
+  description: M365D Queries
   data_environments: [MDATP, MDE, M365D, LogAnalytics]
-  data_families: [MDATP, MDE]
-  tags: ["process"]
+  data_families: [M365D]
+  tags: ["file", "process"]
 defaults:
   metadata:
-    data_source: "process_events"
+    data_source: "file_events"
   parameters:
     table:
       description: Table name
       type: str
-      default: "DeviceProcessEvents"
+      default: "DeviceFileEvents"
     start:
       description: Query start time
       type: datetime
     end:
       description: Query end time
       type: datetime
     add_query_items:
@@ -23,64 +23,72 @@
       type: str
       default: ""
     time_column:
       description: The name of the column detailing the time the event was generated.
       type: str
       default: "Timestamp"
 sources:
-  list_host_processes:
-    description: Lists all process creations for a host
+  list_file_events_for_filename:
+    description: Lists all file events by filename
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
-        | where DeviceName has "{host_name}"
+        | where FileName has "{file_name}"
         {add_query_items}'
       uri: None
     parameters:
-      host_name:
-        description: Name of host
+      file_name:
+        description: Name of file
         type: str
-  process_creations:
-    description: Lists all processes created by name or hash
+  list_file_events_for_path:
+    description: Lists all file events from files in a certain path
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
-        | where FileName contains "{process_identifier}" or SHA1 has "{process_identifier}" or SHA256 has "{process_identifier}" or MD5 has "{process_identifier}"
+        | where FolderPath contains "{path}"
         {add_query_items}'
     parameters:
-      process_identifier:
-        description: Identifier for the process, filename, or hash
+      path:
+        description: Full or partial path to search in
         type: str
-  process_paths:
-    description: Lists all processes created from a path
+  list_file_events_for_hash:
+    description: Lists all file events by hash
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
-        | where FileName contains "{file_path}"
+        | where SHA1 == "{file_hash}" or SHA256 == "{file_hash}" or MD5 == "{file_hash}"
         {add_query_items}'
+      uri: None
     parameters:
-      file_path:
-        description: full or partial path
+      file_hash:
+        description: Hash of file
         type: str
-  process_cmd_line:
-    description: Lists all processes with a command line containing a string
+        aliases: hash
+  list_file_events_for_host:
+    description: Lists all file events for a host/device
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
-        | where ProcessCommandLine contains "{cmd_line}"
+        | where DeviceName == "{host_name}" or DeviceID == "{device_id}"
         {add_query_items}'
+      uri: None
     parameters:
-      cmd_line:
-        description: Command line artifact to search for
+      host_name:
+        description: The name of the host/device
+        type: str
+        default: ""
+      device_id:
+        description: The device ID of the host/device
         type: str
+        default: ""
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/m365d/kql_mdatp_user.yaml` & `msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_user.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 metadata:
   version: 1
-  description: MDATP Queries
+  description: M365D User Queries
   data_environments: [MDATP, MDE, M365D, LogAnalytics]
-  data_families: [MDATP, MDE]
-  tags: ["user"]
+  data_families: [M365D]
+  tags: ["user", "account"]
 defaults:
   metadata:
     data_source: "user_events"
   parameters:
     start:
       description: Query start time
       type: datetime
@@ -20,58 +20,58 @@
       default: ""
     time_column:
       description: The name of the column detailing the time the event was generated.
       type: str
       default: "Timestamp"
 sources:
   user_logons:
-    description: Lists all user logons by user
+    description: Return all user logons for user name
     metadata:
     args:
       query: '
         DeviceLogonEvents
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
         | where AccountName has "{account_name}"
         {add_query_items}'
       uri: None
     parameters:
       account_name:
         description: Name of user
         type: str
   user_processes:
-    description: Lists all processes created by a user
+    description: Return all processes created by a user
     metadata:
     args:
       query: '
         DeviceProcessEvents
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
         | where AccountName has "{account_name}"
         {add_query_items}'
     parameters:
       account_name:
         description: Name of user
         type: str
   user_files:
-    description: Lists all files created by a user
+    description: Return all files created by a user
     metadata:
     args:
       query: '
         DeviceFileEvents
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
         | where InitiatingProcessAccountName contains "{account_name}"
         {add_query_items}'
     parameters:
       account_name:
         description: Name of user
         type: str
   user_network:
-    description: Lists all network connections associated with a user
+    description: Return all network connections associated with a user
     metadata:
     args:
       query: '
         DeviceNetworkEvents
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
         | where InitiatingProcessAccountName contains "{account_name}"
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_alerts.yaml` & `msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_alerts.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 metadata:
   version: 1
-  description: MDATP Queries
+  description: MDE Alert Queries
   data_environments: [MDATP, MDE, M365D]
-  data_families: [MDATP]
+  data_families: [MDE, MDATP]
   tags: ["alert"]
 defaults:
   metadata:
     data_source: "security_alert"
   parameters:
     table:
       description: Table name
@@ -20,15 +20,15 @@
       type: datetime
     add_query_items:
       description: Additional query clauses
       type: str
       default: ""
 sources:
   list_alerts:
-    description: Retrieves list of alerts
+    description: Returns list of alerts for a specified time range
     metadata:
     args:
       query: "
         {table}
         | where Timestamp >= datetime({start})
         | where Timestamp <= datetime({end})
         {add_query_items}"
@@ -47,15 +47,15 @@
         | where DeviceName has "{host_name}"
         {add_query_items}'
     parameters:
       host_name:
         description: Name of host
         type: str
   ip_alerts:
-    description: Lists alerts associated with a specified remote IP
+    description: Returns alerts associated with a specified remote IP
     metadata:
       pivot:
         short_name: alerts
     args:
       query: '
         {table}
         | where Timestamp >= datetime({start})
@@ -63,15 +63,15 @@
         | where RemoteIP has "{ip_address}"
         {add_query_items}'
     parameters:
       ip_address:
         description: Remote IP Address
         type: str
   url_alerts:
-    description: Lists alerts associated with a specified URL
+    description: Returns alerts associated with a specified URL
     metadata:
       pivot:
         short_name: alerts
     args:
       query: '
         {table}
         | where Timestamp >= datetime({start})
@@ -79,15 +79,15 @@
         | where RemoteUrl has "{url}"
         {add_query_items}'
     parameters:
       url:
         description: Remote URL
         type: str
   sha1_alerts:
-    description: Lists alerts associated with a specified SHA1 hash
+    description: Returns alerts associated with a specified SHA1 hash
     metadata:
       pivot:
         short_name: alerts
     args:
       query: '
         {table}
         | where Timestamp >= datetime({start})
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_file.yaml` & `msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_process.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 metadata:
   version: 1
   description: MDATP Queries
   data_environments: [MDATP, MDE, M365D, LogAnalytics]
-  data_families: [MDATP, MDE]
-  tags: ["file"]
+  data_families: [MDE, MDATP]
+  tags: ["process"]
 defaults:
   metadata:
-    data_source: "file_events"
+    data_source: "process_events"
   parameters:
     table:
       description: Table name
       type: str
       default: "DeviceProcessEvents"
     start:
       description: Query start time
@@ -19,58 +19,86 @@
       description: Query end time
       type: datetime
     add_query_items:
       description: Additional query clauses
       type: str
       default: ""
 sources:
-  list_files:
-    description: Lists all file events by filename
+  list_host_processes:
+    description: Return all process creations for a host for the specified time range
     metadata:
       pivot:
-        short_name: file_events_filename
+        short_name: processes
     args:
       query: '
         {table}
         | where Timestamp >= datetime({start})
         | where Timestamp <= datetime({end})
-        | where FileName has "{file_name}"
+        | where DeviceName has "{host_name}"
         {add_query_items}'
       uri: None
     parameters:
-      file_name:
-        description: Name of file
+      host_name:
+        description: Name of host
         type: str
-  file_path:
-    description: Lists all file events from files in a certain path
+  process_creations:
+    description: Return all processes with matching name or hash (all hosts)
     metadata:
-      pivot:
-        short_name: file_events_path
     args:
       query: '
         {table}
         | where Timestamp >= datetime({start})
         | where Timestamp <= datetime({end})
-        | where FolderPath contains "{path}"
+        | where FileName contains "{process_identifier}" or SHA1 has "{process_identifier}" or SHA256 has "{process_identifier}" or MD5 has "{process_identifier}"
         {add_query_items}'
     parameters:
-      path:
-        description: Full or partial path to search in
+      process_identifier:
+        description: Identifier for the process, filename, or hash
         type: str
-  list_filehash:
-    description: Lists all file events by hash
+  process_for_hash:
+    description: Return all processes with a matching hash (all hosts)
     metadata:
       pivot:
-        short_name: file_events_hash
+        short_name: processes_by_hash
     args:
       query: '
         {table}
         | where Timestamp >= datetime({start})
         | where Timestamp <= datetime({end})
-        | where SHA1 == "{file_hash}" or SHA256 == "{file_hash}" or MD5 == "{file_hash}"
+        | where SHA1 has "{file_hash}" or SHA256 has "{file_hash}" or MD5 has "{file_hash}"
         {add_query_items}'
-      uri: None
     parameters:
       file_hash:
-        description: Hash of file
+        description: File hash of the process
+        type: str
+  process_paths:
+    description: Return all processes with a matching path (part path) (all hosts)
+    metadata:
+      pivot:
+        short_name: processes_by_path
+    args:
+      query: '
+        {table}
+        | where Timestamp >= datetime({start})
+        | where Timestamp <= datetime({end})
+        | where FileName contains "{file_path}"
+        {add_query_items}'
+    parameters:
+      file_path:
+        description: full or partial path
+        type: str
+  process_cmd_line:
+    description: Lists all processes with a command line containing a string (all hosts)
+    metadata:
+      pivot:
+        short_name: processes_by_cmdline
+    args:
+      query: '
+        {table}
+        | where Timestamp >= datetime({start})
+        | where Timestamp <= datetime({end})
+        | where ProcessCommandLine contains "{cmd_line}"
+        {add_query_items}'
+    parameters:
+      cmd_line:
+        description: Command line artifact to search for
         type: str
-        aliases: hash
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_hunting.yaml` & `msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_hunting.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 metadata:
   version: 1
   description: MDATP Queries
   data_environments: [MDATP, MDE, M365D, LogAnalytics]
-  data_families: [MDATP, MDE]
+  data_families: [MDEHunting, M365DHunting]
   tags: ['user']
 defaults:
   metadata:
     data_source: 'hunting_queries'
   parameters:
       start:
         description: Query start time
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mde/kql_mdatp_network.yaml` & `msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_user.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,102 @@
 metadata:
   version: 1
   description: MDATP Queries
   data_environments: [MDATP, MDE, M365D, LogAnalytics]
-  data_families: [MDATP, MDE]
-  tags: ["network"]
+  data_families: [MDE, MDATP]
+  tags: ["user"]
 defaults:
   metadata:
-    data_source: "network_events"
+    data_source: "user_events"
   parameters:
-    table:
-      description: Table name
-      type: str
-      default: "DeviceNetworkEvents"
     start:
       description: Query start time
       type: datetime
     end:
       description: Query end time
       type: datetime
     add_query_items:
       description: Additional query clauses
       type: str
       default: ""
 sources:
-  list_connections:
-    description: Retrieves list of network connections
+  user_logons:
+    description: Return all user logons for user name
     metadata:
+      pivot:
+        short_name: logon_events
     args:
-      query: "
+      query: '
         {table}
         | where Timestamp >= datetime({start})
         | where Timestamp <= datetime({end})
-        {add_query_items}"
+        | where AccountName has "{account_name}"
+        {add_query_items}'
       uri: None
     parameters:
-  host_connections:
-    description: Lists alerts by for a specified hostname
+      table:
+        description: Logon events table
+        type: str
+        default: DeviceLogonEvents
+      account_name:
+        description: Name of user
+        type: str
+  user_processes:
+    description: Return all processes created by a user
     metadata:
       pivot:
-        short_name: net_connections
+        short_name: process_events
     args:
       query: '
         {table}
         | where Timestamp >= datetime({start})
         | where Timestamp <= datetime({end})
-        | where DeviceName has "{host_name}"
+        | where AccountName has "{account_name}"
         {add_query_items}'
     parameters:
-      host_name:
-        description: Name of host
+      table:
+        description: Process events table
+        type: str
+        default: DeviceProcessEvents
+      account_name:
+        description: Name of user
         type: str
-        aliases:
-          - hostname
-  ip_connections:
-    description: Lists alerts associated with a specified remote IP
+  user_files:
+    description: Return all files created by a user
     metadata:
       pivot:
-        short_name: net_connections
+        short_name: file_events
     args:
       query: '
         {table}
         | where Timestamp >= datetime({start})
         | where Timestamp <= datetime({end})
-        | where RemoteIP has "{ip_address}" or LocalIP has "{ip_address}"
+        | where InitiatingProcessAccountName contains "{account_name}"
         {add_query_items}'
     parameters:
-      ip_address:
-        description: Remote IP Address
+      table:
+        description: File events table
         type: str
-  url_connections:
-    description: Lists alerts associated with a specified URL
+        default: DeviceFileEvents
+      account_name:
+        description: Name of user
+        type: str
+  user_network:
+    description: Return all network connections associated with a user
     metadata:
       pivot:
-        short_name: net_connections
+        short_name: network_events
     args:
       query: '
         {table}
         | where Timestamp >= datetime({start})
         | where Timestamp <= datetime({end})
-        | where RemoteUrl has "{url}"
+        | where InitiatingProcessAccountName contains "{account_name}"
         {add_query_items}'
     parameters:
-      url:
-        description: Remote URL
+      table:
+        description: Network events table
         type: str
-  protocol_connections:
-    description: Lists alerts associated with a specified protocol
-    metadata:
-    args:
-      query: "
-        {table}
-        | where Timestamp >= datetime({start})
-        | where Timestamp <= datetime({end})
-        | where RemotePort == {protocol}
-        {add_query_items}"
-    parameters:
-      protocol:
-        description: Port to query for
+        default: DeviceNetworkEvents
+      account_name:
+        description: Name of user
         type: str
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/msgraph/graph_alerts.yaml` & `msticpy-2.6.0/msticpy/data/queries/msgraph/graph_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_alert.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_alert.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
           | extend AlertType = iif(isempty(AlertType), AlertName, AlertType)'
       add_query_items:
         description: Additional query clauses
         type: str
         default: ''
 sources:
   list_alerts:
-    description: Retrieves list of alerts
+    description: Returns security alerts for a given time range
     metadata:
     args:
       query: '
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
@@ -42,15 +42,15 @@
       start:
         description: Query start time
         type: datetime
       end:
         description: Query end time
         type: datetime
   list_alerts_counts:
-    description: Retrieves summary count of alerts by type
+    description: Returns summary count of alerts by type
     metadata:
     args:
       query: '
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
@@ -78,15 +78,15 @@
         | where SystemAlertId == "{system_alert_id}"
         {add_query_items}'
     parameters:
       system_alert_id:
         description: 'The ID of the alert'
         type: str
   list_related_alerts:
-    description: Retrieves list of alerts with a common host, account or process
+    description: Returns alerts with a host, account or process entity
     metadata:
       pivot:
         short_name: alerts
         direct_func_entities:
           - Host
           - Account
           - IpAddress
@@ -140,15 +140,15 @@
         description: Query end time
         type: datetime
       path_separator:
         description: Path separator
         type: str
         default: '\\'
   list_alerts_for_ip:
-    description: Retrieves list of alerts with a common IP Address
+    description: Returns alerts with the specified IP Address or addresses.
     metadata:
     args:
       query: '
         let src_ips = "{source_ip_list}";
         let src_ips_arr = split(src_ips, ",");
         let IP_table = toscalar(range idx from 0 to array_length(src_ips_arr) - 1 step 1
         | extend ip = trim(@"\\s*", tostring(src_ips_arr[idx]))
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         type: datetime
       add_query_items:
         description: Additional query clauses
         type: str
         default: ''
 sources:
   dns_lookups_for_domain:
-    description: Dns queries for a domain
+    description: Returns DNS query events for a specified domain
     metadata:
       pivot:
         short_name: queries
         direct_func_entities:
           - Dns
     args:
       query: '
@@ -39,15 +39,15 @@
         | where TimeGenerated <= datetime({end})
         {add_query_items}'
     parameters:
       domain:
         description: Domain to query for
         type: str
   dns_lookups_for_ip:
-    description: Dns queries for a domain
+    description: Returns Dns query events that contain a resolved IP address
     metadata:
       pivot:
         short_name: queries
         direct_func_entities:
           - IpAddress
     args:
       query: '
@@ -58,15 +58,15 @@
         | where TimeGenerated <= datetime({end})
         {add_query_items}'
     parameters:
       ip_address:
         description: IP lookup result to query for
         type: str
   dns_lookups_from_ip:
-    description: Dns queries for a domain
+    description: Returns Dns queries originating from a specified IP address
     metadata:
       pivot:
         short_name: queries_from_ip
         direct_func_entities:
           - IpAddress
     args:
       query: '
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             AllowedInFlows = AllowedInFlows_d,
             DeniedInFlows = DeniedInFlows_d,
             DeniedOutFlows = DeniedOutFlows_d,
             RemoteRegion = AzureRegion_s,
             VMRegion = Region_s'
 sources:
   az_net_analytics:
-    description: All Azure Network Analytics Data
+    description: Returns all Azure Network Flow (NSG) Data for a given host
     metadata:
       pivot:
         short_name: net_flows_depr
     args:
       query: '
         {table}
         | where SubType_s == "FlowLog"
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_azure.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_azure.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       type: datetime
     add_query_items:
       description: Additional query clauses
       type: str
       default: ""
 sources:
   list_aad_signins_for_account:
-    description: Lists Azure AD Signins for Account
+    description: Returns Azure AD Signins for Account
     metadata:
       pivot:
         short_name: signins
         direct_func_entities:
           - Account
     args:
       query: '
@@ -53,15 +53,15 @@
         type: str
         default: "!!DEFAULT!!"
       account_id:
         description: Azure user ID to find
         type: str
         default: "!!DEFAULT!!"
   list_aad_signins_for_ip:
-    description: Lists Azure AD Signins for an IP Address
+    description: Returns Azure AD Signins for an IP Address
     metadata:
       pivot:
         short_name: signins
         direct_func_entities:
           - IpAddress
     args:
       query: "
@@ -75,15 +75,15 @@
         description: Table name
         type: str
         default: SigninLogs
       ip_address_list:
         description: The IP Address or list of Addresses
         type: list
   list_azure_activity_for_account:
-    description: Lists Azure Activity for Account
+    description: Returns Azure Activity for Account
     metadata:
       pivot:
         short_name: activity
         direct_func_entities:
           - Account
     args:
       query: '
@@ -103,15 +103,15 @@
         description: Table name
         type: str
         default: AzureActivity
       account_name:
         description: The account name to find
         type: str
   list_azure_activity_for_ip:
-    description: Lists Azure Activity for Caller IP Address(es)
+    description: Returns Azure Activity for Caller IP Address(es)
     metadata:
       pivot:
         short_name: activity
         direct_func_entities:
           - IpAddress
     args:
       query: "
@@ -125,15 +125,15 @@
         description: Table name
         type: str
         default: AzureActivity
       ip_address_list:
         description: The IP Address or list of Addresses
         type: list
   list_azure_activity_for_resource:
-    description: Lists Azure Activity for a Resource
+    description: Returns Azure Activity for an Azure Resource ID
     metadata:
       pivot:
         short_name: activity
         direct_func_entities:
           - AzureResource
     args:
       query: '
@@ -166,15 +166,15 @@
         {add_query_items}'
     parameters:
       table:
         description: Table name
         type: str
         default: SigninLogs
   list_storage_ops_for_ip:
-    description:
+    description: Returns Storage Operations for an IP Address
     metadata:
       pivot:
         short_name: storage_ops
     args:
       query: '
         union
         StorageFileLogs,
@@ -199,15 +199,15 @@
         description: Table name
         type: str
         default: StorageFileLogs
       ip_address:
         description: Client IP Address
         type: str
   list_storage_ops_for_hash:
-    description:
+    description: Returns Azure Storage Operations for an MD5 file hash
     args:
       query: '
         union
         StorageFileLogs,
         StorageBlobLogs
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
@@ -229,15 +229,15 @@
         description: Table name
         type: str
         default: StorageFileLogs
       file_hash:
         description: MD5 hash of file
         type: str
   get_vmcomputer_for_ip:
-    description: Gets latest VMComputer record for IPAddress
+    description: Returns most recent VMComputer record for IPAddress
     metadata:
       pivot:
         short_name: vmcomputer
     args:
       query: '
         {table}
         | where TimeGenerated >= datetime({start})
@@ -250,15 +250,15 @@
         description: Table name
         type: str
         default: VMComputer
       ip_address:
         description: The IP Address of the VM
         type: str
   get_vmcomputer_for_host:
-    description: Gets latest VMComputer record for Host
+    description: Returns most recent VMComputer record for Host
     metadata:
       pivot:
         short_name: vmcomputer
     args:
       query: '
         {table}
         | where TimeGenerated >= datetime({start})
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       type: datetime
     add_query_items:
       description: Additional query clauses
       type: str
       default: ""
 sources:
   list_bookmarks:
-    description: Retrieves list of bookmarks
+    description: Retrieves list of bookmarks for a time range
     metadata:
     args:
       query: '
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
@@ -41,15 +41,15 @@
         | extend Account = QryResults["Account"]
         | extend Entities = QryResults.__entityMapping
         | project-away QryResults
         | where SoftDeleted == false
         {add_query_items}'
     parameters:
   list_bookmarks_for_entity:
-    description: Retrieves bookmarks for entity string
+    description: Retrieves bookmarks for a host, account, ip address, domain, url or other entity identifier
     metadata:
       pivot:
         short_name: bookmarks
         direct_func_entities:
           - Host
           - Account
           - IpAddress
@@ -100,15 +100,15 @@
         type: str
         default: na
       url:
         description: Url name
         type: str
         default: na
   get_bookmark_by_id:
-    description: Retrieves a single Bookmark by BookmarkId
+    description: Returns a single Bookmark by BookmarkId
     metadata:
     args:
       query: '
         {table}
         {query_project}
         HuntingBookmark
         | where BookmarkId =~ "{bookmark_id}"
@@ -139,15 +139,15 @@
         | where SoftDeleted == false
         {add_query_items}'
     parameters:
       bookmark_name:
         description: Name or part name of Bookmark
         type: str
   list_bookmarks_for_tags:
-    description: Retrieves Bookmark by one or mare Tags
+    description: Returns Bookmark by one or more Tags
     metadata:
     args:
       query: '
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
@@ -162,15 +162,15 @@
         | distinct *
         {add_query_items}'
     parameters:
       bookmark_tags:
         description: Bookmark tags
         type: list
   get_dynamic_summary_by_id:
-    description: Retrieves Dynamic Summary by SummaryId
+    description: Returns a Dynamic Summary by SummaryId
     metadata:
     args:
       query: '
         {table}
         | where SummaryId == "{summary_id}"
         | where SummaryStatus == "Active"
         | summarize arg_max(TimeGenerated, *) by SummaryId
@@ -183,15 +183,15 @@
         description: Table name
         type: str
         default: DynamicSummary
       summary_id:
         description: Dynamic Summary ID
         type: str
   get_dynamic_summary_by_name:
-    description: Retrieves Dynamic Summary by Name
+    description: Returns a Dynamic Summary by Name
     metadata:
     args:
       query: '
         let summary_header = {table}
         | where SummaryName == "{summary_name}" and SummaryStatus == "Active"
         | summarize arg_max(TimeGenerated, *) by SummaryId;
         summary_header
@@ -210,15 +210,15 @@
         description: Table name
         type: str
         default: DynamicSummary
       summary_name:
         description: Dynamic Summary Name
         type: str
   list_dynamic_summaries:
-    description: Retrieves Dynamic Summaries by date range
+    description: Returns all Dynamic Summaries by time range
     metadata:
     args:
       query: '
         {table}
         | where TimeGenerated between(datetime({start}) .. datetime({end}))
         | where SummaryStatus == "Active" or SummaryDataType == "SummaryItem"
         {add_query_items}'
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             SyslogMessage,
             ProcessID,
             ProcessName,
             HostIP,
           | extend TimeCreatedUtc=TimeGenerated'
 sources:
   sudo_activity:
-    description: All sudo activity
+    description: Returns all sudo activity for a host and account name
     args:
       query: '
         {table}
         | where {subscription_filter}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
         | where Computer {host_op} "{host_name}"
@@ -71,28 +71,28 @@
         {add_query_items}'
     parameters:
       account_name:
         description: Username to filter the search by
         type: str
         default: ''
   cron_activity:
-    description: All cron activity
+    description: Returns all cron activity for a host
     args:
       query: '
         {table}
         | where {subscription_filter}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
         | where Computer {host_op} "{host_name}"
         | where ProcessName == "CRON" or Facility == "cron"
         | extend CMD=extract("CMD(.*)",1,SyslogMessage), User=extract("for user ([[:alpha:]]*)",1,SyslogMessage), CronUser=extract("^[(]([[:alpha:]]*)",1,SyslogMessage),EditStatus=extract("[A-Z]+ EDIT",0,SyslogMessage)
         {add_query_items}'
     parameters:
   user_group_activity:
-    description: All user/group additions, deletions, and modifications
+    description: Returns all user/group additions, deletions, and modifications for a host
     args:
       query: '
         {table}
         | where {subscription_filter}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
         | where Computer {host_op} "{host_name}"
@@ -114,27 +114,27 @@
         | where {subscription_filter}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
         | where Computer {host_op} "{host_name}"
         {add_query_items}'
     parameters:
   summarize_events:
-    description: Returns all syslog activity for a host
+    description: Returns summarized syslog activity for a host
     args:
       query: '
          {table}
         | where {subscription_filter}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
         | where Computer {host_op} "{host_name}"
         | summarize count() by Facility, SeverityLevel, ProcessName
         {add_query_items}'
     parameters:
   notable_events:
-    description: Returns all syslog activity for a host
+    description: Returns all 'alert' and 'crit' syslog activity for a host
     args:
       query: '
          {table}
         | where {subscription_filter}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
         | where Computer {host_op} "{host_name}"
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             SyslogMessage,
             ProcessID,
             ProcessName,
             HostIP,
           | extend TimeCreatedUtc=TimeGenerated'
 sources:
   squid_activity:
-    description: All squid proxy activity
+    description: Returns all squid proxy activity for a host
     args:
       query: '
         {table}
         | where {subscription_filter}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
         | where Computer == "{host_name}"
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         SyslogMessage,
         ProcessID,
         ProcessName,
         HostIP,
         | extend TimeCreatedUtc=TimeGenerated"
 sources:
   user_logon:
-    description: All user logon events on a host
+    description: User logon events on a host
     args:
       query: '
         {table}
         | where {subscription_filter}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
         | where Computer has "{host_name}"
@@ -111,15 +111,15 @@
         | extend AccountName = User
         {add_query_items}'
     parameters:
       host_name:
         description: Hostname to query for
         type: str
   list_logons_for_account:
-    description: All successful user logon events for account (all hosts)
+    description: Successful user logon events for account name (all hosts)
     metadata:
       pivot:
         short_name: logons
         direct_func_entities:
           - Account
     args:
       query: '
@@ -164,15 +164,15 @@
         UID = extract("uid=([0-9]+)", 1, SyslogMessage)
         {add_query_items}'
     parameters:
       account_name:
         description: The account name to search on
         type: str
   list_logons_for_source_ip:
-    description: All successful user logon events for source IP (all hosts)
+    description: Successful user logon events for source IP (all hosts)
     metadata:
       pivot:
         short_name: logons
         direct_func_entities:
           - IpAddress
     args:
       query: '
@@ -247,15 +247,15 @@
         | extend LogonProcessName = ProcessName
         {add_query_items}'
     parameters:
       host_name:
         description: Hostname to query for
         type: str
   list_host_logon_failures:
-    description: All failed user logon events on a host
+    description: Failed user logon events on a host
     metadata:
       pivot:
         short_name: logon_failures
         direct_func_entities:
           - Host
     args:
       query: *logon_failures
@@ -264,15 +264,15 @@
         description: Hostname to query for
         type: str
     query_macros:
       query_condition:
         description: Hostname where clause
         value: '| where Computer has "{host_name}"'
   list_ip_logon_failures:
-    description: All failed user logon events from an IP address
+    description: Failed user logon events from an IP address
     metadata:
       pivot:
         short_name: logon_failures
         direct_func_entities:
           - IpAddress
     args:
       query: *logon_failures
@@ -281,15 +281,15 @@
         description: Ip Address to query for
         type: str
     query_macros:
       query_condition:
         description: IP Address where clause
         value: '| where SyslogMessage has "{ip_address}"'
   list_account_logon_failures:
-    description: All failed user logon events from an IP address
+    description: All failed user logon events for account name
     metadata:
       pivot:
         short_name: logon_failures
         direct_func_entities:
           - Account
     args:
       query: *logon_failures
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         default: ''
       subscription_filter:
         description: Optional subscription/tenant filter expression
         type: str
         default: "true"
 sources:
   sysmon_process_events:
-    description: Get Process Events from a specified host
+    description: Sysmon Process Events on host
     metadata:
     args:
       query: |
         let ParsedProcessEvent=(){{
         Syslog
         | where {subscription_filter}
         | where TimeGenerated >= datetime({start})
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_net.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_net.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
       default: "SourceIP"
     dest_ip_field:
       description: The column name containing destination IP
       type: str
       default: "DestinationIP"
 sources:
   get_ips_for_host:
-    description: Gets the latest AzureNetworkAnalytics interface event for a host.
+    description: Returns the most recent Azure Network NSG Interface event for a host.
     metadata:
       pivot:
         short_name: interface
         direct_func_entities:
           - Host
     args:
       query: '
@@ -89,15 +89,15 @@
         description: Name of host
         type: str
       table:
         description: Table name
         type: str
         default: AzureNetworkAnalytics_CL
   get_host_for_ip:
-    description: Gets the latest AzureNetworkAnalytics interface event for a host.
+    description: Returns the most recent Azure NSG Interface event for an IP Address.
     metadata:
       pivot:
         short_name: interface
         direct_func_entities:
           - IpAddress
     args:
       query: '
@@ -115,15 +115,15 @@
         description: IP Address
         type: str
       table:
         description: Table name
         type: str
         default: AzureNetworkAnalytics_CL
   get_heartbeat_for_host:
-    description: Retrieves latest OMS Heartbeat event for host.
+    description: Returns latest OMS Heartbeat event for host.
     metadata:
       data_families: [AzureNetwork, Network, Heartbeat]
       pivot:
         short_name: heartbeat
         direct_func_entities:
           - Host
     args:
@@ -137,15 +137,15 @@
         description: Name of host
         type: str
       table:
         description: Table name
         type: str
         default: Heartbeat
   get_heartbeat_for_ip:
-    description: Retrieves latest OMS Heartbeat event for ip address.
+    description: Returns latest OMS Heartbeat event for ip address.
     metadata:
       data_families: [AzureNetwork, Network, Heartbeat]
       pivot:
         short_name: heartbeat
         direct_func_entities:
           - IpAddress
     args:
@@ -159,15 +159,15 @@
         description: IP Address
         type: str
       table:
         description: Table name
         type: str
         default: Heartbeat
   list_azure_network_flows_by_ip:
-    description: Retrieves Azure network analytics flow events.
+    description: Returns Azure NSG flow events for an IP Address.
     metadata:
       pivot:
         short_name: net_flows
         direct_func_entities:
           - IpAddress
     args:
       query: *azure_network_base_query
@@ -193,15 +193,15 @@
       query_condition:
         description: Query-specific where clause
         value: '| where (VMIP_s in ({ip_address_list})
            or SrcIP_s in ({ip_address_list})
            or DestIP_s in ({ip_address_list})
           )'
   list_azure_network_flows_by_host:
-    description: Retrieves Azure network analytics flow events.
+    description: Returns Azure NSG flow events for a host.
     metadata:
       pivot:
         short_name: net_flows
         direct_func_entities:
           - Host
     args:
       query: *azure_network_base_query
@@ -224,15 +224,15 @@
         type: str
         default: AzureNetworkAnalytics_CL
     query_macros:
       query_condition:
         description: Query-specific where clause
         value: '| where VM_s has "{host_name}"'
   network_connections_to_url:
-    description: List of network connections to a URL
+    description: Returns connections to a URL or domain (CommonSecurityLog)
     metadata:
       pivot:
         short_name: url_connections
         direct_func_entities:
           - URL
     args:
       query: '
@@ -245,18 +245,18 @@
         {add_query_items}'
     parameters:
       table:
         description: The table to run against
         type: str
         default: "CommonSecurityLog"
       url:
-        description: URL to search for
+        description: URL or partial URL to search for
         type: str
   host_network_connections_csl:
-    descritpion: List network connections to and from a host using CommonSecurityLog
+    description: Returns network connections to and from a host (CommonSecurityLog)
     metadata:
       pivot:
         short_name: host_connections_csl
         direct_func_entities:
           - Host
     args:
       query: '
@@ -273,15 +273,15 @@
         type: str
         default: "CommonSecurityLog"
       host_name:
         description: Name of host
         type: str
         default: ""
   ip_network_connections_csl:
-    descritpion: List network connections to and from an IP address using CommonSecurityLog
+    descritpion: Returns network connections to and from an IP address (CommonSecurityLog)
     metadata:
       pivot:
         short_name: ip_connections_csl
         direct_func_entities:
           - IP
     args:
       query: '
@@ -298,15 +298,15 @@
         type: str
         default: "CommonSecurityLog"
       ip_address:
         description: IP address of host
         type: str
         default: ""
   all_network_connections_csl:
-    descritpion: List network connections to and from an IP address using CommonSecurityLog
+    descritpion: Returns all network connections for a time range (CommonSecurityLog)
     args:
       query: '
         {table}
         | where TimeGenerated between(datetime({start})..datetime({end}))
         | where DeviceVendor in ({vendors})
         | extend SourceIP = {source_ip_field}
         | extend DestinationIP = {dest_ip_field}
@@ -314,15 +314,15 @@
         {add_query_items}'
     parameters:
       table:
         description: The table to run against
         type: str
         default: "CommonSecurityLog"
   ips_by_host_csl:
-    descritpion: All IP addresses associated with a host using CommonSecurityLog
+    descritpion: Returns all IP addresses associated with a host (CommonSecurityLog)
     metadata:
       pivot:
         short_name: ips_csl
         direct_func_entities:
           - Host
     args:
       query: '
@@ -340,15 +340,15 @@
         type: str
         default: "CommonSecurityLog"
       host_name:
         description: Name of host
         type: str
         default: ""
   hosts_by_ip_csl:
-    descritpion: All hosts associated with a IP addresses using CommonSecurityLog
+    descritpion: Returns hosts associated with a IP addresses (CommonSecurityLog)
     metadata:
       pivot:
         short_name: hosts_csl
         direct_func_entities:
           - IP
     args:
       query: '
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_o365.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_o365.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 metadata:
   version: 1
   description: Kql Sentinel Azure
   data_environments: [LogAnalytics]
   data_families: [Office365]
-  tags: ['office', 'o365']
+  tags: ['office', 'o365', 'sharepoint', 'exchange', 'onedrive', 'teams']
 defaults:
   metadata:
     data_source: 'OfficeActivity'
   parameters:
       start:
         description: Query start time
         type: datetime
@@ -16,15 +16,15 @@
         type: datetime
       add_query_items:
         description: Additional query clauses
         type: str
         default: ''
 sources:
   list_activity_for_account:
-    description: Lists Office Activity for Account
+    description: Lists Office/O365 Activity for Account
     metadata:
       pivot:
         short_name: activity
         direct_func_entities:
           - Account
     args:
       query: '
@@ -44,15 +44,15 @@
         description: Table name
         type: str
         default: OfficeActivity
       account_name:
         description: The account name to find
         type: str
   list_activity_for_ip:
-    description: Lists Office Activity for Caller IP Address(es)
+    description: Lists Office/O365 Activity for Caller IP Address(es)
     metadata:
       pivot:
         short_name: activity
         direct_func_entities:
           - IpAddress
     args:
       query: '
@@ -66,15 +66,15 @@
         description: Table name
         type: str
         default: OfficeActivity
       ip_address_list:
         description: The IP Address or list of Addresses
         type: list
   list_activity_for_resource:
-    description: Lists Office Activity for a Resource
+    description: Lists Office/O365 Activity for a Resource (OfficeObjectId)
     metadata:
       pivot:
         short_name: activity
         direct_func_entities:
           - AzureResource
     args:
       query: '
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -24,28 +24,28 @@
         type: datetime
       add_query_items:
         description: Additional query clauses
         type: str
         default: ''
 sources:
   list_indicators:
-    description: Retrieves list of all current indicators.
+    description: Returns list of all current indicators.
     metadata:
     args:
       query: '
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
         | summarize arg_max(TimeGenerated, *) by IndicatorId
         {add_query_items}'
       uri: None
     parameters:
   list_indicators_by_ip:
-    description: Retrieves list of indicators by IP Address
+    description: Returns list of indicators by IP Address
     metadata:
     args:
       query: '
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
@@ -67,15 +67,15 @@
     parameters:
       ip_address_list:
         description: Ip Address to query for
         type: list
         aliases:
           - observables
   list_indicators_by_hash:
-    description: Retrieves list of indicators by file hash
+    description: Returns list of indicators by file hash
     metadata:
     args:
       query: '
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
@@ -86,15 +86,15 @@
     parameters:
       file_hash_list:
         description: File hash(es) to query for
         type: list
         aliases:
           - observables
   list_indicators_by_filepath:
-    description: Retrieves list of indicators by file path
+    description: Returns list of indicators by file path
     metadata:
     args:
       query: '
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
@@ -103,15 +103,15 @@
         | summarize arg_max(TimeGenerated, *) by IndicatorId
         {add_query_items}'
     parameters:
       observables:
         description: List of observables
         type: list
   list_indicators_by_domain:
-    description: Retrieves list of indicators by domain
+    description: Returns list of indicators by domain
     metadata:
     args:
       query: '
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
@@ -127,15 +127,15 @@
     parameters:
       domain_list:
         description: Domain(s) to query for
         type: list
         aliases:
           - observables
   list_indicators_by_email:
-    description: Retrieves list of indicators by email address
+    description: Returns list of indicators by email address
     metadata:
     args:
       query: '
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
@@ -149,15 +149,15 @@
         | summarize arg_max(TimeGenerated, *) by IndicatorId
         {add_query_items}'
     parameters:
       observables:
         description: List of observables
         type: list
   list_indicators_by_url:
-    description: Retrieves list of indicators by URL
+    description: Returns list of indicators by URL
     metadata:
     args:
       query: '
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -45,68 +45,68 @@
         default: 'Total'
       aggregatefunction:
         description: Aggregation functions to use - count(), sum(), avg() etc
         type: str
         default: 'count()'
 sources:
   get_timeseries_data:
-    description: Retrieves TimeSeriesData prepared to use with built-in KQL time series functions
+    description: Generic query to return TimeSeriesData for use with native KQL time series functions
     args:
       query: '
             {table}
             {where_clause}
             | project {timestampcolumn},{aggregatecolumn},{groupbycolumn}
             | where {timestampcolumn} >= datetime({start})
             | where {timestampcolumn} <= datetime({end})
             | make-series {aggregatecolumn}={aggregatefunction} on {timestampcolumn} from datetime({start}) to datetime({end}) step {timeframe} by {groupbycolumn}
             {add_query_items}'
   get_timeseries_decompose:
-    description: Time Series decomposition and anomalies generated using built-in KQL time series function- series_decompose
+    description: Generic Time Series decomposition using native KQL analysis (series_decompose)
     args:
       query: '
             {table}
             {where_clause}
             | project {timestampcolumn},{aggregatecolumn},{groupbycolumn}
             | where {timestampcolumn} >= datetime({start})
             | where {timestampcolumn} <= datetime({end})
             | make-series {aggregatecolumn}={aggregatefunction} on {timestampcolumn} from datetime({start}) to datetime({end}) step {timeframe} by {groupbycolumn}
             | extend (baseline,seasonal,trend,residual) = series_decompose({aggregatecolumn})
             | mv-expand {aggregatecolumn} to typeof(double), {timestampcolumn} to typeof(datetime), baseline to typeof(double), seasonal to typeof(double), trend to typeof(long), residual to typeof(long)
             {add_query_items}'
   get_timeseries_anomalies:
-    description: Time Series filtered anomalies detected using built-in KQL time series function-series_decompose_anomalies
+    description: Time Series filtered anomalies using native KQL analysis (series_decompose_anomalies)
     args:
       query: '
             {table}
             {where_clause}
             | project {timestampcolumn},{aggregatecolumn},{groupbycolumn}
             | where {timestampcolumn} >= datetime({start})
             | where {timestampcolumn} <= datetime({end})
             | make-series {aggregatecolumn}={aggregatefunction} on {timestampcolumn} from datetime({start}) to datetime({end}) step {timeframe} by {groupbycolumn}
             | extend (anomalies, score, baseline) = series_decompose_anomalies({aggregatecolumn}, {scorethreshold},-1,"linefit")
             | mv-expand {aggregatecolumn} to typeof(double), {timestampcolumn} to typeof(datetime), anomalies to typeof(double), score to typeof(double), baseline to typeof(long)
             | extend score = round(score,2)
             {add_query_items}'
   plot_timeseries_datawithbaseline:
-    description: Plot timeseries data using built-in KQL time series decomposition using built-in KQL render method
+    description: Plot of Time Series data using native KQL analysis and plot rendering (KQLMagic only)
     args:
       query: '
             {table}
             {where_clause}
             | project {timestampcolumn},{aggregatecolumn},{groupbycolumn}
             | where {timestampcolumn} >= datetime({start})
             | where {timestampcolumn} <= datetime({end})
             | make-series {aggregatecolumn}={aggregatefunction} on {timestampcolumn} from datetime({start}) to datetime({end}) step {timeframe} by {groupbycolumn}
             | extend (baseline,seasonal,trend,residual) = series_decompose({aggregatecolumn})
             | mv-expand {aggregatecolumn} to typeof(double), {timestampcolumn} to typeof(datetime), baseline to typeof(long), seasonal to typeof(long), trend to typeof(long), residual to typeof(long)
             | project {timestampcolumn}, {aggregatecolumn}, baseline
             | render timechart with (title="Time Series Decomposition - Baseline vs Observed TimeChart")
-            {add_query_items}'
+            '
   plot_timeseries_scoreanomolies:
-    description: Plot timeseries anomaly score using built-in KQL render method
+    description: Plot Time Series anomaly score using native KQL render (KQLMagic only)
     args:
       query: '
             {table}
             {where_clause}
             | project {timestampcolumn},{aggregatecolumn},{groupbycolumn}
             | where {timestampcolumn} >= datetime({start})
             | where {timestampcolumn} <= datetime({end})
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         type: datetime
       add_query_items:
         description: Additional query clauses
         type: str
         default: ''
 sources:
   list_host_events:
-    description: Retrieves list of all events on a host
+    description: Returns list of all events on a host
     metadata:
       pivot:
         short_name: all_events
         direct_func_entities:
           - Host
     args:
       query: '
@@ -47,15 +47,15 @@
         description: Name of host
         type: str
       host_op:
         description: The hostname match operator
         type: str
         default: has
   list_host_events_by_id:
-    description: Retrieves list of events on a host
+    description: Returns list of specified event IDs on a host
     metadata:
       pivot:
         short_name: events_by_id
         direct_func_entities:
           - Host
     args:
       query: '
@@ -75,15 +75,15 @@
         type: str
         default: has
       event_list:
         description: List of event IDs to match
         type: list
         default: has
   list_other_events:
-    description: Retrieves list of events other than logon and process on a host
+    description: Returns list of events other than logon and process on a host
     args:
       query: '
         {table}
         {query_project}
         | where EventID !in ("4688", "4624", "4625")
         | where Computer {host_op} "{host_name}"
         | where TimeGenerated >= datetime({start})
@@ -104,29 +104,29 @@
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
         {add_query_items}'
     parameters:
   list_events_by_id:
-    description: Retrieves list of events on a host
+    description: Returns list of events on a host by EventID
     args:
       query: '
         {table}
         {query_project}
         | where EventID in ({event_list})
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
         {add_query_items}'
     parameters:
       event_list:
         description: List of event IDs to match
         type: list
   summarize_events:
-    description: Summarizes a the events on a host
+    description: Summarize the events on a host by event type
     args:
       query: '
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
         | where Computer {host_op} "{host_name}"
@@ -137,15 +137,15 @@
         description: Name of host
         type: str
       host_op:
         description: The hostname match operator
         type: str
         default: has
   schdld_tasks_and_services:
-    description: Gets events related to scheduled tasks and services
+    description: Returns scheduled tasks and services events (4698, 4700, 4697, 4702)
     args:
       query: '
         let account_evnt_ids = dynamic([4698, 4700, 4697, 4702]);
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
@@ -167,15 +167,15 @@
         description: Name of host to get events from
         type: str
       host_op:
         description: The hostname match operator
         type: str
         default: has
   account_change_events:
-    description: Gets events related to account changes
+    description: Returns events related to account changes
     args:
       query: '
         let account_evnt_ids = dynamic([4720, 4725, 4727, 4728, 4731, 4732, 4740, 4754, 4756, 4767]);
         {table}
         {query_project}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
@@ -186,15 +186,15 @@
         description: Name of host to get events from
         type: str
       host_op:
         description: The hostname match operator
         type: str
         default: has
   notable_events:
-    description: Get notebable Windows events not returned in other queries
+    description: Return other significant Windows events not returned in other queries
     args:
       query: '
         let evnt_ids = dynamic([1102, 4657]);
         let excld_evnt_ids = dynamic([4625, 4624, 4688, 4720, 4725, 4727, 4728, 4731, 4732, 4740, 4754, 4756, 4767, 4702]);
         let rare_events = ({table}
         | where TimeGenerated >= datetime({start})
         | where TimeGenerated <= datetime({end})
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
       default: ""
     subscription_filter:
       description: Optional subscription/tenant filter expression
       type: str
       default: "true"
 sources:
   get_host_logon:
-    description: Retrieves the logon event for the session id on the host
+    description: Returns the logon event for the logon session id on a host
     metadata:
       pivot:
         short_name: logon_session
     args:
       query: '
         {table}
         {event_filter}
@@ -77,15 +77,15 @@
       host_name:
         description: Name of host
         type: str
       logon_session_id:
         description: The logon session ID of the source process
         type: str
   list_host_logons:
-    description: Retrieves the logon events on the host
+    description: Returns the logon events on a host for time range
     metadata:
       pivot:
         short_name: logons
         direct_func_entities:
           - Host
     args:
       query: '
@@ -98,15 +98,15 @@
         | where TimeGenerated <= datetime({end})
         {add_query_items}'
     parameters:
       host_name:
         description: Name of host
         type: str
   list_host_logon_failures:
-    description: Retrieves the logon failure events on the host
+    description: Returns the logon failure events on a host for time range
     metadata:
       pivot:
         short_name: logon_failures
         direct_func_entities:
           - Host
     args:
       query: '
@@ -123,15 +123,15 @@
         description: Name of host
         type: str
       event_filter:
         description: Table name
         type: str
         default: "| where EventID == 4625"
   list_logons_by_account:
-    description: Retrieves the logon events for an account
+    description: Returns the logon success events for an account (all hosts)
     metadata:
       pivot:
         short_name: logons
         direct_func_entities:
           - Account
     args:
       query: '
@@ -144,15 +144,15 @@
         | where TimeGenerated <= datetime({end})
         {add_query_items}'
     parameters:
       account_name:
         description: The account name to find
         type: str
   list_logon_attempts_by_account:
-    description: Retrieves the logon events for an account
+    description: Retrieves all logon events for an account (all hosts)
     metadata:
       pivot:
         short_name: logon_attempts
         direct_func_entities:
           - Account
     args:
       query: '
@@ -169,15 +169,15 @@
         description: The account name to find
         type: str
       event_filter:
         description: Event ID filter
         type: str
         default: "| where EventID in (4624, 4625)"
   list_logon_failures_by_account:
-    description: Retrieves the logon failure events  for an account
+    description: Returns the logon failure events for an account (all hosts)
     metadata:
       pivot:
         short_name: logon_failures
         direct_func_entities:
           - Account
     args:
       query: '
@@ -194,15 +194,15 @@
         description: The account name to find
         type: str
       event_filter:
         description: Event ID filter
         type: str
         default: "| where EventID == 4625"
   list_all_logons_by_host:
-    description: account all failed or successful logons to a host
+    description: Returns all failed or successful logons on a host
     metadata:
       pivot:
         short_name: logon_attempts
         direct_func_entities:
           - Host
     args:
       query: '
@@ -221,15 +221,15 @@
         description: Name of host
         type: str
       event_filter:
         description: Event ID filter
         type: str
         default: "| where EventID in (4624, 4625)"
   list_logon_attempts_by_ip:
-    description: Retrieves the logon events for an IP Address
+    description: Returns the logon events for an IP Address (all hosts)
     metadata:
       pivot:
         short_name: logon_attempts
         direct_func_entities:
           - Account
     args:
       query: '
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml` & `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         default: 'true'
       path_separator:
         description: Path separator
         type: str
         default: '\\'
 sources:
   list_host_processes:
-    description: Retrieves list of processes on a host
+    description: Returns list of processes on a host for a time range
     metadata:
       pivot:
         short_name: processes
         direct_func_entities:
           - Host
     args:
       query: '
@@ -82,15 +82,15 @@
         description: Name of host
         type: str
       host_op:
         description: The hostname match operator
         type: str
         default: has
   list_matching_processes:
-    description: Retrieves list of processes matching process name
+    description: Returns list of processes matching process name (all hosts)
     metadata:
       pivot:
         short_name: similar_processes
         direct_func_entities:
           - Process
     args:
       query: '
@@ -109,15 +109,15 @@
         description: Name of process
         type: str
       proc_op:
         description: The process name match operator
         type: str
         default: has
   get_process_tree:
-    description: Retrieves the process tree of a supplied process
+    description: Returns the process tree for process id, session id and host name.
     args:
       query: '
         let start = datetime({start});
         let end = datetime({end});
         let sourceProcessId = "{process_id}";
         let sourceLogonId = "{logon_session_id}";
         let sourceProcess =
@@ -222,15 +222,15 @@
       process_id:
         description: The process ID of the source process
         type: str
       logon_session_id:
         description: The logon session ID of the source process
         type: str
   get_parent_process:
-    description: Retrieves the parent process of a supplied process
+    description: Returns the parent process of process (process id, session id and host name)
     metadata:
       pivot:
         short_name: parent_process
         direct_func_entities:
           - Process
     args:
       query: '
@@ -282,15 +282,15 @@
         description: The logon session ID of the source process
         type: str
       parent_lookback:
         description: The number of hours to look back for parent process
         type: int
         default: 2
   list_hosts_matching_commandline:
-    description: Retrieves processes on hosts with matching commandline
+    description: Returns processes on hosts with matching command line
     metadata:
       pivot:
         short_name: processes_with_same_commandline
         direct_func_entities:
           - Process
     args:
       query: '
@@ -307,15 +307,15 @@
       process_name:
         description: Name of process
         type: str
       commandline:
         description: The command line of the source process
         type: str
   list_processes_in_session:
-    description: Retrieves all processes on the host for a logon session
+    description: Returns all processes on the host for a logon session
     metadata:
       pivot:
         short_name: process_session
         direct_func_entities:
           - Host
           - Process
     args:
@@ -332,16 +332,10 @@
         | extend commandlineparts = arraylength(split(CommandLine, " "))
         | extend commandlinelen = strlen(CommandLine)
         {add_query_items}'
     parameters:
       host_name:
         description: Name of host
         type: str
-      process_name:
-        description: Name of process
-        type: str
-      process_id:
-        description: The process ID of the source process
-        type: str
       logon_session_id:
         description: The logon session ID of the source process
         type: str
```

### Comparing `msticpy-2.5.3/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml` & `msticpy-2.6.0/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/resourcegraph/sentinel_resources.yaml` & `msticpy-2.6.0/msticpy/data/queries/resourcegraph/sentinel_resources.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/splunk/splunk_alert_queries.yaml` & `msticpy-2.6.0/msticpy/data/queries/splunk/splunk_alert_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/splunk/splunk_authentication_queries.yaml` & `msticpy-2.6.0/msticpy/data/queries/splunk/splunk_authentication_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/splunk/splunk_queries.yaml` & `msticpy-2.6.0/msticpy/data/queries/splunk/splunk_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/queries/sumologic/sumologic_queries.yaml` & `msticpy-2.6.0/msticpy/data/queries/sumologic/sumologic_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/query_container.py` & `msticpy-2.6.0/msticpy/data/query_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/query_defns.py` & `msticpy-2.6.0/msticpy/data/query_defns.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/sql_to_kql.py` & `msticpy-2.6.0/msticpy/data/sql_to_kql.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/storage/azure_blob_storage.py` & `msticpy-2.6.0/msticpy/data/storage/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/uploaders/__init__.py` & `msticpy-2.6.0/msticpy/data/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/uploaders/loganalytics_uploader.py` & `msticpy-2.6.0/msticpy/data/uploaders/loganalytics_uploader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/uploaders/splunk_uploader.py` & `msticpy-2.6.0/msticpy/data/uploaders/splunk_uploader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/data/uploaders/uploader_base.py` & `msticpy-2.6.0/msticpy/data/uploaders/uploader_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/__init__.py` & `msticpy-2.6.0/msticpy/datamodel/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/account.py` & `msticpy-2.6.0/msticpy/datamodel/entities/account.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/alert.py` & `msticpy-2.6.0/msticpy/datamodel/entities/alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/azure_resource.py` & `msticpy-2.6.0/msticpy/datamodel/entities/azure_resource.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/cloud_application.py` & `msticpy-2.6.0/msticpy/datamodel/entities/cloud_application.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/cloud_logon_session.py` & `msticpy-2.6.0/msticpy/datamodel/entities/cloud_logon_session.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/dns.py` & `msticpy-2.6.0/msticpy/datamodel/entities/dns.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/entity.py` & `msticpy-2.6.0/msticpy/datamodel/entities/entity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/entity_enums.py` & `msticpy-2.6.0/msticpy/datamodel/entities/entity_enums.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/entity_graph.py` & `msticpy-2.6.0/msticpy/datamodel/entities/entity_graph.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/file.py` & `msticpy-2.6.0/msticpy/datamodel/entities/file.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/file_hash.py` & `msticpy-2.6.0/msticpy/datamodel/entities/file_hash.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/geo_location.py` & `msticpy-2.6.0/msticpy/datamodel/entities/geo_location.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/graph_property.py` & `msticpy-2.6.0/msticpy/datamodel/entities/graph_property.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/host.py` & `msticpy-2.6.0/msticpy/datamodel/entities/host.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/host_logon_session.py` & `msticpy-2.6.0/msticpy/datamodel/entities/host_logon_session.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/iot_device.py` & `msticpy-2.6.0/msticpy/datamodel/entities/iot_device.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/ip_address.py` & `msticpy-2.6.0/msticpy/datamodel/entities/ip_address.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/mail_cluster.py` & `msticpy-2.6.0/msticpy/datamodel/entities/mail_cluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/mail_message.py` & `msticpy-2.6.0/msticpy/datamodel/entities/mail_message.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/mailbox.py` & `msticpy-2.6.0/msticpy/datamodel/entities/mailbox.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/malware.py` & `msticpy-2.6.0/msticpy/datamodel/entities/malware.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/network_connection.py` & `msticpy-2.6.0/msticpy/datamodel/entities/network_connection.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/process.py` & `msticpy-2.6.0/msticpy/datamodel/entities/process.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/registry_key.py` & `msticpy-2.6.0/msticpy/datamodel/entities/registry_key.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/registry_value.py` & `msticpy-2.6.0/msticpy/datamodel/entities/registry_value.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/security_group.py` & `msticpy-2.6.0/msticpy/datamodel/entities/security_group.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/submission_mail.py` & `msticpy-2.6.0/msticpy/datamodel/entities/submission_mail.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/threat_intelligence.py` & `msticpy-2.6.0/msticpy/datamodel/entities/threat_intelligence.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/unknown_entity.py` & `msticpy-2.6.0/msticpy/datamodel/entities/unknown_entity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/entities/url.py` & `msticpy-2.6.0/msticpy/datamodel/entities/url.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/pivot.py` & `msticpy-2.6.0/msticpy/datamodel/pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/soc/incident.py` & `msticpy-2.6.0/msticpy/datamodel/soc/incident.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/datamodel/soc/sentinel_alert.py` & `msticpy-2.6.0/msticpy/datamodel/soc/sentinel_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/__init__.py` & `msticpy-2.6.0/msticpy/init/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/azure_ml_tools.py` & `msticpy-2.6.0/msticpy/init/azure_ml_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/azure_synapse_tools.py` & `msticpy-2.6.0/msticpy/init/azure_synapse_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/logging.py` & `msticpy-2.6.0/msticpy/init/logging.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/mp_pandas_accessors.py` & `msticpy-2.6.0/msticpy/init/mp_pandas_accessors.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/mp_plugins.py` & `msticpy-2.6.0/msticpy/init/mp_plugins.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/nbinit.py` & `msticpy-2.6.0/msticpy/init/nbinit.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,15 +417,15 @@
     else:
         # If not in AML check and print version status
         stdout_cap = io.StringIO()
         with redirect_stdout(stdout_cap):
             check_version()
             output = stdout_cap.getvalue()
             _pr_output(output)
-            logger.info(output)
+            logger.info("Check version failures: %s", output)
 
     if _detect_env("synapse", **kwargs) and is_in_synapse():
         synapse_params = {
             key: val for key, val in kwargs.items() if key in _SYNAPSE_KWARGS
         }
         init_synapse(**synapse_params)
 
@@ -434,15 +434,15 @@
     stdout_cap = io.StringIO()
     with redirect_stdout(stdout_cap):
         imp_ok = _global_imports(
             namespace, additional_packages, user_install, extra_imports, def_imports
         )
         output = stdout_cap.getvalue()
         _pr_output(output)
-        logger.info(output)
+        logger.info("Import failures: %s", output)
 
     # Configuration check
     if no_config_check:
         conf_ok = True
     else:
         _pr_output("Checking configuration....")
         conf_ok = _get_or_create_config()
@@ -464,24 +464,25 @@
     # load pivots
     stdout_cap = io.StringIO()
     with redirect_stdout(stdout_cap):
         _pr_output("Loading pivots.")
         _load_pivots(namespace=namespace)
         output = stdout_cap.getvalue()
         _pr_output(output)
-        logger.info(output)
+        logger.info("Pivot load failures: %s", output)
 
     # User defaults
     stdout_cap = io.StringIO()
     with redirect_stdout(stdout_cap):
         _pr_output("Loading user defaults.")
         prov_dict = load_user_defaults()
         output = stdout_cap.getvalue()
         _pr_output(output)
         logger.info(output)
+        logger.info("User default load failures: %s", output)
 
     if prov_dict:
         namespace.update(prov_dict)
         current_providers = prov_dict
         _pr_output("Auto-loaded components:", ", ".join(prov_dict.keys()))
 
     # show any warnings
```

### Comparing `msticpy-2.5.3/msticpy/init/nbmagics.py` & `msticpy-2.6.0/msticpy/init/nbmagics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/pivot.py` & `msticpy-2.6.0/msticpy/init/pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/pivot_core/pivot_browser.py` & `msticpy-2.6.0/msticpy/init/pivot_core/pivot_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/pivot_core/pivot_container.py` & `msticpy-2.6.0/msticpy/init/pivot_core/pivot_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/pivot_core/pivot_magic_core.py` & `msticpy-2.6.0/msticpy/init/pivot_core/pivot_magic_core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/pivot_core/pivot_pd_accessor.py` & `msticpy-2.6.0/msticpy/init/pivot_core/pivot_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/pivot_core/pivot_pipeline.py` & `msticpy-2.6.0/msticpy/init/pivot_core/pivot_pipeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/pivot_core/pivot_register.py` & `msticpy-2.6.0/msticpy/init/pivot_core/pivot_register.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/pivot_core/pivot_register_reader.py` & `msticpy-2.6.0/msticpy/init/pivot_core/pivot_register_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/pivot_init/pivot_data_queries.py` & `msticpy-2.6.0/msticpy/init/pivot_init/pivot_data_queries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/pivot_init/pivot_ti_provider.py` & `msticpy-2.6.0/msticpy/init/pivot_init/pivot_ti_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/init/pivot_init/vt_pivot.py` & `msticpy-2.6.0/msticpy/init/pivot_init/vt_pivot.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,14 +94,34 @@
 _ENTITY_PROPS = {
     "File": "Sha256",
     "IpAddress": "Address",
     "Dns": "DomainName",
     "Url": "Url",
 }
 
+_FUNC_DOC = """
+{description}
+
+Parameters
+----------
+observable: str
+    The observable value
+limit: int
+    Relations limit
+all_props : bool, optional
+    If True, return all properties, by default False
+full_objects : bool, optional
+    If True, return the full object rather than just ID links.
+
+Returns
+-------
+    Relationship Pandas DataFrame with the relationships of the entity
+
+"""
+
 
 def init():
     """Load VT3 Pivots if vt library is available."""
     if VT3_AVAILABLE:
         add_pivot_functions()
 
 
@@ -162,24 +182,28 @@
         for relationship in ent_relations:
             f_part = partial(
                 _get_relationships,
                 vt_client=vt_client,
                 vt_type=vt_type,
                 relationship=relationship,
             )
-            func_dict[_create_func_name(relationship)] = f_part
+            f_part.__doc__ = _create_func_doc(entity, relationship)
+            func_dict[relationship] = f_part
         ent_funcs[entity] = func_dict
     return ent_funcs
 
 
 # pylint: enable=no-member
 
 
-def _create_func_name(relationship):
-    return f"vt_{relationship}"
+def _create_func_doc(entity, relationship):
+    """Create the relationship docstring."""
+    fmt_name = " ".join(rel.capitalize() for rel in relationship.split("_"))
+    description = f"Lookup VirusTotal {fmt_name} for {entity}."
+    return _FUNC_DOC.format(description=description)
 
 
 def _get_relationships(vt_client, entity_id, vt_type, relationship):
     result_df = vt_client.lookup_ioc_relationships(
         observable=entity_id, vt_type=vt_type, relationship=relationship
     )
     return result_df.reset_index()
```

### Comparing `msticpy-2.5.3/msticpy/init/user_config.py` & `msticpy-2.6.0/msticpy/init/user_config.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/__init__.py` & `msticpy-2.6.0/msticpy/nbtools/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/data_viewer.py` & `msticpy-2.6.0/msticpy/nbtools/data_viewer.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/entityschema.py` & `msticpy-2.6.0/msticpy/nbtools/entityschema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/foliummap.py` & `msticpy-2.6.0/msticpy/nbtools/foliummap.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/morph_charts.py` & `msticpy-2.6.0/msticpy/nbtools/morph_charts.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/nbdisplay.py` & `msticpy-2.6.0/msticpy/nbtools/nbdisplay.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/nbwidgets.py` & `msticpy-2.6.0/msticpy/nbtools/nbwidgets.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/observationlist.py` & `msticpy-2.6.0/msticpy/nbtools/observationlist.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/process_tree.py` & `msticpy-2.6.0/msticpy/nbtools/process_tree.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/security_alert.py` & `msticpy-2.6.0/msticpy/nbtools/security_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/security_alert_graph.py` & `msticpy-2.6.0/msticpy/nbtools/security_alert_graph.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/security_base.py` & `msticpy-2.6.0/msticpy/nbtools/security_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/security_event.py` & `msticpy-2.6.0/msticpy/nbtools/security_event.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/ti_browser.py` & `msticpy-2.6.0/msticpy/nbtools/ti_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/timeline.py` & `msticpy-2.6.0/msticpy/nbtools/timeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/timeline_duration.py` & `msticpy-2.6.0/msticpy/nbtools/timeline_duration.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/timeline_pd_accessor.py` & `msticpy-2.6.0/msticpy/nbtools/timeline_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/timeseries.py` & `msticpy-2.6.0/msticpy/nbtools/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/utility.py` & `msticpy-2.6.0/msticpy/nbtools/utility.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbtools/wsconfig.py` & `msticpy-2.6.0/msticpy/nbtools/wsconfig.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbwidgets/__init__.py` & `msticpy-2.6.0/msticpy/nbwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbwidgets/core.py` & `msticpy-2.6.0/msticpy/nbwidgets/core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbwidgets/get_environment_key.py` & `msticpy-2.6.0/msticpy/nbwidgets/get_environment_key.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbwidgets/get_text.py` & `msticpy-2.6.0/msticpy/nbwidgets/get_text.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbwidgets/lookback.py` & `msticpy-2.6.0/msticpy/nbwidgets/lookback.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbwidgets/option_buttons.py` & `msticpy-2.6.0/msticpy/nbwidgets/option_buttons.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbwidgets/progress.py` & `msticpy-2.6.0/msticpy/nbwidgets/progress.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbwidgets/query_time.py` & `msticpy-2.6.0/msticpy/nbwidgets/query_time.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbwidgets/select_alert.py` & `msticpy-2.6.0/msticpy/nbwidgets/select_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbwidgets/select_item.py` & `msticpy-2.6.0/msticpy/nbwidgets/select_item.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/nbwidgets/select_subset.py` & `msticpy-2.6.0/msticpy/nbwidgets/select_subset.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/resources/WinSecurityEvent.json` & `msticpy-2.6.0/msticpy/resources/WinSecurityEvent.json`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/resources/mp_pivot_reg.yaml` & `msticpy-2.6.0/msticpy/resources/mp_pivot_reg.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/resources/mpconfig_defaults.yaml` & `msticpy-2.6.0/msticpy/resources/mpconfig_defaults.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/resources/obfuscation_cols.yaml` & `msticpy-2.6.0/msticpy/resources/obfuscation_cols.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/__init__.py` & `msticpy-2.6.0/msticpy/sectools/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/auditdextract.py` & `msticpy-2.6.0/msticpy/sectools/auditdextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/base64unpack.py` & `msticpy-2.6.0/msticpy/sectools/base64unpack.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/cmd_line.py` & `msticpy-2.6.0/msticpy/sectools/cmd_line.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/domain_utils.py` & `msticpy-2.6.0/msticpy/sectools/domain_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/eventcluster.py` & `msticpy-2.6.0/msticpy/sectools/eventcluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/geoip.py` & `msticpy-2.6.0/msticpy/sectools/geoip.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/iocextract.py` & `msticpy-2.6.0/msticpy/sectools/iocextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/ip_utils.py` & `msticpy-2.6.0/msticpy/sectools/ip_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/proc_tree_build_mde.py` & `msticpy-2.6.0/msticpy/sectools/proc_tree_build_mde.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/proc_tree_build_winlx.py` & `msticpy-2.6.0/msticpy/sectools/proc_tree_build_winlx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/proc_tree_builder.py` & `msticpy-2.6.0/msticpy/sectools/proc_tree_builder.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/proc_tree_schema.py` & `msticpy-2.6.0/msticpy/sectools/proc_tree_schema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/proc_tree_utils.py` & `msticpy-2.6.0/msticpy/sectools/proc_tree_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/sectools_magics.py` & `msticpy-2.6.0/msticpy/sectools/sectools_magics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/syslog_utils.py` & `msticpy-2.6.0/msticpy/sectools/syslog_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/tilookup.py` & `msticpy-2.6.0/msticpy/sectools/tilookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/tiproviders/ti_provider_base.py` & `msticpy-2.6.0/msticpy/sectools/tiproviders/ti_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/vtlookup.py` & `msticpy-2.6.0/msticpy/sectools/vtlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/vtlookupv3/__init__.py` & `msticpy-2.6.0/msticpy/sectools/vtlookupv3/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/vtlookupv3/vtfile_behavior.py` & `msticpy-2.6.0/msticpy/sectools/vtlookupv3/vtfile_behavior.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/vtlookupv3/vtlookupv3.py` & `msticpy-2.6.0/msticpy/sectools/vtlookupv3/vtlookupv3.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/sectools/vtlookupv3/vtobject_browser.py` & `msticpy-2.6.0/msticpy/sectools/vtlookupv3/vtobject_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/transform/auditdextract.py` & `msticpy-2.6.0/msticpy/transform/auditdextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/transform/base64unpack.py` & `msticpy-2.6.0/msticpy/transform/base64unpack.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/transform/cmd_line.py` & `msticpy-2.6.0/msticpy/transform/cmd_line.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/transform/iocextract.py` & `msticpy-2.6.0/msticpy/transform/iocextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/transform/network.py` & `msticpy-2.6.0/msticpy/transform/network.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/transform/proc_tree_build_mde.py` & `msticpy-2.6.0/msticpy/transform/proc_tree_build_mde.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/transform/proc_tree_build_winlx.py` & `msticpy-2.6.0/msticpy/transform/proc_tree_build_winlx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/transform/proc_tree_builder.py` & `msticpy-2.6.0/msticpy/transform/proc_tree_builder.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/transform/proc_tree_schema.py` & `msticpy-2.6.0/msticpy/transform/proc_tree_schema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/transform/process_tree_utils.py` & `msticpy-2.6.0/msticpy/transform/process_tree_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/__init__.py` & `msticpy-2.6.0/msticpy/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/code_view.py` & `msticpy-2.6.0/msticpy/vis/code_view.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/data_viewer.py` & `msticpy-2.6.0/msticpy/vis/data_viewer.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/data_viewer_panel.py` & `msticpy-2.6.0/msticpy/vis/data_viewer_panel.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/entity_graph_tools.py` & `msticpy-2.6.0/msticpy/vis/entity_graph_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/figure_dimension.py` & `msticpy-2.6.0/msticpy/vis/figure_dimension.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/foliummap.py` & `msticpy-2.6.0/msticpy/vis/foliummap.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/matrix_plot.py` & `msticpy-2.6.0/msticpy/vis/matrix_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/mordor_browser.py` & `msticpy-2.6.0/msticpy/vis/mordor_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/morph_charts.py` & `msticpy-2.6.0/msticpy/vis/morph_charts.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/mp_pandas_plot.py` & `msticpy-2.6.0/msticpy/vis/mp_pandas_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/nbdisplay.py` & `msticpy-2.6.0/msticpy/vis/nbdisplay.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/network_plot.py` & `msticpy-2.6.0/msticpy/vis/network_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/process_tree.py` & `msticpy-2.6.0/msticpy/vis/process_tree.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/query_browser.py` & `msticpy-2.6.0/msticpy/vis/query_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/ti_browser.py` & `msticpy-2.6.0/msticpy/vis/ti_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/timeline.py` & `msticpy-2.6.0/msticpy/vis/timeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/timeline_common.py` & `msticpy-2.6.0/msticpy/vis/timeline_common.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/timeline_duration.py` & `msticpy-2.6.0/msticpy/vis/timeline_duration.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/timeline_pd_accessor.py` & `msticpy-2.6.0/msticpy/vis/timeline_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/timeline_values.py` & `msticpy-2.6.0/msticpy/vis/timeline_values.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/timeseries.py` & `msticpy-2.6.0/msticpy/vis/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy/vis/vtobject_browser.py` & `msticpy-2.6.0/msticpy/vis/vtobject_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/msticpy.egg-info/PKG-INFO` & `msticpy-2.6.0/msticpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msticpy
-Version: 2.5.3
+Version: 2.6.0
 Summary: MSTIC Security Tools
 Home-page: https://github.com/microsoft/msticpy
 Author: Ian Hellen
 Author-email: ianhelle@microsoft.com
 Maintainer: Pete Bryan
 Maintainer-email: peter.bryan@microsoft.com
 License: MIT License
```

### Comparing `msticpy-2.5.3/msticpy.egg-info/SOURCES.txt` & `msticpy-2.6.0/msticpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -159,32 +159,33 @@
 msticpy/data/drivers/cybereason_driver.py
 msticpy/data/drivers/driver_base.py
 msticpy/data/drivers/elastic_driver.py
 msticpy/data/drivers/kql_driver.py
 msticpy/data/drivers/kusto_driver.py
 msticpy/data/drivers/local_data_driver.py
 msticpy/data/drivers/local_osquery_driver.py
+msticpy/data/drivers/local_velociraptor_driver.py
 msticpy/data/drivers/mdatp_driver.py
 msticpy/data/drivers/mordor_driver.py
 msticpy/data/drivers/odata_driver.py
 msticpy/data/drivers/resource_graph_driver.py
 msticpy/data/drivers/security_graph_driver.py
 msticpy/data/drivers/sentinel_query_reader.py
 msticpy/data/drivers/splunk_driver.py
 msticpy/data/drivers/sumologic_driver.py
 msticpy/data/queries/cybereason/cybereason_connections.yaml
 msticpy/data/queries/cybereason/cybereason_hosts.yaml
 msticpy/data/queries/cybereason/cybereason_processes.yaml
 msticpy/data/queries/localdata/local_data.yaml
-msticpy/data/queries/m365d/kql_mdatp_alerts.yaml
-msticpy/data/queries/m365d/kql_mdatp_file.yaml
-msticpy/data/queries/m365d/kql_mdatp_hunting.yaml
-msticpy/data/queries/m365d/kql_mdatp_network.yaml
-msticpy/data/queries/m365d/kql_mdatp_process.yaml
-msticpy/data/queries/m365d/kql_mdatp_user.yaml
+msticpy/data/queries/m365d/kql_m365_alerts.yaml
+msticpy/data/queries/m365d/kql_m365_file.yaml
+msticpy/data/queries/m365d/kql_m365_hunting.yaml
+msticpy/data/queries/m365d/kql_m365_network.yaml
+msticpy/data/queries/m365d/kql_m365_process.yaml
+msticpy/data/queries/m365d/kql_m365_user.yaml
 msticpy/data/queries/mde/kql_mdatp_alerts.yaml
 msticpy/data/queries/mde/kql_mdatp_file.yaml
 msticpy/data/queries/mde/kql_mdatp_hunting.yaml
 msticpy/data/queries/mde/kql_mdatp_network.yaml
 msticpy/data/queries/mde/kql_mdatp_process.yaml
 msticpy/data/queries/mde/kql_mdatp_user.yaml
 msticpy/data/queries/msgraph/graph_alerts.yaml
```

### Comparing `msticpy-2.5.3/msticpy.egg-info/requires.txt` & `msticpy-2.6.0/msticpy.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 beautifulsoup4>=4.0.0
 bokeh<4.0.0,>=1.4.0
 cryptography>=3.1
 deprecated>=1.2.4
 dnspython<3.0.0,>=2.0.0
 folium>=0.9.0
 geoip2>=2.9.0
-httpx==0.24.0
+httpx==0.24.1
 html5lib
 ipywidgets<9.0.0,>=7.4.2
 KqlmagicCustom[auth_code_clipboard,jupyter-basic]>=0.1.114.post22
 lxml>=4.6.5
 msal>=1.12.0
 msal_extensions>=0.3.0
 msrest>=0.6.0
@@ -152,15 +152,15 @@
 pygeohash>=1.2.0
 pylint>=2.5.3
 pyroma>=3.1
 pytest-check>=1.0.1
 pytest-cov>=2.11.1
 pytest-xdist>=2.5.0
 pytest>=5.0.1
-readthedocs-sphinx-ext==2.2.0
+readthedocs-sphinx-ext==2.2.2
 responses>=0.13.2
 respx>=0.20.1
 sphinx-rtd-theme>=1.0.0
 sphinx>=5.0.1
 types-attrs>=19.0.0
 
 [keyvault]
@@ -254,15 +254,15 @@
 pygeohash>=1.2.0
 pylint>=2.5.3
 pyroma>=3.1
 pytest-check>=1.0.1
 pytest-cov>=2.11.1
 pytest-xdist>=2.5.0
 pytest>=5.0.1
-readthedocs-sphinx-ext==2.2.0
+readthedocs-sphinx-ext==2.2.2
 responses>=0.13.2
 respx>=0.20.1
 scikit-learn>=1.0.0
 scipy>=1.1.0
 sphinx-rtd-theme>=1.0.0
 sphinx>=5.0.1
 splunk-sdk>=1.6.0
```

### Comparing `msticpy-2.5.3/requirements-all.txt` & `msticpy-2.6.0/requirements-all.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 beautifulsoup4>=4.0.0
 bokeh>=1.4.0, <4.0.0
 cryptography>=3.1
 deprecated>=1.2.4
 dnspython>=2.0.0, <3.0.0
 folium>=0.9.0
 geoip2>=2.9.0
-httpx==0.24.0
+httpx==0.24.1
 html5lib
 ipython >= 7.1.1; python_version < "3.8"
 ipython >= 7.23.1; python_version >= "3.8"
 ipywidgets>=7.4.2, <9.0.0
 keyring>=13.2.1
 KqlmagicCustom[jupyter-basic,auth_code_clipboard]>=0.1.114.post22
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
```

### Comparing `msticpy-2.5.3/requirements-dev.txt` & `msticpy-2.6.0/requirements-dev.txt`

 * *Files 14% similar despite different names*

```diff
@@ -24,13 +24,13 @@
 pygeohash>=1.2.0
 pylint>=2.5.3
 pyroma>=3.1
 pytest-check>=1.0.1
 pytest-cov>=2.11.1
 pytest-xdist>=2.5.0
 pytest>=5.0.1
-readthedocs-sphinx-ext==2.2.0
+readthedocs-sphinx-ext==2.2.2
 responses>=0.13.2
 respx>=0.20.1
 sphinx-rtd-theme>=1.0.0
 sphinx>=5.0.1
 types-attrs>=19.0.0
```

### Comparing `msticpy-2.5.3/requirements.txt` & `msticpy-2.6.0/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 beautifulsoup4>=4.0.0
 bokeh>=1.4.0, <4.0.0
 cryptography>=3.1
 deprecated>=1.2.4
 dnspython>=2.0.0, <3.0.0
 folium>=0.9.0
 geoip2>=2.9.0
-httpx==0.24.0
+httpx==0.24.1
 html5lib
 ipython >= 7.1.1; python_version < "3.8"
 ipython >= 7.23.1; python_version >= "3.8"
 ipywidgets>=7.4.2, <9.0.0
 KqlmagicCustom[jupyter-basic,auth_code_clipboard]>=0.1.114.post22
 lxml>=4.6.5
 msal>=1.12.0
```

### Comparing `msticpy-2.5.3/setup.cfg` & `msticpy-2.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `msticpy-2.5.3/setup.py` & `msticpy-2.6.0/setup.py`

 * *Files identical despite different names*

