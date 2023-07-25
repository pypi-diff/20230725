# Comparing `tmp/taegis-sdk-python-1.0.1.tar.gz` & `tmp/taegis-sdk-python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taegis-sdk-python-1.0.1.tar", last modified: Tue Jul 18 14:15:37 2023, max compression
+gzip compressed data, was "taegis-sdk-python-1.0.2.tar", last modified: Tue Jul 25 14:51:19 2023, max compression
```

## Comparing `taegis-sdk-python-1.0.1.tar` & `taegis-sdk-python-1.0.2.tar`

### file list

```diff
@@ -1,208 +1,214 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.667305 taegis-sdk-python-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    10173 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6228 2023-07-18 14:15:37.666305 taegis-sdk-python-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5793 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 14:15:37.667305 taegis-sdk-python-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1571 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.637305 taegis-sdk-python-1.0.1/taegis_sdk_python/
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/_consts.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-18 14:15:37.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8618 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    10895 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/service_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.638305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/
--rw-rw-rw-   0 root         (0) root         (0)    13731 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.639305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2419 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.640305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4740 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.641305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3900 2023-07-18 14:14:36.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6693 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    78106 2023-07-18 14:14:36.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.642305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6375 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    14954 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23548 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.643305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    12807 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25755 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.644305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1361 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3089 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10314 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.645305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3135 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.646305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15823 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    24262 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    31817 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.647305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4946 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7300 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5118 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.648305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2932 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.649305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7325 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3523 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8546 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.650305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3998 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7782 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.651305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1818 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.651305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1619 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4437 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.652305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1346 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2775 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10577 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.653305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12999 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    10457 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    24248 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.654305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22228 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    28008 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    37546 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.655305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12204 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7214 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    41182 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.656305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9291 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.657305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.658305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6858 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8811 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.659305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5923 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5961 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    12949 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.660305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6660 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    13046 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.661305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14207 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16097 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    22172 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.662305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.662305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17210 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9170 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    19048 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.663305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12362 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5913 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    34203 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.664305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3443 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    13781 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    53278 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.665305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3905 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7993 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.666305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11558 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7075 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25732 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/types.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     6493 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.638305 taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6228 2023-07-18 14:15:37.000000 taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8246 2023-07-18 14:15:37.000000 taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 14:15:37.000000 taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-18 14:15:37.000000 taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-18 14:15:37.000000 taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.897381 taegis-sdk-python-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)    10173 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6228 2023-07-25 14:51:19.896381 taegis-sdk-python-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5793 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 14:51:19.897381 taegis-sdk-python-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.870383 taegis-sdk-python-1.0.2/taegis_sdk_python/
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-25 14:51:19.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8618 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    10654 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/service_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.871383 taegis-sdk-python-1.0.2/taegis_sdk_python/services/
+-rw-rw-rw-   0 root         (0) root         (0)    14015 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.872383 taegis-sdk-python-1.0.2/taegis_sdk_python/services/access_points/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/access_points/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/access_points/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/access_points/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/access_points/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/access_points/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.873383 taegis-sdk-python-1.0.2/taegis_sdk_python/services/agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/agent/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/agent/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/agent/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4740 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/agent/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.874383 taegis-sdk-python-1.0.2/taegis_sdk_python/services/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3900 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/alerts/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/alerts/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/alerts/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    78106 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/alerts/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.875383 taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6375 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14954 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23548 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.876383 taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets2/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    12807 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    26822 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.876383 taegis-sdk-python-1.0.2/taegis_sdk_python/services/audits/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/audits/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/audits/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/audits/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/audits/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10314 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/audits/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.877383 taegis-sdk-python-1.0.2/taegis_sdk_python/services/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/clients/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/clients/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/clients/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/clients/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.878383 taegis-sdk-python-1.0.2/taegis_sdk_python/services/collector/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/collector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15823 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/collector/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    24262 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/collector/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/collector/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    31817 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/collector/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.879382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/comments/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/comments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4946 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/comments/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7300 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/comments/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/comments/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/comments/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.879382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/detector_registry/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/detector_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/detector_registry/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/detector_registry/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/detector_registry/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/detector_registry/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.880382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_command_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_command_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7325 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_command_manager/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_command_manager/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8546 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_command_manager/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.881382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_management_service/
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_management_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_management_service/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_management_service/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7782 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_management_service/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.882382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/entity_profile/
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/entity_profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/entity_profile/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/entity_profile/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/entity_profile/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/entity_profile/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.882382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/event_search/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/event_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/event_search/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/event_search/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/event_search/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4437 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/event_search/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.883382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/events/
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/events/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/events/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/events/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10577 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.884382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/exports/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/exports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12999 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/exports/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10457 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/exports/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/exports/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24620 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/exports/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.885382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/fast_ioc/
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/fast_ioc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/fast_ioc/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/fast_ioc/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/fast_ioc/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/fast_ioc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.886382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations/
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22228 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    28008 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    37546 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.886382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations2/
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12204 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7214 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    42368 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.887382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/mitre_attack_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/mitre_attack_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/mitre_attack_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9291 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/mitre_attack_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/mitre_attack_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.888382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/notebooks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/notebooks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/notebooks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/notebooks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.889382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6858 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/notifications/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/notifications/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/notifications/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/notifications/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.889382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/preferences/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/preferences/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5923 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/preferences/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5961 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/preferences/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/preferences/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12949 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/preferences/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.890382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/roadrunner/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/roadrunner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/roadrunner/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6660 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/roadrunner/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/roadrunner/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13046 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/roadrunner/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.891382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/rules/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/rules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14207 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/rules/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16097 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/rules/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/rules/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    22172 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/rules/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.892382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/sharelinks/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/sharelinks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/sharelinks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/sharelinks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/sharelinks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/sharelinks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.892382 taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenant_profiles/
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenant_profiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17210 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenant_profiles/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9170 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenant_profiles/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenant_profiles/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    19048 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenant_profiles/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.893381 taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenants/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12362 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenants/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5913 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenants/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenants/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    34203 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenants/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.894381 taegis-sdk-python-1.0.2/taegis_sdk_python/services/threat/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/threat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3443 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/threat/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    13781 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/threat/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/threat/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    53278 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/threat/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.895381 taegis-sdk-python-1.0.2/taegis_sdk_python/services/trip/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/trip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/trip/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/trip/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/trip/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7993 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/trip/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.896381 taegis-sdk-python-1.0.2/taegis_sdk_python/services/users/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11558 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/users/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7075 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/users/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/users/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25732 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/services/users/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2023-07-25 14:50:59.000000 taegis-sdk-python-1.0.2/taegis_sdk_python/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:51:19.871383 taegis-sdk-python-1.0.2/taegis_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6228 2023-07-25 14:51:19.000000 taegis-sdk-python-1.0.2/taegis_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8488 2023-07-25 14:51:19.000000 taegis-sdk-python-1.0.2/taegis_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 14:51:19.000000 taegis-sdk-python-1.0.2/taegis_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-25 14:51:19.000000 taegis-sdk-python-1.0.2/taegis_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 14:51:19.000000 taegis-sdk-python-1.0.2/taegis_sdk_python.egg-info/top_level.txt
```

### Comparing `taegis-sdk-python-1.0.1/LICENSE` & `taegis-sdk-python-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/PKG-INFO` & `taegis-sdk-python-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.1/README.md` & `taegis-sdk-python-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/setup.py` & `taegis-sdk-python-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/_consts.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/_consts.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/authentication.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/authentication.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/config.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/config.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/errors.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/errors.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/service_core.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/service_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from gql import Client, gql
 from gql.transport.requests import RequestsHTTPTransport
 from gql.transport.websockets import WebsocketsTransport
 from graphql import GraphQLField, GraphQLSchema, GraphQLError
 from taegis_sdk_python._version import __version__
 from taegis_sdk_python.errors import InvalidGraphQLEndpoint
-from taegis_sdk_python.utils import async_block, prepare_variables
+from taegis_sdk_python.utils import async_block, prepare_variables, remove_node
 
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services import GraphQLService
 
 
 log = logging.getLogger(__name__)
 
@@ -248,43 +248,39 @@
             Output string
 
         Returns
         -------
         str
             GraphQL string
         """
+        query_string = self._build_output_query(
+            operation_type=operation_type,
+            endpoint=endpoint,
+            graphql_field=graphql_field,
+            output=output,
+        )
+        query_string = " ".join(query_string.split())
+
         # open a connection for introspection and download schema
         with self.sync_client as session:
             # if multiple fields are invalid, we want to iterate until the
             # output string is valid
-            while True:
-                query_string = self._build_output_query(
-                    operation_type=operation_type,
-                    endpoint=endpoint,
-                    graphql_field=graphql_field,
-                    output=output,
-                )
-
-                # we don't want to infinitely process this, so if we break
-                # if the output string doesn't exist, or all the fields have been
-                # removed
-                if not (output or any(char not in {" ", "{", "}"} for char in output)):
-                    break
-
+            for _ in range(10000):
                 try:
                     session.client.validate(gql(query_string))
                     break
 
                 except GraphQLError as exc:
                     if "Cannot query field" in exc.message:
-                        for node in exc.nodes:
-                            log.warning(
-                                f"{self.service.environment} - field {node.name.value} not found.  Removing from query string..."
-                            )
-                            output = output.replace(node.name.value, "")
+                        log.warning(
+                            f"{self.service.environment} - field {exc.nodes[0].name.value} not found.  Removing from query string..."
+                        )
+                        query_string = remove_node(
+                            query_string, exc.nodes[0], exc.locations[0]
+                        )
                     else:
                         raise exc
 
         return query_string
 
     @staticmethod
     def _build_output_query(
```

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from taegis_sdk_python.services.endpoint_management_service import (
     EndpointManagementServiceService,
 )
 from taegis_sdk_python.services.entity_profile import EntityProfileService
 from taegis_sdk_python.services.event_search import EventSearchService
 from taegis_sdk_python.services.events import EventsService
 from taegis_sdk_python.services.exports import ExportsService
+from taegis_sdk_python.services.fast_ioc import FastIocService
 from taegis_sdk_python.services.investigations import InvestigationsService
 from taegis_sdk_python.services.investigations2 import Investigations2Service
 from taegis_sdk_python.services.mitre_attack_info import MitreAttackInfoService
 from taegis_sdk_python.services.notebooks import NotebooksService
 from taegis_sdk_python.services.notifications import NotificationsService
 from taegis_sdk_python.services.preferences import PreferencesService
 from taegis_sdk_python.services.roadrunner import RoadrunnerService
@@ -105,14 +106,15 @@
         self._detector_registry = None
         self._endpoint_command_manager = None
         self._endpoint_management_service = None
         self._entity_profile = None
         self._event_search = None
         self._events = None
         self._exports = None
+        self._fast_ioc = None
         self._investigations = None
         self._investigations2 = None
         self._mitre_attack_info = None
         self._notebooks = None
         self._notifications = None
         self._preferences = None
         self._roadrunner = None
@@ -312,14 +314,21 @@
     def exports(self):
         """Exports Service Endpoint."""
         if not self._exports:
             self._exports = ExportsService(self)
         return self._exports
 
     @property
+    def fast_ioc(self):
+        """Fast IOC Service Endpoint."""
+        if not self._fast_ioc:
+            self._fast_ioc = FastIocService(self)
+        return self._fast_ioc
+
+    @property
     def investigations(self):
         """Investigations Service Endpoint."""
         if not self._investigations:
             self._investigations = InvestigationsService(self)
         return self._investigations
 
     @property
```

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/access_points/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/access_points/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/access_points/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/access_points/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/access_points/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/agent/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/agent/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/agent/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/agent/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/alerts/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/alerts/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/alerts/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/alerts/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/assets2/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -421,36 +421,51 @@
     )
     group_name: Optional[str] = field(
         default=None, metadata=config(field_name="groupName")
     )
     group_name_contains: Optional[str] = field(
         default=None, metadata=config(field_name="groupName_contains")
     )
+    group_name_autocomplete: Optional[str] = field(
+        default=None, metadata=config(field_name="groupName_autocomplete")
+    )
     host_id: Optional[str] = field(default=None, metadata=config(field_name="hostId"))
     host_id_contains: Optional[str] = field(
         default=None, metadata=config(field_name="hostId_contains")
     )
+    host_id_autocomplete: Optional[str] = field(
+        default=None, metadata=config(field_name="hostId_autocomplete")
+    )
     hostname: Optional[str] = field(
         default=None, metadata=config(field_name="hostname")
     )
     hostname_contains: Optional[str] = field(
         default=None, metadata=config(field_name="hostname_contains")
     )
+    hostname_autocomplete: Optional[str] = field(
+        default=None, metadata=config(field_name="hostname_autocomplete")
+    )
     investigation_id: Optional[str] = field(
         default=None, metadata=config(field_name="investigationId")
     )
     investigation_id_contains: Optional[str] = field(
         default=None, metadata=config(field_name="investigationId_contains")
     )
+    investigation_id_autocomplete: Optional[str] = field(
+        default=None, metadata=config(field_name="investigationId_autocomplete")
+    )
     ip_address: Optional[str] = field(
         default=None, metadata=config(field_name="ipAddress")
     )
     ip_address_contains: Optional[str] = field(
         default=None, metadata=config(field_name="ipAddress_contains")
     )
+    ip_address_autocomplete: Optional[str] = field(
+        default=None, metadata=config(field_name="ipAddress_autocomplete")
+    )
     isolation_status: Optional[str] = field(
         default=None, metadata=config(field_name="isolationStatus")
     )
     last_seen_at: Optional[str] = field(
         default=None, metadata=config(field_name="lastSeenAt")
     )
     last_seen_at_lt: Optional[str] = field(
@@ -467,14 +482,17 @@
     )
     mac_address: Optional[str] = field(
         default=None, metadata=config(field_name="macAddress")
     )
     mac_address_contains: Optional[str] = field(
         default=None, metadata=config(field_name="macAddress_contains")
     )
+    mac_address_autocomplete: Optional[str] = field(
+        default=None, metadata=config(field_name="macAddress_autocomplete")
+    )
     os_distributor: Optional[str] = field(
         default=None, metadata=config(field_name="osDistributor")
     )
     os_family: Optional[str] = field(
         default=None, metadata=config(field_name="osFamily")
     )
     os_version: Optional[str] = field(
@@ -503,14 +521,17 @@
     )
     username: Optional[str] = field(
         default=None, metadata=config(field_name="username")
     )
     username_contains: Optional[str] = field(
         default=None, metadata=config(field_name="username_contains")
     )
+    username_autocomplete: Optional[str] = field(
+        default=None, metadata=config(field_name="username_autocomplete")
+    )
     and_: Optional[List["AssetWhereInputV2"]] = field(
         default=None, metadata=config(field_name="and")
     )
     or_: Optional[List["AssetWhereInputV2"]] = field(
         default=None, metadata=config(field_name="or")
     )
     not_: Optional["AssetWhereInputV2"] = field(
@@ -518,14 +539,17 @@
     )
     tags: Optional[TagWhereInputV2] = field(
         default=None, metadata=config(field_name="tags")
     )
     tags_contains: Optional[TagWhereInputV2] = field(
         default=None, metadata=config(field_name="tags_contains")
     )
+    tags_autocomplete: Optional[TagWhereInputV2] = field(
+        default=None, metadata=config(field_name="tags_autocomplete")
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AssetV2:
     """AssetV2."""
```

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/audits/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/audits/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/audits/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/audits/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/audits/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/clients/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/clients/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/clients/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/collector/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/collector/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/collector/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/collector/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/comments/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/comments/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/comments/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/comments/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/comments/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/detector_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/detector_registry/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/detector_registry/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/detector_registry/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/detector_registry/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_command_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_command_manager/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_command_manager/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_command_manager/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_management_service/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_management_service/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_management_service/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_management_service/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/endpoint_management_service/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/entity_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/entity_profile/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/entity_profile/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/entity_profile/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/entity_profile/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/event_search/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/event_search/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/event_search/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/event_search/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/event_search/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/events/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/events/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/events/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/events/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/events/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/exports/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/exports/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/exports/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/exports/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,53 +308,14 @@
     sort_order: Optional[SortOrder] = field(
         default=None, metadata=config(field_name="sortOrder")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class ScheduleEditInput:
-    """ScheduleEditInput."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
-    description: Optional[str] = field(
-        default=None, metadata=config(field_name="description")
-    )
-    filters: Optional[dict] = field(default=None, metadata=config(field_name="filters"))
-    interval: Optional[int] = field(
-        default=None, metadata=config(field_name="interval")
-    )
-    day_of_month: Optional[int] = field(
-        default=None, metadata=config(field_name="dayOfMonth")
-    )
-    recipients: Optional[List[str]] = field(
-        default=None, metadata=config(field_name="recipients")
-    )
-    red_ql_query: Optional[str] = field(
-        default=None, metadata=config(field_name="redQLQuery")
-    )
-    generate_csv_export: Optional[bool] = field(
-        default=None, metadata=config(field_name="generateCSVExport")
-    )
-    run_at: Optional[str] = field(default=None, metadata=config(field_name="runAt"))
-    share_with_admin_group: Optional[bool] = field(
-        default=None, metadata=config(field_name="shareWithAdminGroup")
-    )
-    locale: Optional[str] = field(default=None, metadata=config(field_name="locale"))
-    chart_type: Optional[ReportChartType] = field(
-        default=None, metadata=config(field_name="chartType")
-    )
-    cadence: Optional[Cadence] = field(
-        default=None, metadata=config(field_name="cadence")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
 class ReportsFilters:
     """ReportsFilters."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
     created_before: Optional[str] = field(
         default=None, metadata=config(field_name="createdBefore")
     )
@@ -511,14 +472,56 @@
     filters: Optional[SchedulesFilters] = field(
         default=None, metadata=config(field_name="filters")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class ScheduleEditInput:
+    """ScheduleEditInput."""
+
+    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
+    description: Optional[str] = field(
+        default=None, metadata=config(field_name="description")
+    )
+    filters: Optional[dict] = field(default=None, metadata=config(field_name="filters"))
+    interval: Optional[int] = field(
+        default=None, metadata=config(field_name="interval")
+    )
+    day_of_month: Optional[int] = field(
+        default=None, metadata=config(field_name="dayOfMonth")
+    )
+    recipients: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="recipients")
+    )
+    red_ql_query: Optional[str] = field(
+        default=None, metadata=config(field_name="redQLQuery")
+    )
+    generate_csv_export: Optional[bool] = field(
+        default=None, metadata=config(field_name="generateCSVExport")
+    )
+    run_at: Optional[str] = field(default=None, metadata=config(field_name="runAt"))
+    share_with_admin_group: Optional[bool] = field(
+        default=None, metadata=config(field_name="shareWithAdminGroup")
+    )
+    locale: Optional[str] = field(default=None, metadata=config(field_name="locale"))
+    chart_type: Optional[ReportChartType] = field(
+        default=None, metadata=config(field_name="chartType")
+    )
+    cadence: Optional[Cadence] = field(
+        default=None, metadata=config(field_name="cadence")
+    )
+    export_types: Optional[List[ExportType]] = field(
+        default=None, metadata=config(field_name="exportTypes")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class NewScheduleInput:
     """NewScheduleInput."""
 
     name: Optional[str] = field(default=None, metadata=config(field_name="name"))
     filters: Optional[dict] = field(default=None, metadata=config(field_name="filters"))
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
@@ -554,14 +557,17 @@
     )
     report_type: Optional[ReportType] = field(
         default=None, metadata=config(field_name="reportType")
     )
     cadence: Optional[Cadence] = field(
         default=None, metadata=config(field_name="cadence")
     )
+    export_types: Optional[List[ExportType]] = field(
+        default=None, metadata=config(field_name="exportTypes")
+    )
     visualizations: Optional[List[VisualizationInput]] = field(
         default=None, metadata=config(field_name="visualizations")
     )
     report_timeframe: Optional[ReportTimeframeInput] = field(
         default=None, metadata=config(field_name="reportTimeframe")
     )
 
@@ -616,14 +622,17 @@
     )
     recipients: Optional[List[TDRUser]] = field(
         default=None, metadata=config(field_name="recipients")
     )
     creator: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="creator")
     )
+    export_types: Optional[List[ExportType]] = field(
+        default=None, metadata=config(field_name="exportTypes")
+    )
     visualizations: Optional[List[Visualization]] = field(
         default=None, metadata=config(field_name="visualizations")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
```

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/investigations2/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,16 +299,31 @@
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationTemplatesArguments:
     """InvestigationTemplatesArguments."""
 
-    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
-    tags: Optional[List[str]] = field(default=None, metadata=config(field_name="tags"))
+    page: Optional[int] = field(default=None, metadata=config(field_name="page"))
+    per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
+    cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
+    name: Optional[str] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "no-op; use cql"},
+            field_name="name",
+        ),
+    )
+    tags: Optional[List[str]] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "no-op; use cql"},
+            field_name="tags",
+        ),
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationRuleArguments:
     """InvestigationRuleArguments."""
 
@@ -317,16 +332,31 @@
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationRulesArguments:
     """InvestigationRulesArguments."""
 
-    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
-    tags: Optional[List[str]] = field(default=None, metadata=config(field_name="tags"))
+    page: Optional[int] = field(default=None, metadata=config(field_name="page"))
+    per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
+    cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
+    name: Optional[str] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "no-op; use cql"},
+            field_name="name",
+        ),
+    )
+    tags: Optional[List[str]] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "no-op; use cql"},
+            field_name="tags",
+        ),
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class ExportInvestigationResourceInput:
     """ExportInvestigationResourceInput."""
 
@@ -468,22 +498,14 @@
     """TDRUser."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class Client:
-    """Client."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
 class CreateInvestigationRuleInput:
     """CreateInvestigationRuleInput."""
 
     name: Optional[str] = field(default=None, metadata=config(field_name="name"))
     title: Optional[str] = field(default=None, metadata=config(field_name="title"))
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
@@ -696,14 +718,20 @@
     )
     events: Optional[List[str]] = field(
         default=None, metadata=config(field_name="events")
     )
     search_queries: Optional[List[str]] = field(
         default=None, metadata=config(field_name="searchQueries")
     )
+    service_desk_id: Optional[str] = field(
+        default=None, metadata=config(field_name="serviceDeskId")
+    )
+    service_desk_type: Optional[str] = field(
+        default=None, metadata=config(field_name="serviceDeskType")
+    )
     rule_id: Optional[str] = field(default=None, metadata=config(field_name="ruleId"))
     template_id: Optional[str] = field(
         default=None, metadata=config(field_name="templateId")
     )
     type: Optional[InvestigationType] = field(
         default=None, metadata=config(field_name="type")
     )
@@ -725,14 +753,20 @@
     tags: Optional[List[str]] = field(default=None, metadata=config(field_name="tags"))
     key_findings: Optional[str] = field(
         default=None, metadata=config(field_name="keyFindings")
     )
     assignee_id: Optional[str] = field(
         default=None, metadata=config(field_name="assigneeId")
     )
+    service_desk_id: Optional[str] = field(
+        default=None, metadata=config(field_name="serviceDeskId")
+    )
+    service_desk_type: Optional[str] = field(
+        default=None, metadata=config(field_name="serviceDeskType")
+    )
     type: Optional[InvestigationType] = field(
         default=None, metadata=config(field_name="type")
     )
     status: Optional[InvestigationStatus] = field(
         default=None, metadata=config(field_name="status")
     )
 
@@ -1053,14 +1087,20 @@
     priority: Optional[int] = field(
         default=None, metadata=config(field_name="priority")
     )
     close_reason: Optional[str] = field(
         default=None, metadata=config(field_name="closeReason")
     )
     rule_id: Optional[str] = field(default=None, metadata=config(field_name="ruleId"))
+    service_desk_id: Optional[str] = field(
+        default=None, metadata=config(field_name="serviceDeskId")
+    )
+    service_desk_type: Optional[str] = field(
+        default=None, metadata=config(field_name="serviceDeskType")
+    )
     alerts_evidence: Optional[List[AlertEvidence]] = field(
         default=None, metadata=config(field_name="alertsEvidence")
     )
     assets_evidence: Optional[List[AssetEvidence]] = field(
         default=None, metadata=config(field_name="assetsEvidence")
     )
     events_evidence: Optional[List[EventEvidence]] = field(
@@ -1071,29 +1111,20 @@
     )
     contributors: Optional[List[TDRUser]] = field(
         default=None, metadata=config(field_name="contributors")
     )
     assignee: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="assignee")
     )
-    assignee_client: Optional[Client] = field(
-        default=None, metadata=config(field_name="assigneeClient")
-    )
     created_by: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="createdBy")
     )
-    created_by_client: Optional[Client] = field(
-        default=None, metadata=config(field_name="createdByClient")
-    )
     updated_by: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="updatedBy")
     )
-    updated_by_client: Optional[Client] = field(
-        default=None, metadata=config(field_name="updatedByClient")
-    )
     type: Optional[InvestigationType] = field(
         default=None, metadata=config(field_name="type")
     )
     processing_status: Optional[InvestigationProcessingStatus] = field(
         default=None, metadata=config(field_name="processingStatus")
     )
     comments_count: Optional[InvestigationCommentsCount] = field(
```

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/mitre_attack_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/mitre_attack_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/mitre_attack_info/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/mitre_attack_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/mitre_attack_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/notebooks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/notebooks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/notebooks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/notebooks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/notifications/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/notifications/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/notifications/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/notifications/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/preferences/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/preferences/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/preferences/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/preferences/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/preferences/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/roadrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/roadrunner/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/roadrunner/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/roadrunner/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/roadrunner/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/rules/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/rules/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/rules/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/rules/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/sharelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/sharelinks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/sharelinks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/sharelinks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/sharelinks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenant_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenant_profiles/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenant_profiles/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenant_profiles/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenant_profiles/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenants/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenants/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenants/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenants/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/tenants/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/threat/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/threat/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/threat/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/threat/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/threat/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/trip/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/trip/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/trip/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/trip/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/trip/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/__init__.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/users/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/mutations.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/users/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/queries.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/users/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/subscriptions.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/users/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/types.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/services/users/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/tokens.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/tokens.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python/utils.py` & `taegis-sdk-python-1.0.2/taegis_sdk_python/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import concurrent
 import logging
 from dataclasses import fields as dc_fields
 from dataclasses import is_dataclass
 from enum import Enum
 from typing import Any, Callable, Dict, Optional, Union
 
+from graphql.language.ast import FieldNode
+from graphql.language.location import SourceLocation
 from graphql.type import is_object_type, is_scalar_type
 from graphql.type import is_union_type as is_gql_union_type
 from graphql.type import is_wrapping_type
 from typing_inspect import get_args, is_union_type
 
 log = logging.getLogger(__name__)
 
@@ -239,15 +241,60 @@
     """
     for item in get_args(union):
         if result.get("__typename") == item.__name__:
             return item.from_dict(result)
     return result
 
 
+def remove_node(query: str, node: FieldNode, location: SourceLocation) -> str:
+    """Remove a GraphQL node with subnodes.
+
+    Parameters
+    ----------
+    query : str
+        GraphQL Query string
+    node : FieldNode
+        GraphQL Node
+    location : SourceLocation
+        GraphQL Node Location
+
+    Returns
+    -------
+    str
+        GraphQL Query string without erroring node (and subnodes)
+    """
+    key = node.name.value
+    start_idx = location.column - 1
+    end_idx = None
+
+    brackets_found = 0
+    for idx, char in enumerate(query):
+        if idx < start_idx + len(key):
+            continue
+
+        if char == " ":
+            continue
+
+        if brackets_found == 0 and char != "{":
+            end_idx = idx
+            break
+
+        if char == "{":
+            brackets_found += 1
+
+        elif char == "}":
+            brackets_found -= 1
+
+        end_idx = idx
+
+    return query[:start_idx] + query[end_idx:]
+
+
 __all__ = [
     "build_output_string",
     "async_block",
     "prepare_input",
     "prepare_variables",
     "parse_union_result",
     "build_output_string_from_introspection",
+    "remove_node",
 ]
```

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/PKG-INFO` & `taegis-sdk-python-1.0.2/taegis_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/SOURCES.txt` & `taegis-sdk-python-1.0.2/taegis_sdk_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,19 @@
 taegis_sdk_python/services/events/subscriptions.py
 taegis_sdk_python/services/events/types.py
 taegis_sdk_python/services/exports/__init__.py
 taegis_sdk_python/services/exports/mutations.py
 taegis_sdk_python/services/exports/queries.py
 taegis_sdk_python/services/exports/subscriptions.py
 taegis_sdk_python/services/exports/types.py
+taegis_sdk_python/services/fast_ioc/__init__.py
+taegis_sdk_python/services/fast_ioc/mutations.py
+taegis_sdk_python/services/fast_ioc/queries.py
+taegis_sdk_python/services/fast_ioc/subscriptions.py
+taegis_sdk_python/services/fast_ioc/types.py
 taegis_sdk_python/services/investigations/__init__.py
 taegis_sdk_python/services/investigations/mutations.py
 taegis_sdk_python/services/investigations/queries.py
 taegis_sdk_python/services/investigations/subscriptions.py
 taegis_sdk_python/services/investigations/types.py
 taegis_sdk_python/services/investigations2/__init__.py
 taegis_sdk_python/services/investigations2/mutations.py
```

