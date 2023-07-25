# Comparing `tmp/google-cloud-dataplex-1.5.1.tar.gz` & `tmp/google-cloud-dataplex-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-dataplex-1.5.1.tar", last modified: Wed Jul  5 15:52:12 2023, max compression
+gzip compressed data, was "google-cloud-dataplex-1.6.0.tar", last modified: Tue Jul 25 14:42:54 2023, max compression
```

## Comparing `google-cloud-dataplex-1.5.1.tar` & `google-cloud-dataplex-1.6.0.tar`

### file list

```diff
@@ -1,93 +1,106 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4696 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3773 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.665150 google-cloud-dataplex-1.5.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.665150 google-cloud-dataplex-1.5.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.665150 google-cloud-dataplex-1.5.1/google/cloud/dataplex/
--rw-rw-r--   0 root         (0)     1003     7243 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.669150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/
--rw-rw-r--   0 root         (0)     1003     6436 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    15314 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.669150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.669150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/
--rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    62854 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    71605 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/client.py
--rw-rw-r--   0 root         (0)     1003     5658 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.669150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12118 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25618 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25992 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.669150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    62259 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    73395 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/client.py
--rw-rw-r--   0 root         (0)     1003    10807 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.673150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10921 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25499 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25983 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.673150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   186272 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   199302 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/client.py
--rw-rw-r--   0 root         (0)     1003    49482 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.673150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    26223 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    52208 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    53320 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.677150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    61629 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    72083 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/client.py
--rw-rw-r--   0 root         (0)     1003    10685 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.677150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12419 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25614 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26039 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.677150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/
--rw-rw-r--   0 root         (0)     1003     5638 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16335 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/analyze.py
--rw-rw-r--   0 root         (0)     1003     6555 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/content.py
--rw-rw-r--   0 root         (0)     1003    15619 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/data_profile.py
--rw-rw-r--   0 root         (0)     1003    16628 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/data_quality.py
--rw-rw-r--   0 root         (0)     1003    24703 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/datascans.py
--rw-rw-r--   0 root         (0)     1003    22735 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/logs.py
--rw-rw-r--   0 root         (0)     1003    38144 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/metadata_.py
--rw-rw-r--   0 root         (0)     1003     5857 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/processing.py
--rw-rw-r--   0 root         (0)     1003    50791 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    39146 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/service.py
--rw-rw-r--   0 root         (0)     1003    26001 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/tasks.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/
--rw-r--r--   0 root         (0)     1003     4696 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3701 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2976 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   154372 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_content_service.py
--rw-rw-r--   0 root         (0)     1003   169258 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_data_scan_service.py
--rw-rw-r--   0 root         (0)     1003   431726 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_dataplex_service.py
--rw-rw-r--   0 root         (0)     1003   175809 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_metadata_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.446795 google-cloud-dataplex-1.6.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4802 2023-07-25 14:42:54.446795 google-cloud-dataplex-1.6.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3879 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.426792 google-cloud-dataplex-1.6.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.426792 google-cloud-dataplex-1.6.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.430793 google-cloud-dataplex-1.6.0/google/cloud/dataplex/
+-rw-rw-r--   0 root         (0)     1003     9177 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.430793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/
+-rw-rw-r--   0 root         (0)     1003     8227 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19755 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.430793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.430793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62854 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    71605 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5658 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.430793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12118 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25618 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25992 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.430793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62559 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    74218 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10807 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.434793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10921 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25499 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25983 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.434793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   100461 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   112949 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16556 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.434793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14730 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    35102 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    35794 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.434793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   186272 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   199302 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/client.py
+-rw-rw-r--   0 root         (0)     1003    49482 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.438794 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26223 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    52208 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    53320 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.438794 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    61629 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    72083 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10685 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.438794 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12419 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25614 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26039 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.442794 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/
+-rw-rw-r--   0 root         (0)     1003     7231 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16335 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/analyze.py
+-rw-rw-r--   0 root         (0)     1003     6555 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/content.py
+-rw-rw-r--   0 root         (0)     1003    22473 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/data_profile.py
+-rw-rw-r--   0 root         (0)     1003    22328 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/data_quality.py
+-rw-rw-r--   0 root         (0)     1003    31056 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/data_taxonomy.py
+-rw-rw-r--   0 root         (0)     1003    25542 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/datascans.py
+-rw-rw-r--   0 root         (0)     1003    34752 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/logs.py
+-rw-rw-r--   0 root         (0)     1003    38145 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/metadata_.py
+-rw-rw-r--   0 root         (0)     1003     5857 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/processing.py
+-rw-rw-r--   0 root         (0)     1003    50791 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003     2922 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/security.py
+-rw-rw-r--   0 root         (0)     1003    40691 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/service.py
+-rw-rw-r--   0 root         (0)     1003    27261 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/tasks.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.442794 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/
+-rw-r--r--   0 root         (0)     1003     4802 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4435 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-25 14:42:54.446795 google-cloud-dataplex-1.6.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2976 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.442794 google-cloud-dataplex-1.6.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.442794 google-cloud-dataplex-1.6.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.442794 google-cloud-dataplex-1.6.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.446795 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   154372 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_content_service.py
+-rw-rw-r--   0 root         (0)     1003   169945 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_data_scan_service.py
+-rw-rw-r--   0 root         (0)     1003   249588 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_data_taxonomy_service.py
+-rw-rw-r--   0 root         (0)     1003   431954 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_dataplex_service.py
+-rw-rw-r--   0 root         (0)     1003   175809 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_metadata_service.py
```

### Comparing `google-cloud-dataplex-1.5.1/LICENSE` & `google-cloud-dataplex-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.1/MANIFEST.in` & `google-cloud-dataplex-1.6.0/MANIFEST.in`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2020 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/PKG-INFO` & `google-cloud-dataplex-1.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataplex
-Version: 1.5.1
+Version: 1.6.0
 Summary: Google Cloud Dataplex API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Cloud Dataplex.:  https://cloud.google.com/dataplex
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
-Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
+creates isolated Python environments. These isolated environments can have separate
+versions of Python packages, which allows you to isolate one project's dependencies
+from the dependencies of other projects.
 
-With `virtualenv`_, it's possible to install this library without needing system
+With `venv`_, it's possible to install this library without needing system
 install permissions, and without clashing with the installed system
 dependencies.
 
-.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
+.. _`venv`: https://docs.python.org/3/library/venv.html
 
 
 Code samples and snippets
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Code samples and snippets live in the `samples/` folder.
+Code samples and snippets live in the `samples/`_ folder.
+
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-dataplex/samples
 
 
 Supported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
 Python.
 
@@ -97,29 +100,27 @@
 .. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
+    python3 -m venv <your-env>
     source <your-env>/bin/activate
-    <your-env>/bin/pip install google-cloud-dataplex
+    pip install google-cloud-dataplex
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-dataplex
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-dataplex
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Cloud Dataplex
    to see other available methods on the client.
 -  Read the `Cloud Dataplex Product documentation`_ to learn
```

### Comparing `google-cloud-dataplex-1.5.1/README.rst` & `google-cloud-dataplex-1.6.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -32,29 +32,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Cloud Dataplex.:  https://cloud.google.com/dataplex
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
-Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
+creates isolated Python environments. These isolated environments can have separate
+versions of Python packages, which allows you to isolate one project's dependencies
+from the dependencies of other projects.
 
-With `virtualenv`_, it's possible to install this library without needing system
+With `venv`_, it's possible to install this library without needing system
 install permissions, and without clashing with the installed system
 dependencies.
 
-.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
+.. _`venv`: https://docs.python.org/3/library/venv.html
 
 
 Code samples and snippets
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Code samples and snippets live in the `samples/` folder.
+Code samples and snippets live in the `samples/`_ folder.
+
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-dataplex/samples
 
 
 Supported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
 Python.
 
@@ -73,29 +76,27 @@
 .. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
+    python3 -m venv <your-env>
     source <your-env>/bin/activate
-    <your-env>/bin/pip install google-cloud-dataplex
+    pip install google-cloud-dataplex
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-dataplex
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-dataplex
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Cloud Dataplex
    to see other available methods on the client.
 -  Read the `Cloud Dataplex Product documentation`_ to learn
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex/__init__.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,79 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.dataplex import gapic_version as package_version
+from google.cloud.dataplex_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from google.cloud.dataplex_v1.services.content_service.async_client import (
-    ContentServiceAsyncClient,
-)
-from google.cloud.dataplex_v1.services.content_service.client import (
-    ContentServiceClient,
-)
-from google.cloud.dataplex_v1.services.data_scan_service.async_client import (
+from .services.content_service import ContentServiceAsyncClient, ContentServiceClient
+from .services.data_scan_service import (
     DataScanServiceAsyncClient,
-)
-from google.cloud.dataplex_v1.services.data_scan_service.client import (
     DataScanServiceClient,
 )
-from google.cloud.dataplex_v1.services.dataplex_service.async_client import (
-    DataplexServiceAsyncClient,
-)
-from google.cloud.dataplex_v1.services.dataplex_service.client import (
-    DataplexServiceClient,
-)
-from google.cloud.dataplex_v1.services.metadata_service.async_client import (
-    MetadataServiceAsyncClient,
-)
-from google.cloud.dataplex_v1.services.metadata_service.client import (
-    MetadataServiceClient,
-)
-from google.cloud.dataplex_v1.types.analyze import Content, Environment, Session
-from google.cloud.dataplex_v1.types.content import (
+from .services.data_taxonomy_service import (
+    DataTaxonomyServiceAsyncClient,
+    DataTaxonomyServiceClient,
+)
+from .services.dataplex_service import DataplexServiceAsyncClient, DataplexServiceClient
+from .services.metadata_service import MetadataServiceAsyncClient, MetadataServiceClient
+from .types.analyze import Content, Environment, Session
+from .types.content import (
     CreateContentRequest,
     DeleteContentRequest,
     GetContentRequest,
     ListContentRequest,
     ListContentResponse,
     UpdateContentRequest,
 )
-from google.cloud.dataplex_v1.types.data_profile import (
-    DataProfileResult,
-    DataProfileSpec,
-)
-from google.cloud.dataplex_v1.types.data_quality import (
+from .types.data_profile import DataProfileResult, DataProfileSpec
+from .types.data_quality import (
     DataQualityDimensionResult,
     DataQualityResult,
     DataQualityRule,
     DataQualityRuleResult,
     DataQualitySpec,
 )
-from google.cloud.dataplex_v1.types.datascans import (
+from .types.data_taxonomy import (
+    CreateDataAttributeBindingRequest,
+    CreateDataAttributeRequest,
+    CreateDataTaxonomyRequest,
+    DataAttribute,
+    DataAttributeBinding,
+    DataTaxonomy,
+    DeleteDataAttributeBindingRequest,
+    DeleteDataAttributeRequest,
+    DeleteDataTaxonomyRequest,
+    GetDataAttributeBindingRequest,
+    GetDataAttributeRequest,
+    GetDataTaxonomyRequest,
+    ListDataAttributeBindingsRequest,
+    ListDataAttributeBindingsResponse,
+    ListDataAttributesRequest,
+    ListDataAttributesResponse,
+    ListDataTaxonomiesRequest,
+    ListDataTaxonomiesResponse,
+    UpdateDataAttributeBindingRequest,
+    UpdateDataAttributeRequest,
+    UpdateDataTaxonomyRequest,
+)
+from .types.datascans import (
     CreateDataScanRequest,
     DataScan,
     DataScanJob,
     DataScanType,
     DeleteDataScanRequest,
     GetDataScanJobRequest,
     GetDataScanRequest,
@@ -74,21 +81,22 @@
     ListDataScanJobsResponse,
     ListDataScansRequest,
     ListDataScansResponse,
     RunDataScanRequest,
     RunDataScanResponse,
     UpdateDataScanRequest,
 )
-from google.cloud.dataplex_v1.types.logs import (
+from .types.logs import (
+    DataQualityScanRuleResult,
     DataScanEvent,
     DiscoveryEvent,
     JobEvent,
     SessionEvent,
 )
-from google.cloud.dataplex_v1.types.metadata_ import (
+from .types.metadata_ import (
     CreateEntityRequest,
     CreatePartitionRequest,
     DeleteEntityRequest,
     DeletePartitionRequest,
     Entity,
     GetEntityRequest,
     GetPartitionRequest,
@@ -99,24 +107,18 @@
     Partition,
     Schema,
     StorageAccess,
     StorageFormat,
     StorageSystem,
     UpdateEntityRequest,
 )
-from google.cloud.dataplex_v1.types.processing import DataSource, ScannedData, Trigger
-from google.cloud.dataplex_v1.types.resources import (
-    Action,
-    Asset,
-    AssetStatus,
-    Lake,
-    State,
-    Zone,
-)
-from google.cloud.dataplex_v1.types.service import (
+from .types.processing import DataSource, ScannedData, Trigger
+from .types.resources import Action, Asset, AssetStatus, Lake, State, Zone
+from .types.security import DataAccessSpec, ResourceAccessSpec
+from .types.service import (
     CancelJobRequest,
     CreateAssetRequest,
     CreateEnvironmentRequest,
     CreateLakeRequest,
     CreateTaskRequest,
     CreateZoneRequest,
     DeleteAssetRequest,
@@ -153,124 +155,150 @@
     RunTaskResponse,
     UpdateAssetRequest,
     UpdateEnvironmentRequest,
     UpdateLakeRequest,
     UpdateTaskRequest,
     UpdateZoneRequest,
 )
-from google.cloud.dataplex_v1.types.tasks import Job, Task
+from .types.tasks import Job, Task
 
 __all__ = (
-    "ContentServiceClient",
     "ContentServiceAsyncClient",
-    "DataplexServiceClient",
-    "DataplexServiceAsyncClient",
-    "DataScanServiceClient",
     "DataScanServiceAsyncClient",
-    "MetadataServiceClient",
+    "DataTaxonomyServiceAsyncClient",
+    "DataplexServiceAsyncClient",
     "MetadataServiceAsyncClient",
+    "Action",
+    "Asset",
+    "AssetStatus",
+    "CancelJobRequest",
     "Content",
-    "Environment",
-    "Session",
+    "ContentServiceClient",
+    "CreateAssetRequest",
     "CreateContentRequest",
-    "DeleteContentRequest",
-    "GetContentRequest",
-    "ListContentRequest",
-    "ListContentResponse",
-    "UpdateContentRequest",
+    "CreateDataAttributeBindingRequest",
+    "CreateDataAttributeRequest",
+    "CreateDataScanRequest",
+    "CreateDataTaxonomyRequest",
+    "CreateEntityRequest",
+    "CreateEnvironmentRequest",
+    "CreateLakeRequest",
+    "CreatePartitionRequest",
+    "CreateTaskRequest",
+    "CreateZoneRequest",
+    "DataAccessSpec",
+    "DataAttribute",
+    "DataAttributeBinding",
     "DataProfileResult",
     "DataProfileSpec",
     "DataQualityDimensionResult",
     "DataQualityResult",
     "DataQualityRule",
     "DataQualityRuleResult",
+    "DataQualityScanRuleResult",
     "DataQualitySpec",
-    "CreateDataScanRequest",
     "DataScan",
+    "DataScanEvent",
     "DataScanJob",
-    "DeleteDataScanRequest",
-    "GetDataScanJobRequest",
-    "GetDataScanRequest",
-    "ListDataScanJobsRequest",
-    "ListDataScanJobsResponse",
-    "ListDataScansRequest",
-    "ListDataScansResponse",
-    "RunDataScanRequest",
-    "RunDataScanResponse",
-    "UpdateDataScanRequest",
+    "DataScanServiceClient",
     "DataScanType",
-    "DataScanEvent",
-    "DiscoveryEvent",
-    "JobEvent",
-    "SessionEvent",
-    "CreateEntityRequest",
-    "CreatePartitionRequest",
-    "DeleteEntityRequest",
-    "DeletePartitionRequest",
-    "Entity",
-    "GetEntityRequest",
-    "GetPartitionRequest",
-    "ListEntitiesRequest",
-    "ListEntitiesResponse",
-    "ListPartitionsRequest",
-    "ListPartitionsResponse",
-    "Partition",
-    "Schema",
-    "StorageAccess",
-    "StorageFormat",
-    "UpdateEntityRequest",
-    "StorageSystem",
     "DataSource",
-    "ScannedData",
-    "Trigger",
-    "Action",
-    "Asset",
-    "AssetStatus",
-    "Lake",
-    "Zone",
-    "State",
-    "CancelJobRequest",
-    "CreateAssetRequest",
-    "CreateEnvironmentRequest",
-    "CreateLakeRequest",
-    "CreateTaskRequest",
-    "CreateZoneRequest",
+    "DataTaxonomy",
+    "DataTaxonomyServiceClient",
+    "DataplexServiceClient",
     "DeleteAssetRequest",
+    "DeleteContentRequest",
+    "DeleteDataAttributeBindingRequest",
+    "DeleteDataAttributeRequest",
+    "DeleteDataScanRequest",
+    "DeleteDataTaxonomyRequest",
+    "DeleteEntityRequest",
     "DeleteEnvironmentRequest",
     "DeleteLakeRequest",
+    "DeletePartitionRequest",
     "DeleteTaskRequest",
     "DeleteZoneRequest",
+    "DiscoveryEvent",
+    "Entity",
+    "Environment",
     "GetAssetRequest",
+    "GetContentRequest",
+    "GetDataAttributeBindingRequest",
+    "GetDataAttributeRequest",
+    "GetDataScanJobRequest",
+    "GetDataScanRequest",
+    "GetDataTaxonomyRequest",
+    "GetEntityRequest",
     "GetEnvironmentRequest",
     "GetJobRequest",
     "GetLakeRequest",
+    "GetPartitionRequest",
     "GetTaskRequest",
     "GetZoneRequest",
+    "Job",
+    "JobEvent",
+    "Lake",
     "ListActionsResponse",
     "ListAssetActionsRequest",
     "ListAssetsRequest",
     "ListAssetsResponse",
+    "ListContentRequest",
+    "ListContentResponse",
+    "ListDataAttributeBindingsRequest",
+    "ListDataAttributeBindingsResponse",
+    "ListDataAttributesRequest",
+    "ListDataAttributesResponse",
+    "ListDataScanJobsRequest",
+    "ListDataScanJobsResponse",
+    "ListDataScansRequest",
+    "ListDataScansResponse",
+    "ListDataTaxonomiesRequest",
+    "ListDataTaxonomiesResponse",
+    "ListEntitiesRequest",
+    "ListEntitiesResponse",
     "ListEnvironmentsRequest",
     "ListEnvironmentsResponse",
     "ListJobsRequest",
     "ListJobsResponse",
     "ListLakeActionsRequest",
     "ListLakesRequest",
     "ListLakesResponse",
+    "ListPartitionsRequest",
+    "ListPartitionsResponse",
     "ListSessionsRequest",
     "ListSessionsResponse",
     "ListTasksRequest",
     "ListTasksResponse",
     "ListZoneActionsRequest",
     "ListZonesRequest",
     "ListZonesResponse",
+    "MetadataServiceClient",
     "OperationMetadata",
+    "Partition",
+    "ResourceAccessSpec",
+    "RunDataScanRequest",
+    "RunDataScanResponse",
     "RunTaskRequest",
     "RunTaskResponse",
+    "ScannedData",
+    "Schema",
+    "Session",
+    "SessionEvent",
+    "State",
+    "StorageAccess",
+    "StorageFormat",
+    "StorageSystem",
+    "Task",
+    "Trigger",
     "UpdateAssetRequest",
+    "UpdateContentRequest",
+    "UpdateDataAttributeBindingRequest",
+    "UpdateDataAttributeRequest",
+    "UpdateDataScanRequest",
+    "UpdateDataTaxonomyRequest",
+    "UpdateEntityRequest",
     "UpdateEnvironmentRequest",
     "UpdateLakeRequest",
     "UpdateTaskRequest",
     "UpdateZoneRequest",
-    "Job",
-    "Task",
+    "Zone",
 )
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex/gapic_version.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.1"  # {x-release-please-version}
+__version__ = "1.6.0"  # {x-release-please-version}
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/__init__.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.dataplex_v1 import gapic_version as package_version
-
-__version__ = package_version.__version__
-
-
-from .services.content_service import ContentServiceAsyncClient, ContentServiceClient
-from .services.data_scan_service import (
-    DataScanServiceAsyncClient,
-    DataScanServiceClient,
-)
-from .services.dataplex_service import DataplexServiceAsyncClient, DataplexServiceClient
-from .services.metadata_service import MetadataServiceAsyncClient, MetadataServiceClient
-from .types.analyze import Content, Environment, Session
-from .types.content import (
+from .analyze import Content, Environment, Session
+from .content import (
     CreateContentRequest,
     DeleteContentRequest,
     GetContentRequest,
     ListContentRequest,
     ListContentResponse,
     UpdateContentRequest,
 )
-from .types.data_profile import DataProfileResult, DataProfileSpec
-from .types.data_quality import (
+from .data_profile import DataProfileResult, DataProfileSpec
+from .data_quality import (
     DataQualityDimensionResult,
     DataQualityResult,
     DataQualityRule,
     DataQualityRuleResult,
     DataQualitySpec,
 )
-from .types.datascans import (
+from .data_taxonomy import (
+    CreateDataAttributeBindingRequest,
+    CreateDataAttributeRequest,
+    CreateDataTaxonomyRequest,
+    DataAttribute,
+    DataAttributeBinding,
+    DataTaxonomy,
+    DeleteDataAttributeBindingRequest,
+    DeleteDataAttributeRequest,
+    DeleteDataTaxonomyRequest,
+    GetDataAttributeBindingRequest,
+    GetDataAttributeRequest,
+    GetDataTaxonomyRequest,
+    ListDataAttributeBindingsRequest,
+    ListDataAttributeBindingsResponse,
+    ListDataAttributesRequest,
+    ListDataAttributesResponse,
+    ListDataTaxonomiesRequest,
+    ListDataTaxonomiesResponse,
+    UpdateDataAttributeBindingRequest,
+    UpdateDataAttributeRequest,
+    UpdateDataTaxonomyRequest,
+)
+from .datascans import (
     CreateDataScanRequest,
     DataScan,
     DataScanJob,
     DataScanType,
     DeleteDataScanRequest,
     GetDataScanJobRequest,
     GetDataScanRequest,
@@ -54,16 +65,22 @@
     ListDataScanJobsResponse,
     ListDataScansRequest,
     ListDataScansResponse,
     RunDataScanRequest,
     RunDataScanResponse,
     UpdateDataScanRequest,
 )
-from .types.logs import DataScanEvent, DiscoveryEvent, JobEvent, SessionEvent
-from .types.metadata_ import (
+from .logs import (
+    DataQualityScanRuleResult,
+    DataScanEvent,
+    DiscoveryEvent,
+    JobEvent,
+    SessionEvent,
+)
+from .metadata_ import (
     CreateEntityRequest,
     CreatePartitionRequest,
     DeleteEntityRequest,
     DeletePartitionRequest,
     Entity,
     GetEntityRequest,
     GetPartitionRequest,
@@ -74,17 +91,18 @@
     Partition,
     Schema,
     StorageAccess,
     StorageFormat,
     StorageSystem,
     UpdateEntityRequest,
 )
-from .types.processing import DataSource, ScannedData, Trigger
-from .types.resources import Action, Asset, AssetStatus, Lake, State, Zone
-from .types.service import (
+from .processing import DataSource, ScannedData, Trigger
+from .resources import Action, Asset, AssetStatus, Lake, State, Zone
+from .security import DataAccessSpec, ResourceAccessSpec
+from .service import (
     CancelJobRequest,
     CreateAssetRequest,
     CreateEnvironmentRequest,
     CreateLakeRequest,
     CreateTaskRequest,
     CreateZoneRequest,
     DeleteAssetRequest,
@@ -121,124 +139,140 @@
     RunTaskResponse,
     UpdateAssetRequest,
     UpdateEnvironmentRequest,
     UpdateLakeRequest,
     UpdateTaskRequest,
     UpdateZoneRequest,
 )
-from .types.tasks import Job, Task
+from .tasks import Job, Task
 
 __all__ = (
-    "ContentServiceAsyncClient",
-    "DataScanServiceAsyncClient",
-    "DataplexServiceAsyncClient",
-    "MetadataServiceAsyncClient",
-    "Action",
-    "Asset",
-    "AssetStatus",
-    "CancelJobRequest",
     "Content",
-    "ContentServiceClient",
-    "CreateAssetRequest",
+    "Environment",
+    "Session",
     "CreateContentRequest",
-    "CreateDataScanRequest",
-    "CreateEntityRequest",
-    "CreateEnvironmentRequest",
-    "CreateLakeRequest",
-    "CreatePartitionRequest",
-    "CreateTaskRequest",
-    "CreateZoneRequest",
+    "DeleteContentRequest",
+    "GetContentRequest",
+    "ListContentRequest",
+    "ListContentResponse",
+    "UpdateContentRequest",
     "DataProfileResult",
     "DataProfileSpec",
     "DataQualityDimensionResult",
     "DataQualityResult",
     "DataQualityRule",
     "DataQualityRuleResult",
     "DataQualitySpec",
+    "CreateDataAttributeBindingRequest",
+    "CreateDataAttributeRequest",
+    "CreateDataTaxonomyRequest",
+    "DataAttribute",
+    "DataAttributeBinding",
+    "DataTaxonomy",
+    "DeleteDataAttributeBindingRequest",
+    "DeleteDataAttributeRequest",
+    "DeleteDataTaxonomyRequest",
+    "GetDataAttributeBindingRequest",
+    "GetDataAttributeRequest",
+    "GetDataTaxonomyRequest",
+    "ListDataAttributeBindingsRequest",
+    "ListDataAttributeBindingsResponse",
+    "ListDataAttributesRequest",
+    "ListDataAttributesResponse",
+    "ListDataTaxonomiesRequest",
+    "ListDataTaxonomiesResponse",
+    "UpdateDataAttributeBindingRequest",
+    "UpdateDataAttributeRequest",
+    "UpdateDataTaxonomyRequest",
+    "CreateDataScanRequest",
     "DataScan",
-    "DataScanEvent",
     "DataScanJob",
-    "DataScanServiceClient",
+    "DeleteDataScanRequest",
+    "GetDataScanJobRequest",
+    "GetDataScanRequest",
+    "ListDataScanJobsRequest",
+    "ListDataScanJobsResponse",
+    "ListDataScansRequest",
+    "ListDataScansResponse",
+    "RunDataScanRequest",
+    "RunDataScanResponse",
+    "UpdateDataScanRequest",
     "DataScanType",
+    "DataQualityScanRuleResult",
+    "DataScanEvent",
+    "DiscoveryEvent",
+    "JobEvent",
+    "SessionEvent",
+    "CreateEntityRequest",
+    "CreatePartitionRequest",
+    "DeleteEntityRequest",
+    "DeletePartitionRequest",
+    "Entity",
+    "GetEntityRequest",
+    "GetPartitionRequest",
+    "ListEntitiesRequest",
+    "ListEntitiesResponse",
+    "ListPartitionsRequest",
+    "ListPartitionsResponse",
+    "Partition",
+    "Schema",
+    "StorageAccess",
+    "StorageFormat",
+    "UpdateEntityRequest",
+    "StorageSystem",
     "DataSource",
-    "DataplexServiceClient",
+    "ScannedData",
+    "Trigger",
+    "Action",
+    "Asset",
+    "AssetStatus",
+    "Lake",
+    "Zone",
+    "State",
+    "DataAccessSpec",
+    "ResourceAccessSpec",
+    "CancelJobRequest",
+    "CreateAssetRequest",
+    "CreateEnvironmentRequest",
+    "CreateLakeRequest",
+    "CreateTaskRequest",
+    "CreateZoneRequest",
     "DeleteAssetRequest",
-    "DeleteContentRequest",
-    "DeleteDataScanRequest",
-    "DeleteEntityRequest",
     "DeleteEnvironmentRequest",
     "DeleteLakeRequest",
-    "DeletePartitionRequest",
     "DeleteTaskRequest",
     "DeleteZoneRequest",
-    "DiscoveryEvent",
-    "Entity",
-    "Environment",
     "GetAssetRequest",
-    "GetContentRequest",
-    "GetDataScanJobRequest",
-    "GetDataScanRequest",
-    "GetEntityRequest",
     "GetEnvironmentRequest",
     "GetJobRequest",
     "GetLakeRequest",
-    "GetPartitionRequest",
     "GetTaskRequest",
     "GetZoneRequest",
-    "Job",
-    "JobEvent",
-    "Lake",
     "ListActionsResponse",
     "ListAssetActionsRequest",
     "ListAssetsRequest",
     "ListAssetsResponse",
-    "ListContentRequest",
-    "ListContentResponse",
-    "ListDataScanJobsRequest",
-    "ListDataScanJobsResponse",
-    "ListDataScansRequest",
-    "ListDataScansResponse",
-    "ListEntitiesRequest",
-    "ListEntitiesResponse",
     "ListEnvironmentsRequest",
     "ListEnvironmentsResponse",
     "ListJobsRequest",
     "ListJobsResponse",
     "ListLakeActionsRequest",
     "ListLakesRequest",
     "ListLakesResponse",
-    "ListPartitionsRequest",
-    "ListPartitionsResponse",
     "ListSessionsRequest",
     "ListSessionsResponse",
     "ListTasksRequest",
     "ListTasksResponse",
     "ListZoneActionsRequest",
     "ListZonesRequest",
     "ListZonesResponse",
-    "MetadataServiceClient",
     "OperationMetadata",
-    "Partition",
-    "RunDataScanRequest",
-    "RunDataScanResponse",
     "RunTaskRequest",
     "RunTaskResponse",
-    "ScannedData",
-    "Schema",
-    "Session",
-    "SessionEvent",
-    "State",
-    "StorageAccess",
-    "StorageFormat",
-    "StorageSystem",
-    "Task",
-    "Trigger",
     "UpdateAssetRequest",
-    "UpdateContentRequest",
-    "UpdateDataScanRequest",
-    "UpdateEntityRequest",
     "UpdateEnvironmentRequest",
     "UpdateLakeRequest",
     "UpdateTaskRequest",
     "UpdateZoneRequest",
-    "Zone",
+    "Job",
+    "Task",
 )
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/gapic_version.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.1"  # {x-release-please-version}
+__version__ = "1.6.0"  # {x-release-please-version}
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/__init__.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/__init__.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/async_client.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -700,16 +700,16 @@
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]]):
                 The request object. Request message for ``GetIamPolicy`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
-                policy is being requested. See the
-                operation documentation for the
+                policy is being requested.
+                See the operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/client.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -940,16 +940,16 @@
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
                 The request object. Request message for ``GetIamPolicy`` method.
             resource (str):
                 REQUIRED: The resource for which the
-                policy is being requested. See the
-                operation documentation for the
+                policy is being requested.
+                See the operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/pagers.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/__init__.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/base.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/grpc.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/__init__.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/async_client.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -83,14 +83,16 @@
     parse_data_scan_path = staticmethod(DataScanServiceClient.parse_data_scan_path)
     data_scan_job_path = staticmethod(DataScanServiceClient.data_scan_job_path)
     parse_data_scan_job_path = staticmethod(
         DataScanServiceClient.parse_data_scan_job_path
     )
     entity_path = staticmethod(DataScanServiceClient.entity_path)
     parse_entity_path = staticmethod(DataScanServiceClient.parse_entity_path)
+    table_path = staticmethod(DataScanServiceClient.table_path)
+    parse_table_path = staticmethod(DataScanServiceClient.parse_table_path)
     common_billing_account_path = staticmethod(
         DataScanServiceClient.common_billing_account_path
     )
     parse_common_billing_account_path = staticmethod(
         DataScanServiceClient.parse_common_billing_account_path
     )
     common_folder_path = staticmethod(DataScanServiceClient.common_folder_path)
@@ -267,14 +269,15 @@
 
             async def sample_create_data_scan():
                 # Create a client
                 client = dataplex_v1.DataScanServiceAsyncClient()
 
                 # Initialize request argument(s)
                 data_scan = dataplex_v1.DataScan()
+                data_scan.data_quality_spec.rules.dimension = "dimension_value"
                 data_scan.data.entity = "entity_value"
 
                 request = dataplex_v1.CreateDataScanRequest(
                     parent="parent_value",
                     data_scan=data_scan,
                     data_scan_id="data_scan_id_value",
                 )
@@ -423,14 +426,15 @@
 
             async def sample_update_data_scan():
                 # Create a client
                 client = dataplex_v1.DataScanServiceAsyncClient()
 
                 # Initialize request argument(s)
                 data_scan = dataplex_v1.DataScan()
+                data_scan.data_quality_spec.rules.dimension = "dimension_value"
                 data_scan.data.entity = "entity_value"
 
                 request = dataplex_v1.UpdateDataScanRequest(
                     data_scan=data_scan,
                 )
 
                 # Make the request
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/client.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -265,14 +265,36 @@
         m = re.match(
             r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)/lakes/(?P<lake>.+?)/zones/(?P<zone>.+?)/entities/(?P<entity>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
+    def table_path(
+        project: str,
+        dataset: str,
+        table: str,
+    ) -> str:
+        """Returns a fully-qualified table string."""
+        return "projects/{project}/datasets/{dataset}/tables/{table}".format(
+            project=project,
+            dataset=dataset,
+            table=table,
+        )
+
+    @staticmethod
+    def parse_table_path(path: str) -> Dict[str, str]:
+        """Parses a table path into its component segments."""
+        m = re.match(
+            r"^projects/(?P<project>.+?)/datasets/(?P<dataset>.+?)/tables/(?P<table>.+?)$",
+            path,
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
     def common_billing_account_path(
         billing_account: str,
     ) -> str:
         """Returns a fully-qualified billing_account string."""
         return "billingAccounts/{billing_account}".format(
             billing_account=billing_account,
         )
@@ -538,14 +560,15 @@
 
             def sample_create_data_scan():
                 # Create a client
                 client = dataplex_v1.DataScanServiceClient()
 
                 # Initialize request argument(s)
                 data_scan = dataplex_v1.DataScan()
+                data_scan.data_quality_spec.rules.dimension = "dimension_value"
                 data_scan.data.entity = "entity_value"
 
                 request = dataplex_v1.CreateDataScanRequest(
                     parent="parent_value",
                     data_scan=data_scan,
                     data_scan_id="data_scan_id_value",
                 )
@@ -694,14 +717,15 @@
 
             def sample_update_data_scan():
                 # Create a client
                 client = dataplex_v1.DataScanServiceClient()
 
                 # Initialize request argument(s)
                 data_scan = dataplex_v1.DataScan()
+                data_scan.data_quality_spec.rules.dimension = "dimension_value"
                 data_scan.data.entity = "entity_value"
 
                 request = dataplex_v1.UpdateDataScanRequest(
                     data_scan=data_scan,
                 )
 
                 # Make the request
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/pagers.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/__init__.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/async_client.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/client.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/pagers.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/__init__.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/async_client.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/client.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/pagers.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/base.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/__init__.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,101 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from .analyze import Content, Environment, Session
-from .content import (
+from google.cloud.dataplex import gapic_version as package_version
+
+__version__ = package_version.__version__
+
+
+from google.cloud.dataplex_v1.services.content_service.async_client import (
+    ContentServiceAsyncClient,
+)
+from google.cloud.dataplex_v1.services.content_service.client import (
+    ContentServiceClient,
+)
+from google.cloud.dataplex_v1.services.data_scan_service.async_client import (
+    DataScanServiceAsyncClient,
+)
+from google.cloud.dataplex_v1.services.data_scan_service.client import (
+    DataScanServiceClient,
+)
+from google.cloud.dataplex_v1.services.data_taxonomy_service.async_client import (
+    DataTaxonomyServiceAsyncClient,
+)
+from google.cloud.dataplex_v1.services.data_taxonomy_service.client import (
+    DataTaxonomyServiceClient,
+)
+from google.cloud.dataplex_v1.services.dataplex_service.async_client import (
+    DataplexServiceAsyncClient,
+)
+from google.cloud.dataplex_v1.services.dataplex_service.client import (
+    DataplexServiceClient,
+)
+from google.cloud.dataplex_v1.services.metadata_service.async_client import (
+    MetadataServiceAsyncClient,
+)
+from google.cloud.dataplex_v1.services.metadata_service.client import (
+    MetadataServiceClient,
+)
+from google.cloud.dataplex_v1.types.analyze import Content, Environment, Session
+from google.cloud.dataplex_v1.types.content import (
     CreateContentRequest,
     DeleteContentRequest,
     GetContentRequest,
     ListContentRequest,
     ListContentResponse,
     UpdateContentRequest,
 )
-from .data_profile import DataProfileResult, DataProfileSpec
-from .data_quality import (
+from google.cloud.dataplex_v1.types.data_profile import (
+    DataProfileResult,
+    DataProfileSpec,
+)
+from google.cloud.dataplex_v1.types.data_quality import (
     DataQualityDimensionResult,
     DataQualityResult,
     DataQualityRule,
     DataQualityRuleResult,
     DataQualitySpec,
 )
-from .datascans import (
+from google.cloud.dataplex_v1.types.data_taxonomy import (
+    CreateDataAttributeBindingRequest,
+    CreateDataAttributeRequest,
+    CreateDataTaxonomyRequest,
+    DataAttribute,
+    DataAttributeBinding,
+    DataTaxonomy,
+    DeleteDataAttributeBindingRequest,
+    DeleteDataAttributeRequest,
+    DeleteDataTaxonomyRequest,
+    GetDataAttributeBindingRequest,
+    GetDataAttributeRequest,
+    GetDataTaxonomyRequest,
+    ListDataAttributeBindingsRequest,
+    ListDataAttributeBindingsResponse,
+    ListDataAttributesRequest,
+    ListDataAttributesResponse,
+    ListDataTaxonomiesRequest,
+    ListDataTaxonomiesResponse,
+    UpdateDataAttributeBindingRequest,
+    UpdateDataAttributeRequest,
+    UpdateDataTaxonomyRequest,
+)
+from google.cloud.dataplex_v1.types.datascans import (
     CreateDataScanRequest,
     DataScan,
     DataScanJob,
     DataScanType,
     DeleteDataScanRequest,
     GetDataScanJobRequest,
     GetDataScanRequest,
@@ -42,16 +103,22 @@
     ListDataScanJobsResponse,
     ListDataScansRequest,
     ListDataScansResponse,
     RunDataScanRequest,
     RunDataScanResponse,
     UpdateDataScanRequest,
 )
-from .logs import DataScanEvent, DiscoveryEvent, JobEvent, SessionEvent
-from .metadata_ import (
+from google.cloud.dataplex_v1.types.logs import (
+    DataQualityScanRuleResult,
+    DataScanEvent,
+    DiscoveryEvent,
+    JobEvent,
+    SessionEvent,
+)
+from google.cloud.dataplex_v1.types.metadata_ import (
     CreateEntityRequest,
     CreatePartitionRequest,
     DeleteEntityRequest,
     DeletePartitionRequest,
     Entity,
     GetEntityRequest,
     GetPartitionRequest,
@@ -62,17 +129,25 @@
     Partition,
     Schema,
     StorageAccess,
     StorageFormat,
     StorageSystem,
     UpdateEntityRequest,
 )
-from .processing import DataSource, ScannedData, Trigger
-from .resources import Action, Asset, AssetStatus, Lake, State, Zone
-from .service import (
+from google.cloud.dataplex_v1.types.processing import DataSource, ScannedData, Trigger
+from google.cloud.dataplex_v1.types.resources import (
+    Action,
+    Asset,
+    AssetStatus,
+    Lake,
+    State,
+    Zone,
+)
+from google.cloud.dataplex_v1.types.security import DataAccessSpec, ResourceAccessSpec
+from google.cloud.dataplex_v1.types.service import (
     CancelJobRequest,
     CreateAssetRequest,
     CreateEnvironmentRequest,
     CreateLakeRequest,
     CreateTaskRequest,
     CreateZoneRequest,
     DeleteAssetRequest,
@@ -109,17 +184,27 @@
     RunTaskResponse,
     UpdateAssetRequest,
     UpdateEnvironmentRequest,
     UpdateLakeRequest,
     UpdateTaskRequest,
     UpdateZoneRequest,
 )
-from .tasks import Job, Task
+from google.cloud.dataplex_v1.types.tasks import Job, Task
 
 __all__ = (
+    "ContentServiceClient",
+    "ContentServiceAsyncClient",
+    "DataplexServiceClient",
+    "DataplexServiceAsyncClient",
+    "DataScanServiceClient",
+    "DataScanServiceAsyncClient",
+    "DataTaxonomyServiceClient",
+    "DataTaxonomyServiceAsyncClient",
+    "MetadataServiceClient",
+    "MetadataServiceAsyncClient",
     "Content",
     "Environment",
     "Session",
     "CreateContentRequest",
     "DeleteContentRequest",
     "GetContentRequest",
     "ListContentRequest",
@@ -128,28 +213,50 @@
     "DataProfileResult",
     "DataProfileSpec",
     "DataQualityDimensionResult",
     "DataQualityResult",
     "DataQualityRule",
     "DataQualityRuleResult",
     "DataQualitySpec",
+    "CreateDataAttributeBindingRequest",
+    "CreateDataAttributeRequest",
+    "CreateDataTaxonomyRequest",
+    "DataAttribute",
+    "DataAttributeBinding",
+    "DataTaxonomy",
+    "DeleteDataAttributeBindingRequest",
+    "DeleteDataAttributeRequest",
+    "DeleteDataTaxonomyRequest",
+    "GetDataAttributeBindingRequest",
+    "GetDataAttributeRequest",
+    "GetDataTaxonomyRequest",
+    "ListDataAttributeBindingsRequest",
+    "ListDataAttributeBindingsResponse",
+    "ListDataAttributesRequest",
+    "ListDataAttributesResponse",
+    "ListDataTaxonomiesRequest",
+    "ListDataTaxonomiesResponse",
+    "UpdateDataAttributeBindingRequest",
+    "UpdateDataAttributeRequest",
+    "UpdateDataTaxonomyRequest",
     "CreateDataScanRequest",
     "DataScan",
     "DataScanJob",
     "DeleteDataScanRequest",
     "GetDataScanJobRequest",
     "GetDataScanRequest",
     "ListDataScanJobsRequest",
     "ListDataScanJobsResponse",
     "ListDataScansRequest",
     "ListDataScansResponse",
     "RunDataScanRequest",
     "RunDataScanResponse",
     "UpdateDataScanRequest",
     "DataScanType",
+    "DataQualityScanRuleResult",
     "DataScanEvent",
     "DiscoveryEvent",
     "JobEvent",
     "SessionEvent",
     "CreateEntityRequest",
     "CreatePartitionRequest",
     "DeleteEntityRequest",
@@ -172,14 +279,16 @@
     "Trigger",
     "Action",
     "Asset",
     "AssetStatus",
     "Lake",
     "Zone",
     "State",
+    "DataAccessSpec",
+    "ResourceAccessSpec",
     "CancelJobRequest",
     "CreateAssetRequest",
     "CreateEnvironmentRequest",
     "CreateLakeRequest",
     "CreateTaskRequest",
     "CreateZoneRequest",
     "DeleteAssetRequest",
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/analyze.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/analyze.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/content.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/data_profile.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/data_profile.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -27,28 +27,140 @@
         "DataProfileSpec",
         "DataProfileResult",
     },
 )
 
 
 class DataProfileSpec(proto.Message):
-    r"""DataProfileScan related setting."""
+    r"""DataProfileScan related setting.
+
+    Attributes:
+        sampling_percent (float):
+            Optional. The percentage of the records to be selected from
+            the dataset for DataScan.
+
+            -  Value can range between 0.0 and 100.0 with up to 3
+               significant decimal digits.
+            -  Sampling is not applied if ``sampling_percent`` is not
+               specified, 0 or
+
+            100.
+        row_filter (str):
+            Optional. A filter applied to all rows in a
+            single DataScan job. The filter needs to be a
+            valid SQL expression for a WHERE clause in
+            BigQuery standard SQL syntax.
+            Example: col1 >= 0 AND col2 < 10
+        post_scan_actions (google.cloud.dataplex_v1.types.DataProfileSpec.PostScanActions):
+            Optional. Actions to take upon job
+            completion..
+        include_fields (google.cloud.dataplex_v1.types.DataProfileSpec.SelectedFields):
+            Optional. The fields to include in data profile.
+
+            If not specified, all fields at the time of profile scan job
+            execution are included, except for ones listed in
+            ``exclude_fields``.
+        exclude_fields (google.cloud.dataplex_v1.types.DataProfileSpec.SelectedFields):
+            Optional. The fields to exclude from data profile.
+
+            If specified, the fields will be excluded from data profile,
+            regardless of ``include_fields`` value.
+    """
+
+    class PostScanActions(proto.Message):
+        r"""The configuration of post scan actions of DataProfileScan
+        job.
+
+        Attributes:
+            bigquery_export (google.cloud.dataplex_v1.types.DataProfileSpec.PostScanActions.BigQueryExport):
+                Optional. If set, results will be exported to
+                the provided BigQuery table.
+        """
+
+        class BigQueryExport(proto.Message):
+            r"""The configuration of BigQuery export post scan action.
+
+            Attributes:
+                results_table (str):
+                    Optional. The BigQuery table to export
+                    DataProfileScan results to. Format:
+
+                    projects/{project}/datasets/{dataset}/tables/{table}
+            """
+
+            results_table: str = proto.Field(
+                proto.STRING,
+                number=1,
+            )
+
+        bigquery_export: "DataProfileSpec.PostScanActions.BigQueryExport" = proto.Field(
+            proto.MESSAGE,
+            number=1,
+            message="DataProfileSpec.PostScanActions.BigQueryExport",
+        )
+
+    class SelectedFields(proto.Message):
+        r"""The specification for fields to include or exclude in data
+        profile scan.
+
+        Attributes:
+            field_names (MutableSequence[str]):
+                Optional. Expected input is a list of fully
+                qualified names of fields as in the schema.
+
+                Only top-level field names for nested fields are
+                supported. For instance, if 'x' is of nested
+                field type, listing 'x' is supported but 'x.y.z'
+                is not supported. Here 'y' and 'y.z' are nested
+                fields of 'x'.
+        """
+
+        field_names: MutableSequence[str] = proto.RepeatedField(
+            proto.STRING,
+            number=1,
+        )
+
+    sampling_percent: float = proto.Field(
+        proto.FLOAT,
+        number=2,
+    )
+    row_filter: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    post_scan_actions: PostScanActions = proto.Field(
+        proto.MESSAGE,
+        number=4,
+        message=PostScanActions,
+    )
+    include_fields: SelectedFields = proto.Field(
+        proto.MESSAGE,
+        number=5,
+        message=SelectedFields,
+    )
+    exclude_fields: SelectedFields = proto.Field(
+        proto.MESSAGE,
+        number=6,
+        message=SelectedFields,
+    )
 
 
 class DataProfileResult(proto.Message):
     r"""DataProfileResult defines the output of DataProfileScan. Each
     field of the table will have field type specific profile result.
 
     Attributes:
         row_count (int):
             The count of rows scanned.
         profile (google.cloud.dataplex_v1.types.DataProfileResult.Profile):
             The profile information per field.
         scanned_data (google.cloud.dataplex_v1.types.ScannedData):
             The data scanned for this result.
+        post_scan_actions_result (google.cloud.dataplex_v1.types.DataProfileResult.PostScanActionsResult):
+            Output only. The result of post scan actions.
     """
 
     class Profile(proto.Message):
         r"""Contains name, type, mode and field type specific profile
         information.
 
         Attributes:
@@ -97,20 +209,20 @@
                         scanned rows.
                     distinct_ratio (float):
                         Ratio of rows with distinct values against
                         total scanned rows. Not available for complex
                         non-groupable field type RECORD and fields with
                         REPEATABLE mode.
                     top_n_values (MutableSequence[google.cloud.dataplex_v1.types.DataProfileResult.Profile.Field.ProfileInfo.TopNValue]):
-                        The list of top N non-null values and number
-                        of times they occur in the scanned data. N is 10
-                        or equal to the number of distinct values in the
-                        field, whichever is smaller. Not available for
-                        complex non-groupable field type RECORD and
-                        fields with REPEATABLE mode.
+                        The list of top N non-null values, frequency
+                        and ratio with which they occur in the scanned
+                        data. N is 10 or equal to the number of distinct
+                        values in the field, whichever is smaller. Not
+                        available for complex non-groupable field type
+                        RECORD and fields with REPEATABLE mode.
                     string_profile (google.cloud.dataplex_v1.types.DataProfileResult.Profile.Field.ProfileInfo.StringFieldInfo):
                         String type field information.
 
                         This field is a member of `oneof`_ ``field_info``.
                     integer_profile (google.cloud.dataplex_v1.types.DataProfileResult.Profile.Field.ProfileInfo.IntegerFieldInfo):
                         Integer type field information.
 
@@ -172,17 +284,17 @@
                             the data is below this point. The second
                             quartile (Q2) is the median of a data set. So,
                             50% of the data lies below this point. The third
                             quartile (Q3) splits off the highest 25% of data
                             from the lowest 75%. It is known as the upper or
                             75th empirical quartile, as 75% of the data lies
                             below this point. Here, the quartiles is
-                            provided as an ordered list of quartile values
-                            for the scanned data, occurring in order Q1,
-                            median, Q3.
+                            provided as an ordered list of approximate
+                            quartile values for the scanned data, occurring
+                            in order Q1, median, Q3.
                         max_ (int):
                             Maximum of non-null values in the scanned
                             data. NaN, if the field has a NaN.
                     """
 
                     average: float = proto.Field(
                         proto.DOUBLE,
@@ -266,24 +378,32 @@
 
                     Attributes:
                         value (str):
                             String value of a top N non-null value.
                         count (int):
                             Count of the corresponding value in the
                             scanned data.
+                        ratio (float):
+                            Ratio of the corresponding value in the field
+                            against the total number of rows in the scanned
+                            data.
                     """
 
                     value: str = proto.Field(
                         proto.STRING,
                         number=1,
                     )
                     count: int = proto.Field(
                         proto.INT64,
                         number=2,
                     )
+                    ratio: float = proto.Field(
+                        proto.DOUBLE,
+                        number=3,
+                    )
 
                 null_ratio: float = proto.Field(
                     proto.DOUBLE,
                     number=2,
                 )
                 distinct_ratio: float = proto.Field(
                     proto.DOUBLE,
@@ -337,24 +457,87 @@
             "DataProfileResult.Profile.Field"
         ] = proto.RepeatedField(
             proto.MESSAGE,
             number=2,
             message="DataProfileResult.Profile.Field",
         )
 
+    class PostScanActionsResult(proto.Message):
+        r"""The result of post scan actions of DataProfileScan job.
+
+        Attributes:
+            bigquery_export_result (google.cloud.dataplex_v1.types.DataProfileResult.PostScanActionsResult.BigQueryExportResult):
+                Output only. The result of BigQuery export
+                post scan action.
+        """
+
+        class BigQueryExportResult(proto.Message):
+            r"""The result of BigQuery export post scan action.
+
+            Attributes:
+                state (google.cloud.dataplex_v1.types.DataProfileResult.PostScanActionsResult.BigQueryExportResult.State):
+                    Output only. Execution state for the BigQuery
+                    exporting.
+                message (str):
+                    Output only. Additional information about the
+                    BigQuery exporting.
+            """
+
+            class State(proto.Enum):
+                r"""Execution state for the exporting.
+
+                Values:
+                    STATE_UNSPECIFIED (0):
+                        The exporting state is unspecified.
+                    SUCCEEDED (1):
+                        The exporting completed successfully.
+                    FAILED (2):
+                        The exporting is no longer running due to an
+                        error.
+                    SKIPPED (3):
+                        The exporting is skipped due to no valid scan
+                        result to export (usually caused by scan
+                        failed).
+                """
+                STATE_UNSPECIFIED = 0
+                SUCCEEDED = 1
+                FAILED = 2
+                SKIPPED = 3
+
+            state: "DataProfileResult.PostScanActionsResult.BigQueryExportResult.State" = proto.Field(
+                proto.ENUM,
+                number=1,
+                enum="DataProfileResult.PostScanActionsResult.BigQueryExportResult.State",
+            )
+            message: str = proto.Field(
+                proto.STRING,
+                number=2,
+            )
+
+        bigquery_export_result: "DataProfileResult.PostScanActionsResult.BigQueryExportResult" = proto.Field(
+            proto.MESSAGE,
+            number=1,
+            message="DataProfileResult.PostScanActionsResult.BigQueryExportResult",
+        )
+
     row_count: int = proto.Field(
         proto.INT64,
         number=3,
     )
     profile: Profile = proto.Field(
         proto.MESSAGE,
         number=4,
         message=Profile,
     )
     scanned_data: processing.ScannedData = proto.Field(
         proto.MESSAGE,
         number=5,
         message=processing.ScannedData,
     )
+    post_scan_actions_result: PostScanActionsResult = proto.Field(
+        proto.MESSAGE,
+        number=6,
+        message=PostScanActionsResult,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/data_quality.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/data_quality.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -34,23 +34,87 @@
 
 
 class DataQualitySpec(proto.Message):
     r"""DataQualityScan related setting.
 
     Attributes:
         rules (MutableSequence[google.cloud.dataplex_v1.types.DataQualityRule]):
-            The list of rules to evaluate against a data
-            source. At least one rule is required.
+            Required. The list of rules to evaluate
+            against a data source. At least one rule is
+            required.
+        sampling_percent (float):
+            Optional. The percentage of the records to be selected from
+            the dataset for DataScan.
+
+            -  Value can range between 0.0 and 100.0 with up to 3
+               significant decimal digits.
+            -  Sampling is not applied if ``sampling_percent`` is not
+               specified, 0 or
+
+            100.
+        row_filter (str):
+            Optional. A filter applied to all rows in a
+            single DataScan job. The filter needs to be a
+            valid SQL expression for a WHERE clause in
+            BigQuery standard SQL syntax.
+            Example: col1 >= 0 AND col2 < 10
+        post_scan_actions (google.cloud.dataplex_v1.types.DataQualitySpec.PostScanActions):
+            Optional. Actions to take upon job
+            completion.
     """
 
+    class PostScanActions(proto.Message):
+        r"""The configuration of post scan actions of DataQualityScan.
+
+        Attributes:
+            bigquery_export (google.cloud.dataplex_v1.types.DataQualitySpec.PostScanActions.BigQueryExport):
+                Optional. If set, results will be exported to
+                the provided BigQuery table.
+        """
+
+        class BigQueryExport(proto.Message):
+            r"""The configuration of BigQuery export post scan action.
+
+            Attributes:
+                results_table (str):
+                    Optional. The BigQuery table to export
+                    DataQualityScan results to. Format:
+
+                    projects/{project}/datasets/{dataset}/tables/{table}
+            """
+
+            results_table: str = proto.Field(
+                proto.STRING,
+                number=1,
+            )
+
+        bigquery_export: "DataQualitySpec.PostScanActions.BigQueryExport" = proto.Field(
+            proto.MESSAGE,
+            number=1,
+            message="DataQualitySpec.PostScanActions.BigQueryExport",
+        )
+
     rules: MutableSequence["DataQualityRule"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="DataQualityRule",
     )
+    sampling_percent: float = proto.Field(
+        proto.FLOAT,
+        number=4,
+    )
+    row_filter: str = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+    post_scan_actions: PostScanActions = proto.Field(
+        proto.MESSAGE,
+        number=6,
+        message=PostScanActions,
+    )
 
 
 class DataQualityResult(proto.Message):
     r"""The output of a DataQualityScan.
 
     Attributes:
         passed (bool):
@@ -60,16 +124,76 @@
         rules (MutableSequence[google.cloud.dataplex_v1.types.DataQualityRuleResult]):
             A list of all the rules in a job, and their
             results.
         row_count (int):
             The count of rows processed.
         scanned_data (google.cloud.dataplex_v1.types.ScannedData):
             The data scanned for this result.
+        post_scan_actions_result (google.cloud.dataplex_v1.types.DataQualityResult.PostScanActionsResult):
+            Output only. The result of post scan actions.
     """
 
+    class PostScanActionsResult(proto.Message):
+        r"""The result of post scan actions of DataQualityScan job.
+
+        Attributes:
+            bigquery_export_result (google.cloud.dataplex_v1.types.DataQualityResult.PostScanActionsResult.BigQueryExportResult):
+                Output only. The result of BigQuery export
+                post scan action.
+        """
+
+        class BigQueryExportResult(proto.Message):
+            r"""The result of BigQuery export post scan action.
+
+            Attributes:
+                state (google.cloud.dataplex_v1.types.DataQualityResult.PostScanActionsResult.BigQueryExportResult.State):
+                    Output only. Execution state for the BigQuery
+                    exporting.
+                message (str):
+                    Output only. Additional information about the
+                    BigQuery exporting.
+            """
+
+            class State(proto.Enum):
+                r"""Execution state for the exporting.
+
+                Values:
+                    STATE_UNSPECIFIED (0):
+                        The exporting state is unspecified.
+                    SUCCEEDED (1):
+                        The exporting completed successfully.
+                    FAILED (2):
+                        The exporting is no longer running due to an
+                        error.
+                    SKIPPED (3):
+                        The exporting is skipped due to no valid scan
+                        result to export (usually caused by scan
+                        failed).
+                """
+                STATE_UNSPECIFIED = 0
+                SUCCEEDED = 1
+                FAILED = 2
+                SKIPPED = 3
+
+            state: "DataQualityResult.PostScanActionsResult.BigQueryExportResult.State" = proto.Field(
+                proto.ENUM,
+                number=1,
+                enum="DataQualityResult.PostScanActionsResult.BigQueryExportResult.State",
+            )
+            message: str = proto.Field(
+                proto.STRING,
+                number=2,
+            )
+
+        bigquery_export_result: "DataQualityResult.PostScanActionsResult.BigQueryExportResult" = proto.Field(
+            proto.MESSAGE,
+            number=1,
+            message="DataQualityResult.PostScanActionsResult.BigQueryExportResult",
+        )
+
     passed: bool = proto.Field(
         proto.BOOL,
         number=5,
     )
     dimensions: MutableSequence["DataQualityDimensionResult"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
@@ -85,49 +209,58 @@
         number=4,
     )
     scanned_data: processing.ScannedData = proto.Field(
         proto.MESSAGE,
         number=7,
         message=processing.ScannedData,
     )
+    post_scan_actions_result: PostScanActionsResult = proto.Field(
+        proto.MESSAGE,
+        number=8,
+        message=PostScanActionsResult,
+    )
 
 
 class DataQualityRuleResult(proto.Message):
     r"""DataQualityRuleResult provides a more detailed, per-rule view
     of the results.
 
     Attributes:
         rule (google.cloud.dataplex_v1.types.DataQualityRule):
             The rule specified in the DataQualitySpec, as
             is.
         passed (bool):
             Whether the rule passed or failed.
         evaluated_count (int):
-            The number of rows a rule was evaluated against. This field
-            is only valid for ColumnMap type rules.
+            The number of rows a rule was evaluated against.
+
+            This field is only valid for row-level type rules.
 
             Evaluated count can be configured to either
 
             -  include all rows (default) - with ``null`` rows
                automatically failing rule evaluation, or
             -  exclude ``null`` rows from the ``evaluated_count``, by
                setting ``ignore_nulls = true``.
         passed_count (int):
             The number of rows which passed a rule
-            evaluation. This field is only valid for
-            ColumnMap type rules.
+            evaluation.
+            This field is only valid for row-level type
+            rules.
         null_count (int):
             The number of rows with null values in the
             specified column.
         pass_ratio (float):
-            The ratio of **passed_count / evaluated_count**. This field
-            is only valid for ColumnMap type rules.
+            The ratio of **passed_count / evaluated_count**.
+
+            This field is only valid for row-level type rules.
         failing_rows_query (str):
             The query to find rows that did not pass this
-            rule. Only applies to ColumnMap and RowCondition
+            rule.
+            This field is only valid for row-level type
             rules.
     """
 
     rule: "DataQualityRule" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="DataQualityRule",
@@ -181,73 +314,87 @@
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         range_expectation (google.cloud.dataplex_v1.types.DataQualityRule.RangeExpectation):
-            ColumnMap rule which evaluates whether each
+            Row-level rule which evaluates whether each
             column value lies between a specified range.
 
             This field is a member of `oneof`_ ``rule_type``.
         non_null_expectation (google.cloud.dataplex_v1.types.DataQualityRule.NonNullExpectation):
-            ColumnMap rule which evaluates whether each
+            Row-level rule which evaluates whether each
             column value is null.
 
             This field is a member of `oneof`_ ``rule_type``.
         set_expectation (google.cloud.dataplex_v1.types.DataQualityRule.SetExpectation):
-            ColumnMap rule which evaluates whether each
+            Row-level rule which evaluates whether each
             column value is contained by a specified set.
 
             This field is a member of `oneof`_ ``rule_type``.
         regex_expectation (google.cloud.dataplex_v1.types.DataQualityRule.RegexExpectation):
-            ColumnMap rule which evaluates whether each
+            Row-level rule which evaluates whether each
             column value matches a specified regex.
 
             This field is a member of `oneof`_ ``rule_type``.
         uniqueness_expectation (google.cloud.dataplex_v1.types.DataQualityRule.UniquenessExpectation):
-            ColumnAggregate rule which evaluates whether
-            the column has duplicates.
+            Row-level rule which evaluates whether each
+            column value is unique.
 
             This field is a member of `oneof`_ ``rule_type``.
         statistic_range_expectation (google.cloud.dataplex_v1.types.DataQualityRule.StatisticRangeExpectation):
-            ColumnAggregate rule which evaluates whether
-            the column aggregate statistic lies between a
+            Aggregate rule which evaluates whether the
+            column aggregate statistic lies between a
             specified range.
 
             This field is a member of `oneof`_ ``rule_type``.
         row_condition_expectation (google.cloud.dataplex_v1.types.DataQualityRule.RowConditionExpectation):
-            Table rule which evaluates whether each row
-            passes the specified condition.
+            Row-level rule which evaluates whether each
+            row in a table passes the specified condition.
 
             This field is a member of `oneof`_ ``rule_type``.
         table_condition_expectation (google.cloud.dataplex_v1.types.DataQualityRule.TableConditionExpectation):
-            Table rule which evaluates whether the
-            provided expression is true.
+            Aggregate rule which evaluates whether the
+            provided expression is true for a table.
 
             This field is a member of `oneof`_ ``rule_type``.
         column (str):
             Optional. The unnested column which this rule
             is evaluated against.
         ignore_null (bool):
             Optional. Rows with ``null`` values will automatically fail
             a rule, unless ``ignore_null`` is ``true``. In that case,
             such ``null`` rows are trivially considered passing.
 
-            Only applicable to ColumnMap rules.
+            This field is only valid for row-level type rules.
         dimension (str):
             Required. The dimension a rule belongs to. Results are also
             aggregated at the dimension level. Supported dimensions are
             **["COMPLETENESS", "ACCURACY", "CONSISTENCY", "VALIDITY",
             "UNIQUENESS", "INTEGRITY"]**
         threshold (float):
             Optional. The minimum ratio of **passing_rows / total_rows**
             required to pass this rule, with a range of [0.0, 1.0].
 
             0 indicates default value (i.e. 1.0).
+
+            This field is only valid for row-level type rules.
+        name (str):
+            Optional. A mutable name for the rule.
+
+            -  The name must contain only letters (a-z, A-Z), numbers
+               (0-9), or hyphens (-).
+            -  The maximum length is 63 characters.
+            -  Must start with a letter.
+            -  Must end with a number or a letter.
+        description (str):
+            Optional. Description of the rule.
+
+            -  The maximum length is 1,024 characters.
     """
 
     class RangeExpectation(proto.Message):
         r"""Evaluates whether each column value lies between a specified
         range.
 
         Attributes:
@@ -295,30 +442,31 @@
 
     class SetExpectation(proto.Message):
         r"""Evaluates whether each column value is contained by a
         specified set.
 
         Attributes:
             values (MutableSequence[str]):
-                Expected values for the column value.
+                Optional. Expected values for the column
+                value.
         """
 
         values: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=1,
         )
 
     class RegexExpectation(proto.Message):
         r"""Evaluates whether each column value matches a specified
         regex.
 
         Attributes:
             regex (str):
-                A regular expression the column value is
-                expected to match.
+                Optional. A regular expression the column
+                value is expected to match.
         """
 
         regex: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
@@ -327,36 +475,36 @@
 
     class StatisticRangeExpectation(proto.Message):
         r"""Evaluates whether the column aggregate statistic lies between
         a specified range.
 
         Attributes:
             statistic (google.cloud.dataplex_v1.types.DataQualityRule.StatisticRangeExpectation.ColumnStatistic):
-                The aggregate metric to evaluate.
+                Optional. The aggregate metric to evaluate.
             min_value (str):
-                The minimum column statistic value allowed for a row to pass
-                this validation.
+                Optional. The minimum column statistic value allowed for a
+                row to pass this validation.
 
                 At least one of ``min_value`` and ``max_value`` need to be
                 provided.
             max_value (str):
-                The maximum column statistic value allowed for a row to pass
-                this validation.
+                Optional. The maximum column statistic value allowed for a
+                row to pass this validation.
 
                 At least one of ``min_value`` and ``max_value`` need to be
                 provided.
             strict_min_enabled (bool):
-                Whether column statistic needs to be strictly greater than
-                ('>') the minimum, or if equality is allowed.
+                Optional. Whether column statistic needs to be strictly
+                greater than ('>') the minimum, or if equality is allowed.
 
                 Only relevant if a ``min_value`` has been defined. Default =
                 false.
             strict_max_enabled (bool):
-                Whether column statistic needs to be strictly lesser than
-                ('<') the maximum, or if equality is allowed.
+                Optional. Whether column statistic needs to be strictly
+                lesser than ('<') the maximum, or if equality is allowed.
 
                 Only relevant if a ``max_value`` has been defined. Default =
                 false.
         """
 
         class ColumnStatistic(proto.Enum):
             r"""The list of aggregate metrics a rule can be evaluated
@@ -406,15 +554,15 @@
         The SQL expression needs to use BigQuery standard SQL syntax and
         should produce a boolean value per row as the result.
 
         Example: col1 >= 0 AND col2 < 10
 
         Attributes:
             sql_expression (str):
-                The SQL expression.
+                Optional. The SQL expression.
         """
 
         sql_expression: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
@@ -423,15 +571,15 @@
         The SQL expression needs to use BigQuery standard SQL syntax and
         should produce a scalar boolean result.
 
         Example: MIN(col1) >= 0
 
         Attributes:
             sql_expression (str):
-                The SQL expression.
+                Optional. The SQL expression.
         """
 
         sql_expression: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
@@ -495,10 +643,18 @@
         proto.STRING,
         number=502,
     )
     threshold: float = proto.Field(
         proto.DOUBLE,
         number=503,
     )
+    name: str = proto.Field(
+        proto.STRING,
+        number=504,
+    )
+    description: str = proto.Field(
+        proto.STRING,
+        number=505,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/datascans.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/datascans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -371,28 +371,52 @@
             values above 1000 will be coerced to 1000.
         page_token (str):
             Optional. Page token received from a previous
             ``ListDataScanJobs`` call. Provide this to retrieve the
             subsequent page. When paginating, all other parameters
             provided to ``ListDataScanJobs`` must match the call that
             provided the page token.
+        filter (str):
+            Optional. An expression for filtering the results of the
+            ListDataScanJobs request.
+
+            If unspecified, all datascan jobs will be returned. Multiple
+            filters can be applied (with ``AND``, ``OR`` logical
+            operators). Filters are case-sensitive.
+
+            Allowed fields are:
+
+            -  ``start_time``
+            -  ``end_time``
+
+            ``start_time`` and ``end_time`` expect RFC-3339 formatted
+            strings (e.g. 2018-10-08T18:30:00-07:00).
+
+            For instance, 'start_time > 2018-10-08T00:00:00.123456789Z
+            AND end_time < 2018-10-09T00:00:00.123456789Z' limits
+            results to DataScanJobs between specified start and end
+            times.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     page_size: int = proto.Field(
         proto.INT32,
         number=2,
     )
     page_token: str = proto.Field(
         proto.STRING,
         number=3,
     )
+    filter: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
 
 
 class ListDataScanJobsResponse(proto.Message):
     r"""List DataScanJobs response.
 
     Attributes:
         data_scan_jobs (MutableSequence[google.cloud.dataplex_v1.types.DataScanJob]):
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/logs.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/logs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,14 +24,15 @@
 __protobuf__ = proto.module(
     package="google.cloud.dataplex.v1",
     manifest={
         "DiscoveryEvent",
         "JobEvent",
         "SessionEvent",
         "DataScanEvent",
+        "DataQualityScanRuleResult",
     },
 )
 
 
 class DiscoveryEvent(proto.Message):
     r"""The payload associated with Discovery data processing.
 
@@ -288,14 +289,16 @@
             The number of retries.
         type_ (google.cloud.dataplex_v1.types.JobEvent.Type):
             The type of the job.
         service (google.cloud.dataplex_v1.types.JobEvent.Service):
             The service used to execute the job.
         service_job (str):
             The reference to the job within the service.
+        execution_trigger (google.cloud.dataplex_v1.types.JobEvent.ExecutionTrigger):
+            Job execution trigger.
     """
 
     class Type(proto.Enum):
         r"""The type of the job.
 
         Values:
             TYPE_UNSPECIFIED (0):
@@ -339,14 +342,31 @@
                 Unspecified service.
             DATAPROC (1):
                 Cloud Dataproc.
         """
         SERVICE_UNSPECIFIED = 0
         DATAPROC = 1
 
+    class ExecutionTrigger(proto.Enum):
+        r"""Job Execution trigger.
+
+        Values:
+            EXECUTION_TRIGGER_UNSPECIFIED (0):
+                The job execution trigger is unspecified.
+            TASK_CONFIG (1):
+                The job was triggered by Dataplex based on
+                trigger spec from task definition.
+            RUN_REQUEST (2):
+                The job was triggered by the explicit call of
+                Task API.
+        """
+        EXECUTION_TRIGGER_UNSPECIFIED = 0
+        TASK_CONFIG = 1
+        RUN_REQUEST = 2
+
     message: str = proto.Field(
         proto.STRING,
         number=1,
     )
     job_id: str = proto.Field(
         proto.STRING,
         number=2,
@@ -380,14 +400,19 @@
         number=8,
         enum=Service,
     )
     service_job: str = proto.Field(
         proto.STRING,
         number=9,
     )
+    execution_trigger: ExecutionTrigger = proto.Field(
+        proto.ENUM,
+        number=11,
+        enum=ExecutionTrigger,
+    )
 
 
 class SessionEvent(proto.Message):
     r"""These messages contain information about sessions within an
     environment. The monitored resource is 'Environment'.
 
 
@@ -539,28 +564,31 @@
         message=duration_pb2.Duration,
     )
 
 
 class DataScanEvent(proto.Message):
     r"""These messages contain information about the execution of a
     datascan. The monitored resource is 'DataScan'
+    Next ID: 13
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         data_source (str):
             The data source of the data scan
         job_id (str):
             The identifier of the specific data scan job
             this log entry is for.
+        create_time (google.protobuf.timestamp_pb2.Timestamp):
+            The time when the data scan job was created.
         start_time (google.protobuf.timestamp_pb2.Timestamp):
             The time when the data scan job started to
             run.
         end_time (google.protobuf.timestamp_pb2.Timestamp):
             The time when the data scan job finished.
         type_ (google.cloud.dataplex_v1.types.DataScanEvent.ScanType):
             The type of the data scan.
@@ -583,14 +611,26 @@
 
             This field is a member of `oneof`_ ``result``.
         data_quality (google.cloud.dataplex_v1.types.DataScanEvent.DataQualityResult):
             Data quality result for data quality type
             data scan.
 
             This field is a member of `oneof`_ ``result``.
+        data_profile_configs (google.cloud.dataplex_v1.types.DataScanEvent.DataProfileAppliedConfigs):
+            Applied configs for data profile type data
+            scan.
+
+            This field is a member of `oneof`_ ``appliedConfigs``.
+        data_quality_configs (google.cloud.dataplex_v1.types.DataScanEvent.DataQualityAppliedConfigs):
+            Applied configs for data quality type data
+            scan.
+
+            This field is a member of `oneof`_ ``appliedConfigs``.
+        post_scan_actions_result (google.cloud.dataplex_v1.types.DataScanEvent.PostScanActionsResult):
+            The result of post scan actions.
     """
 
     class ScanType(proto.Enum):
         r"""The type of the data scan.
 
         Values:
             SCAN_TYPE_UNSPECIFIED (0):
@@ -607,27 +647,30 @@
     class State(proto.Enum):
         r"""The job state of the data scan.
 
         Values:
             STATE_UNSPECIFIED (0):
                 Unspecified job state.
             STARTED (1):
-                Data scan started.
+                Data scan job started.
             SUCCEEDED (2):
-                Data scan successfully completed.
+                Data scan job successfully completed.
             FAILED (3):
-                Data scan was unsuccessful.
+                Data scan job was unsuccessful.
             CANCELLED (4):
-                Data scan was cancelled.
+                Data scan job was cancelled.
+            CREATED (5):
+                Data scan job was createed.
         """
         STATE_UNSPECIFIED = 0
         STARTED = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLED = 4
+        CREATED = 5
 
     class Trigger(proto.Enum):
         r"""The trigger type for the data scan.
 
         Values:
             TRIGGER_UNSPECIFIED (0):
                 An unspecified trigger type.
@@ -695,22 +738,139 @@
         )
         dimension_passed: MutableMapping[str, bool] = proto.MapField(
             proto.STRING,
             proto.BOOL,
             number=3,
         )
 
+    class DataProfileAppliedConfigs(proto.Message):
+        r"""Applied configs for data profile type data scan job.
+
+        Attributes:
+            sampling_percent (float):
+                The percentage of the records selected from the dataset for
+                DataScan.
+
+                -  Value ranges between 0.0 and 100.0.
+                -  Value 0.0 or 100.0 imply that sampling was not applied.
+            row_filter_applied (bool):
+                Boolean indicating whether a row filter was
+                applied in the DataScan job.
+            column_filter_applied (bool):
+                Boolean indicating whether a column filter
+                was applied in the DataScan job.
+        """
+
+        sampling_percent: float = proto.Field(
+            proto.FLOAT,
+            number=1,
+        )
+        row_filter_applied: bool = proto.Field(
+            proto.BOOL,
+            number=2,
+        )
+        column_filter_applied: bool = proto.Field(
+            proto.BOOL,
+            number=3,
+        )
+
+    class DataQualityAppliedConfigs(proto.Message):
+        r"""Applied configs for data quality type data scan job.
+
+        Attributes:
+            sampling_percent (float):
+                The percentage of the records selected from the dataset for
+                DataScan.
+
+                -  Value ranges between 0.0 and 100.0.
+                -  Value 0.0 or 100.0 imply that sampling was not applied.
+            row_filter_applied (bool):
+                Boolean indicating whether a row filter was
+                applied in the DataScan job.
+        """
+
+        sampling_percent: float = proto.Field(
+            proto.FLOAT,
+            number=1,
+        )
+        row_filter_applied: bool = proto.Field(
+            proto.BOOL,
+            number=2,
+        )
+
+    class PostScanActionsResult(proto.Message):
+        r"""Post scan actions result for data scan job.
+
+        Attributes:
+            bigquery_export_result (google.cloud.dataplex_v1.types.DataScanEvent.PostScanActionsResult.BigQueryExportResult):
+                The result of BigQuery export post scan
+                action.
+        """
+
+        class BigQueryExportResult(proto.Message):
+            r"""The result of BigQuery export post scan action.
+
+            Attributes:
+                state (google.cloud.dataplex_v1.types.DataScanEvent.PostScanActionsResult.BigQueryExportResult.State):
+                    Execution state for the BigQuery exporting.
+                message (str):
+                    Additional information about the BigQuery
+                    exporting.
+            """
+
+            class State(proto.Enum):
+                r"""Execution state for the exporting.
+
+                Values:
+                    STATE_UNSPECIFIED (0):
+                        The exporting state is unspecified.
+                    SUCCEEDED (1):
+                        The exporting completed successfully.
+                    FAILED (2):
+                        The exporting is no longer running due to an
+                        error.
+                    SKIPPED (3):
+                        The exporting is skipped due to no valid scan
+                        result to export (usually caused by scan
+                        failed).
+                """
+                STATE_UNSPECIFIED = 0
+                SUCCEEDED = 1
+                FAILED = 2
+                SKIPPED = 3
+
+            state: "DataScanEvent.PostScanActionsResult.BigQueryExportResult.State" = proto.Field(
+                proto.ENUM,
+                number=1,
+                enum="DataScanEvent.PostScanActionsResult.BigQueryExportResult.State",
+            )
+            message: str = proto.Field(
+                proto.STRING,
+                number=2,
+            )
+
+        bigquery_export_result: "DataScanEvent.PostScanActionsResult.BigQueryExportResult" = proto.Field(
+            proto.MESSAGE,
+            number=1,
+            message="DataScanEvent.PostScanActionsResult.BigQueryExportResult",
+        )
+
     data_source: str = proto.Field(
         proto.STRING,
         number=1,
     )
     job_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
+    create_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=12,
+        message=timestamp_pb2.Timestamp,
+    )
     start_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
     end_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
@@ -753,10 +913,191 @@
     )
     data_quality: DataQualityResult = proto.Field(
         proto.MESSAGE,
         number=102,
         oneof="result",
         message=DataQualityResult,
     )
+    data_profile_configs: DataProfileAppliedConfigs = proto.Field(
+        proto.MESSAGE,
+        number=201,
+        oneof="appliedConfigs",
+        message=DataProfileAppliedConfigs,
+    )
+    data_quality_configs: DataQualityAppliedConfigs = proto.Field(
+        proto.MESSAGE,
+        number=202,
+        oneof="appliedConfigs",
+        message=DataQualityAppliedConfigs,
+    )
+    post_scan_actions_result: PostScanActionsResult = proto.Field(
+        proto.MESSAGE,
+        number=11,
+        message=PostScanActionsResult,
+    )
+
+
+class DataQualityScanRuleResult(proto.Message):
+    r"""Information about the result of a data quality rule for data
+    quality scan. The monitored resource is 'DataScan'.
+
+    Attributes:
+        job_id (str):
+            Identifier of the specific data scan job this
+            log entry is for.
+        data_source (str):
+            The data source of the data scan (e.g.
+            BigQuery table name).
+        column (str):
+            The column which this rule is evaluated
+            against.
+        rule_name (str):
+            The name of the data quality rule.
+        rule_type (google.cloud.dataplex_v1.types.DataQualityScanRuleResult.RuleType):
+            The type of the data quality rule.
+        evalution_type (google.cloud.dataplex_v1.types.DataQualityScanRuleResult.EvaluationType):
+            The evaluation type of the data quality rule.
+        rule_dimension (str):
+            The dimension of the data quality rule.
+        threshold_percent (float):
+            The passing threshold ([0.0, 100.0]) of the data quality
+            rule.
+        result (google.cloud.dataplex_v1.types.DataQualityScanRuleResult.Result):
+            The result of the data quality rule.
+        evaluated_row_count (int):
+            The number of rows evaluated against the data quality rule.
+            This field is only valid for rules of PER_ROW evaluation
+            type.
+        passed_row_count (int):
+            The number of rows which passed a rule evaluation. This
+            field is only valid for rules of PER_ROW evaluation type.
+        null_row_count (int):
+            The number of rows with null values in the
+            specified column.
+    """
+
+    class RuleType(proto.Enum):
+        r"""The type of the data quality rule.
+
+        Values:
+            RULE_TYPE_UNSPECIFIED (0):
+                An unspecified rule type.
+            NON_NULL_EXPECTATION (1):
+                Please see
+                https://cloud.google.com/dataplex/docs/reference/rest/v1/DataQualityRule#nonnullexpectation.
+            RANGE_EXPECTATION (2):
+                Please see
+                https://cloud.google.com/dataplex/docs/reference/rest/v1/DataQualityRule#rangeexpectation.
+            REGEX_EXPECTATION (3):
+                Please see
+                https://cloud.google.com/dataplex/docs/reference/rest/v1/DataQualityRule#regexexpectation.
+            ROW_CONDITION_EXPECTATION (4):
+                Please see
+                https://cloud.google.com/dataplex/docs/reference/rest/v1/DataQualityRule#rowconditionexpectation.
+            SET_EXPECTATION (5):
+                Please see
+                https://cloud.google.com/dataplex/docs/reference/rest/v1/DataQualityRule#setexpectation.
+            STATISTIC_RANGE_EXPECTATION (6):
+                Please see
+                https://cloud.google.com/dataplex/docs/reference/rest/v1/DataQualityRule#statisticrangeexpectation.
+            TABLE_CONDITION_EXPECTATION (7):
+                Please see
+                https://cloud.google.com/dataplex/docs/reference/rest/v1/DataQualityRule#tableconditionexpectation.
+            UNIQUENESS_EXPECTATION (8):
+                Please see
+                https://cloud.google.com/dataplex/docs/reference/rest/v1/DataQualityRule#uniquenessexpectation.
+        """
+        RULE_TYPE_UNSPECIFIED = 0
+        NON_NULL_EXPECTATION = 1
+        RANGE_EXPECTATION = 2
+        REGEX_EXPECTATION = 3
+        ROW_CONDITION_EXPECTATION = 4
+        SET_EXPECTATION = 5
+        STATISTIC_RANGE_EXPECTATION = 6
+        TABLE_CONDITION_EXPECTATION = 7
+        UNIQUENESS_EXPECTATION = 8
+
+    class EvaluationType(proto.Enum):
+        r"""The evaluation type of the data quality rule.
+
+        Values:
+            EVALUATION_TYPE_UNSPECIFIED (0):
+                An unspecified evaluation type.
+            PER_ROW (1):
+                The rule evaluation is done at per row level.
+            AGGREGATE (2):
+                The rule evaluation is done for an aggregate
+                of rows.
+        """
+        EVALUATION_TYPE_UNSPECIFIED = 0
+        PER_ROW = 1
+        AGGREGATE = 2
+
+    class Result(proto.Enum):
+        r"""Whether the data quality rule passed or failed.
+
+        Values:
+            RESULT_UNSPECIFIED (0):
+                An unspecified result.
+            PASSED (1):
+                The data quality rule passed.
+            FAILED (2):
+                The data quality rule failed.
+        """
+        RESULT_UNSPECIFIED = 0
+        PASSED = 1
+        FAILED = 2
+
+    job_id: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    data_source: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    column: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    rule_name: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    rule_type: RuleType = proto.Field(
+        proto.ENUM,
+        number=5,
+        enum=RuleType,
+    )
+    evalution_type: EvaluationType = proto.Field(
+        proto.ENUM,
+        number=6,
+        enum=EvaluationType,
+    )
+    rule_dimension: str = proto.Field(
+        proto.STRING,
+        number=7,
+    )
+    threshold_percent: float = proto.Field(
+        proto.DOUBLE,
+        number=8,
+    )
+    result: Result = proto.Field(
+        proto.ENUM,
+        number=9,
+        enum=Result,
+    )
+    evaluated_row_count: int = proto.Field(
+        proto.INT64,
+        number=10,
+    )
+    passed_row_count: int = proto.Field(
+        proto.INT64,
+        number=11,
+    )
+    null_row_count: int = proto.Field(
+        proto.INT64,
+        number=12,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/metadata_.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/metadata_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -948,14 +948,15 @@
             Optional. The compression type associated
             with the stored data. If unspecified, the data
             is uncompressed.
         mime_type (str):
             Required. The mime type descriptor for the
             data. Must match the pattern {type}/{subtype}.
             Supported values:
+
             - application/x-parquet
             - application/x-avro
             - application/x-orc
             - application/x-tfrecord
             - application/x-parquet+iceberg
             - application/x-avro+iceberg
             - application/x-orc+iceberg
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/processing.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/resources.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/service.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1000,20 +1000,54 @@
 class RunTaskRequest(proto.Message):
     r"""
 
     Attributes:
         name (str):
             Required. The resource name of the task:
             ``projects/{project_number}/locations/{location_id}/lakes/{lake_id}/tasks/{task_id}``.
+        labels (MutableMapping[str, str]):
+            Optional. User-defined labels for the task.
+            If the map is left empty, the task will run with
+            existing labels from task definition. If the map
+            contains an entry with a new key, the same will
+            be added to existing set of labels. If the map
+            contains an entry with an existing label key in
+            task definition, the task will run with new
+            label value for that entry. Clearing an existing
+            label will require label value to be explicitly
+            set to a hyphen "-". The label value cannot be
+            empty.
+        args (MutableMapping[str, str]):
+            Optional. Execution spec arguments. If the
+            map is left empty, the task will run with
+            existing execution spec args from task
+            definition. If the map contains an entry with a
+            new key, the same will be added to existing set
+            of args. If the map contains an entry with an
+            existing arg key in task definition, the task
+            will run with new arg value for that entry.
+            Clearing an existing arg will require arg value
+            to be explicitly set to a hyphen "-". The arg
+            value cannot be empty.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
+    labels: MutableMapping[str, str] = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=3,
+    )
+    args: MutableMapping[str, str] = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=4,
+    )
 
 
 class RunTaskResponse(proto.Message):
     r"""
 
     Attributes:
         job (google.cloud.dataplex_v1.types.Job):
```

### Comparing `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/tasks.py` & `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -623,14 +623,22 @@
             job.
         service_job (str):
             Output only. The full resource name for the
             job run under a particular service.
         message (str):
             Output only. Additional information about the
             current state.
+        labels (MutableMapping[str, str]):
+            Output only. User-defined labels for the
+            task.
+        trigger (google.cloud.dataplex_v1.types.Job.Trigger):
+            Output only. Job execution trigger.
+        execution_spec (google.cloud.dataplex_v1.types.Task.ExecutionSpec):
+            Output only. Spec related to how a task is
+            executed.
     """
 
     class Service(proto.Enum):
         r"""
 
         Values:
             SERVICE_UNSPECIFIED (0):
@@ -664,14 +672,31 @@
         RUNNING = 1
         CANCELLING = 2
         CANCELLED = 3
         SUCCEEDED = 4
         FAILED = 5
         ABORTED = 6
 
+    class Trigger(proto.Enum):
+        r"""Job execution trigger.
+
+        Values:
+            TRIGGER_UNSPECIFIED (0):
+                The trigger is unspecified.
+            TASK_CONFIG (1):
+                The job was triggered by Dataplex based on
+                trigger spec from task definition.
+            RUN_REQUEST (2):
+                The job was triggered by the explicit call of
+                Task API.
+        """
+        TRIGGER_UNSPECIFIED = 0
+        TASK_CONFIG = 1
+        RUN_REQUEST = 2
+
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     uid: str = proto.Field(
         proto.STRING,
         number=2,
@@ -704,10 +729,25 @@
         proto.STRING,
         number=8,
     )
     message: str = proto.Field(
         proto.STRING,
         number=9,
     )
+    labels: MutableMapping[str, str] = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=10,
+    )
+    trigger: Trigger = proto.Field(
+        proto.ENUM,
+        number=11,
+        enum=Trigger,
+    )
+    execution_spec: "Task.ExecutionSpec" = proto.Field(
+        proto.MESSAGE,
+        number=100,
+        message="Task.ExecutionSpec",
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/PKG-INFO` & `google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataplex
-Version: 1.5.1
+Version: 1.6.0
 Summary: Google Cloud Dataplex API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Cloud Dataplex.:  https://cloud.google.com/dataplex
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
-Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
+creates isolated Python environments. These isolated environments can have separate
+versions of Python packages, which allows you to isolate one project's dependencies
+from the dependencies of other projects.
 
-With `virtualenv`_, it's possible to install this library without needing system
+With `venv`_, it's possible to install this library without needing system
 install permissions, and without clashing with the installed system
 dependencies.
 
-.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
+.. _`venv`: https://docs.python.org/3/library/venv.html
 
 
 Code samples and snippets
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Code samples and snippets live in the `samples/` folder.
+Code samples and snippets live in the `samples/`_ folder.
+
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-dataplex/samples
 
 
 Supported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
 Python.
 
@@ -97,29 +100,27 @@
 .. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
+    python3 -m venv <your-env>
     source <your-env>/bin/activate
-    <your-env>/bin/pip install google-cloud-dataplex
+    pip install google-cloud-dataplex
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-dataplex
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-dataplex
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Cloud Dataplex
    to see other available methods on the client.
 -  Read the `Cloud Dataplex Product documentation`_ to learn
```

### Comparing `google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/SOURCES.txt` & `google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,22 @@
 google/cloud/dataplex_v1/services/data_scan_service/async_client.py
 google/cloud/dataplex_v1/services/data_scan_service/client.py
 google/cloud/dataplex_v1/services/data_scan_service/pagers.py
 google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py
 google/cloud/dataplex_v1/services/data_scan_service/transports/base.py
 google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py
 google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py
+google/cloud/dataplex_v1/services/data_taxonomy_service/__init__.py
+google/cloud/dataplex_v1/services/data_taxonomy_service/async_client.py
+google/cloud/dataplex_v1/services/data_taxonomy_service/client.py
+google/cloud/dataplex_v1/services/data_taxonomy_service/pagers.py
+google/cloud/dataplex_v1/services/data_taxonomy_service/transports/__init__.py
+google/cloud/dataplex_v1/services/data_taxonomy_service/transports/base.py
+google/cloud/dataplex_v1/services/data_taxonomy_service/transports/grpc.py
+google/cloud/dataplex_v1/services/data_taxonomy_service/transports/grpc_asyncio.py
 google/cloud/dataplex_v1/services/dataplex_service/__init__.py
 google/cloud/dataplex_v1/services/dataplex_service/async_client.py
 google/cloud/dataplex_v1/services/dataplex_service/client.py
 google/cloud/dataplex_v1/services/dataplex_service/pagers.py
 google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py
 google/cloud/dataplex_v1/services/dataplex_service/transports/base.py
 google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py
@@ -44,19 +52,21 @@
 google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py
 google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py
 google/cloud/dataplex_v1/types/__init__.py
 google/cloud/dataplex_v1/types/analyze.py
 google/cloud/dataplex_v1/types/content.py
 google/cloud/dataplex_v1/types/data_profile.py
 google/cloud/dataplex_v1/types/data_quality.py
+google/cloud/dataplex_v1/types/data_taxonomy.py
 google/cloud/dataplex_v1/types/datascans.py
 google/cloud/dataplex_v1/types/logs.py
 google/cloud/dataplex_v1/types/metadata_.py
 google/cloud/dataplex_v1/types/processing.py
 google/cloud/dataplex_v1/types/resources.py
+google/cloud/dataplex_v1/types/security.py
 google/cloud/dataplex_v1/types/service.py
 google/cloud/dataplex_v1/types/tasks.py
 google_cloud_dataplex.egg-info/PKG-INFO
 google_cloud_dataplex.egg-info/SOURCES.txt
 google_cloud_dataplex.egg-info/dependency_links.txt
 google_cloud_dataplex.egg-info/namespace_packages.txt
 google_cloud_dataplex.egg-info/not-zip-safe
@@ -64,9 +74,10 @@
 google_cloud_dataplex.egg-info/top_level.txt
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
 tests/unit/gapic/dataplex_v1/__init__.py
 tests/unit/gapic/dataplex_v1/test_content_service.py
 tests/unit/gapic/dataplex_v1/test_data_scan_service.py
+tests/unit/gapic/dataplex_v1/test_data_taxonomy_service.py
 tests/unit/gapic/dataplex_v1/test_dataplex_service.py
 tests/unit/gapic/dataplex_v1/test_metadata_service.py
```

### Comparing `google-cloud-dataplex-1.5.1/setup.py` & `google-cloud-dataplex-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/tests/__init__.py` & `google-cloud-dataplex-1.6.0/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/tests/unit/__init__.py` & `google-cloud-dataplex-1.6.0/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/tests/unit/gapic/__init__.py` & `google-cloud-dataplex-1.6.0/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/__init__.py` & `google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_content_service.py` & `google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_content_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_data_scan_service.py` & `google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_data_scan_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -3650,109 +3650,135 @@
     path = DataScanServiceClient.entity_path(**expected)
 
     # Check that the path construction is reversible.
     actual = DataScanServiceClient.parse_entity_path(path)
     assert expected == actual
 
 
+def test_table_path():
+    project = "squid"
+    dataset = "clam"
+    table = "whelk"
+    expected = "projects/{project}/datasets/{dataset}/tables/{table}".format(
+        project=project,
+        dataset=dataset,
+        table=table,
+    )
+    actual = DataScanServiceClient.table_path(project, dataset, table)
+    assert expected == actual
+
+
+def test_parse_table_path():
+    expected = {
+        "project": "octopus",
+        "dataset": "oyster",
+        "table": "nudibranch",
+    }
+    path = DataScanServiceClient.table_path(**expected)
+
+    # Check that the path construction is reversible.
+    actual = DataScanServiceClient.parse_table_path(path)
+    assert expected == actual
+
+
 def test_common_billing_account_path():
-    billing_account = "squid"
+    billing_account = "cuttlefish"
     expected = "billingAccounts/{billing_account}".format(
         billing_account=billing_account,
     )
     actual = DataScanServiceClient.common_billing_account_path(billing_account)
     assert expected == actual
 
 
 def test_parse_common_billing_account_path():
     expected = {
-        "billing_account": "clam",
+        "billing_account": "mussel",
     }
     path = DataScanServiceClient.common_billing_account_path(**expected)
 
     # Check that the path construction is reversible.
     actual = DataScanServiceClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
-    folder = "whelk"
+    folder = "winkle"
     expected = "folders/{folder}".format(
         folder=folder,
     )
     actual = DataScanServiceClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
-        "folder": "octopus",
+        "folder": "nautilus",
     }
     path = DataScanServiceClient.common_folder_path(**expected)
 
     # Check that the path construction is reversible.
     actual = DataScanServiceClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
-    organization = "oyster"
+    organization = "scallop"
     expected = "organizations/{organization}".format(
         organization=organization,
     )
     actual = DataScanServiceClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
-        "organization": "nudibranch",
+        "organization": "abalone",
     }
     path = DataScanServiceClient.common_organization_path(**expected)
 
     # Check that the path construction is reversible.
     actual = DataScanServiceClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
-    project = "cuttlefish"
+    project = "squid"
     expected = "projects/{project}".format(
         project=project,
     )
     actual = DataScanServiceClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
-        "project": "mussel",
+        "project": "clam",
     }
     path = DataScanServiceClient.common_project_path(**expected)
 
     # Check that the path construction is reversible.
     actual = DataScanServiceClient.parse_common_project_path(path)
     assert expected == actual
 
 
 def test_common_location_path():
-    project = "winkle"
-    location = "nautilus"
+    project = "whelk"
+    location = "octopus"
     expected = "projects/{project}/locations/{location}".format(
         project=project,
         location=location,
     )
     actual = DataScanServiceClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
-        "project": "scallop",
-        "location": "abalone",
+        "project": "oyster",
+        "location": "nudibranch",
     }
     path = DataScanServiceClient.common_location_path(**expected)
 
     # Check that the path construction is reversible.
     actual = DataScanServiceClient.parse_common_location_path(path)
     assert expected == actual
```

### Comparing `google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_dataplex_service.py` & `google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_dataplex_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -8228,14 +8228,15 @@
             name="name_value",
             uid="uid_value",
             state=tasks.Job.State.RUNNING,
             retry_count=1214,
             service=tasks.Job.Service.DATAPROC,
             service_job="service_job_value",
             message="message_value",
+            trigger=tasks.Job.Trigger.TASK_CONFIG,
         )
         response = client.get_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetJobRequest()
@@ -8245,14 +8246,15 @@
     assert response.name == "name_value"
     assert response.uid == "uid_value"
     assert response.state == tasks.Job.State.RUNNING
     assert response.retry_count == 1214
     assert response.service == tasks.Job.Service.DATAPROC
     assert response.service_job == "service_job_value"
     assert response.message == "message_value"
+    assert response.trigger == tasks.Job.Trigger.TASK_CONFIG
 
 
 def test_get_job_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = DataplexServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -8288,14 +8290,15 @@
                 name="name_value",
                 uid="uid_value",
                 state=tasks.Job.State.RUNNING,
                 retry_count=1214,
                 service=tasks.Job.Service.DATAPROC,
                 service_job="service_job_value",
                 message="message_value",
+                trigger=tasks.Job.Trigger.TASK_CONFIG,
             )
         )
         response = await client.get_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -8306,14 +8309,15 @@
     assert response.name == "name_value"
     assert response.uid == "uid_value"
     assert response.state == tasks.Job.State.RUNNING
     assert response.retry_count == 1214
     assert response.service == tasks.Job.Service.DATAPROC
     assert response.service_job == "service_job_value"
     assert response.message == "message_value"
+    assert response.trigger == tasks.Job.Trigger.TASK_CONFIG
 
 
 @pytest.mark.asyncio
 async def test_get_job_async_from_dict():
     await test_get_job_async(request_type=dict)
```

### Comparing `google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_metadata_service.py` & `google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_metadata_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

