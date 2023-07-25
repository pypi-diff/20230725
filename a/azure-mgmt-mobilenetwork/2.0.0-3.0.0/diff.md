# Comparing `tmp/azure-mgmt-mobilenetwork-2.0.0.zip` & `tmp/azure-mgmt-mobilenetwork-3.0.0.zip`

## zipinfo {}

```diff
@@ -1,73 +1,77 @@
-Zip file size: 191252 bytes, number of entries: 71
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure/
--rw-rw-r--  2.0 unx     2832 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/setup.py
--rw-rw-r--  2.0 unx       38 b- defN 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/setup.cfg
--rw-rw-r--  2.0 unx     1074 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/LICENSE
--rw-rw-r--  2.0 unx    11496 b- defN 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/PKG-INFO
--rw-rw-r--  2.0 unx      634 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/_meta.json
--rw-rw-r--  2.0 unx     2157 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/README.md
--rw-rw-r--  2.0 unx      219 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/MANIFEST.in
--rw-rw-r--  2.0 unx     8440 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/CHANGELOG.md
--rw-rw-r--  2.0 unx     3071 b- defN 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx    11496 b- defN 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx      116 b- defN 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/requires.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/top_level.txt
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/
--rw-rw-r--  2.0 unx       65 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/
--rw-rw-r--  2.0 unx       26 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/py.typed
--rw-rw-r--  2.0 unx     1169 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_vendor.py
--rw-rw-r--  2.0 unx      928 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/__init__.py
--rw-rw-r--  2.0 unx     7925 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_mobile_network_management_client.py
--rw-rw-r--  2.0 unx      486 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_version.py
--rw-rw-r--  2.0 unx    77872 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_serialization.py
--rw-rw-r--  2.0 unx     3762 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_configuration.py
--rw-rw-r--  2.0 unx     1530 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_patch.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:37 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/
--rw-rw-r--  2.0 unx      875 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/__init__.py
--rw-rw-r--  2.0 unx     8104 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/_mobile_network_management_client.py
--rw-rw-r--  2.0 unx     3810 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/_configuration.py
--rw-rw-r--  2.0 unx     1530 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/_patch.py
--rw-rw-r--  2.0 unx    34954 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_services_operations.py
--rw-rw-r--  2.0 unx    33970 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_slices_operations.py
--rw-rw-r--  2.0 unx    34622 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_data_networks_operations.py
--rw-rw-r--  2.0 unx    35710 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_sim_groups_operations.py
--rw-rw-r--  2.0 unx     1923 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    39148 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_attached_data_networks_operations.py
--rw-rw-r--  2.0 unx    34378 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_sim_policies_operations.py
--rw-rw-r--  2.0 unx    59903 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_sims_operations.py
--rw-rw-r--  2.0 unx    34045 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_sites_operations.py
--rw-rw-r--  2.0 unx     8840 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_plane_versions_operations.py
--rw-rw-r--  2.0 unx    36470 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_mobile_networks_operations.py
--rw-rw-r--  2.0 unx     5999 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    36647 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_data_planes_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    62711 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_planes_operations.py
--rw-rw-r--  2.0 unx     8339 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/_mobile_network_management_client_enums.py
--rw-rw-r--  2.0 unx     8535 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/_patch.py
--rw-rw-r--  2.0 unx   220501 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/_models_py3.py
--rw-rw-r--  2.0 unx    43603 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_services_operations.py
--rw-rw-r--  2.0 unx    42260 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_slices_operations.py
--rw-rw-r--  2.0 unx    43501 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_data_networks_operations.py
--rw-rw-r--  2.0 unx    43857 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_sim_groups_operations.py
--rw-rw-r--  2.0 unx     1923 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/__init__.py
--rw-rw-r--  2.0 unx    50465 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_attached_data_networks_operations.py
--rw-rw-r--  2.0 unx    42766 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_sim_policies_operations.py
--rw-rw-r--  2.0 unx    70676 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_sims_operations.py
--rw-rw-r--  2.0 unx    42311 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_sites_operations.py
--rw-rw-r--  2.0 unx    10474 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_control_plane_versions_operations.py
--rw-rw-r--  2.0 unx    44769 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_mobile_networks_operations.py
--rw-rw-r--  2.0 unx     6722 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_operations.py
--rw-rw-r--  2.0 unx    46089 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_data_planes_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_patch.py
--rw-rw-r--  2.0 unx    76183 b- defN 23-Jan-17 07:36 azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_control_planes_operations.py
-71 files, 1414044 bytes uncompressed, 174948 bytes compressed:  87.6%
+Zip file size: 209820 bytes, number of entries: 75
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure/
+-rw-rw-r--  2.0 unx     9288 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/CHANGELOG.md
+-rw-rw-r--  2.0 unx      634 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/_meta.json
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/LICENSE
+-rw-rw-r--  2.0 unx      219 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/MANIFEST.in
+-rw-rw-r--  2.0 unx     2186 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/README.md
+-rw-rw-r--  2.0 unx     2865 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/setup.py
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/setup.cfg
+-rw-rw-r--  2.0 unx    12386 b- defN 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/PKG-INFO
+-rw-rw-r--  2.0 unx      124 b- defN 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     3357 b- defN 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx    12386 b- defN 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/not-zip-safe
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/
+-rw-rw-r--  2.0 unx     1302 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_vendor.py
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_patch.py
+-rw-rw-r--  2.0 unx     8646 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_mobile_network_management_client.py
+-rw-rw-r--  2.0 unx      486 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_version.py
+-rw-rw-r--  2.0 unx      928 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/__init__.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/py.typed
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_configuration.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_serialization.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/_patch.py
+-rw-rw-r--  2.0 unx     9959 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/_mobile_network_management_client_enums.py
+-rw-rw-r--  2.0 unx     9691 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/__init__.py
+-rw-rw-r--  2.0 unx   235008 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/_models_py3.py
+-rw-rw-r--  2.0 unx    43104 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_services_operations.py
+-rw-rw-r--  2.0 unx    43374 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_packet_captures_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_patch.py
+-rw-rw-r--  2.0 unx     2134 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/__init__.py
+-rw-rw-r--  2.0 unx    43430 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_sim_groups_operations.py
+-rw-rw-r--  2.0 unx    69997 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_sims_operations.py
+-rw-rw-r--  2.0 unx    75532 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_control_planes_operations.py
+-rw-rw-r--  2.0 unx    54718 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_sites_operations.py
+-rw-rw-r--  2.0 unx     6464 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_operations.py
+-rw-rw-r--  2.0 unx    49978 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_attached_data_networks_operations.py
+-rw-rw-r--  2.0 unx    43006 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_data_networks_operations.py
+-rw-rw-r--  2.0 unx    42269 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_sim_policies_operations.py
+-rw-rw-r--  2.0 unx    19024 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_control_plane_versions_operations.py
+-rw-rw-r--  2.0 unx    30182 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_diagnostics_packages_operations.py
+-rw-rw-r--  2.0 unx    45602 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_data_planes_operations.py
+-rw-rw-r--  2.0 unx    41759 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_slices_operations.py
+-rw-rw-r--  2.0 unx    44234 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_mobile_networks_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 02:20 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/_patch.py
+-rw-rw-r--  2.0 unx     8838 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/_mobile_network_management_client.py
+-rw-rw-r--  2.0 unx      875 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/__init__.py
+-rw-rw-r--  2.0 unx     3588 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/_configuration.py
+-rw-rw-r--  2.0 unx    34615 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_services_operations.py
+-rw-rw-r--  2.0 unx    34709 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_captures_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx     2134 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    35475 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_sim_groups_operations.py
+-rw-rw-r--  2.0 unx    59448 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_sims_operations.py
+-rw-rw-r--  2.0 unx    62348 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_planes_operations.py
+-rw-rw-r--  2.0 unx    44876 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_sites_operations.py
+-rw-rw-r--  2.0 unx     5759 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    38821 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_attached_data_networks_operations.py
+-rw-rw-r--  2.0 unx    34287 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_data_networks_operations.py
+-rw-rw-r--  2.0 unx    34041 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_sim_policies_operations.py
+-rw-rw-r--  2.0 unx    15277 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_plane_versions_operations.py
+-rw-rw-r--  2.0 unx    23186 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_diagnostics_packages_operations.py
+-rw-rw-r--  2.0 unx    36320 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_data_planes_operations.py
+-rw-rw-r--  2.0 unx    33629 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_slices_operations.py
+-rw-rw-r--  2.0 unx    36127 b- defN 23-Jul-25 02:19 azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_mobile_networks_operations.py
+75 files, 1597359 bytes uncompressed, 192400 bytes compressed:  88.0%
```

## zipnote {}

```diff
@@ -1,214 +1,226 @@
-Filename: azure-mgmt-mobilenetwork-2.0.0/
+Filename: azure-mgmt-mobilenetwork-3.0.0/
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/setup.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/setup.cfg
+Filename: azure-mgmt-mobilenetwork-3.0.0/_meta.json
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/LICENSE
+Filename: azure-mgmt-mobilenetwork-3.0.0/LICENSE
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/PKG-INFO
+Filename: azure-mgmt-mobilenetwork-3.0.0/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/_meta.json
+Filename: azure-mgmt-mobilenetwork-3.0.0/README.md
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/README.md
+Filename: azure-mgmt-mobilenetwork-3.0.0/setup.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/MANIFEST.in
+Filename: azure-mgmt-mobilenetwork-3.0.0/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/CHANGELOG.md
+Filename: azure-mgmt-mobilenetwork-3.0.0/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/SOURCES.txt
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/not-zip-safe
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/PKG-INFO
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/dependency_links.txt
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/requires.txt
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/top_level.txt
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/__init__.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/__init__.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/py.typed
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_vendor.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_patch.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/__init__.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_mobile_network_management_client.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_mobile_network_management_client.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_version.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_version.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/__init__.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_serialization.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/py.typed
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_configuration.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_patch.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/__init__.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/_mobile_network_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/_mobile_network_management_client.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/_configuration.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/_patch.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_services_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_services_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_packet_captures_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_slices_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_data_networks_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_sim_groups_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_sim_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/__init__.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_sims_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_attached_data_networks_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_control_planes_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_sim_policies_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_sites_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_sims_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_sites_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_attached_data_networks_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_plane_versions_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_data_networks_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_mobile_networks_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_sim_policies_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_control_plane_versions_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_data_planes_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_diagnostics_packages_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_patch.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_data_planes_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_planes_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_slices_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/_mobile_network_management_client_enums.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_mobile_networks_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/__init__.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/_patch.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/_models_py3.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/_mobile_network_management_client.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_services_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_slices_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_data_networks_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_services_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_sim_groups_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_captures_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/__init__.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_attached_data_networks_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_sim_policies_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_sim_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_sims_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_sims_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_sites_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_planes_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_control_plane_versions_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_sites_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_mobile_networks_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_attached_data_networks_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_data_planes_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_data_networks_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_patch.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_sim_policies_operations.py
 Comment: 
 
-Filename: azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_control_planes_operations.py
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_plane_versions_operations.py
+Comment: 
+
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_diagnostics_packages_operations.py
+Comment: 
+
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_data_planes_operations.py
+Comment: 
+
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_slices_operations.py
+Comment: 
+
+Filename: azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_mobile_networks_operations.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/setup.py` & `azure-mgmt-mobilenetwork-3.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,79 +1,83 @@
 #!/usr/bin/env python
 
-#-------------------------------------------------------------------------
+# -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
-#--------------------------------------------------------------------------
+# --------------------------------------------------------------------------
 
 import re
 import os.path
 from io import open
 from setuptools import find_packages, setup
 
 # Change the PACKAGE_NAME only to change folder and different name
 PACKAGE_NAME = "azure-mgmt-mobilenetwork"
 PACKAGE_PPRINT_NAME = "Mobilenetwork Management"
 
 # a-b-c => a/b/c
-package_folder_path = PACKAGE_NAME.replace('-', '/')
+package_folder_path = PACKAGE_NAME.replace("-", "/")
 # a-b-c => a.b.c
-namespace_name = PACKAGE_NAME.replace('-', '.')
+namespace_name = PACKAGE_NAME.replace("-", ".")
 
 # Version extraction inspired from 'requests'
-with open(os.path.join(package_folder_path, 'version.py')
-          if os.path.exists(os.path.join(package_folder_path, 'version.py'))
-          else os.path.join(package_folder_path, '_version.py'), 'r') as fd:
-    version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]',
-                        fd.read(), re.MULTILINE).group(1)
+with open(
+    os.path.join(package_folder_path, "version.py")
+    if os.path.exists(os.path.join(package_folder_path, "version.py"))
+    else os.path.join(package_folder_path, "_version.py"),
+    "r",
+) as fd:
+    version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE).group(1)
 
 if not version:
-    raise RuntimeError('Cannot find version information')
+    raise RuntimeError("Cannot find version information")
 
-with open('README.md', encoding='utf-8') as f:
+with open("README.md", encoding="utf-8") as f:
     readme = f.read()
-with open('CHANGELOG.md', encoding='utf-8') as f:
+with open("CHANGELOG.md", encoding="utf-8") as f:
     changelog = f.read()
 
 setup(
     name=PACKAGE_NAME,
     version=version,
-    description='Microsoft Azure {} Client Library for Python'.format(PACKAGE_PPRINT_NAME),
-    long_description=readme + '\n\n' + changelog,
-    long_description_content_type='text/markdown',
-    license='MIT License',
-    author='Microsoft Corporation',
-    author_email='azpysdkhelp@microsoft.com',
-    url='https://github.com/Azure/azure-sdk-for-python',
+    description="Microsoft Azure {} Client Library for Python".format(PACKAGE_PPRINT_NAME),
+    long_description=readme + "\n\n" + changelog,
+    long_description_content_type="text/markdown",
+    license="MIT License",
+    author="Microsoft Corporation",
+    author_email="azpysdkhelp@microsoft.com",
+    url="https://github.com/Azure/azure-sdk-for-python",
     keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'License :: OSI Approved :: MIT License',
+        "Development Status :: 5 - Production/Stable",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
     ],
     zip_safe=False,
-    packages=find_packages(exclude=[
-        'tests',
-        # Exclude packages that will be covered by PEP420 or nspkg
-        'azure',
-        'azure.mgmt',
-    ]),
+    packages=find_packages(
+        exclude=[
+            "tests",
+            # Exclude packages that will be covered by PEP420 or nspkg
+            "azure",
+            "azure.mgmt",
+        ]
+    ),
     include_package_data=True,
     package_data={
-        'pytyped': ['py.typed'],
+        "pytyped": ["py.typed"],
     },
     install_requires=[
-        "msrest>=0.7.1",
+        "isodate<1.0.0,>=0.6.1",
         "azure-common~=1.1",
         "azure-mgmt-core>=1.3.2,<2.0.0",
         "typing-extensions>=4.3.0; python_version<'3.8.0'",
     ],
-    python_requires=">=3.7"
+    python_requires=">=3.7",
 )
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/LICENSE` & `azure-mgmt-mobilenetwork-3.0.0/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-mobilenetwork-2.0.0/PKG-INFO` & `azure-mgmt-mobilenetwork-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-mobilenetwork
-Version: 2.0.0
+Version: 3.0.0
 Summary: Microsoft Azure Mobilenetwork Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -64,16 +64,17 @@
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
 client = MobileNetworkManagementClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-
-Code samples for this package can be found at [Mobilenetwork Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+Code samples for this package can be found at:
+- [Search Mobilenetwork Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
@@ -84,14 +85,34 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-mobilenetwork%2FREADME.png)
 
 
 # Release History
 
+## 3.0.0 (2023-07-21)
+
+### Features Added
+
+  - Added operation PacketCoreControlPlaneVersionsOperations.get_by_subscription
+  - Added operation PacketCoreControlPlaneVersionsOperations.list_by_subscription
+  - Added operation SitesOperations.begin_delete_packet_core
+  - Added operation group DiagnosticsPackagesOperations
+  - Added operation group PacketCapturesOperations
+  - Model Installation has a new parameter desired_state
+  - Model Installation has a new parameter reasons
+  - Model Installation has a new parameter reinstall_required
+  - Model PacketCoreControlPlane has a new parameter diagnostics_upload
+  - Model PacketCoreControlPlane has a new parameter installed_version
+
+### Breaking Changes
+
+  - Model ManagedServiceIdentity no longer has parameter principal_id
+  - Model ManagedServiceIdentity no longer has parameter tenant_id
+
 ## 2.0.0 (2023-01-16)
 
 ### Features Added
 
   - Added operation PacketCoreControlPlanesOperations.begin_collect_diagnostics_package
   - Added operation PacketCoreControlPlanesOperations.begin_reinstall
   - Added operation PacketCoreControlPlanesOperations.begin_rollback
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/_meta.json` & `azure-mgmt-mobilenetwork-3.0.0/_meta.json`

 * *Files 23% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7777777777777777%*

 * *Differences: {"'autorest_command'": "'autorest specification/mobilenetwork/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.6.0 --use=@autorest/modelerfour@4.24.3 '*

 * *                       "--version=3.9.2 --version-tolerant=False'",*

 * * "'commit'": "'d8fbbdf15d10f5c708c4cc4a795b3df3a24c6a26'",*

 * * "'use'": "{i […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
-    "autorest_command": "autorest specification/mobilenetwork/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.2.7 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "340d577969b7bff5ad0488d79543314bc17daa50",
+    "autorest_command": "autorest specification/mobilenetwork/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.6.0 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
+    "commit": "d8fbbdf15d10f5c708c4cc4a795b3df3a24c6a26",
     "readme": "specification/mobilenetwork/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.2.7",
+        "@autorest/python@6.6.0",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/README.md` & `azure-mgmt-mobilenetwork-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,17 @@
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
 client = MobileNetworkManagementClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-
-Code samples for this package can be found at [Mobilenetwork Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+Code samples for this package can be found at:
+- [Search Mobilenetwork Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/CHANGELOG.md` & `azure-mgmt-mobilenetwork-3.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 # Release History
 
+## 3.0.0 (2023-07-21)
+
+### Features Added
+
+  - Added operation PacketCoreControlPlaneVersionsOperations.get_by_subscription
+  - Added operation PacketCoreControlPlaneVersionsOperations.list_by_subscription
+  - Added operation SitesOperations.begin_delete_packet_core
+  - Added operation group DiagnosticsPackagesOperations
+  - Added operation group PacketCapturesOperations
+  - Model Installation has a new parameter desired_state
+  - Model Installation has a new parameter reasons
+  - Model Installation has a new parameter reinstall_required
+  - Model PacketCoreControlPlane has a new parameter diagnostics_upload
+  - Model PacketCoreControlPlane has a new parameter installed_version
+
+### Breaking Changes
+
+  - Model ManagedServiceIdentity no longer has parameter principal_id
+  - Model ManagedServiceIdentity no longer has parameter tenant_id
+
 ## 2.0.0 (2023-01-16)
 
 ### Features Added
 
   - Added operation PacketCoreControlPlanesOperations.begin_collect_diagnostics_package
   - Added operation PacketCoreControlPlanesOperations.begin_reinstall
   - Added operation PacketCoreControlPlanesOperations.begin_rollback
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/SOURCES.txt` & `azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 azure/mgmt/mobilenetwork/aio/__init__.py
 azure/mgmt/mobilenetwork/aio/_configuration.py
 azure/mgmt/mobilenetwork/aio/_mobile_network_management_client.py
 azure/mgmt/mobilenetwork/aio/_patch.py
 azure/mgmt/mobilenetwork/aio/operations/__init__.py
 azure/mgmt/mobilenetwork/aio/operations/_attached_data_networks_operations.py
 azure/mgmt/mobilenetwork/aio/operations/_data_networks_operations.py
+azure/mgmt/mobilenetwork/aio/operations/_diagnostics_packages_operations.py
 azure/mgmt/mobilenetwork/aio/operations/_mobile_networks_operations.py
 azure/mgmt/mobilenetwork/aio/operations/_operations.py
+azure/mgmt/mobilenetwork/aio/operations/_packet_captures_operations.py
 azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_plane_versions_operations.py
 azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_planes_operations.py
 azure/mgmt/mobilenetwork/aio/operations/_packet_core_data_planes_operations.py
 azure/mgmt/mobilenetwork/aio/operations/_patch.py
 azure/mgmt/mobilenetwork/aio/operations/_services_operations.py
 azure/mgmt/mobilenetwork/aio/operations/_sim_groups_operations.py
 azure/mgmt/mobilenetwork/aio/operations/_sim_policies_operations.py
@@ -36,16 +38,18 @@
 azure/mgmt/mobilenetwork/models/__init__.py
 azure/mgmt/mobilenetwork/models/_mobile_network_management_client_enums.py
 azure/mgmt/mobilenetwork/models/_models_py3.py
 azure/mgmt/mobilenetwork/models/_patch.py
 azure/mgmt/mobilenetwork/operations/__init__.py
 azure/mgmt/mobilenetwork/operations/_attached_data_networks_operations.py
 azure/mgmt/mobilenetwork/operations/_data_networks_operations.py
+azure/mgmt/mobilenetwork/operations/_diagnostics_packages_operations.py
 azure/mgmt/mobilenetwork/operations/_mobile_networks_operations.py
 azure/mgmt/mobilenetwork/operations/_operations.py
+azure/mgmt/mobilenetwork/operations/_packet_captures_operations.py
 azure/mgmt/mobilenetwork/operations/_packet_core_control_plane_versions_operations.py
 azure/mgmt/mobilenetwork/operations/_packet_core_control_planes_operations.py
 azure/mgmt/mobilenetwork/operations/_packet_core_data_planes_operations.py
 azure/mgmt/mobilenetwork/operations/_patch.py
 azure/mgmt/mobilenetwork/operations/_services_operations.py
 azure/mgmt/mobilenetwork/operations/_sim_groups_operations.py
 azure/mgmt/mobilenetwork/operations/_sim_policies_operations.py
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure_mgmt_mobilenetwork.egg-info/PKG-INFO` & `azure-mgmt-mobilenetwork-3.0.0/azure_mgmt_mobilenetwork.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-mobilenetwork
-Version: 2.0.0
+Version: 3.0.0
 Summary: Microsoft Azure Mobilenetwork Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -64,16 +64,17 @@
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
 client = MobileNetworkManagementClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-
-Code samples for this package can be found at [Mobilenetwork Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+Code samples for this package can be found at:
+- [Search Mobilenetwork Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
@@ -84,14 +85,34 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-mobilenetwork%2FREADME.png)
 
 
 # Release History
 
+## 3.0.0 (2023-07-21)
+
+### Features Added
+
+  - Added operation PacketCoreControlPlaneVersionsOperations.get_by_subscription
+  - Added operation PacketCoreControlPlaneVersionsOperations.list_by_subscription
+  - Added operation SitesOperations.begin_delete_packet_core
+  - Added operation group DiagnosticsPackagesOperations
+  - Added operation group PacketCapturesOperations
+  - Model Installation has a new parameter desired_state
+  - Model Installation has a new parameter reasons
+  - Model Installation has a new parameter reinstall_required
+  - Model PacketCoreControlPlane has a new parameter diagnostics_upload
+  - Model PacketCoreControlPlane has a new parameter installed_version
+
+### Breaking Changes
+
+  - Model ManagedServiceIdentity no longer has parameter principal_id
+  - Model ManagedServiceIdentity no longer has parameter tenant_id
+
 ## 2.0.0 (2023-01-16)
 
 ### Features Added
 
   - Added operation PacketCoreControlPlanesOperations.begin_collect_diagnostics_package
   - Added operation PacketCoreControlPlanesOperations.begin_reinstall
   - Added operation PacketCoreControlPlanesOperations.begin_rollback
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_vendor.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_vendor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from typing import List, cast
+
 from azure.core.pipeline.transport import HttpRequest
 
 
 def _convert_request(request, files=None):
     data = request.content if not files else None
     request = HttpRequest(method=request.method, url=request.url, headers=request.headers, data=data)
     if files:
@@ -18,10 +20,11 @@
 
 def _format_url_section(template, **kwargs):
     components = template.split("/")
     while components:
         try:
             return template.format(**kwargs)
         except KeyError as key:
-            formatted_components = template.split("/")
+            # Need the cast, as for some reasons "split" is typed as list[str | Any]
+            formatted_components = cast(List[str], template.split("/"))
             components = [c for c in formatted_components if "{}".format(key.args[0]) not in c]
             template = "/".join(components)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/__init__.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_mobile_network_management_client.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_mobile_network_management_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 
 from . import models as _models
 from ._configuration import MobileNetworkManagementClientConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
     AttachedDataNetworksOperations,
     DataNetworksOperations,
+    DiagnosticsPackagesOperations,
     MobileNetworksOperations,
     Operations,
+    PacketCapturesOperations,
     PacketCoreControlPlaneVersionsOperations,
     PacketCoreControlPlanesOperations,
     PacketCoreDataPlanesOperations,
     ServicesOperations,
     SimGroupsOperations,
     SimPoliciesOperations,
     SimsOperations,
@@ -41,18 +43,23 @@
     in mobile network attached to a particular packet core instance.
 
     :ivar attached_data_networks: AttachedDataNetworksOperations operations
     :vartype attached_data_networks:
      azure.mgmt.mobilenetwork.operations.AttachedDataNetworksOperations
     :ivar data_networks: DataNetworksOperations operations
     :vartype data_networks: azure.mgmt.mobilenetwork.operations.DataNetworksOperations
+    :ivar diagnostics_packages: DiagnosticsPackagesOperations operations
+    :vartype diagnostics_packages:
+     azure.mgmt.mobilenetwork.operations.DiagnosticsPackagesOperations
     :ivar mobile_networks: MobileNetworksOperations operations
     :vartype mobile_networks: azure.mgmt.mobilenetwork.operations.MobileNetworksOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.mobilenetwork.operations.Operations
+    :ivar packet_captures: PacketCapturesOperations operations
+    :vartype packet_captures: azure.mgmt.mobilenetwork.operations.PacketCapturesOperations
     :ivar packet_core_control_planes: PacketCoreControlPlanesOperations operations
     :vartype packet_core_control_planes:
      azure.mgmt.mobilenetwork.operations.PacketCoreControlPlanesOperations
     :ivar packet_core_control_plane_versions: PacketCoreControlPlaneVersionsOperations operations
     :vartype packet_core_control_plane_versions:
      azure.mgmt.mobilenetwork.operations.PacketCoreControlPlaneVersionsOperations
     :ivar packet_core_data_planes: PacketCoreDataPlanesOperations operations
@@ -68,19 +75,19 @@
     :vartype sim_policies: azure.mgmt.mobilenetwork.operations.SimPoliciesOperations
     :ivar sites: SitesOperations operations
     :vartype sites: azure.mgmt.mobilenetwork.operations.SitesOperations
     :ivar slices: SlicesOperations operations
     :vartype slices: azure.mgmt.mobilenetwork.operations.SlicesOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: The ID of the target subscription. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-11-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2023-06-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -89,26 +96,30 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = MobileNetworkManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.attached_data_networks = AttachedDataNetworksOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.data_networks = DataNetworksOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.diagnostics_packages = DiagnosticsPackagesOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.mobile_networks = MobileNetworksOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
+        self.packet_captures = PacketCapturesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.packet_core_control_planes = PacketCoreControlPlanesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.packet_core_control_plane_versions = PacketCoreControlPlaneVersionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.packet_core_data_planes = PacketCoreDataPlanesOperations(
@@ -146,9 +157,9 @@
     def close(self) -> None:
         self._client.close()
 
     def __enter__(self) -> "MobileNetworkManagementClient":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details) -> None:
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_serialization.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,30 +34,47 @@
 import email
 from enum import Enum
 import json
 import logging
 import re
 import sys
 import codecs
-from typing import Optional, Union, AnyStr, IO, Mapping
+from typing import (
+    Dict,
+    Any,
+    cast,
+    Optional,
+    Union,
+    AnyStr,
+    IO,
+    Mapping,
+    Callable,
+    TypeVar,
+    MutableMapping,
+    Type,
+    List,
+    Mapping,
+)
 
 try:
     from urllib import quote  # type: ignore
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
-from typing import Dict, Any, cast
-
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
+ModelType = TypeVar("ModelType", bound="Model")
+JSON = MutableMapping[str, Any]
+
 
 class RawDeserializer:
 
     # Accept "text" because we're open minded people...
     JSON_REGEXP = re.compile(r"^(application|text)/([a-z+.]+\+)?json$")
 
     # Name used in context
@@ -273,43 +290,43 @@
     serialization and deserialization.
     """
 
     _subtype_map: Dict[str, Dict[str, Any]] = {}
     _attribute_map: Dict[str, Dict[str, Any]] = {}
     _validation: Dict[str, Dict[str, Any]] = {}
 
-    def __init__(self, **kwargs):
-        self.additional_properties = {}
+    def __init__(self, **kwargs: Any) -> None:
+        self.additional_properties: Dict[str, Any] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         if isinstance(other, self.__class__):
             return self.__dict__ == other.__dict__
         return False
 
-    def __ne__(self, other):
+    def __ne__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         return not self.__eq__(other)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.__dict__)
 
     @classmethod
-    def enable_additional_properties_sending(cls):
+    def enable_additional_properties_sending(cls) -> None:
         cls._attribute_map["additional_properties"] = {"key": "", "type": "{object}"}
 
     @classmethod
-    def is_xml_model(cls):
+    def is_xml_model(cls) -> bool:
         try:
             cls._xml_map  # type: ignore
         except AttributeError:
             return False
         return True
 
     @classmethod
@@ -318,30 +335,35 @@
         try:
             xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
-    def serialize(self, keep_readonly=False, **kwargs):
+    def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
         """Return the JSON that would be sent to azure from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
         return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
 
-    def as_dict(self, keep_readonly=True, key_transformer=attribute_transformer, **kwargs):
-        """Return a dict that can be JSONify using json.dump.
+    def as_dict(
+        self,
+        keep_readonly: bool = True,
+        key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
+        **kwargs: Any
+    ) -> JSON:
+        """Return a dict that can be serialized using json.dump.
 
         Advanced usage might optionally use a callback as parameter:
 
         .. code::python
 
             def my_key_transformer(key, attr_desc, value):
                 return key
@@ -380,41 +402,46 @@
                 raise ValueError("Not Autorest generated code")
         except Exception:
             # Assume it's not Autorest generated (tests?). Add ourselves as dependencies.
             client_models = {cls.__name__: cls}
         return client_models
 
     @classmethod
-    def deserialize(cls, data, content_type=None):
+    def deserialize(cls: Type[ModelType], data: Any, content_type: Optional[str] = None) -> ModelType:
         """Parse a str using the RestAPI syntax and return a model.
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
         return deserializer(cls.__name__, data, content_type=content_type)
 
     @classmethod
-    def from_dict(cls, data, key_extractors=None, content_type=None):
+    def from_dict(
+        cls: Type[ModelType],
+        data: Any,
+        key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
+        content_type: Optional[str] = None,
+    ) -> ModelType:
         """Parse a dict using given key extractor return a model.
 
         By default consider key
         extractors (rest_key_case_insensitive_extractor, attribute_key_case_insensitive_extractor
         and last_rest_key_case_insensitive_extractor)
 
         :param dict data: A dict using RestAPI structure
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        deserializer.key_extractors = (
-            [
+        deserializer.key_extractors = (  # type: ignore
+            [  # type: ignore
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
@@ -514,15 +541,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -530,15 +557,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -598,15 +625,15 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{}{}".format(xml_ns, xml_name)
+                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
                             serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
                             serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
                             serialized.extend(new_attr)  # type: ignore
@@ -622,16 +649,15 @@
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
                             local_node.text = unicode_str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
-                            unflattened = {k: new_attr}
-                            new_attr = unflattened
+                            new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
                         for k in keys:  # type: ignore
                             if k not in _serialized:
                                 _serialized.update(_new_attr)  # type: ignore
                             _new_attr = _new_attr[k]  # type: ignore
@@ -652,16 +678,16 @@
         :param str data_type: The type to be serialized from.
         :rtype: dict
         :raises: SerializationError if serialization fails.
         :raises: ValueError if data is None
         """
 
         # Just in case this is a dict
-        internal_data_type = data_type.strip("[]{}")
-        internal_data_type = self.dependencies.get(internal_data_type, None)
+        internal_data_type_str = data_type.strip("[]{}")
+        internal_data_type = self.dependencies.get(internal_data_type_str, None)
         try:
             is_xml_model_serialization = kwargs["is_xml"]
         except KeyError:
             if internal_data_type and issubclass(internal_data_type, Model):
                 is_xml_model_serialization = kwargs.setdefault("is_xml", internal_data_type.is_xml_model())
             else:
                 is_xml_model_serialization = False
@@ -773,14 +799,16 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
+            if data is AzureCoreNull:
+                return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
             # If dependencies is empty, try with current data class
@@ -1157,15 +1185,16 @@
 
 
 def rest_key_extractor(attr, attr_desc, data):
     key = attr_desc["key"]
     working_data = data
 
     while "." in key:
-        dict_keys = _FLATTEN.split(key)
+        # Need the cast, as for some reasons "split" is typed as list[str | Any]
+        dict_keys = cast(List[str], _FLATTEN.split(key))
         if len(dict_keys) == 1:
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
@@ -1238,15 +1267,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1262,15 +1291,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
@@ -1328,15 +1357,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1348,15 +1377,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1467,40 +1496,40 @@
 
     def _classify_target(self, target, data):
         """Check to see whether the deserialization target object can
         be classified into a subclass.
         Once classification has been determined, initialize object.
 
         :param str target: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
         if isinstance(target, basestring):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
             target = target._classify(data, self.dependencies)
         except AttributeError:
             pass  # Target is not a Model, no classify
-        return target, target.__class__.__name__
+        return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
         for use in error deserialization, as we want to return the
         HttpResponseError to users, and not have them deal with
         a deserialization error.
 
         :param str target_obj: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         :param str content_type: Swagger "produces" if available.
         """
         try:
             return self(target_obj, data, content_type=content_type)
         except:
             _LOGGER.debug(
                 "Ran into a deserialization error. Ignoring since this is failsafe deserialization", exc_info=True
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_configuration.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_configuration.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,51 +2,45 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
 from ._version import VERSION
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
 class MobileNetworkManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for MobileNetworkManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: The ID of the target subscription. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-11-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2023-06-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(MobileNetworkManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2022-11-01"] = kwargs.pop("api_version", "2022-11-01")
+        api_version: str = kwargs.pop("api_version", "2023-06-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/_patch.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/__init__.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/_mobile_network_management_client.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/_mobile_network_management_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import MobileNetworkManagementClientConfiguration
 from .operations import (
     AttachedDataNetworksOperations,
     DataNetworksOperations,
+    DiagnosticsPackagesOperations,
     MobileNetworksOperations,
     Operations,
+    PacketCapturesOperations,
     PacketCoreControlPlaneVersionsOperations,
     PacketCoreControlPlanesOperations,
     PacketCoreDataPlanesOperations,
     ServicesOperations,
     SimGroupsOperations,
     SimPoliciesOperations,
     SimsOperations,
@@ -41,18 +43,23 @@
     in mobile network attached to a particular packet core instance.
 
     :ivar attached_data_networks: AttachedDataNetworksOperations operations
     :vartype attached_data_networks:
      azure.mgmt.mobilenetwork.aio.operations.AttachedDataNetworksOperations
     :ivar data_networks: DataNetworksOperations operations
     :vartype data_networks: azure.mgmt.mobilenetwork.aio.operations.DataNetworksOperations
+    :ivar diagnostics_packages: DiagnosticsPackagesOperations operations
+    :vartype diagnostics_packages:
+     azure.mgmt.mobilenetwork.aio.operations.DiagnosticsPackagesOperations
     :ivar mobile_networks: MobileNetworksOperations operations
     :vartype mobile_networks: azure.mgmt.mobilenetwork.aio.operations.MobileNetworksOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.mobilenetwork.aio.operations.Operations
+    :ivar packet_captures: PacketCapturesOperations operations
+    :vartype packet_captures: azure.mgmt.mobilenetwork.aio.operations.PacketCapturesOperations
     :ivar packet_core_control_planes: PacketCoreControlPlanesOperations operations
     :vartype packet_core_control_planes:
      azure.mgmt.mobilenetwork.aio.operations.PacketCoreControlPlanesOperations
     :ivar packet_core_control_plane_versions: PacketCoreControlPlaneVersionsOperations operations
     :vartype packet_core_control_plane_versions:
      azure.mgmt.mobilenetwork.aio.operations.PacketCoreControlPlaneVersionsOperations
     :ivar packet_core_data_planes: PacketCoreDataPlanesOperations operations
@@ -68,19 +75,19 @@
     :vartype sim_policies: azure.mgmt.mobilenetwork.aio.operations.SimPoliciesOperations
     :ivar sites: SitesOperations operations
     :vartype sites: azure.mgmt.mobilenetwork.aio.operations.SitesOperations
     :ivar slices: SlicesOperations operations
     :vartype slices: azure.mgmt.mobilenetwork.aio.operations.SlicesOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: The ID of the target subscription. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-11-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2023-06-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -89,26 +96,30 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = MobileNetworkManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.attached_data_networks = AttachedDataNetworksOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.data_networks = DataNetworksOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.diagnostics_packages = DiagnosticsPackagesOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.mobile_networks = MobileNetworksOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
+        self.packet_captures = PacketCapturesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.packet_core_control_planes = PacketCoreControlPlanesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.packet_core_control_plane_versions = PacketCoreControlPlaneVersionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.packet_core_data_planes = PacketCoreDataPlanesOperations(
@@ -146,9 +157,9 @@
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "MobileNetworkManagementClient":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/_configuration.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/_configuration.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,51 +2,45 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
 from .._version import VERSION
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class MobileNetworkManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for MobileNetworkManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: The ID of the target subscription. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-11-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2023-06-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(MobileNetworkManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2022-11-01"] = kwargs.pop("api_version", "2022-11-01")
+        api_version: str = kwargs.pop("api_version", "2023-06-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/_patch.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_services_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_services_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -35,18 +35,14 @@
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_mobile_network_request,
     build_update_tags_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ServicesOperations:
     """
     .. warning::
@@ -76,17 +72,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             service_name=service_name,
             subscription_id=self._config.subscription_id,
@@ -94,16 +88,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -141,17 +136,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -216,17 +209,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Service] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             service_name=service_name,
             subscription_id=self._config.subscription_id,
@@ -234,16 +225,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -275,24 +267,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Service] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Service")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -305,16 +295,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -434,15 +425,15 @@
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param service_name: The name of the service. You must not use any of the following reserved
          strings - ``default``\ , ``requested`` or ``service``. Required.
         :type service_name: str
         :param parameters: Parameters supplied to the create or update service operation. Is either a
-         model type or a IO type. Required.
+         Service type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.Service or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -455,17 +446,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.Service]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Service] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -589,16 +578,16 @@
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param service_name: The name of the service. You must not use any of the following reserved
          strings - ``default``\ , ``requested`` or ``service``. Required.
         :type service_name: str
-        :param parameters: Parameters supplied to update service tags. Is either a model type or a IO
-         type. Required.
+        :param parameters: Parameters supplied to update service tags. Is either a TagsObject type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Service or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.Service
@@ -611,24 +600,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Service] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -641,16 +628,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -682,17 +670,15 @@
         :return: An iterator like instance of either Service or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.Service]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ServiceListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -738,16 +724,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_slices_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_slices_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -35,18 +35,14 @@
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_mobile_network_request,
     build_update_tags_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class SlicesOperations:
     """
     .. warning::
@@ -76,17 +72,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             slice_name=slice_name,
             subscription_id=self._config.subscription_id,
@@ -94,16 +88,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -140,17 +135,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -214,17 +207,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Slice] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             slice_name=slice_name,
             subscription_id=self._config.subscription_id,
@@ -232,16 +223,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -273,24 +265,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Slice] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Slice")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -303,16 +293,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -429,15 +420,15 @@
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param slice_name: The name of the network slice. Required.
         :type slice_name: str
         :param parameters: Parameters supplied to the create or update network slice operation. Is
-         either a model type or a IO type. Required.
+         either a Slice type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.Slice or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -449,17 +440,15 @@
         :return: An instance of AsyncLROPoller that returns either Slice or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.Slice]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Slice] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -580,16 +569,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param slice_name: The name of the network slice. Required.
         :type slice_name: str
-        :param parameters: Parameters supplied to update network slice tags. Is either a model type or
-         a IO type. Required.
+        :param parameters: Parameters supplied to update network slice tags. Is either a TagsObject
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Slice or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.Slice
@@ -602,24 +591,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Slice] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -632,16 +619,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -673,17 +661,15 @@
         :return: An iterator like instance of either Slice or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.Slice]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SliceListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -729,16 +715,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_data_networks_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_data_networks_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -35,18 +35,14 @@
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_mobile_network_request,
     build_update_tags_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DataNetworksOperations:
     """
     .. warning::
@@ -76,17 +72,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             data_network_name=data_network_name,
             subscription_id=self._config.subscription_id,
@@ -94,16 +88,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -140,17 +135,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -214,17 +207,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DataNetwork] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             data_network_name=data_network_name,
             subscription_id=self._config.subscription_id,
@@ -232,16 +223,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -273,24 +265,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DataNetwork] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "DataNetwork")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -303,16 +293,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -431,15 +422,15 @@
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param data_network_name: The name of the data network. Required.
         :type data_network_name: str
         :param parameters: Parameters supplied to the create or update data network operation. Is
-         either a model type or a IO type. Required.
+         either a DataNetwork type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.DataNetwork or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -452,17 +443,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.DataNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DataNetwork] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -583,16 +572,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param data_network_name: The name of the data network. Required.
         :type data_network_name: str
-        :param parameters: Parameters supplied to update data network tags. Is either a model type or a
-         IO type. Required.
+        :param parameters: Parameters supplied to update data network tags. Is either a TagsObject type
+         or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DataNetwork or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.DataNetwork
@@ -605,24 +594,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DataNetwork] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -635,16 +622,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -676,17 +664,15 @@
         :return: An iterator like instance of either DataNetwork or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.DataNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DataNetworkListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -732,16 +718,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_sim_groups_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_sim_groups_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -36,18 +36,14 @@
     build_delete_request,
     build_get_request,
     build_list_by_resource_group_request,
     build_list_by_subscription_request,
     build_update_tags_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class SimGroupsOperations:
     """
     .. warning::
@@ -77,33 +73,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -136,17 +131,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -205,33 +198,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SimGroup] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -258,24 +250,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SimGroup] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "SimGroup")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
@@ -287,16 +277,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -397,15 +388,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
         :param parameters: Parameters supplied to the create or update SIM group operation. Is either a
-         model type or a IO type. Required.
+         SimGroup type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.SimGroup or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -418,17 +409,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.SimGroup]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SimGroup] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -473,28 +462,28 @@
     }
 
     @overload
     async def update_tags(
         self,
         resource_group_name: str,
         sim_group_name: str,
-        parameters: _models.TagsObject,
+        parameters: _models.IdentityAndTagsObject,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.SimGroup:
-        """Updates SIM group tags.
+        """Patch SIM group resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
-        :param parameters: Parameters supplied to update SIM group tags. Required.
-        :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject
+        :param parameters: Parameters supplied to patch SIM group resource. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.IdentityAndTagsObject
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SimGroup or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.SimGroup
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -506,46 +495,50 @@
         resource_group_name: str,
         sim_group_name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.SimGroup:
-        """Updates SIM group tags.
+        """Patch SIM group resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
-        :param parameters: Parameters supplied to update SIM group tags. Required.
+        :param parameters: Parameters supplied to patch SIM group resource. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SimGroup or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.SimGroup
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update_tags(
-        self, resource_group_name: str, sim_group_name: str, parameters: Union[_models.TagsObject, IO], **kwargs: Any
+        self,
+        resource_group_name: str,
+        sim_group_name: str,
+        parameters: Union[_models.IdentityAndTagsObject, IO],
+        **kwargs: Any
     ) -> _models.SimGroup:
-        """Updates SIM group tags.
+        """Patch SIM group resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
-        :param parameters: Parameters supplied to update SIM group tags. Is either a model type or a IO
-         type. Required.
-        :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
+        :param parameters: Parameters supplied to patch SIM group resource. Is either a
+         IdentityAndTagsObject type or a IO type. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.IdentityAndTagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SimGroup or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.SimGroup
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -557,27 +550,25 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SimGroup] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
-            _json = self._serialize.body(parameters, "TagsObject")
+            _json = self._serialize.body(parameters, "IdentityAndTagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
@@ -586,16 +577,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -620,17 +612,15 @@
         :return: An iterator like instance of either SimGroup or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.SimGroup]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SimGroupListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -674,16 +664,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -707,17 +698,15 @@
         :return: An iterator like instance of either SimGroup or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.SimGroup]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SimGroupListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -762,16 +751,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/__init__.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._attached_data_networks_operations import AttachedDataNetworksOperations
 from ._data_networks_operations import DataNetworksOperations
+from ._diagnostics_packages_operations import DiagnosticsPackagesOperations
 from ._mobile_networks_operations import MobileNetworksOperations
 from ._operations import Operations
+from ._packet_captures_operations import PacketCapturesOperations
 from ._packet_core_control_planes_operations import PacketCoreControlPlanesOperations
 from ._packet_core_control_plane_versions_operations import PacketCoreControlPlaneVersionsOperations
 from ._packet_core_data_planes_operations import PacketCoreDataPlanesOperations
 from ._services_operations import ServicesOperations
 from ._sims_operations import SimsOperations
 from ._sim_groups_operations import SimGroupsOperations
 from ._sim_policies_operations import SimPoliciesOperations
@@ -23,16 +25,18 @@
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AttachedDataNetworksOperations",
     "DataNetworksOperations",
+    "DiagnosticsPackagesOperations",
     "MobileNetworksOperations",
     "Operations",
+    "PacketCapturesOperations",
     "PacketCoreControlPlanesOperations",
     "PacketCoreControlPlaneVersionsOperations",
     "PacketCoreDataPlanesOperations",
     "ServicesOperations",
     "SimsOperations",
     "SimGroupsOperations",
     "SimPoliciesOperations",
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_attached_data_networks_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_attached_data_networks_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -35,18 +35,14 @@
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_packet_core_data_plane_request,
     build_update_tags_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class AttachedDataNetworksOperations:
     """
     .. warning::
@@ -81,17 +77,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             packet_core_data_plane_name=packet_core_data_plane_name,
             attached_data_network_name=attached_data_network_name,
@@ -100,16 +94,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -153,17 +148,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -235,17 +228,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AttachedDataNetwork] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             packet_core_data_plane_name=packet_core_data_plane_name,
             attached_data_network_name=attached_data_network_name,
@@ -254,16 +245,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -296,24 +288,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AttachedDataNetwork] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "AttachedDataNetwork")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
@@ -327,16 +317,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -466,15 +457,15 @@
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
         :param packet_core_data_plane_name: The name of the packet core data plane. Required.
         :type packet_core_data_plane_name: str
         :param attached_data_network_name: The name of the attached data network. Required.
         :type attached_data_network_name: str
         :param parameters: Parameters supplied to the create or update attached data network operation.
-         Is either a model type or a IO type. Required.
+         Is either a AttachedDataNetwork type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.AttachedDataNetwork or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -488,17 +479,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.AttachedDataNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AttachedDataNetwork] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -629,16 +618,16 @@
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
         :param packet_core_data_plane_name: The name of the packet core data plane. Required.
         :type packet_core_data_plane_name: str
         :param attached_data_network_name: The name of the attached data network. Required.
         :type attached_data_network_name: str
-        :param parameters: Parameters supplied to update attached data network tags. Is either a model
-         type or a IO type. Required.
+        :param parameters: Parameters supplied to update attached data network tags. Is either a
+         TagsObject type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AttachedDataNetwork or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.AttachedDataNetwork
@@ -651,24 +640,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AttachedDataNetwork] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
@@ -682,16 +669,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -730,17 +718,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.AttachedDataNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AttachedDataNetworkListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -787,16 +773,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_sim_policies_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_sim_policies_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -35,18 +35,14 @@
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_mobile_network_request,
     build_update_tags_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class SimPoliciesOperations:
     """
     .. warning::
@@ -76,17 +72,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             sim_policy_name=sim_policy_name,
             subscription_id=self._config.subscription_id,
@@ -94,16 +88,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -140,17 +135,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -214,17 +207,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SimPolicy] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             sim_policy_name=sim_policy_name,
             subscription_id=self._config.subscription_id,
@@ -232,16 +223,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -273,24 +265,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SimPolicy] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "SimPolicy")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -303,16 +293,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -429,15 +420,15 @@
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param sim_policy_name: The name of the SIM policy. Required.
         :type sim_policy_name: str
         :param parameters: Parameters supplied to the create or update SIM policy operation. Is either
-         a model type or a IO type. Required.
+         a SimPolicy type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.SimPolicy or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -450,17 +441,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.SimPolicy]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SimPolicy] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -581,16 +570,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param sim_policy_name: The name of the SIM policy. Required.
         :type sim_policy_name: str
-        :param parameters: Parameters supplied to update SIM policy tags. Is either a model type or a
-         IO type. Required.
+        :param parameters: Parameters supplied to update SIM policy tags. Is either a TagsObject type
+         or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SimPolicy or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.SimPolicy
@@ -603,24 +592,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SimPolicy] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -633,16 +620,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -674,17 +662,15 @@
         :return: An iterator like instance of either SimPolicy or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.SimPolicy]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SimPolicyListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -730,16 +716,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_sims_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_sims_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -37,18 +37,14 @@
     build_bulk_upload_request,
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_group_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class SimsOperations:
     """
     .. warning::
@@ -78,17 +74,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
             sim_name=sim_name,
             subscription_id=self._config.subscription_id,
@@ -96,16 +90,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -142,17 +137,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -214,17 +207,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Sim] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
             sim_name=sim_name,
             subscription_id=self._config.subscription_id,
@@ -232,16 +223,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -273,24 +265,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Sim] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Sim")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
@@ -303,16 +293,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -423,15 +414,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
         :param sim_name: The name of the SIM. Required.
         :type sim_name: str
-        :param parameters: Parameters supplied to the create or update SIM operation. Is either a model
+        :param parameters: Parameters supplied to the create or update SIM operation. Is either a Sim
          type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.Sim or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
@@ -444,17 +435,15 @@
         :return: An instance of AsyncLROPoller that returns either Sim or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.Sim]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Sim] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -514,17 +503,15 @@
         :return: An iterator like instance of either Sim or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.Sim]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SimListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -570,16 +557,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -602,24 +590,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.AsyncOperationStatus]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "SimUploadList")
 
         request = build_bulk_upload_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
@@ -631,16 +617,17 @@
             template_url=self._bulk_upload_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -740,16 +727,16 @@
         """Bulk upload SIMs to a SIM group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
-        :param parameters: Parameters supplied to the bulk SIM upload operation. Is either a model type
-         or a IO type. Required.
+        :param parameters: Parameters supplied to the bulk SIM upload operation. Is either a
+         SimUploadList type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.SimUploadList or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -763,17 +750,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.AsyncOperationStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AsyncOperationStatus] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._bulk_upload_initial(
@@ -826,24 +811,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.AsyncOperationStatus]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "SimDeleteList")
 
         request = build_bulk_delete_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
@@ -855,16 +838,17 @@
             template_url=self._bulk_delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -964,16 +948,16 @@
         """Bulk delete SIMs from a SIM group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
-        :param parameters: Parameters supplied to the bulk SIM delete operation. Is either a model type
-         or a IO type. Required.
+        :param parameters: Parameters supplied to the bulk SIM delete operation. Is either a
+         SimDeleteList type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.SimDeleteList or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -987,17 +971,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.AsyncOperationStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AsyncOperationStatus] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._bulk_delete_initial(
@@ -1054,24 +1036,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.AsyncOperationStatus]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "EncryptedSimUploadList")
 
         request = build_bulk_upload_encrypted_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
@@ -1083,16 +1063,17 @@
             template_url=self._bulk_upload_encrypted_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1197,15 +1178,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
         :param parameters: Parameters supplied to the encrypted SIMs upload operation. Is either a
-         model type or a IO type. Required.
+         EncryptedSimUploadList type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.EncryptedSimUploadList or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -1219,17 +1200,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.AsyncOperationStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AsyncOperationStatus] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._bulk_upload_encrypted_initial(
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_sites_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_mobile_networks_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -27,113 +27,105 @@
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._sites_operations import (
+from ...operations._mobile_networks_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
-    build_list_by_mobile_network_request,
+    build_list_by_resource_group_request,
+    build_list_by_subscription_request,
     build_update_tags_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class SitesOperations:
+class MobileNetworksOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.mobilenetwork.aio.MobileNetworkManagementClient`'s
-        :attr:`sites` attribute.
+        :attr:`mobile_networks` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, mobile_network_name: str, site_name: str, **kwargs: Any
+        self, resource_group_name: str, mobile_network_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
-            site_name=site_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}"
     }
 
     @distributed_trace_async
     async def begin_delete(
-        self, resource_group_name: str, mobile_network_name: str, site_name: str, **kwargs: Any
+        self, resource_group_name: str, mobile_network_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
-        """Deletes the specified mobile network site. This will also delete any network functions that are
-        a part of this site.
+        """Deletes the specified mobile network.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param site_name: The name of the mobile network site. Required.
-        :type site_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
@@ -141,26 +133,23 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 mobile_network_name=mobile_network_name,
-                site_name=site_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
@@ -183,306 +172,285 @@
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}"
     }
 
     @distributed_trace_async
-    async def get(
-        self, resource_group_name: str, mobile_network_name: str, site_name: str, **kwargs: Any
-    ) -> _models.Site:
-        """Gets information about the specified mobile network site.
+    async def get(self, resource_group_name: str, mobile_network_name: str, **kwargs: Any) -> _models.MobileNetwork:
+        """Gets information about the specified mobile network.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param site_name: The name of the mobile network site. Required.
-        :type site_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Site or the result of cls(response)
-        :rtype: ~azure.mgmt.mobilenetwork.models.Site
+        :return: MobileNetwork or the result of cls(response)
+        :rtype: ~azure.mgmt.mobilenetwork.models.MobileNetwork
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.Site] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.MobileNetwork] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
-            site_name=site_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("Site", pipeline_response)
+        deserialized = self._deserialize("MobileNetwork", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}"
     }
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         mobile_network_name: str,
-        site_name: str,
-        parameters: Union[_models.Site, IO],
+        parameters: Union[_models.MobileNetwork, IO],
         **kwargs: Any
-    ) -> _models.Site:
+    ) -> _models.MobileNetwork:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.Site] = kwargs.pop("cls", None)
+        cls: ClsType[_models.MobileNetwork] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
-            _json = self._serialize.body(parameters, "Site")
+            _json = self._serialize.body(parameters, "MobileNetwork")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
-            site_name=site_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize("Site", pipeline_response)
+            deserialized = self._deserialize("MobileNetwork", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize("Site", pipeline_response)
+            deserialized = self._deserialize("MobileNetwork", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}"
     }
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         mobile_network_name: str,
-        site_name: str,
-        parameters: _models.Site,
+        parameters: _models.MobileNetwork,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.Site]:
-        """Creates or updates a mobile network site. Must be created in the same location as its parent
-        mobile network.
+    ) -> AsyncLROPoller[_models.MobileNetwork]:
+        """Creates or updates a mobile network.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param site_name: The name of the mobile network site. Required.
-        :type site_name: str
-        :param parameters: Parameters supplied to the create or update mobile network site operation.
+        :param parameters: Parameters supplied to the create or update mobile network operation.
          Required.
-        :type parameters: ~azure.mgmt.mobilenetwork.models.Site
+        :type parameters: ~azure.mgmt.mobilenetwork.models.MobileNetwork
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either Site or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.Site]
+        :return: An instance of AsyncLROPoller that returns either MobileNetwork or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.MobileNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         mobile_network_name: str,
-        site_name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.Site]:
-        """Creates or updates a mobile network site. Must be created in the same location as its parent
-        mobile network.
+    ) -> AsyncLROPoller[_models.MobileNetwork]:
+        """Creates or updates a mobile network.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param site_name: The name of the mobile network site. Required.
-        :type site_name: str
-        :param parameters: Parameters supplied to the create or update mobile network site operation.
+        :param parameters: Parameters supplied to the create or update mobile network operation.
          Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either Site or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.Site]
+        :return: An instance of AsyncLROPoller that returns either MobileNetwork or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.MobileNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         mobile_network_name: str,
-        site_name: str,
-        parameters: Union[_models.Site, IO],
+        parameters: Union[_models.MobileNetwork, IO],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.Site]:
-        """Creates or updates a mobile network site. Must be created in the same location as its parent
-        mobile network.
+    ) -> AsyncLROPoller[_models.MobileNetwork]:
+        """Creates or updates a mobile network.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param site_name: The name of the mobile network site. Required.
-        :type site_name: str
-        :param parameters: Parameters supplied to the create or update mobile network site operation.
-         Is either a model type or a IO type. Required.
-        :type parameters: ~azure.mgmt.mobilenetwork.models.Site or IO
+        :param parameters: Parameters supplied to the create or update mobile network operation. Is
+         either a MobileNetwork type or a IO type. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.MobileNetwork or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either Site or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.Site]
+        :return: An instance of AsyncLROPoller that returns either MobileNetwork or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.MobileNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.Site] = kwargs.pop("cls", None)
+        cls: ClsType[_models.MobileNetwork] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 mobile_network_name=mobile_network_name,
-                site_name=site_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("Site", pipeline_response)
+            deserialized = self._deserialize("MobileNetwork", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
@@ -498,212 +466,277 @@
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}"
     }
 
     @overload
     async def update_tags(
         self,
         resource_group_name: str,
         mobile_network_name: str,
-        site_name: str,
         parameters: _models.TagsObject,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.Site:
-        """Updates site tags.
+    ) -> _models.MobileNetwork:
+        """Updates mobile network tags.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param site_name: The name of the mobile network site. Required.
-        :type site_name: str
-        :param parameters: Parameters supplied to update network site tags. Required.
+        :param parameters: Parameters supplied to update mobile network tags. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Site or the result of cls(response)
-        :rtype: ~azure.mgmt.mobilenetwork.models.Site
+        :return: MobileNetwork or the result of cls(response)
+        :rtype: ~azure.mgmt.mobilenetwork.models.MobileNetwork
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def update_tags(
         self,
         resource_group_name: str,
         mobile_network_name: str,
-        site_name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.Site:
-        """Updates site tags.
+    ) -> _models.MobileNetwork:
+        """Updates mobile network tags.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param site_name: The name of the mobile network site. Required.
-        :type site_name: str
-        :param parameters: Parameters supplied to update network site tags. Required.
+        :param parameters: Parameters supplied to update mobile network tags. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Site or the result of cls(response)
-        :rtype: ~azure.mgmt.mobilenetwork.models.Site
+        :return: MobileNetwork or the result of cls(response)
+        :rtype: ~azure.mgmt.mobilenetwork.models.MobileNetwork
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update_tags(
         self,
         resource_group_name: str,
         mobile_network_name: str,
-        site_name: str,
         parameters: Union[_models.TagsObject, IO],
         **kwargs: Any
-    ) -> _models.Site:
-        """Updates site tags.
+    ) -> _models.MobileNetwork:
+        """Updates mobile network tags.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param site_name: The name of the mobile network site. Required.
-        :type site_name: str
-        :param parameters: Parameters supplied to update network site tags. Is either a model type or a
-         IO type. Required.
+        :param parameters: Parameters supplied to update mobile network tags. Is either a TagsObject
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Site or the result of cls(response)
-        :rtype: ~azure.mgmt.mobilenetwork.models.Site
+        :return: MobileNetwork or the result of cls(response)
+        :rtype: ~azure.mgmt.mobilenetwork.models.MobileNetwork
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.Site] = kwargs.pop("cls", None)
+        cls: ClsType[_models.MobileNetwork] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
-            site_name=site_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("Site", pipeline_response)
+        deserialized = self._deserialize("MobileNetwork", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     update_tags.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}"
     }
 
     @distributed_trace
-    def list_by_mobile_network(
-        self, resource_group_name: str, mobile_network_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.Site"]:
-        """Lists all sites in the mobile network.
+    def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.MobileNetwork"]:
+        """Lists all the mobile networks in a subscription.
+
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: An iterator like instance of either MobileNetwork or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.MobileNetwork]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.MobileNetworkListResult] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                request = build_list_by_subscription_request(
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    template_url=self.list_by_subscription.metadata["url"],
+                    headers=_headers,
+                    params=_params,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
+            return request
+
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("MobileNetworkListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, AsyncList(list_of_elem)
+
+        async def get_next(next_link=None):
+            request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+            return pipeline_response
+
+        return AsyncItemPaged(get_next, extract_data)
+
+    list_by_subscription.metadata = {
+        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.MobileNetwork/mobileNetworks"
+    }
+
+    @distributed_trace
+    def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> AsyncIterable["_models.MobileNetwork"]:
+        """Lists all the mobile networks in a resource group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param mobile_network_name: The name of the mobile network. Required.
-        :type mobile_network_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either Site or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.Site]
+        :return: An iterator like instance of either MobileNetwork or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.MobileNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.SiteListResult] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.MobileNetworkListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_mobile_network_request(
+                request = build_list_by_resource_group_request(
                     resource_group_name=resource_group_name,
-                    mobile_network_name=mobile_network_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_mobile_network.metadata["url"],
+                    template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
 
             else:
@@ -721,33 +754,34 @@
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("SiteListResult", pipeline_response)
+            deserialized = self._deserialize("MobileNetworkListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_mobile_network.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites"
+    list_by_resource_group.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks"
     }
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_plane_versions_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -19,124 +18,58 @@
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._packet_core_control_plane_versions_operations import build_get_request, build_list_request
+from ...operations._operations import build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class PacketCoreControlPlaneVersionsOperations:
+class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.mobilenetwork.aio.MobileNetworkManagementClient`'s
-        :attr:`packet_core_control_plane_versions` attribute.
+        :attr:`operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @distributed_trace_async
-    async def get(self, version_name: str, **kwargs: Any) -> _models.PacketCoreControlPlaneVersion:
-        """Gets information about the specified packet core control plane version.
-
-        :param version_name: The name of the packet core control plane version. Required.
-        :type version_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: PacketCoreControlPlaneVersion or the result of cls(response)
-        :rtype: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlaneVersion
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.PacketCoreControlPlaneVersion] = kwargs.pop("cls", None)
-
-        request = build_get_request(
-            version_name=version_name,
-            api_version=api_version,
-            template_url=self.get.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("PacketCoreControlPlaneVersion", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
-
-    get.metadata = {"url": "/providers/Microsoft.MobileNetwork/packetCoreControlPlaneVersions/{versionName}"}
-
     @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.PacketCoreControlPlaneVersion"]:
-        """Lists all supported packet core control planes versions.
+    def list(self, **kwargs: Any) -> AsyncIterable["_models.Operation"]:
+        """Gets a list of the operations.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either PacketCoreControlPlaneVersion or the result of
-         cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.PacketCoreControlPlaneVersion]
+        :return: An iterator like instance of either Operation or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.PacketCoreControlPlaneVersionListResult] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.OperationList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -169,31 +102,32 @@
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("PacketCoreControlPlaneVersionListResult", pipeline_response)
+            deserialized = self._deserialize("OperationList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/providers/Microsoft.MobileNetwork/packetCoreControlPlaneVersions"}
+    list.metadata = {"url": "/providers/Microsoft.MobileNetwork/operations"}
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_mobile_networks_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_sites_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -27,110 +27,109 @@
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._mobile_networks_operations import (
+from ...operations._sites_operations import (
     build_create_or_update_request,
+    build_delete_packet_core_request,
     build_delete_request,
     build_get_request,
-    build_list_by_resource_group_request,
-    build_list_by_subscription_request,
+    build_list_by_mobile_network_request,
     build_update_tags_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class MobileNetworksOperations:
+class SitesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.mobilenetwork.aio.MobileNetworkManagementClient`'s
-        :attr:`mobile_networks` attribute.
+        :attr:`sites` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, mobile_network_name: str, **kwargs: Any
+        self, resource_group_name: str, mobile_network_name: str, site_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
+            site_name=site_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}"
     }
 
     @distributed_trace_async
     async def begin_delete(
-        self, resource_group_name: str, mobile_network_name: str, **kwargs: Any
+        self, resource_group_name: str, mobile_network_name: str, site_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
-        """Deletes the specified mobile network.
+        """Deletes the specified mobile network site. This will also delete any network functions that are
+        a part of this site.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
@@ -138,25 +137,24 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 mobile_network_name=mobile_network_name,
+                site_name=site_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
@@ -179,289 +177,302 @@
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}"
     }
 
     @distributed_trace_async
-    async def get(self, resource_group_name: str, mobile_network_name: str, **kwargs: Any) -> _models.MobileNetwork:
-        """Gets information about the specified mobile network.
+    async def get(
+        self, resource_group_name: str, mobile_network_name: str, site_name: str, **kwargs: Any
+    ) -> _models.Site:
+        """Gets information about the specified mobile network site.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: MobileNetwork or the result of cls(response)
-        :rtype: ~azure.mgmt.mobilenetwork.models.MobileNetwork
+        :return: Site or the result of cls(response)
+        :rtype: ~azure.mgmt.mobilenetwork.models.Site
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.MobileNetwork] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.Site] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
+            site_name=site_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("MobileNetwork", pipeline_response)
+        deserialized = self._deserialize("Site", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}"
     }
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         mobile_network_name: str,
-        parameters: Union[_models.MobileNetwork, IO],
+        site_name: str,
+        parameters: Union[_models.Site, IO],
         **kwargs: Any
-    ) -> _models.MobileNetwork:
+    ) -> _models.Site:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.MobileNetwork] = kwargs.pop("cls", None)
+        cls: ClsType[_models.Site] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
-            _json = self._serialize.body(parameters, "MobileNetwork")
+            _json = self._serialize.body(parameters, "Site")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
+            site_name=site_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize("MobileNetwork", pipeline_response)
+            deserialized = self._deserialize("Site", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize("MobileNetwork", pipeline_response)
+            deserialized = self._deserialize("Site", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}"
     }
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         mobile_network_name: str,
-        parameters: _models.MobileNetwork,
+        site_name: str,
+        parameters: _models.Site,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.MobileNetwork]:
-        """Creates or updates a mobile network.
+    ) -> AsyncLROPoller[_models.Site]:
+        """Creates or updates a mobile network site. Must be created in the same location as its parent
+        mobile network.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param parameters: Parameters supplied to the create or update mobile network operation.
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
+        :param parameters: Parameters supplied to the create or update mobile network site operation.
          Required.
-        :type parameters: ~azure.mgmt.mobilenetwork.models.MobileNetwork
+        :type parameters: ~azure.mgmt.mobilenetwork.models.Site
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MobileNetwork or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.MobileNetwork]
+        :return: An instance of AsyncLROPoller that returns either Site or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.Site]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         mobile_network_name: str,
+        site_name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.MobileNetwork]:
-        """Creates or updates a mobile network.
+    ) -> AsyncLROPoller[_models.Site]:
+        """Creates or updates a mobile network site. Must be created in the same location as its parent
+        mobile network.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param parameters: Parameters supplied to the create or update mobile network operation.
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
+        :param parameters: Parameters supplied to the create or update mobile network site operation.
          Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MobileNetwork or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.MobileNetwork]
+        :return: An instance of AsyncLROPoller that returns either Site or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.Site]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         mobile_network_name: str,
-        parameters: Union[_models.MobileNetwork, IO],
+        site_name: str,
+        parameters: Union[_models.Site, IO],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.MobileNetwork]:
-        """Creates or updates a mobile network.
+    ) -> AsyncLROPoller[_models.Site]:
+        """Creates or updates a mobile network site. Must be created in the same location as its parent
+        mobile network.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param parameters: Parameters supplied to the create or update mobile network operation. Is
-         either a model type or a IO type. Required.
-        :type parameters: ~azure.mgmt.mobilenetwork.models.MobileNetwork or IO
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
+        :param parameters: Parameters supplied to the create or update mobile network site operation.
+         Is either a Site type or a IO type. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.Site or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MobileNetwork or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.MobileNetwork]
+        :return: An instance of AsyncLROPoller that returns either Site or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.Site]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.MobileNetwork] = kwargs.pop("cls", None)
+        cls: ClsType[_models.Site] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 mobile_network_name=mobile_network_name,
+                site_name=site_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("MobileNetwork", pipeline_response)
+            deserialized = self._deserialize("Site", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
@@ -477,193 +488,209 @@
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}"
     }
 
     @overload
     async def update_tags(
         self,
         resource_group_name: str,
         mobile_network_name: str,
+        site_name: str,
         parameters: _models.TagsObject,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.MobileNetwork:
-        """Updates mobile network tags.
+    ) -> _models.Site:
+        """Updates site tags.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param parameters: Parameters supplied to update mobile network tags. Required.
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
+        :param parameters: Parameters supplied to update network site tags. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: MobileNetwork or the result of cls(response)
-        :rtype: ~azure.mgmt.mobilenetwork.models.MobileNetwork
+        :return: Site or the result of cls(response)
+        :rtype: ~azure.mgmt.mobilenetwork.models.Site
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def update_tags(
         self,
         resource_group_name: str,
         mobile_network_name: str,
+        site_name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.MobileNetwork:
-        """Updates mobile network tags.
+    ) -> _models.Site:
+        """Updates site tags.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param parameters: Parameters supplied to update mobile network tags. Required.
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
+        :param parameters: Parameters supplied to update network site tags. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: MobileNetwork or the result of cls(response)
-        :rtype: ~azure.mgmt.mobilenetwork.models.MobileNetwork
+        :return: Site or the result of cls(response)
+        :rtype: ~azure.mgmt.mobilenetwork.models.Site
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update_tags(
         self,
         resource_group_name: str,
         mobile_network_name: str,
+        site_name: str,
         parameters: Union[_models.TagsObject, IO],
         **kwargs: Any
-    ) -> _models.MobileNetwork:
-        """Updates mobile network tags.
+    ) -> _models.Site:
+        """Updates site tags.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param parameters: Parameters supplied to update mobile network tags. Is either a model type or
-         a IO type. Required.
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
+        :param parameters: Parameters supplied to update network site tags. Is either a TagsObject type
+         or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: MobileNetwork or the result of cls(response)
-        :rtype: ~azure.mgmt.mobilenetwork.models.MobileNetwork
+        :return: Site or the result of cls(response)
+        :rtype: ~azure.mgmt.mobilenetwork.models.Site
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.MobileNetwork] = kwargs.pop("cls", None)
+        cls: ClsType[_models.Site] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
+            site_name=site_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("MobileNetwork", pipeline_response)
+        deserialized = self._deserialize("Site", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     update_tags.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}"
     }
 
     @distributed_trace
-    def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.MobileNetwork"]:
-        """Lists all the mobile networks in a subscription.
+    def list_by_mobile_network(
+        self, resource_group_name: str, mobile_network_name: str, **kwargs: Any
+    ) -> AsyncIterable["_models.Site"]:
+        """Lists all sites in the mobile network.
 
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param mobile_network_name: The name of the mobile network. Required.
+        :type mobile_network_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either MobileNetwork or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.MobileNetwork]
+        :return: An iterator like instance of either Site or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.Site]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.MobileNetworkListResult] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SiteListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_subscription_request(
+                request = build_list_by_mobile_network_request(
+                    resource_group_name=resource_group_name,
+                    mobile_network_name=mobile_network_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_subscription.metadata["url"],
+                    template_url=self.list_by_mobile_network.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
 
             else:
@@ -681,121 +708,261 @@
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("MobileNetworkListResult", pipeline_response)
+            deserialized = self._deserialize("SiteListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_subscription.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.MobileNetwork/mobileNetworks"
+    list_by_mobile_network.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites"
     }
 
-    @distributed_trace
-    def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> AsyncIterable["_models.MobileNetwork"]:
-        """Lists all the mobile networks in a resource group.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either MobileNetwork or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.MobileNetwork]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.MobileNetworkListResult] = kwargs.pop("cls", None)
-
+    async def _delete_packet_core_initial(  # pylint: disable=inconsistent-return-statements
+        self,
+        resource_group_name: str,
+        mobile_network_name: str,
+        site_name: str,
+        parameters: Union[_models.SiteDeletePacketCore, IO],
+        **kwargs: Any
+    ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        def prepare_request(next_link=None):
-            if not next_link:
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-                request = build_list_by_resource_group_request(
-                    resource_group_name=resource_group_name,
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(parameters, (IOBase, bytes)):
+            _content = parameters
+        else:
+            _json = self._serialize.body(parameters, "SiteDeletePacketCore")
 
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("MobileNetworkListResult", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+        request = build_delete_packet_core_request(
+            resource_group_name=resource_group_name,
+            mobile_network_name=mobile_network_name,
+            site_name=site_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self._delete_packet_core_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
 
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
-            )
-            response = pipeline_response.http_response
+        response = pipeline_response.http_response
 
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-            return pipeline_response
+        if cls:
+            return cls(pipeline_response, None, {})
 
-        return AsyncItemPaged(get_next, extract_data)
+    _delete_packet_core_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}/deletePacketCore"
+    }
+
+    @overload
+    async def begin_delete_packet_core(
+        self,
+        resource_group_name: str,
+        mobile_network_name: str,
+        site_name: str,
+        parameters: _models.SiteDeletePacketCore,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[None]:
+        """Deletes a packet core under the specified mobile network site.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param mobile_network_name: The name of the mobile network. Required.
+        :type mobile_network_name: str
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
+        :param parameters: Parameters supplied to delete a packet core under a site. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.SiteDeletePacketCore
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def begin_delete_packet_core(
+        self,
+        resource_group_name: str,
+        mobile_network_name: str,
+        site_name: str,
+        parameters: IO,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[None]:
+        """Deletes a packet core under the specified mobile network site.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param mobile_network_name: The name of the mobile network. Required.
+        :type mobile_network_name: str
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
+        :param parameters: Parameters supplied to delete a packet core under a site. Required.
+        :type parameters: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def begin_delete_packet_core(
+        self,
+        resource_group_name: str,
+        mobile_network_name: str,
+        site_name: str,
+        parameters: Union[_models.SiteDeletePacketCore, IO],
+        **kwargs: Any
+    ) -> AsyncLROPoller[None]:
+        """Deletes a packet core under the specified mobile network site.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param mobile_network_name: The name of the mobile network. Required.
+        :type mobile_network_name: str
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
+        :param parameters: Parameters supplied to delete a packet core under a site. Is either a
+         SiteDeletePacketCore type or a IO type. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.SiteDeletePacketCore or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._delete_packet_core_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                mobile_network_name=mobile_network_name,
+                site_name=site_name,
+                parameters=parameters,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+            if cls:
+                return cls(pipeline_response, None, {})
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks"
+    begin_delete_packet_core.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}/deletePacketCore"
     }
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,80 +2,95 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
-from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._operations import build_list_request
-
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
+
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_list_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/providers/Microsoft.MobileNetwork/operations")
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.mobilenetwork.aio.MobileNetworkManagementClient`'s
+        :class:`~azure.mgmt.mobilenetwork.MobileNetworkManagementClient`'s
         :attr:`operations` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.Operation"]:
+    def list(self, **kwargs: Any) -> Iterable["_models.Operation"]:
         """Gets a list of the operations.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Operation or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.Operation]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -108,32 +123,33 @@
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
-        async def extract_data(pipeline_response):
+        def extract_data(pipeline_response):
             deserialized = self._deserialize("OperationList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+            return deserialized.next_link or None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
+        def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(get_next, extract_data)
+        return ItemPaged(get_next, extract_data)
 
     list.metadata = {"url": "/providers/Microsoft.MobileNetwork/operations"}
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_data_planes_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_data_planes_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -35,18 +35,14 @@
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_packet_core_control_plane_request,
     build_update_tags_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class PacketCoreDataPlanesOperations:
     """
     .. warning::
@@ -80,17 +76,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             packet_core_data_plane_name=packet_core_data_plane_name,
             subscription_id=self._config.subscription_id,
@@ -98,16 +92,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -148,17 +143,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -226,17 +219,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PacketCoreDataPlane] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             packet_core_data_plane_name=packet_core_data_plane_name,
             subscription_id=self._config.subscription_id,
@@ -244,16 +235,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -285,24 +277,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PacketCoreDataPlane] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "PacketCoreDataPlane")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
@@ -315,16 +305,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -445,15 +436,15 @@
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
         :param packet_core_data_plane_name: The name of the packet core data plane. Required.
         :type packet_core_data_plane_name: str
         :param parameters: Parameters supplied to the create or update packet core data plane
-         operation. Is either a model type or a IO type. Required.
+         operation. Is either a PacketCoreDataPlane type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.PacketCoreDataPlane or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -467,17 +458,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.PacketCoreDataPlane]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PacketCoreDataPlane] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -598,16 +587,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
         :param packet_core_data_plane_name: The name of the packet core data plane. Required.
         :type packet_core_data_plane_name: str
-        :param parameters: Parameters supplied to update packet core data plane tags. Is either a model
-         type or a IO type. Required.
+        :param parameters: Parameters supplied to update packet core data plane tags. Is either a
+         TagsObject type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PacketCoreDataPlane or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.PacketCoreDataPlane
@@ -620,24 +609,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PacketCoreDataPlane] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
@@ -650,16 +637,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -692,17 +680,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.PacketCoreDataPlane]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PacketCoreDataPlaneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -748,16 +734,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_patch.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_planes_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_planes_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -39,18 +39,14 @@
     build_list_by_resource_group_request,
     build_list_by_subscription_request,
     build_reinstall_request,
     build_rollback_request,
     build_update_tags_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class PacketCoreControlPlanesOperations:
     """
     .. warning::
@@ -80,33 +76,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -141,17 +136,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -212,33 +205,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PacketCoreControlPlane] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -269,24 +261,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PacketCoreControlPlane] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "PacketCoreControlPlane")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
@@ -298,16 +288,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -416,15 +407,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
         :param parameters: Parameters supplied to the create or update packet core control plane
-         operation. Is either a model type or a IO type. Required.
+         operation. Is either a PacketCoreControlPlane type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -438,17 +429,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PacketCoreControlPlane] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -493,28 +482,28 @@
     }
 
     @overload
     async def update_tags(
         self,
         resource_group_name: str,
         packet_core_control_plane_name: str,
-        parameters: _models.TagsObject,
+        parameters: _models.IdentityAndTagsObject,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.PacketCoreControlPlane:
-        """Updates packet core control planes tags.
+        """Patch packet core control plane resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
-        :param parameters: Parameters supplied to update packet core control plane tags. Required.
-        :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject
+        :param parameters: Parameters supplied to patch packet core control plane resource. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.IdentityAndTagsObject
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PacketCoreControlPlane or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -526,22 +515,22 @@
         resource_group_name: str,
         packet_core_control_plane_name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.PacketCoreControlPlane:
-        """Updates packet core control planes tags.
+        """Patch packet core control plane resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
-        :param parameters: Parameters supplied to update packet core control plane tags. Required.
+        :param parameters: Parameters supplied to patch packet core control plane resource. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PacketCoreControlPlane or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane
@@ -549,27 +538,27 @@
         """
 
     @distributed_trace_async
     async def update_tags(
         self,
         resource_group_name: str,
         packet_core_control_plane_name: str,
-        parameters: Union[_models.TagsObject, IO],
+        parameters: Union[_models.IdentityAndTagsObject, IO],
         **kwargs: Any
     ) -> _models.PacketCoreControlPlane:
-        """Updates packet core control planes tags.
+        """Patch packet core control plane resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
-        :param parameters: Parameters supplied to update packet core control plane tags. Is either a
-         model type or a IO type. Required.
-        :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
+        :param parameters: Parameters supplied to patch packet core control plane resource. Is either a
+         IdentityAndTagsObject type or a IO type. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.IdentityAndTagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PacketCoreControlPlane or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -581,27 +570,25 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PacketCoreControlPlane] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
-            _json = self._serialize.body(parameters, "TagsObject")
+            _json = self._serialize.body(parameters, "IdentityAndTagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
@@ -610,16 +597,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -646,17 +634,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PacketCoreControlPlaneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -700,16 +686,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -737,17 +724,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PacketCoreControlPlaneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -792,16 +777,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -824,33 +810,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.AsyncOperationStatus]] = kwargs.pop("cls", None)
 
         request = build_rollback_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._rollback_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -894,17 +879,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.AsyncOperationStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AsyncOperationStatus] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._rollback_initial(
                 resource_group_name=resource_group_name,
@@ -954,33 +937,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.AsyncOperationStatus]] = kwargs.pop("cls", None)
 
         request = build_reinstall_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._reinstall_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1025,17 +1007,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.AsyncOperationStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AsyncOperationStatus] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._reinstall_initial(
                 resource_group_name=resource_group_name,
@@ -1089,24 +1069,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.AsyncOperationStatus]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "PacketCoreControlPlaneCollectDiagnosticsPackage")
 
         request = build_collect_diagnostics_package_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
@@ -1118,16 +1096,17 @@
             template_url=self._collect_diagnostics_package_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1238,15 +1217,16 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
         :param parameters: Parameters supplied to the packet core control plane collect diagnostics
-         package operation. Is either a model type or a IO type. Required.
+         package operation. Is either a PacketCoreControlPlaneCollectDiagnosticsPackage type or a IO
+         type. Required.
         :type parameters:
          ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlaneCollectDiagnosticsPackage or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
@@ -1261,17 +1241,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.mobilenetwork.models.AsyncOperationStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AsyncOperationStatus] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._collect_diagnostics_package_initial(
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/_mobile_network_management_client_enums.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/_mobile_network_management_client_enums.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,156 +9,188 @@
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
 
 
 class AuthenticationType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """How to authenticate users who access local diagnostics APIs."""
 
-    #: Use AAD SSO to authenticate the user (this requires internet access).
     AAD = "AAD"
-    #: Use locally stored passwords to authenticate the user.
+    """Use AAD SSO to authenticate the user (this requires internet access)."""
     PASSWORD = "Password"
+    """Use locally stored passwords to authenticate the user."""
 
 
 class BillingSku(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The SKU of the packet core control plane resource. The SKU list may change over time when a new
     SKU gets added or an exiting SKU gets removed.
     """
 
-    #: 100 Mbps, 20 active SIMs plan
     G0 = "G0"
-    #: 1 Gbps, 100 active SIMs plan
+    """100 Mbps, 20 active SIMs plan, 2 RANs"""
     G1 = "G1"
-    #: 2 Gbps, 200 active SIMs plan
+    """1 Gbps, 100 active SIMs plan, 5 RANs"""
     G2 = "G2"
-    #: 3 Gbps, 300 active SIMs plan
-    G3 = "G3"
-    #: 4 Gbps, 400 active SIMs plan
-    G4 = "G4"
-    #: 5 Gbps, 500 active SIMs plan
+    """2 Gbps, 200 active SIMs plan, 10 RANs"""
     G5 = "G5"
-    #: 10 Gbps, 1000 active SIMs plan
+    """5 Gbps, 500 active SIMs plan"""
     G10 = "G10"
+    """10 Gbps, 1000 active SIMs plan"""
 
 
 class CertificateProvisioningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The certificate's provisioning state."""
 
-    #: The certificate has not been provisioned.
     NOT_PROVISIONED = "NotProvisioned"
-    #: The certificate has been provisioned.
+    """The certificate has not been provisioned."""
     PROVISIONED = "Provisioned"
-    #: The certificate failed to be provisioned. The "reason" property explains why.
+    """The certificate has been provisioned."""
     FAILED = "Failed"
+    """The certificate failed to be provisioned. The "reason" property explains why."""
 
 
 class CoreNetworkType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """The core network technology generation (5G core or EPC / 4G core)."""
+    """The core network technology generation (5G core, EPC / 4G core or EPC / 4G + 5G core)."""
 
-    #: 5G core
     FIVE_GC = "5GC"
-    #: EPC / 4G core
+    """5G core"""
     EPC = "EPC"
+    """EPC / 4G core"""
+    EPC5_GC = "EPC + 5GC"
+    """Combined EPC / 4G and 5G core"""
 
 
 class CreatedByType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of identity that created the resource."""
 
     USER = "User"
     APPLICATION = "Application"
     MANAGED_IDENTITY = "ManagedIdentity"
     KEY = "Key"
 
 
+class DesiredInstallationState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The desired installation state of the packet core."""
+
+    UNINSTALLED = "Uninstalled"
+    """Don't install the packet core."""
+    INSTALLED = "Installed"
+    """Install the packet core."""
+
+
+class DiagnosticsPackageStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The status of the diagnostics package collection."""
+
+    NOT_STARTED = "NotStarted"
+    COLLECTING = "Collecting"
+    COLLECTED = "Collected"
+    ERROR = "Error"
+
+
+class InstallationReason(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The reason for the installation state of the packet core."""
+
+    NO_SLICES = "NoSlices"
+    """The mobile network does not have any applicable configured slices."""
+    NO_PACKET_CORE_DATA_PLANE = "NoPacketCoreDataPlane"
+    """There is no configured data plane for this packet core."""
+    NO_ATTACHED_DATA_NETWORKS = "NoAttachedDataNetworks"
+    """The packet core has no attached data networks."""
+
+
 class InstallationState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The installation state of the packet core."""
 
-    #: The packet core is uninstalled.
     UNINSTALLED = "Uninstalled"
-    #: The packet core is installing.
+    """The packet core is uninstalled."""
     INSTALLING = "Installing"
-    #: The packet core is installed.
+    """The packet core is installing."""
     INSTALLED = "Installed"
-    #: The packet core is updating its configuration.
+    """The packet core is installed."""
     UPDATING = "Updating"
-    #: The packet core is upgrading to a different software version.
+    """The packet core is updating its configuration."""
     UPGRADING = "Upgrading"
-    #: The packet core is uninstalling.
+    """The packet core is upgrading to a different software version."""
     UNINSTALLING = "Uninstalling"
-    #: The packet core is reinstalling.
+    """The packet core is uninstalling."""
     REINSTALLING = "Reinstalling"
-    #: The packet core is rolling back to its previous version.
+    """The packet core is reinstalling."""
     ROLLING_BACK = "RollingBack"
-    #: The packet core is in failed state.
+    """The packet core is rolling back to its previous version."""
     FAILED = "Failed"
+    """The packet core is in failed state."""
 
 
 class ManagedServiceIdentityType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Type of managed service identity (where both SystemAssigned and UserAssigned types are
-    allowed).
-    """
+    """Type of managed service identity (currently only UserAssigned allowed)."""
 
     NONE = "None"
-    SYSTEM_ASSIGNED = "SystemAssigned"
     USER_ASSIGNED = "UserAssigned"
-    SYSTEM_ASSIGNED_USER_ASSIGNED = "SystemAssigned,UserAssigned"
 
 
 class NaptEnabled(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Whether network address and port translation is enabled."""
 
-    #: NAPT is enabled
     ENABLED = "Enabled"
-    #: NAPT is disabled
+    """NAPT is enabled"""
     DISABLED = "Disabled"
+    """NAPT is disabled"""
 
 
 class ObsoleteVersion(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Indicates whether this version is obsolete."""
 
-    #: This version is obsolete for use in new packet core control plane deployments.
     OBSOLETE = "Obsolete"
-    #: This version is not obsolete for use in new packet core control plane deployments.
+    """This version is obsolete for use in new packet core control plane deployments."""
     NOT_OBSOLETE = "NotObsolete"
+    """This version is not obsolete for use in new packet core control plane deployments."""
+
+
+class PacketCaptureStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The status of the packet capture session."""
+
+    NOT_STARTED = "NotStarted"
+    RUNNING = "Running"
+    STOPPED = "Stopped"
+    ERROR = "Error"
 
 
 class PduSessionType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """PDU session type (IPv4/IPv6)."""
 
     I_PV4 = "IPv4"
     I_PV6 = "IPv6"
 
 
 class PlatformType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The platform type where packet core is deployed. The contents of this enum can change."""
 
-    #: If this option is chosen, you must set one of "azureStackEdgeDevice", "connectedCluster" or
-    #: "customLocation". If multiple are set, they must be consistent with each other.
     AKS_HCI = "AKS-HCI"
-    #: If this option is chosen, you must set one of "azureStackHciCluster", "connectedCluster" or
-    #: "customLocation". If multiple are set, they must be consistent with each other.
+    """If this option is chosen, you must set one of "azureStackEdgeDevice", "connectedCluster" or
+    #: "customLocation". If multiple are set, they must be consistent with each other."""
     THREE_P_AZURE_STACK_HCI = "3P-AZURE-STACK-HCI"
+    """If this option is chosen, you must set one of "azureStackHciCluster", "connectedCluster" or
+    #: "customLocation". If multiple are set, they must be consistent with each other."""
 
 
 class PreemptionCapability(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Preemption capability."""
 
-    #: Cannot preempt
     NOT_PREEMPT = "NotPreempt"
-    #: May preempt
+    """Cannot preempt"""
     MAY_PREEMPT = "MayPreempt"
+    """May preempt"""
 
 
 class PreemptionVulnerability(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Preemption vulnerability."""
 
-    #: Cannot be preempted
     NOT_PREEMPTABLE = "NotPreemptable"
-    #: May be preempted
+    """Cannot be preempted"""
     PREEMPTABLE = "Preemptable"
+    """May be preempted"""
 
 
 class ProvisioningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The current provisioning state."""
 
     UNKNOWN = "Unknown"
     SUCCEEDED = "Succeeded"
@@ -170,76 +202,85 @@
 
 
 class RecommendedVersion(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Indicates whether this is the recommended version to use for new packet core control plane
     deployments.
     """
 
-    #: This is the recommended version to use for new packet core control plane deployments.
     RECOMMENDED = "Recommended"
-    #: This is not the recommended version to use for new packet core control plane deployments.
+    """This is the recommended version to use for new packet core control plane deployments."""
     NOT_RECOMMENDED = "NotRecommended"
+    """This is not the recommended version to use for new packet core control plane deployments."""
+
+
+class ReinstallRequired(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Whether a reinstall of the packet core is required to pick up the latest configuration changes."""
+
+    REQUIRED = "Required"
+    """A reinstall of the packet core is required."""
+    NOT_REQUIRED = "NotRequired"
+    """A reinstall of the packet core is not required."""
 
 
 class SdfDirection(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Service data flow direction."""
 
-    #: Traffic flowing from the UE to the data network.
     UPLINK = "Uplink"
-    #: Traffic flowing from the data network to the UE.
+    """Traffic flowing from the UE to the data network."""
     DOWNLINK = "Downlink"
-    #: Traffic flowing both to and from the UE.
+    """Traffic flowing from the data network to the UE."""
     BIDIRECTIONAL = "Bidirectional"
+    """Traffic flowing both to and from the UE."""
 
 
 class SimState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The state of the SIM resource."""
 
-    #: The SIM is disabled because not all configuration required for enabling is present.
     DISABLED = "Disabled"
-    #: The SIM is enabled.
+    """The SIM is disabled because not all configuration required for enabling is present."""
     ENABLED = "Enabled"
-    #: The SIM cannot be enabled because some of the associated configuration is invalid.
+    """The SIM is enabled."""
     INVALID = "Invalid"
+    """The SIM cannot be enabled because some of the associated configuration is invalid."""
 
 
 class SiteProvisioningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The provisioning state of a resource e.g. SIM/SIM policy on a site."""
 
-    #: The resource should not be provisioned on this site.
     NOT_APPLICABLE = "NotApplicable"
-    #: The resource is being added to this site.
+    """The resource should not be provisioned on this site."""
     ADDING = "Adding"
-    #: The resource is being updated on this site.
+    """The resource is being added to this site."""
     UPDATING = "Updating"
-    #: The resource is being deleted from this site.
+    """The resource is being updated on this site."""
     DELETING = "Deleting"
-    #: The resource is provisioned on this site.
+    """The resource is being deleted from this site."""
     PROVISIONED = "Provisioned"
-    #: The resource failed to be provisioned on this site.
+    """The resource is provisioned on this site."""
     FAILED = "Failed"
+    """The resource failed to be provisioned on this site."""
 
 
 class TrafficControlPermission(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Traffic control permission."""
 
-    #: Traffic matching this rule is allowed to flow.
     ENABLED = "Enabled"
-    #: Traffic matching this rule is not allowed to flow.
+    """Traffic matching this rule is allowed to flow."""
     BLOCKED = "Blocked"
+    """Traffic matching this rule is not allowed to flow."""
 
 
 class VersionState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The state of this packet core control plane version."""
 
-    #: The state of this version is unknown.
     UNKNOWN = "Unknown"
-    #: This version is a preview and is not suitable for production use.
+    """The state of this version is unknown."""
     PREVIEW = "Preview"
-    #: This version is currently being validated.
+    """This version is a preview and is not suitable for production use."""
     VALIDATING = "Validating"
-    #: This version failed validation.
+    """This version is currently being validated."""
     VALIDATION_FAILED = "ValidationFailed"
-    #: This version is active and suitable for production use.
+    """This version failed validation."""
     ACTIVE = "Active"
-    #: This version is deprecated and is no longer supported.
+    """This version is active and suitable for production use."""
     DEPRECATED = "Deprecated"
+    """This version is deprecated and is no longer supported."""
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/__init__.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,35 +19,42 @@
 from ._models_py3 import CommonSimPropertiesFormat
 from ._models_py3 import ConnectedClusterResourceId
 from ._models_py3 import CustomLocationResourceId
 from ._models_py3 import DataNetwork
 from ._models_py3 import DataNetworkConfiguration
 from ._models_py3 import DataNetworkListResult
 from ._models_py3 import DataNetworkResourceId
+from ._models_py3 import DiagnosticsPackage
+from ._models_py3 import DiagnosticsPackageListResult
+from ._models_py3 import DiagnosticsUploadConfiguration
 from ._models_py3 import EncryptedSimPropertiesFormat
 from ._models_py3 import EncryptedSimUploadList
 from ._models_py3 import ErrorAdditionalInfo
 from ._models_py3 import ErrorDetail
 from ._models_py3 import ErrorResponse
 from ._models_py3 import HttpsServerCertificate
+from ._models_py3 import IdentityAndTagsObject
 from ._models_py3 import Installation
 from ._models_py3 import InterfaceProperties
 from ._models_py3 import KeyVaultKey
 from ._models_py3 import LocalDiagnosticsAccessConfiguration
 from ._models_py3 import ManagedServiceIdentity
 from ._models_py3 import MobileNetwork
 from ._models_py3 import MobileNetworkListResult
 from ._models_py3 import MobileNetworkResourceId
 from ._models_py3 import NaptConfiguration
 from ._models_py3 import Operation
 from ._models_py3 import OperationDisplay
 from ._models_py3 import OperationList
+from ._models_py3 import PacketCapture
+from ._models_py3 import PacketCaptureListResult
 from ._models_py3 import PacketCoreControlPlane
 from ._models_py3 import PacketCoreControlPlaneCollectDiagnosticsPackage
 from ._models_py3 import PacketCoreControlPlaneListResult
+from ._models_py3 import PacketCoreControlPlaneResourceId
 from ._models_py3 import PacketCoreControlPlaneVersion
 from ._models_py3 import PacketCoreControlPlaneVersionListResult
 from ._models_py3 import PacketCoreDataPlane
 from ._models_py3 import PacketCoreDataPlaneListResult
 from ._models_py3 import PccRuleConfiguration
 from ._models_py3 import PccRuleQosPolicy
 from ._models_py3 import PinholeTimeouts
@@ -75,14 +82,15 @@
 from ._models_py3 import SimPolicyListResult
 from ._models_py3 import SimPolicyResourceId
 from ._models_py3 import SimPropertiesFormat
 from ._models_py3 import SimStaticIpProperties
 from ._models_py3 import SimStaticIpPropertiesStaticIp
 from ._models_py3 import SimUploadList
 from ._models_py3 import Site
+from ._models_py3 import SiteDeletePacketCore
 from ._models_py3 import SiteListResult
 from ._models_py3 import SiteResourceId
 from ._models_py3 import Slice
 from ._models_py3 import SliceConfiguration
 from ._models_py3 import SliceListResult
 from ._models_py3 import SliceResourceId
 from ._models_py3 import Snssai
@@ -93,24 +101,29 @@
 from ._models_py3 import UserAssignedIdentity
 
 from ._mobile_network_management_client_enums import AuthenticationType
 from ._mobile_network_management_client_enums import BillingSku
 from ._mobile_network_management_client_enums import CertificateProvisioningState
 from ._mobile_network_management_client_enums import CoreNetworkType
 from ._mobile_network_management_client_enums import CreatedByType
+from ._mobile_network_management_client_enums import DesiredInstallationState
+from ._mobile_network_management_client_enums import DiagnosticsPackageStatus
+from ._mobile_network_management_client_enums import InstallationReason
 from ._mobile_network_management_client_enums import InstallationState
 from ._mobile_network_management_client_enums import ManagedServiceIdentityType
 from ._mobile_network_management_client_enums import NaptEnabled
 from ._mobile_network_management_client_enums import ObsoleteVersion
+from ._mobile_network_management_client_enums import PacketCaptureStatus
 from ._mobile_network_management_client_enums import PduSessionType
 from ._mobile_network_management_client_enums import PlatformType
 from ._mobile_network_management_client_enums import PreemptionCapability
 from ._mobile_network_management_client_enums import PreemptionVulnerability
 from ._mobile_network_management_client_enums import ProvisioningState
 from ._mobile_network_management_client_enums import RecommendedVersion
+from ._mobile_network_management_client_enums import ReinstallRequired
 from ._mobile_network_management_client_enums import SdfDirection
 from ._mobile_network_management_client_enums import SimState
 from ._mobile_network_management_client_enums import SiteProvisioningState
 from ._mobile_network_management_client_enums import TrafficControlPermission
 from ._mobile_network_management_client_enums import VersionState
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
@@ -130,35 +143,42 @@
     "CommonSimPropertiesFormat",
     "ConnectedClusterResourceId",
     "CustomLocationResourceId",
     "DataNetwork",
     "DataNetworkConfiguration",
     "DataNetworkListResult",
     "DataNetworkResourceId",
+    "DiagnosticsPackage",
+    "DiagnosticsPackageListResult",
+    "DiagnosticsUploadConfiguration",
     "EncryptedSimPropertiesFormat",
     "EncryptedSimUploadList",
     "ErrorAdditionalInfo",
     "ErrorDetail",
     "ErrorResponse",
     "HttpsServerCertificate",
+    "IdentityAndTagsObject",
     "Installation",
     "InterfaceProperties",
     "KeyVaultKey",
     "LocalDiagnosticsAccessConfiguration",
     "ManagedServiceIdentity",
     "MobileNetwork",
     "MobileNetworkListResult",
     "MobileNetworkResourceId",
     "NaptConfiguration",
     "Operation",
     "OperationDisplay",
     "OperationList",
+    "PacketCapture",
+    "PacketCaptureListResult",
     "PacketCoreControlPlane",
     "PacketCoreControlPlaneCollectDiagnosticsPackage",
     "PacketCoreControlPlaneListResult",
+    "PacketCoreControlPlaneResourceId",
     "PacketCoreControlPlaneVersion",
     "PacketCoreControlPlaneVersionListResult",
     "PacketCoreDataPlane",
     "PacketCoreDataPlaneListResult",
     "PccRuleConfiguration",
     "PccRuleQosPolicy",
     "PinholeTimeouts",
@@ -186,14 +206,15 @@
     "SimPolicyListResult",
     "SimPolicyResourceId",
     "SimPropertiesFormat",
     "SimStaticIpProperties",
     "SimStaticIpPropertiesStaticIp",
     "SimUploadList",
     "Site",
+    "SiteDeletePacketCore",
     "SiteListResult",
     "SiteResourceId",
     "Slice",
     "SliceConfiguration",
     "SliceListResult",
     "SliceResourceId",
     "Snssai",
@@ -203,24 +224,29 @@
     "TrackedResource",
     "UserAssignedIdentity",
     "AuthenticationType",
     "BillingSku",
     "CertificateProvisioningState",
     "CoreNetworkType",
     "CreatedByType",
+    "DesiredInstallationState",
+    "DiagnosticsPackageStatus",
+    "InstallationReason",
     "InstallationState",
     "ManagedServiceIdentityType",
     "NaptEnabled",
     "ObsoleteVersion",
+    "PacketCaptureStatus",
     "PduSessionType",
     "PlatformType",
     "PreemptionCapability",
     "PreemptionVulnerability",
     "ProvisioningState",
     "RecommendedVersion",
+    "ReinstallRequired",
     "SdfDirection",
     "SimState",
     "SiteProvisioningState",
     "TrafficControlPermission",
     "VersionState",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/_patch.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/models/_models_py3.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/models/_models_py3.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     }
 
     _attribute_map = {
         "uplink": {"key": "uplink", "type": "str"},
         "downlink": {"key": "downlink", "type": "str"},
     }
 
-    def __init__(self, *, uplink: str, downlink: str, **kwargs):
+    def __init__(self, *, uplink: str, downlink: str, **kwargs: Any) -> None:
         """
         :keyword uplink: Uplink bit rate. Required.
         :paramtype uplink: str
         :keyword downlink: Downlink bit rate. Required.
         :paramtype downlink: str
         """
         super().__init__(**kwargs)
@@ -86,16 +86,16 @@
 
     def __init__(
         self,
         *,
         priority_level: int,
         preempt_cap: Union[str, "_models.PreemptionCapability"],
         preempt_vuln: Union[str, "_models.PreemptionVulnerability"],
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword priority_level: ARP priority level. Required.
         :paramtype priority_level: int
         :keyword preempt_cap: ARP preemption capability. Required. Known values are: "NotPreempt" and
          "MayPreempt".
         :paramtype preempt_cap: str or ~azure.mgmt.mobilenetwork.models.PreemptionCapability
         :keyword preempt_vuln: ARP preemption vulnerability. Required. Known values are:
@@ -124,15 +124,15 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Azure Async Operation ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -188,16 +188,16 @@
         name: Optional[str] = None,
         resource_id: Optional[str] = None,
         start_time: Optional[datetime.datetime] = None,
         end_time: Optional[datetime.datetime] = None,
         percent_complete: Optional[float] = None,
         properties: Optional[JSON] = None,
         error: Optional["_models.ErrorDetail"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword id: Fully qualified ID for the async operation.
         :paramtype id: str
         :keyword name: Name of the async operation.
         :paramtype name: str
         :keyword status: The operation status. Required.
         :paramtype status: str
@@ -228,16 +228,16 @@
 
 
 class Resource(_serialization.Model):
     """Common fields that are returned in the response for all Azure Resource Manager resources.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -255,32 +255,33 @@
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.system_data = None
 
 
 class TrackedResource(Resource):
-    """The resource model definition for an Azure Resource Manager tracked top level resource which has 'tags' and a 'location'.
+    """The resource model definition for an Azure Resource Manager tracked top level resource which
+    has 'tags' and a 'location'.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -305,35 +306,36 @@
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
     }
 
-    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         """
         super().__init__(**kwargs)
         self.tags = tags
         self.location = location
 
 
 class AttachedDataNetwork(TrackedResource):  # pylint: disable=too-many-instance-attributes
-    """Attached data network resource. Must be created in the same location as its parent packet core data plane.
+    """Attached data network resource. Must be created in the same location as its parent packet core
+    data plane.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -413,16 +415,16 @@
         location: str,
         user_plane_data_interface: "_models.InterfaceProperties",
         dns_addresses: List[str],
         tags: Optional[Dict[str, str]] = None,
         napt_configuration: Optional["_models.NaptConfiguration"] = None,
         user_equipment_address_pool_prefix: Optional[List[str]] = None,
         user_equipment_static_address_pool_prefix: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword user_plane_data_interface: The user plane interface on the data network. For 5G
          networks, this is the N6 interface. For 4G networks, this is the SGi interface. Required.
@@ -477,15 +479,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[AttachedDataNetwork]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.AttachedDataNetwork"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.AttachedDataNetwork"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: A list of data networks in a resource group.
         :paramtype value: list[~azure.mgmt.mobilenetwork.models.AttachedDataNetwork]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -507,15 +509,15 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Attached data network resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -536,15 +538,15 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Azure Stack Edge device resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -565,15 +567,15 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Azure Stack HCI cluster resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -596,15 +598,15 @@
     }
 
     _attribute_map = {
         "state": {"key": "state", "type": "str"},
         "reason": {"key": "reason", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.state = None
         self.reason = None
 
 
 class CommonSimPropertiesFormat(_serialization.Model):
@@ -674,16 +676,16 @@
         self,
         *,
         international_mobile_subscriber_identity: str,
         integrated_circuit_card_identifier: Optional[str] = None,
         device_type: Optional[str] = None,
         sim_policy: Optional["_models.SimPolicyResourceId"] = None,
         static_ip_configuration: Optional[List["_models.SimStaticIpProperties"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword international_mobile_subscriber_identity: The international mobile subscriber identity
          (IMSI) for the SIM. Required.
         :paramtype international_mobile_subscriber_identity: str
         :keyword integrated_circuit_card_identifier: The integrated circuit card ID (ICCID) for the
          SIM.
         :paramtype integrated_circuit_card_identifier: str
@@ -728,15 +730,15 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Azure Arc connected cluster resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -757,15 +759,15 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Azure Arc custom location resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -773,16 +775,16 @@
 class DataNetwork(TrackedResource):
     """Data network resource. Must be created in the same location as its parent mobile network.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -816,16 +818,16 @@
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "description": {"key": "properties.description", "type": "str"},
     }
 
     def __init__(
-        self, *, location: str, tags: Optional[Dict[str, str]] = None, description: Optional[str] = None, **kwargs
-    ):
+        self, *, location: str, tags: Optional[Dict[str, str]] = None, description: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword description: An optional description for this data network.
         :paramtype description: str
@@ -843,20 +845,17 @@
     :ivar data_network: A reference to the data network that these settings apply to. The data
      network must be in the same location as the SIM policy. Required.
     :vartype data_network: ~azure.mgmt.mobilenetwork.models.DataNetworkResourceId
     :ivar session_ambr: Aggregate maximum bit rate across all non-GBR QoS flows of a given PDU
      session. See 3GPP TS23.501 section 5.7.2.6 for a full description of the Session-AMBR.
      Required.
     :vartype session_ambr: ~azure.mgmt.mobilenetwork.models.Ambr
-    :ivar five_qi: Default QoS Flow 5G QoS Indicator value. The 5QI identifies a specific QoS
-     forwarding treatment to be provided to a flow. This must not be a standardized 5QI value
-     corresponding to a GBR (guaranteed bit rate) QoS Flow. The illegal GBR 5QI values are: 1, 2, 3,
-     4, 65, 66, 67, 71, 72, 73, 74, 75, 76, 82, 83, 84, and 85. See 3GPP TS23.501 section 5.7.2.1
-     for a full description of the 5QI parameter, and table 5.7.4-1 for the definition of which are
-     the GBR 5QI values.
+    :ivar five_qi: Default 5G QoS Flow Indicator value. The 5QI identifies a specific QoS
+     forwarding treatment to be provided to a flow. See 3GPP TS23.501 section 5.7.2.1 for a full
+     description of the 5QI parameter, and table 5.7.4-1 for the definition the 5QI values.
     :vartype five_qi: int
     :ivar allocation_and_retention_priority_level: Default QoS Flow allocation and retention
      priority (ARP) level. Flows with higher priority preempt flows with lower priority, if the
      settings of ``preemptionCapability`` and ``preemptionVulnerability`` allow it. 1 is the highest
      level of priority. If this field is not specified then ``5qi`` is used to derive the ARP value.
      See 3GPP TS23.501 section 5.7.2.2 for a full description of the ARP parameters.
     :vartype allocation_and_retention_priority_level: int
@@ -921,30 +920,27 @@
         five_qi: Optional[int] = None,
         allocation_and_retention_priority_level: Optional[int] = None,
         preemption_capability: Optional[Union[str, "_models.PreemptionCapability"]] = None,
         preemption_vulnerability: Optional[Union[str, "_models.PreemptionVulnerability"]] = None,
         default_session_type: Optional[Union[str, "_models.PduSessionType"]] = None,
         additional_allowed_session_types: Optional[List[Union[str, "_models.PduSessionType"]]] = None,
         maximum_number_of_buffered_packets: int = 10,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword data_network: A reference to the data network that these settings apply to. The data
          network must be in the same location as the SIM policy. Required.
         :paramtype data_network: ~azure.mgmt.mobilenetwork.models.DataNetworkResourceId
         :keyword session_ambr: Aggregate maximum bit rate across all non-GBR QoS flows of a given PDU
          session. See 3GPP TS23.501 section 5.7.2.6 for a full description of the Session-AMBR.
          Required.
         :paramtype session_ambr: ~azure.mgmt.mobilenetwork.models.Ambr
-        :keyword five_qi: Default QoS Flow 5G QoS Indicator value. The 5QI identifies a specific QoS
-         forwarding treatment to be provided to a flow. This must not be a standardized 5QI value
-         corresponding to a GBR (guaranteed bit rate) QoS Flow. The illegal GBR 5QI values are: 1, 2, 3,
-         4, 65, 66, 67, 71, 72, 73, 74, 75, 76, 82, 83, 84, and 85. See 3GPP TS23.501 section 5.7.2.1
-         for a full description of the 5QI parameter, and table 5.7.4-1 for the definition of which are
-         the GBR 5QI values.
+        :keyword five_qi: Default 5G QoS Flow Indicator value. The 5QI identifies a specific QoS
+         forwarding treatment to be provided to a flow. See 3GPP TS23.501 section 5.7.2.1 for a full
+         description of the 5QI parameter, and table 5.7.4-1 for the definition the 5QI values.
         :paramtype five_qi: int
         :keyword allocation_and_retention_priority_level: Default QoS Flow allocation and retention
          priority (ARP) level. Flows with higher priority preempt flows with lower priority, if the
          settings of ``preemptionCapability`` and ``preemptionVulnerability`` allow it. 1 is the highest
          level of priority. If this field is not specified then ``5qi`` is used to derive the ARP value.
          See 3GPP TS23.501 section 5.7.2.2 for a full description of the ARP parameters.
         :paramtype allocation_and_retention_priority_level: int
@@ -1005,15 +1001,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[DataNetwork]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.DataNetwork"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.DataNetwork"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: A list of data networks.
         :paramtype value: list[~azure.mgmt.mobilenetwork.models.DataNetwork]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -1035,23 +1031,174 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Data network resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
 
+class ProxyResource(Resource):
+    """The resource model definition for a Azure Resource Manager proxy resource. It will not have
+    tags and a location.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.mobilenetwork.models.SystemData
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+
+
+class DiagnosticsPackage(ProxyResource):
+    """Diagnostics package resource.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.mobilenetwork.models.SystemData
+    :ivar provisioning_state: The provisioning state of the diagnostics package resource. Known
+     values are: "Unknown", "Succeeded", "Accepted", "Deleting", "Failed", "Canceled", and
+     "Deleted".
+    :vartype provisioning_state: str or ~azure.mgmt.mobilenetwork.models.ProvisioningState
+    :ivar status: The status of the diagnostics package collection. Known values are: "NotStarted",
+     "Collecting", "Collected", and "Error".
+    :vartype status: str or ~azure.mgmt.mobilenetwork.models.DiagnosticsPackageStatus
+    :ivar reason: The reason for the current state of the diagnostics package collection.
+    :vartype reason: str
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "provisioning_state": {"readonly": True},
+        "status": {"readonly": True},
+        "reason": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "status": {"key": "properties.status", "type": "str"},
+        "reason": {"key": "properties.reason", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.provisioning_state = None
+        self.status = None
+        self.reason = None
+
+
+class DiagnosticsPackageListResult(_serialization.Model):
+    """Response for diagnostics package API service call.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar value: A list of diagnostics packages under a packet core control plane.
+    :vartype value: list[~azure.mgmt.mobilenetwork.models.DiagnosticsPackage]
+    :ivar next_link: The URL to get the next set of results.
+    :vartype next_link: str
+    """
+
+    _validation = {
+        "next_link": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[DiagnosticsPackage]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(self, *, value: Optional[List["_models.DiagnosticsPackage"]] = None, **kwargs: Any) -> None:
+        """
+        :keyword value: A list of diagnostics packages under a packet core control plane.
+        :paramtype value: list[~azure.mgmt.mobilenetwork.models.DiagnosticsPackage]
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = None
+
+
+class DiagnosticsUploadConfiguration(_serialization.Model):
+    """Configuration for uploading packet core diagnostics.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar storage_account_container_url: The Storage Account Container URL to upload diagnostics
+     to. Required.
+    :vartype storage_account_container_url: str
+    """
+
+    _validation = {
+        "storage_account_container_url": {"required": True},
+    }
+
+    _attribute_map = {
+        "storage_account_container_url": {"key": "storageAccountContainerUrl", "type": "str"},
+    }
+
+    def __init__(self, *, storage_account_container_url: str, **kwargs: Any) -> None:
+        """
+        :keyword storage_account_container_url: The Storage Account Container URL to upload diagnostics
+         to. Required.
+        :paramtype storage_account_container_url: str
+        """
+        super().__init__(**kwargs)
+        self.storage_account_container_url = storage_account_container_url
+
+
 class EncryptedSimPropertiesFormat(CommonSimPropertiesFormat):  # pylint: disable=too-many-instance-attributes
     """Encrypted SIM properties.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -1120,16 +1267,16 @@
         *,
         international_mobile_subscriber_identity: str,
         integrated_circuit_card_identifier: Optional[str] = None,
         device_type: Optional[str] = None,
         sim_policy: Optional["_models.SimPolicyResourceId"] = None,
         static_ip_configuration: Optional[List["_models.SimStaticIpProperties"]] = None,
         encrypted_credentials: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword international_mobile_subscriber_identity: The international mobile subscriber identity
          (IMSI) for the SIM. Required.
         :paramtype international_mobile_subscriber_identity: str
         :keyword integrated_circuit_card_identifier: The integrated circuit card ID (ICCID) for the
          SIM.
         :paramtype integrated_circuit_card_identifier: str
@@ -1204,16 +1351,16 @@
         *,
         version: int,
         azure_key_identifier: int,
         vendor_key_fingerprint: str,
         encrypted_transport_key: str,
         signed_transport_key: str,
         sims: List["_models.SimNameAndEncryptedProperties"],
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword version: The upload file format version. Required.
         :paramtype version: int
         :keyword azure_key_identifier: An identifier for the Azure SIM onboarding public key used for
          encrypted upload. Required.
         :paramtype azure_key_identifier: int
         :keyword vendor_key_fingerprint: The fingerprint of the SIM vendor public key. The private
@@ -1254,15 +1401,15 @@
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "info": {"key": "info", "type": "object"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.type = None
         self.info = None
 
 
 class ErrorDetail(_serialization.Model):
@@ -1294,36 +1441,37 @@
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "target": {"key": "target", "type": "str"},
         "details": {"key": "details", "type": "[ErrorDetail]"},
         "additional_info": {"key": "additionalInfo", "type": "[ErrorAdditionalInfo]"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.code = None
         self.message = None
         self.target = None
         self.details = None
         self.additional_info = None
 
 
 class ErrorResponse(_serialization.Model):
-    """Common error response for all Azure Resource Manager APIs to return error details for failed operations. (This also follows the OData error response format.).
+    """Common error response for all Azure Resource Manager APIs to return error details for failed
+    operations. (This also follows the OData error response format.).
 
     :ivar error: The error object.
     :vartype error: ~azure.mgmt.mobilenetwork.models.ErrorDetail
     """
 
     _attribute_map = {
         "error": {"key": "error", "type": "ErrorDetail"},
     }
 
-    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs):
+    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs: Any) -> None:
         """
         :keyword error: The error object.
         :paramtype error: ~azure.mgmt.mobilenetwork.models.ErrorDetail
         """
         super().__init__(**kwargs)
         self.error = error
 
@@ -1348,57 +1496,106 @@
     }
 
     _attribute_map = {
         "certificate_url": {"key": "certificateUrl", "type": "str"},
         "provisioning": {"key": "provisioning", "type": "CertificateProvisioning"},
     }
 
-    def __init__(self, *, certificate_url: str, **kwargs):
+    def __init__(self, *, certificate_url: str, **kwargs: Any) -> None:
         """
         :keyword certificate_url: The certificate URL, unversioned. For example:
          https://contosovault.vault.azure.net/certificates/ingress. Required.
         :paramtype certificate_url: str
         """
         super().__init__(**kwargs)
         self.certificate_url = certificate_url
         self.provisioning = None
 
 
+class IdentityAndTagsObject(_serialization.Model):
+    """Identity and Tags object for patch operations.
+
+    :ivar identity: The managed service identity associated with this resource.
+    :vartype identity: ~azure.mgmt.mobilenetwork.models.ManagedServiceIdentity
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    """
+
+    _attribute_map = {
+        "identity": {"key": "identity", "type": "ManagedServiceIdentity"},
+        "tags": {"key": "tags", "type": "{str}"},
+    }
+
+    def __init__(
+        self,
+        *,
+        identity: Optional["_models.ManagedServiceIdentity"] = None,
+        tags: Optional[Dict[str, str]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword identity: The managed service identity associated with this resource.
+        :paramtype identity: ~azure.mgmt.mobilenetwork.models.ManagedServiceIdentity
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        """
+        super().__init__(**kwargs)
+        self.identity = identity
+        self.tags = tags
+
+
 class Installation(_serialization.Model):
     """The installation state of the packet core.
 
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar desired_state: The desired installation state. Known values are: "Uninstalled" and
+     "Installed".
+    :vartype desired_state: str or ~azure.mgmt.mobilenetwork.models.DesiredInstallationState
     :ivar state: Installation state. Known values are: "Uninstalled", "Installing", "Installed",
      "Updating", "Upgrading", "Uninstalling", "Reinstalling", "RollingBack", and "Failed".
     :vartype state: str or ~azure.mgmt.mobilenetwork.models.InstallationState
+    :ivar reinstall_required: Whether a reinstall of the packet core is required to pick up the
+     latest configuration changes. Known values are: "Required" and "NotRequired".
+    :vartype reinstall_required: str or ~azure.mgmt.mobilenetwork.models.ReinstallRequired
+    :ivar reasons: Reason(s) for the current installation state of the packet core.
+    :vartype reasons: list[str or ~azure.mgmt.mobilenetwork.models.InstallationReason]
     :ivar operation: A reference to an in-progress installation operation.
     :vartype operation: ~azure.mgmt.mobilenetwork.models.AsyncOperationId
     """
 
+    _validation = {
+        "state": {"readonly": True},
+        "reinstall_required": {"readonly": True},
+        "reasons": {"readonly": True, "unique": True},
+        "operation": {"readonly": True},
+    }
+
     _attribute_map = {
+        "desired_state": {"key": "desiredState", "type": "str"},
         "state": {"key": "state", "type": "str"},
+        "reinstall_required": {"key": "reinstallRequired", "type": "str"},
+        "reasons": {"key": "reasons", "type": "[str]"},
         "operation": {"key": "operation", "type": "AsyncOperationId"},
     }
 
     def __init__(
-        self,
-        *,
-        state: Optional[Union[str, "_models.InstallationState"]] = None,
-        operation: Optional["_models.AsyncOperationId"] = None,
-        **kwargs
-    ):
-        """
-        :keyword state: Installation state. Known values are: "Uninstalled", "Installing", "Installed",
-         "Updating", "Upgrading", "Uninstalling", "Reinstalling", "RollingBack", and "Failed".
-        :paramtype state: str or ~azure.mgmt.mobilenetwork.models.InstallationState
-        :keyword operation: A reference to an in-progress installation operation.
-        :paramtype operation: ~azure.mgmt.mobilenetwork.models.AsyncOperationId
+        self, *, desired_state: Optional[Union[str, "_models.DesiredInstallationState"]] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword desired_state: The desired installation state. Known values are: "Uninstalled" and
+         "Installed".
+        :paramtype desired_state: str or ~azure.mgmt.mobilenetwork.models.DesiredInstallationState
         """
         super().__init__(**kwargs)
-        self.state = state
-        self.operation = operation
+        self.desired_state = desired_state
+        self.state = None
+        self.reinstall_required = None
+        self.reasons = None
+        self.operation = None
 
 
 class InterfaceProperties(_serialization.Model):
     """Interface properties.
 
     :ivar name: The logical name for this interface. This should match one of the interfaces
      configured on your Azure Stack Edge device.
@@ -1433,16 +1630,16 @@
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         ipv4_address: Optional[str] = None,
         ipv4_subnet: Optional[str] = None,
         ipv4_gateway: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: The logical name for this interface. This should match one of the interfaces
          configured on your Azure Stack Edge device.
         :paramtype name: str
         :keyword ipv4_address: The IPv4 address.
         :paramtype ipv4_address: str
         :keyword ipv4_subnet: The IPv4 subnet.
@@ -1465,26 +1662,27 @@
     :vartype key_url: str
     """
 
     _attribute_map = {
         "key_url": {"key": "keyUrl", "type": "str"},
     }
 
-    def __init__(self, *, key_url: Optional[str] = None, **kwargs):
+    def __init__(self, *, key_url: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword key_url: The key URL, unversioned. For example:
          https://contosovault.vault.azure.net/keys/azureKey.
         :paramtype key_url: str
         """
         super().__init__(**kwargs)
         self.key_url = key_url
 
 
 class LocalDiagnosticsAccessConfiguration(_serialization.Model):
-    """The kubernetes ingress configuration to control access to packet core diagnostics over local APIs.
+    """The kubernetes ingress configuration to control access to packet core diagnostics over local
+    APIs.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar authentication_type: How to authenticate users who access local diagnostics APIs.
      Required. Known values are: "AAD" and "Password".
     :vartype authentication_type: str or ~azure.mgmt.mobilenetwork.models.AuthenticationType
     :ivar https_server_certificate: The HTTPS server TLS certificate used to secure local access to
@@ -1502,102 +1700,86 @@
     }
 
     def __init__(
         self,
         *,
         authentication_type: Union[str, "_models.AuthenticationType"],
         https_server_certificate: Optional["_models.HttpsServerCertificate"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword authentication_type: How to authenticate users who access local diagnostics APIs.
          Required. Known values are: "AAD" and "Password".
         :paramtype authentication_type: str or ~azure.mgmt.mobilenetwork.models.AuthenticationType
         :keyword https_server_certificate: The HTTPS server TLS certificate used to secure local access
          to diagnostics.
         :paramtype https_server_certificate: ~azure.mgmt.mobilenetwork.models.HttpsServerCertificate
         """
         super().__init__(**kwargs)
         self.authentication_type = authentication_type
         self.https_server_certificate = https_server_certificate
 
 
 class ManagedServiceIdentity(_serialization.Model):
-    """Managed service identity (system assigned and/or user assigned identities).
-
-    Variables are only populated by the server, and will be ignored when sending a request.
+    """Managed service identity (User assigned identity).
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar principal_id: The service principal ID of the system assigned identity. This property
-     will only be provided for a system assigned identity.
-    :vartype principal_id: str
-    :ivar tenant_id: The tenant ID of the system assigned identity. This property will only be
-     provided for a system assigned identity.
-    :vartype tenant_id: str
-    :ivar type: Type of managed service identity (where both SystemAssigned and UserAssigned types
-     are allowed). Required. Known values are: "None", "SystemAssigned", "UserAssigned", and
-     "SystemAssigned,UserAssigned".
+    :ivar type: Type of managed service identity (currently only UserAssigned allowed). Required.
+     Known values are: "None" and "UserAssigned".
     :vartype type: str or ~azure.mgmt.mobilenetwork.models.ManagedServiceIdentityType
     :ivar user_assigned_identities: The set of user assigned identities associated with the
      resource. The userAssignedIdentities dictionary keys will be ARM resource ids in the form:
      '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}.
      The dictionary values can be empty objects ({}) in requests.
     :vartype user_assigned_identities: dict[str,
      ~azure.mgmt.mobilenetwork.models.UserAssignedIdentity]
     """
 
     _validation = {
-        "principal_id": {"readonly": True},
-        "tenant_id": {"readonly": True},
         "type": {"required": True},
     }
 
     _attribute_map = {
-        "principal_id": {"key": "principalId", "type": "str"},
-        "tenant_id": {"key": "tenantId", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "user_assigned_identities": {"key": "userAssignedIdentities", "type": "{UserAssignedIdentity}"},
     }
 
     def __init__(
         self,
         *,
         type: Union[str, "_models.ManagedServiceIdentityType"],
         user_assigned_identities: Optional[Dict[str, "_models.UserAssignedIdentity"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword type: Type of managed service identity (where both SystemAssigned and UserAssigned
-         types are allowed). Required. Known values are: "None", "SystemAssigned", "UserAssigned", and
-         "SystemAssigned,UserAssigned".
+        :keyword type: Type of managed service identity (currently only UserAssigned allowed).
+         Required. Known values are: "None" and "UserAssigned".
         :paramtype type: str or ~azure.mgmt.mobilenetwork.models.ManagedServiceIdentityType
         :keyword user_assigned_identities: The set of user assigned identities associated with the
          resource. The userAssignedIdentities dictionary keys will be ARM resource ids in the form:
          '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}.
          The dictionary values can be empty objects ({}) in requests.
         :paramtype user_assigned_identities: dict[str,
          ~azure.mgmt.mobilenetwork.models.UserAssignedIdentity]
         """
         super().__init__(**kwargs)
-        self.principal_id = None
-        self.tenant_id = None
         self.type = type
         self.user_assigned_identities = user_assigned_identities
 
 
 class MobileNetwork(TrackedResource):
     """Mobile network resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -1647,16 +1829,16 @@
 
     def __init__(
         self,
         *,
         location: str,
         public_land_mobile_network_identifier: "_models.PlmnId",
         tags: Optional[Dict[str, str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword public_land_mobile_network_identifier: The unique public land mobile network
          identifier for the network. This is made up of the mobile country code and mobile network code,
@@ -1687,15 +1869,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[MobileNetwork]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.MobileNetwork"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.MobileNetwork"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: A list of mobile networks in a resource group.
         :paramtype value: list[~azure.mgmt.mobilenetwork.models.MobileNetwork]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -1717,15 +1899,15 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Mobile network resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -1770,16 +1952,16 @@
         self,
         *,
         enabled: Union[str, "_models.NaptEnabled"] = "Enabled",
         port_range: Optional["_models.PortRange"] = None,
         port_reuse_hold_time: Optional["_models.PortReuseHoldTimes"] = None,
         pinhole_limits: int = 65536,
         pinhole_timeouts: Optional["_models.PinholeTimeouts"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword enabled: Whether NAPT is enabled for connections to this attached data network. Known
          values are: "Enabled" and "Disabled".
         :paramtype enabled: str or ~azure.mgmt.mobilenetwork.models.NaptEnabled
         :keyword port_range: Range of port numbers to use as translated ports on each translated
          address.
          If not specified and NAPT is enabled, this range defaults to 1,024 - 49,999.
@@ -1826,15 +2008,15 @@
 
     _attribute_map = {
         "is_data_action": {"key": "isDataAction", "type": "bool"},
         "name": {"key": "name", "type": "str"},
         "display": {"key": "display", "type": "OperationDisplay"},
     }
 
-    def __init__(self, *, is_data_action: Optional[bool] = None, **kwargs):
+    def __init__(self, *, is_data_action: Optional[bool] = None, **kwargs: Any) -> None:
         """
         :keyword is_data_action: Indicates whether the operation applies to data-plane.
         :paramtype is_data_action: bool
         """
         super().__init__(**kwargs)
         self.is_data_action = is_data_action
         self.name = None
@@ -1865,16 +2047,16 @@
     def __init__(
         self,
         *,
         provider: Optional[str] = None,
         resource: Optional[str] = None,
         operation: Optional[str] = None,
         description: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword provider: Service provider: Microsoft.MobileNetwork.
         :paramtype provider: str
         :keyword resource: Resource on which the operation is performed: Registration definition,
          registration assignment etc.
         :paramtype resource: str
         :keyword operation: Operation type: Read, write, delete, etc.
@@ -1906,30 +2088,159 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Operation]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.value = None
         self.next_link = None
 
 
+class PacketCapture(ProxyResource):  # pylint: disable=too-many-instance-attributes
+    """Packet capture session resource.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.mobilenetwork.models.SystemData
+    :ivar provisioning_state: The provisioning state of the packet capture session resource. Known
+     values are: "Unknown", "Succeeded", "Accepted", "Deleting", "Failed", "Canceled", and
+     "Deleted".
+    :vartype provisioning_state: str or ~azure.mgmt.mobilenetwork.models.ProvisioningState
+    :ivar status: The status of the packet capture session. Known values are: "NotStarted",
+     "Running", "Stopped", and "Error".
+    :vartype status: str or ~azure.mgmt.mobilenetwork.models.PacketCaptureStatus
+    :ivar reason: The reason the current packet capture session state.
+    :vartype reason: str
+    :ivar capture_start_time: The start time of the packet capture session.
+    :vartype capture_start_time: ~datetime.datetime
+    :ivar network_interfaces: List of network interfaces to capture on.
+    :vartype network_interfaces: list[str]
+    :ivar bytes_to_capture_per_packet: Number of bytes captured per packet, the remaining bytes are
+     truncated. The default "0" means the entire packet is captured.
+    :vartype bytes_to_capture_per_packet: int
+    :ivar total_bytes_per_session: Maximum size of the capture output.
+    :vartype total_bytes_per_session: int
+    :ivar time_limit_in_seconds: Maximum duration of the capture session in seconds.
+    :vartype time_limit_in_seconds: int
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "provisioning_state": {"readonly": True},
+        "status": {"readonly": True},
+        "reason": {"readonly": True},
+        "capture_start_time": {"readonly": True},
+        "network_interfaces": {"min_items": 1, "unique": True},
+        "bytes_to_capture_per_packet": {"maximum": 4294967295, "minimum": 0},
+        "total_bytes_per_session": {"maximum": 4294967295, "minimum": 0},
+        "time_limit_in_seconds": {"maximum": 18000, "minimum": 0},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "status": {"key": "properties.status", "type": "str"},
+        "reason": {"key": "properties.reason", "type": "str"},
+        "capture_start_time": {"key": "properties.captureStartTime", "type": "iso-8601"},
+        "network_interfaces": {"key": "properties.networkInterfaces", "type": "[str]"},
+        "bytes_to_capture_per_packet": {"key": "properties.bytesToCapturePerPacket", "type": "int"},
+        "total_bytes_per_session": {"key": "properties.totalBytesPerSession", "type": "int"},
+        "time_limit_in_seconds": {"key": "properties.timeLimitInSeconds", "type": "int"},
+    }
+
+    def __init__(
+        self,
+        *,
+        network_interfaces: Optional[List[str]] = None,
+        bytes_to_capture_per_packet: int = 0,
+        total_bytes_per_session: int = 67108864,
+        time_limit_in_seconds: int = 18000,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword network_interfaces: List of network interfaces to capture on.
+        :paramtype network_interfaces: list[str]
+        :keyword bytes_to_capture_per_packet: Number of bytes captured per packet, the remaining bytes
+         are truncated. The default "0" means the entire packet is captured.
+        :paramtype bytes_to_capture_per_packet: int
+        :keyword total_bytes_per_session: Maximum size of the capture output.
+        :paramtype total_bytes_per_session: int
+        :keyword time_limit_in_seconds: Maximum duration of the capture session in seconds.
+        :paramtype time_limit_in_seconds: int
+        """
+        super().__init__(**kwargs)
+        self.provisioning_state = None
+        self.status = None
+        self.reason = None
+        self.capture_start_time = None
+        self.network_interfaces = network_interfaces
+        self.bytes_to_capture_per_packet = bytes_to_capture_per_packet
+        self.total_bytes_per_session = total_bytes_per_session
+        self.time_limit_in_seconds = time_limit_in_seconds
+
+
+class PacketCaptureListResult(_serialization.Model):
+    """Response for packet capture API service call.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar value: A list of packet capture sessions under a packet core control plane.
+    :vartype value: list[~azure.mgmt.mobilenetwork.models.PacketCapture]
+    :ivar next_link: The URL to get the next set of results.
+    :vartype next_link: str
+    """
+
+    _validation = {
+        "next_link": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[PacketCapture]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(self, *, value: Optional[List["_models.PacketCapture"]] = None, **kwargs: Any) -> None:
+        """
+        :keyword value: A list of packet capture sessions under a packet core control plane.
+        :paramtype value: list[~azure.mgmt.mobilenetwork.models.PacketCapture]
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = None
+
+
 class PacketCoreControlPlane(TrackedResource):  # pylint: disable=too-many-instance-attributes
     """Packet core control plane resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -1949,50 +2260,54 @@
     :vartype installation: ~azure.mgmt.mobilenetwork.models.Installation
     :ivar sites: Site(s) under which this packet core control plane should be deployed. The sites
      must be in the same location as the packet core control plane. Required.
     :vartype sites: list[~azure.mgmt.mobilenetwork.models.SiteResourceId]
     :ivar platform: The platform where the packet core is deployed. Required.
     :vartype platform: ~azure.mgmt.mobilenetwork.models.PlatformConfiguration
     :ivar core_network_technology: The core network technology generation (5G core or EPC / 4G
-     core). Known values are: "5GC" and "EPC".
+     core). Known values are: "5GC", "EPC", and "EPC + 5GC".
     :vartype core_network_technology: str or ~azure.mgmt.mobilenetwork.models.CoreNetworkType
-    :ivar version: The version of the packet core software that is deployed.
+    :ivar version: The desired version of the packet core software.
     :vartype version: str
+    :ivar installed_version: The currently installed version of the packet core software.
+    :vartype installed_version: str
     :ivar rollback_version: The previous version of the packet core software that was deployed.
      Used when performing the rollback action.
     :vartype rollback_version: str
     :ivar control_plane_access_interface: The control plane interface on the access network. For 5G
      networks, this is the N2 interface. For 4G networks, this is the S1-MME interface. Required.
     :vartype control_plane_access_interface: ~azure.mgmt.mobilenetwork.models.InterfaceProperties
     :ivar sku: The SKU defining the throughput and SIM allowances for this packet core control
-     plane deployment. Required. Known values are: "G0", "G1", "G2", "G3", "G4", "G5", and "G10".
+     plane deployment. Required. Known values are: "G0", "G1", "G2", "G5", and "G10".
     :vartype sku: str or ~azure.mgmt.mobilenetwork.models.BillingSku
     :ivar ue_mtu: The MTU (in bytes) signaled to the UE. The same MTU is set on the user plane data
      links for all data networks. The MTU set on the user plane access link is calculated to be 60
      bytes greater than this value to allow for GTP encapsulation.
     :vartype ue_mtu: int
     :ivar local_diagnostics_access: The kubernetes ingress configuration to control access to
      packet core diagnostics over local APIs. Required.
     :vartype local_diagnostics_access:
      ~azure.mgmt.mobilenetwork.models.LocalDiagnosticsAccessConfiguration
+    :ivar diagnostics_upload: Configuration for uploading packet core diagnostics.
+    :vartype diagnostics_upload: ~azure.mgmt.mobilenetwork.models.DiagnosticsUploadConfiguration
     :ivar interop_settings: Settings to allow interoperability with third party components e.g.
      RANs and UEs.
     :vartype interop_settings: JSON
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
         "location": {"required": True},
         "provisioning_state": {"readonly": True},
-        "installation": {"readonly": True},
         "sites": {"required": True, "min_items": 1, "unique": True},
         "platform": {"required": True},
+        "installed_version": {"readonly": True},
         "rollback_version": {"readonly": True},
         "control_plane_access_interface": {"required": True},
         "sku": {"required": True},
         "ue_mtu": {"maximum": 1930, "minimum": 1280},
         "local_diagnostics_access": {"required": True},
     }
 
@@ -2006,93 +2321,103 @@
         "identity": {"key": "identity", "type": "ManagedServiceIdentity"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "installation": {"key": "properties.installation", "type": "Installation"},
         "sites": {"key": "properties.sites", "type": "[SiteResourceId]"},
         "platform": {"key": "properties.platform", "type": "PlatformConfiguration"},
         "core_network_technology": {"key": "properties.coreNetworkTechnology", "type": "str"},
         "version": {"key": "properties.version", "type": "str"},
+        "installed_version": {"key": "properties.installedVersion", "type": "str"},
         "rollback_version": {"key": "properties.rollbackVersion", "type": "str"},
         "control_plane_access_interface": {
             "key": "properties.controlPlaneAccessInterface",
             "type": "InterfaceProperties",
         },
         "sku": {"key": "properties.sku", "type": "str"},
         "ue_mtu": {"key": "properties.ueMtu", "type": "int"},
         "local_diagnostics_access": {
             "key": "properties.localDiagnosticsAccess",
             "type": "LocalDiagnosticsAccessConfiguration",
         },
+        "diagnostics_upload": {"key": "properties.diagnosticsUpload", "type": "DiagnosticsUploadConfiguration"},
         "interop_settings": {"key": "properties.interopSettings", "type": "object"},
     }
 
     def __init__(
         self,
         *,
         location: str,
         sites: List["_models.SiteResourceId"],
         platform: "_models.PlatformConfiguration",
         control_plane_access_interface: "_models.InterfaceProperties",
         sku: Union[str, "_models.BillingSku"],
         local_diagnostics_access: "_models.LocalDiagnosticsAccessConfiguration",
         tags: Optional[Dict[str, str]] = None,
         identity: Optional["_models.ManagedServiceIdentity"] = None,
+        installation: Optional["_models.Installation"] = None,
         core_network_technology: Union[str, "_models.CoreNetworkType"] = "5GC",
         version: Optional[str] = None,
         ue_mtu: int = 1440,
+        diagnostics_upload: Optional["_models.DiagnosticsUploadConfiguration"] = None,
         interop_settings: Optional[JSON] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword identity: The identity used to retrieve the ingress certificate from Azure key vault.
         :paramtype identity: ~azure.mgmt.mobilenetwork.models.ManagedServiceIdentity
+        :keyword installation: The installation state of the packet core control plane resource.
+        :paramtype installation: ~azure.mgmt.mobilenetwork.models.Installation
         :keyword sites: Site(s) under which this packet core control plane should be deployed. The
          sites must be in the same location as the packet core control plane. Required.
         :paramtype sites: list[~azure.mgmt.mobilenetwork.models.SiteResourceId]
         :keyword platform: The platform where the packet core is deployed. Required.
         :paramtype platform: ~azure.mgmt.mobilenetwork.models.PlatformConfiguration
         :keyword core_network_technology: The core network technology generation (5G core or EPC / 4G
-         core). Known values are: "5GC" and "EPC".
+         core). Known values are: "5GC", "EPC", and "EPC + 5GC".
         :paramtype core_network_technology: str or ~azure.mgmt.mobilenetwork.models.CoreNetworkType
-        :keyword version: The version of the packet core software that is deployed.
+        :keyword version: The desired version of the packet core software.
         :paramtype version: str
         :keyword control_plane_access_interface: The control plane interface on the access network. For
          5G networks, this is the N2 interface. For 4G networks, this is the S1-MME interface. Required.
         :paramtype control_plane_access_interface: ~azure.mgmt.mobilenetwork.models.InterfaceProperties
         :keyword sku: The SKU defining the throughput and SIM allowances for this packet core control
-         plane deployment. Required. Known values are: "G0", "G1", "G2", "G3", "G4", "G5", and "G10".
+         plane deployment. Required. Known values are: "G0", "G1", "G2", "G5", and "G10".
         :paramtype sku: str or ~azure.mgmt.mobilenetwork.models.BillingSku
         :keyword ue_mtu: The MTU (in bytes) signaled to the UE. The same MTU is set on the user plane
          data links for all data networks. The MTU set on the user plane access link is calculated to be
          60 bytes greater than this value to allow for GTP encapsulation.
         :paramtype ue_mtu: int
         :keyword local_diagnostics_access: The kubernetes ingress configuration to control access to
          packet core diagnostics over local APIs. Required.
         :paramtype local_diagnostics_access:
          ~azure.mgmt.mobilenetwork.models.LocalDiagnosticsAccessConfiguration
+        :keyword diagnostics_upload: Configuration for uploading packet core diagnostics.
+        :paramtype diagnostics_upload: ~azure.mgmt.mobilenetwork.models.DiagnosticsUploadConfiguration
         :keyword interop_settings: Settings to allow interoperability with third party components e.g.
          RANs and UEs.
         :paramtype interop_settings: JSON
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.identity = identity
         self.provisioning_state = None
-        self.installation = None
+        self.installation = installation
         self.sites = sites
         self.platform = platform
         self.core_network_technology = core_network_technology
         self.version = version
+        self.installed_version = None
         self.rollback_version = None
         self.control_plane_access_interface = control_plane_access_interface
         self.sku = sku
         self.ue_mtu = ue_mtu
         self.local_diagnostics_access = local_diagnostics_access
+        self.diagnostics_upload = diagnostics_upload
         self.interop_settings = interop_settings
 
 
 class PacketCoreControlPlaneCollectDiagnosticsPackage(_serialization.Model):
     """Packet core control plane collect diagnostics package options.
 
     All required parameters must be populated in order to send to Azure.
@@ -2106,15 +2431,15 @@
         "storage_account_blob_url": {"required": True},
     }
 
     _attribute_map = {
         "storage_account_blob_url": {"key": "storageAccountBlobUrl", "type": "str"},
     }
 
-    def __init__(self, *, storage_account_blob_url: str, **kwargs):
+    def __init__(self, *, storage_account_blob_url: str, **kwargs: Any) -> None:
         """
         :keyword storage_account_blob_url: The Storage Account Blob URL to upload the diagnostics
          package to. Required.
         :paramtype storage_account_blob_url: str
         """
         super().__init__(**kwargs)
         self.storage_account_blob_url = storage_account_blob_url
@@ -2136,68 +2461,60 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[PacketCoreControlPlane]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.PacketCoreControlPlane"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.PacketCoreControlPlane"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: A list of packet core control planes in a resource group.
         :paramtype value: list[~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
 
 
-class ProxyResource(Resource):
-    """The resource model definition for a Azure Resource Manager proxy resource. It will not have tags and a location.
+class PacketCoreControlPlaneResourceId(_serialization.Model):
+    """Reference to an packet core control plane resource.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
+    All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Packet core control plane resource ID. Required.
     :vartype id: str
-    :ivar name: The name of the resource.
-    :vartype name: str
-    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
-     "Microsoft.Storage/storageAccounts".
-    :vartype type: str
-    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
-     information.
-    :vartype system_data: ~azure.mgmt.mobilenetwork.models.SystemData
     """
 
     _validation = {
-        "id": {"readonly": True},
-        "name": {"readonly": True},
-        "type": {"readonly": True},
-        "system_data": {"readonly": True},
+        "id": {
+            "required": True,
+            "pattern": r"^/[sS][uU][bB][sS][cC][rR][iI][pP][tT][iI][oO][nN][sS]/[^/?#]+/[rR][eE][sS][oO][uU][rR][cC][eE][gG][rR][oO][uU][pP][sS]/[^/?#]+/[pP][rR][oO][vV][iI][dD][eE][rR][sS]/[mM][iI][cC][rR][oO][sS][oO][fF][tT]\.[mM][oO][bB][iI][lL][eE][nN][eE][tT][wW][oO][rR][kK]/[pP][aA][cC][kK][eE][tT][cC][oO][rR][eE][cC][oO][nN][tT][rR][oO][lL][pP][lL][aA][nN][eE][sS]/[^/?#]+$",
+        },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
-        "name": {"key": "name", "type": "str"},
-        "type": {"key": "type", "type": "str"},
-        "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, **kwargs):
-        """ """
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
+        """
+        :keyword id: Packet core control plane resource ID. Required.
+        :paramtype id: str
+        """
         super().__init__(**kwargs)
+        self.id = id
 
 
 class PacketCoreControlPlaneVersion(ProxyResource):
     """Packet core control plane version resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -2224,15 +2541,15 @@
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "platforms": {"key": "properties.platforms", "type": "[Platform]"},
     }
 
-    def __init__(self, *, platforms: Optional[List["_models.Platform"]] = None, **kwargs):
+    def __init__(self, *, platforms: Optional[List["_models.Platform"]] = None, **kwargs: Any) -> None:
         """
         :keyword platforms: Platform specific packet core control plane version properties.
         :paramtype platforms: list[~azure.mgmt.mobilenetwork.models.Platform]
         """
         super().__init__(**kwargs)
         self.provisioning_state = None
         self.platforms = platforms
@@ -2254,33 +2571,34 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[PacketCoreControlPlaneVersion]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.PacketCoreControlPlaneVersion"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.PacketCoreControlPlaneVersion"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: A list of supported packet core control plane versions.
         :paramtype value: list[~azure.mgmt.mobilenetwork.models.PacketCoreControlPlaneVersion]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
 
 
 class PacketCoreDataPlane(TrackedResource):
-    """Packet core data plane resource. Must be created in the same location as its parent packet core control plane.
+    """Packet core data plane resource. Must be created in the same location as its parent packet core
+    control plane.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -2322,16 +2640,16 @@
 
     def __init__(
         self,
         *,
         location: str,
         user_plane_access_interface: "_models.InterfaceProperties",
         tags: Optional[Dict[str, str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword user_plane_access_interface: The user plane interface on the access network. For 5G
          networks, this is the N3 interface. For 4G networks, this is the S1-U interface. Required.
@@ -2358,15 +2676,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[PacketCoreDataPlane]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.PacketCoreDataPlane"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.PacketCoreDataPlane"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: A list of packet core data planes in a resource group.
         :paramtype value: list[~azure.mgmt.mobilenetwork.models.PacketCoreDataPlane]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -2401,15 +2719,15 @@
     _validation = {
         "rule_name": {
             "required": True,
             "max_length": 64,
             "pattern": r"^(?!(default|requested|service)$)[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         },
         "rule_precedence": {"required": True, "maximum": 255, "minimum": 0},
-        "service_data_flow_templates": {"required": True, "min_items": 1, "unique": True},
+        "service_data_flow_templates": {"required": True, "max_items": 15, "min_items": 1, "unique": True},
     }
 
     _attribute_map = {
         "rule_name": {"key": "ruleName", "type": "str"},
         "rule_precedence": {"key": "rulePrecedence", "type": "int"},
         "rule_qos_policy": {"key": "ruleQosPolicy", "type": "PccRuleQosPolicy"},
         "traffic_control": {"key": "trafficControl", "type": "str"},
@@ -2420,16 +2738,16 @@
         self,
         *,
         rule_name: str,
         rule_precedence: int,
         service_data_flow_templates: List["_models.ServiceDataFlowTemplate"],
         rule_qos_policy: Optional["_models.PccRuleQosPolicy"] = None,
         traffic_control: Optional[Union[str, "_models.TrafficControlPermission"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword rule_name: The name of the rule. This must be unique within the parent service. You
          must not use any of the following reserved strings - ``default``\ , ``requested`` or
          ``service``. Required.
         :paramtype rule_name: str
         :keyword rule_precedence: A precedence value that is used to decide between data flow policy
          rules when identifying the QoS values to use for a particular SIM. A lower value means a higher
@@ -2456,20 +2774,17 @@
 
 
 class QosPolicy(_serialization.Model):
     """QoS policy.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar five_qi: QoS Flow 5G QoS Indicator value. The 5QI identifies a specific QoS forwarding
-     treatment to be provided to a flow. This must not be a standardized 5QI value corresponding to
-     a GBR (guaranteed bit rate) QoS Flow. The illegal GBR 5QI values are: 1, 2, 3, 4, 65, 66, 67,
-     71, 72, 73, 74, 75, 76, 82, 83, 84, and 85. See 3GPP TS23.501 section 5.7.2.1 for a full
-     description of the 5QI parameter, and table 5.7.4-1 for the definition of which are the GBR 5QI
-     values.
+    :ivar five_qi: 5G QoS Flow Indicator value. The 5QI identifies a specific QoS forwarding
+     treatment to be provided to a flow. See 3GPP TS23.501 section 5.7.2.1 for a full description of
+     the 5QI parameter, and table 5.7.4-1 for the definition the 5QI values.
     :vartype five_qi: int
     :ivar allocation_and_retention_priority_level: QoS Flow allocation and retention priority (ARP)
      level. Flows with higher priority preempt flows with lower priority, if the settings of
      ``preemptionCapability`` and ``preemptionVulnerability`` allow it. 1 is the highest level of
      priority. If this field is not specified then ``5qi`` is used to derive the ARP value. See 3GPP
      TS23.501 section 5.7.2.2 for a full description of the ARP parameters.
     :vartype allocation_and_retention_priority_level: int
@@ -2507,23 +2822,20 @@
         self,
         *,
         maximum_bit_rate: "_models.Ambr",
         five_qi: Optional[int] = None,
         allocation_and_retention_priority_level: Optional[int] = None,
         preemption_capability: Optional[Union[str, "_models.PreemptionCapability"]] = None,
         preemption_vulnerability: Optional[Union[str, "_models.PreemptionVulnerability"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword five_qi: QoS Flow 5G QoS Indicator value. The 5QI identifies a specific QoS forwarding
-         treatment to be provided to a flow. This must not be a standardized 5QI value corresponding to
-         a GBR (guaranteed bit rate) QoS Flow. The illegal GBR 5QI values are: 1, 2, 3, 4, 65, 66, 67,
-         71, 72, 73, 74, 75, 76, 82, 83, 84, and 85. See 3GPP TS23.501 section 5.7.2.1 for a full
-         description of the 5QI parameter, and table 5.7.4-1 for the definition of which are the GBR 5QI
-         values.
+        :keyword five_qi: 5G QoS Flow Indicator value. The 5QI identifies a specific QoS forwarding
+         treatment to be provided to a flow. See 3GPP TS23.501 section 5.7.2.1 for a full description of
+         the 5QI parameter, and table 5.7.4-1 for the definition the 5QI values.
         :paramtype five_qi: int
         :keyword allocation_and_retention_priority_level: QoS Flow allocation and retention priority
          (ARP) level. Flows with higher priority preempt flows with lower priority, if the settings of
          ``preemptionCapability`` and ``preemptionVulnerability`` allow it. 1 is the highest level of
          priority. If this field is not specified then ``5qi`` is used to derive the ARP value. See 3GPP
          TS23.501 section 5.7.2.2 for a full description of the ARP parameters.
         :paramtype allocation_and_retention_priority_level: int
@@ -2551,20 +2863,17 @@
 
 
 class PccRuleQosPolicy(QosPolicy):
     """Data flow policy rule QoS policy.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar five_qi: QoS Flow 5G QoS Indicator value. The 5QI identifies a specific QoS forwarding
-     treatment to be provided to a flow. This must not be a standardized 5QI value corresponding to
-     a GBR (guaranteed bit rate) QoS Flow. The illegal GBR 5QI values are: 1, 2, 3, 4, 65, 66, 67,
-     71, 72, 73, 74, 75, 76, 82, 83, 84, and 85. See 3GPP TS23.501 section 5.7.2.1 for a full
-     description of the 5QI parameter, and table 5.7.4-1 for the definition of which are the GBR 5QI
-     values.
+    :ivar five_qi: 5G QoS Flow Indicator value. The 5QI identifies a specific QoS forwarding
+     treatment to be provided to a flow. See 3GPP TS23.501 section 5.7.2.1 for a full description of
+     the 5QI parameter, and table 5.7.4-1 for the definition the 5QI values.
     :vartype five_qi: int
     :ivar allocation_and_retention_priority_level: QoS Flow allocation and retention priority (ARP)
      level. Flows with higher priority preempt flows with lower priority, if the settings of
      ``preemptionCapability`` and ``preemptionVulnerability`` allow it. 1 is the highest level of
      priority. If this field is not specified then ``5qi`` is used to derive the ARP value. See 3GPP
      TS23.501 section 5.7.2.2 for a full description of the ARP parameters.
     :vartype allocation_and_retention_priority_level: int
@@ -2608,23 +2917,20 @@
         *,
         maximum_bit_rate: "_models.Ambr",
         five_qi: Optional[int] = None,
         allocation_and_retention_priority_level: Optional[int] = None,
         preemption_capability: Optional[Union[str, "_models.PreemptionCapability"]] = None,
         preemption_vulnerability: Optional[Union[str, "_models.PreemptionVulnerability"]] = None,
         guaranteed_bit_rate: Optional["_models.Ambr"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword five_qi: QoS Flow 5G QoS Indicator value. The 5QI identifies a specific QoS forwarding
-         treatment to be provided to a flow. This must not be a standardized 5QI value corresponding to
-         a GBR (guaranteed bit rate) QoS Flow. The illegal GBR 5QI values are: 1, 2, 3, 4, 65, 66, 67,
-         71, 72, 73, 74, 75, 76, 82, 83, 84, and 85. See 3GPP TS23.501 section 5.7.2.1 for a full
-         description of the 5QI parameter, and table 5.7.4-1 for the definition of which are the GBR 5QI
-         values.
+        :keyword five_qi: 5G QoS Flow Indicator value. The 5QI identifies a specific QoS forwarding
+         treatment to be provided to a flow. See 3GPP TS23.501 section 5.7.2.1 for a full description of
+         the 5QI parameter, and table 5.7.4-1 for the definition the 5QI values.
         :paramtype five_qi: int
         :keyword allocation_and_retention_priority_level: QoS Flow allocation and retention priority
          (ARP) level. Flows with higher priority preempt flows with lower priority, if the settings of
          ``preemptionCapability`` and ``preemptionVulnerability`` allow it. 1 is the highest level of
          priority. If this field is not specified then ``5qi`` is used to derive the ARP value. See 3GPP
          TS23.501 section 5.7.2.2 for a full description of the ARP parameters.
         :paramtype allocation_and_retention_priority_level: int
@@ -2677,15 +2983,15 @@
 
     _attribute_map = {
         "tcp": {"key": "tcp", "type": "int"},
         "udp": {"key": "udp", "type": "int"},
         "icmp": {"key": "icmp", "type": "int"},
     }
 
-    def __init__(self, *, tcp: int = 180, udp: int = 30, icmp: int = 30, **kwargs):
+    def __init__(self, *, tcp: int = 180, udp: int = 30, icmp: int = 30, **kwargs: Any) -> None:
         """
         :keyword tcp: Pinhole timeout for TCP pinholes in seconds. Default for TCP is 3 minutes.
         :paramtype tcp: int
         :keyword udp: Pinhole timeout for UDP pinholes in seconds. Default for UDP is 30 seconds.
         :paramtype udp: int
         :keyword icmp: Pinhole timeout for ICMP pinholes in seconds. Default for ICMP Echo is 30
          seconds.
@@ -2735,16 +3041,16 @@
         *,
         platform_type: Optional[Union[str, "_models.PlatformType"]] = None,
         version_state: Optional[Union[str, "_models.VersionState"]] = None,
         minimum_platform_software_version: Optional[str] = None,
         maximum_platform_software_version: Optional[str] = None,
         recommended_version: Optional[Union[str, "_models.RecommendedVersion"]] = None,
         obsolete_version: Optional[Union[str, "_models.ObsoleteVersion"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword platform_type: The platform type where this version can be deployed. Known values are:
          "AKS-HCI" and "3P-AZURE-STACK-HCI".
         :paramtype platform_type: str or ~azure.mgmt.mobilenetwork.models.PlatformType
         :keyword version_state: The state of this packet core control plane version on this platform.
          Known values are: "Unknown", "Preview", "Validating", "ValidationFailed", "Active", and
          "Deprecated".
@@ -2816,16 +3122,16 @@
         self,
         *,
         type: Union[str, "_models.PlatformType"],
         azure_stack_edge_device: Optional["_models.AzureStackEdgeDeviceResourceId"] = None,
         azure_stack_hci_cluster: Optional["_models.AzureStackHCIClusterResourceId"] = None,
         connected_cluster: Optional["_models.ConnectedClusterResourceId"] = None,
         custom_location: Optional["_models.CustomLocationResourceId"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword type: The platform type where packet core is deployed. Required. Known values are:
          "AKS-HCI" and "3P-AZURE-STACK-HCI".
         :paramtype type: str or ~azure.mgmt.mobilenetwork.models.PlatformType
         :keyword azure_stack_edge_device: The Azure Stack Edge device where the packet core is
          deployed. If the device is part of a fault tolerant pair, either device in the pair can be
          specified.
@@ -2866,61 +3172,63 @@
     }
 
     _attribute_map = {
         "mcc": {"key": "mcc", "type": "str"},
         "mnc": {"key": "mnc", "type": "str"},
     }
 
-    def __init__(self, *, mcc: str, mnc: str, **kwargs):
+    def __init__(self, *, mcc: str, mnc: str, **kwargs: Any) -> None:
         """
         :keyword mcc: Mobile country code (MCC). Required.
         :paramtype mcc: str
         :keyword mnc: Mobile network code (MNC). Required.
         :paramtype mnc: str
         """
         super().__init__(**kwargs)
         self.mcc = mcc
         self.mnc = mnc
 
 
 class PortRange(_serialization.Model):
     """Range of port numbers to use as translated ports on each translated address.
     If not specified and NAPT is enabled, this range defaults to 1,024 - 49,999.
-    (Ports under 1,024 should not be used because these are special purpose ports reserved by IANA. Ports 50,000 and above are reserved for non-NAPT use.).
+    (Ports under 1,024 should not be used because these are special purpose ports reserved by IANA.
+    Ports 50,000 and above are reserved for non-NAPT use.).
 
-        :ivar min_port: The minimum port number.
-        :vartype min_port: int
-        :ivar max_port: The maximum port number.
-        :vartype max_port: int
+    :ivar min_port: The minimum port number.
+    :vartype min_port: int
+    :ivar max_port: The maximum port number.
+    :vartype max_port: int
     """
 
     _validation = {
         "min_port": {"maximum": 65535, "minimum": 1024},
         "max_port": {"maximum": 65535, "minimum": 1024},
     }
 
     _attribute_map = {
         "min_port": {"key": "minPort", "type": "int"},
         "max_port": {"key": "maxPort", "type": "int"},
     }
 
-    def __init__(self, *, min_port: int = 1024, max_port: int = 49999, **kwargs):
+    def __init__(self, *, min_port: int = 1024, max_port: int = 49999, **kwargs: Any) -> None:
         """
         :keyword min_port: The minimum port number.
         :paramtype min_port: int
         :keyword max_port: The maximum port number.
         :paramtype max_port: int
         """
         super().__init__(**kwargs)
         self.min_port = min_port
         self.max_port = max_port
 
 
 class PortReuseHoldTimes(_serialization.Model):
-    """The minimum time (in seconds) that will pass before a port that was used by a closed pinhole can be recycled for use by another pinhole. All hold times must be minimum 1 second.
+    """The minimum time (in seconds) that will pass before a port that was used by a closed pinhole
+    can be recycled for use by another pinhole. All hold times must be minimum 1 second.
 
     :ivar tcp: Minimum time in seconds that will pass before a TCP port that was used by a closed
      pinhole can be reused. Default for TCP is 2 minutes.
     :vartype tcp: int
     :ivar udp: Minimum time in seconds that will pass before a UDP port that was used by a closed
      pinhole can be reused. Default for UDP is 1 minute.
     :vartype udp: int
@@ -2932,15 +3240,15 @@
     }
 
     _attribute_map = {
         "tcp": {"key": "tcp", "type": "int"},
         "udp": {"key": "udp", "type": "int"},
     }
 
-    def __init__(self, *, tcp: int = 120, udp: int = 60, **kwargs):
+    def __init__(self, *, tcp: int = 120, udp: int = 60, **kwargs: Any) -> None:
         """
         :keyword tcp: Minimum time in seconds that will pass before a TCP port that was used by a
          closed pinhole can be reused. Default for TCP is 2 minutes.
         :paramtype tcp: int
         :keyword udp: Minimum time in seconds that will pass before a UDP port that was used by a
          closed pinhole can be reused. Default for UDP is 1 minute.
         :paramtype udp: int
@@ -2953,16 +3261,16 @@
 class Service(TrackedResource):
     """Service resource. Must be created in the same location as its parent mobile network.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -3015,16 +3323,16 @@
         self,
         *,
         location: str,
         service_precedence: int,
         pcc_rules: List["_models.PccRuleConfiguration"],
         tags: Optional[Dict[str, str]] = None,
         service_qos_policy: Optional["_models.QosPolicy"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword service_precedence: A precedence value that is used to decide between services when
          identifying the QoS values to use for a particular SIM. A lower value means a higher priority.
@@ -3102,16 +3410,16 @@
         self,
         *,
         template_name: str,
         direction: Union[str, "_models.SdfDirection"],
         protocol: List[str],
         remote_ip_list: List[str],
         ports: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword template_name: The name of the data flow template. This must be unique within the
          parent data flow policy rule. You must not use any of the following reserved strings -
          ``default``\ , ``requested`` or ``service``. Required.
         :paramtype template_name: str
         :keyword direction: The direction of this flow. Required. Known values are: "Uplink",
          "Downlink", and "Bidirectional".
@@ -3162,15 +3470,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Service]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.Service"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.Service"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: A list of services.
         :paramtype value: list[~azure.mgmt.mobilenetwork.models.Service]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -3192,15 +3500,15 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Service resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -3208,16 +3516,16 @@
 class Sim(ProxyResource):  # pylint: disable=too-many-instance-attributes
     """SIM resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -3304,16 +3612,16 @@
         international_mobile_subscriber_identity: str,
         integrated_circuit_card_identifier: Optional[str] = None,
         device_type: Optional[str] = None,
         sim_policy: Optional["_models.SimPolicyResourceId"] = None,
         static_ip_configuration: Optional[List["_models.SimStaticIpProperties"]] = None,
         authentication_key: Optional[str] = None,
         operator_key_code: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword international_mobile_subscriber_identity: The international mobile subscriber identity
          (IMSI) for the SIM. Required.
         :paramtype international_mobile_subscriber_identity: str
         :keyword integrated_circuit_card_identifier: The integrated circuit card ID (ICCID) for the
          SIM.
         :paramtype integrated_circuit_card_identifier: str
@@ -3361,15 +3669,15 @@
         "sims": {"required": True, "min_items": 1},
     }
 
     _attribute_map = {
         "sims": {"key": "sims", "type": "[str]"},
     }
 
-    def __init__(self, *, sims: List[str], **kwargs):
+    def __init__(self, *, sims: List[str], **kwargs: Any) -> None:
         """
         :keyword sims: A list of SIM resource names to delete. Required.
         :paramtype sims: list[str]
         """
         super().__init__(**kwargs)
         self.sims = sims
 
@@ -3377,16 +3685,16 @@
 class SimGroup(TrackedResource):
     """SIM group resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -3434,16 +3742,16 @@
         self,
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
         identity: Optional["_models.ManagedServiceIdentity"] = None,
         encryption_key: Optional["_models.KeyVaultKey"] = None,
         mobile_network: Optional["_models.MobileNetworkResourceId"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword identity: The identity used to retrieve the encryption key from Azure key vault.
         :paramtype identity: ~azure.mgmt.mobilenetwork.models.ManagedServiceIdentity
@@ -3476,15 +3784,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[SimGroup]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.SimGroup"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.SimGroup"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: A list of SIM groups in a resource group.
         :paramtype value: list[~azure.mgmt.mobilenetwork.models.SimGroup]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -3506,15 +3814,15 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: SIM group resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -3535,15 +3843,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Sim]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.Sim"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.Sim"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: A list of SIMs in a resource group.
         :paramtype value: list[~azure.mgmt.mobilenetwork.models.Sim]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -3629,16 +3937,16 @@
         name: str,
         international_mobile_subscriber_identity: str,
         integrated_circuit_card_identifier: Optional[str] = None,
         device_type: Optional[str] = None,
         sim_policy: Optional["_models.SimPolicyResourceId"] = None,
         static_ip_configuration: Optional[List["_models.SimStaticIpProperties"]] = None,
         encrypted_credentials: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: The name of the SIM. Required.
         :paramtype name: str
         :keyword international_mobile_subscriber_identity: The international mobile subscriber identity
          (IMSI) for the SIM. Required.
         :paramtype international_mobile_subscriber_identity: str
         :keyword integrated_circuit_card_identifier: The integrated circuit card ID (ICCID) for the
@@ -3758,16 +4066,16 @@
         international_mobile_subscriber_identity: str,
         integrated_circuit_card_identifier: Optional[str] = None,
         device_type: Optional[str] = None,
         sim_policy: Optional["_models.SimPolicyResourceId"] = None,
         static_ip_configuration: Optional[List["_models.SimStaticIpProperties"]] = None,
         authentication_key: Optional[str] = None,
         operator_key_code: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: The name of the SIM. Required.
         :paramtype name: str
         :keyword international_mobile_subscriber_identity: The international mobile subscriber identity
          (IMSI) for the SIM. Required.
         :paramtype international_mobile_subscriber_identity: str
         :keyword integrated_circuit_card_identifier: The integrated circuit card ID (ICCID) for the
@@ -3808,16 +4116,16 @@
 class SimPolicy(TrackedResource):  # pylint: disable=too-many-instance-attributes
     """SIM policy resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -3840,16 +4148,16 @@
     :ivar default_slice: The default slice to use if the UE does not explicitly specify it. This
      slice must exist in the ``sliceConfigurations`` map. The slice must be in the same location as
      the SIM policy. Required.
     :vartype default_slice: ~azure.mgmt.mobilenetwork.models.SliceResourceId
     :ivar rfsp_index: RAT/Frequency Selection Priority Index, defined in 3GPP TS 36.413. This is an
      optional setting and by default is unspecified.
     :vartype rfsp_index: int
-    :ivar registration_timer: Interval for the UE periodic registration update procedure, in
-     seconds.
+    :ivar registration_timer: UE periodic registration update timer (5G) or UE periodic tracking
+     area update timer (4G), in seconds.
     :vartype registration_timer: int
     :ivar slice_configurations: The allowed slices and the settings to use for them. The list must
      not contain duplicate items and must contain at least one item. Required.
     :vartype slice_configurations: list[~azure.mgmt.mobilenetwork.models.SliceConfiguration]
     """
 
     _validation = {
@@ -3889,16 +4197,16 @@
         location: str,
         ue_ambr: "_models.Ambr",
         default_slice: "_models.SliceResourceId",
         slice_configurations: List["_models.SliceConfiguration"],
         tags: Optional[Dict[str, str]] = None,
         rfsp_index: Optional[int] = None,
         registration_timer: int = 3240,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword ue_ambr: Aggregate maximum bit rate across all non-GBR QoS flows of all PDU sessions
          of a given UE. See 3GPP TS23.501 section 5.7.2.6 for a full description of the UE-AMBR.
@@ -3907,16 +4215,16 @@
         :keyword default_slice: The default slice to use if the UE does not explicitly specify it. This
          slice must exist in the ``sliceConfigurations`` map. The slice must be in the same location as
          the SIM policy. Required.
         :paramtype default_slice: ~azure.mgmt.mobilenetwork.models.SliceResourceId
         :keyword rfsp_index: RAT/Frequency Selection Priority Index, defined in 3GPP TS 36.413. This is
          an optional setting and by default is unspecified.
         :paramtype rfsp_index: int
-        :keyword registration_timer: Interval for the UE periodic registration update procedure, in
-         seconds.
+        :keyword registration_timer: UE periodic registration update timer (5G) or UE periodic tracking
+         area update timer (4G), in seconds.
         :paramtype registration_timer: int
         :keyword slice_configurations: The allowed slices and the settings to use for them. The list
          must not contain duplicate items and must contain at least one item. Required.
         :paramtype slice_configurations: list[~azure.mgmt.mobilenetwork.models.SliceConfiguration]
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.provisioning_state = None
@@ -3944,15 +4252,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[SimPolicy]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.SimPolicy"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.SimPolicy"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: A list of SIM policies.
         :paramtype value: list[~azure.mgmt.mobilenetwork.models.SimPolicy]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -3974,15 +4282,15 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: SIM policy resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -4064,16 +4372,16 @@
         international_mobile_subscriber_identity: str,
         integrated_circuit_card_identifier: Optional[str] = None,
         device_type: Optional[str] = None,
         sim_policy: Optional["_models.SimPolicyResourceId"] = None,
         static_ip_configuration: Optional[List["_models.SimStaticIpProperties"]] = None,
         authentication_key: Optional[str] = None,
         operator_key_code: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword international_mobile_subscriber_identity: The international mobile subscriber identity
          (IMSI) for the SIM. Required.
         :paramtype international_mobile_subscriber_identity: str
         :keyword integrated_circuit_card_identifier: The integrated circuit card ID (ICCID) for the
          SIM.
         :paramtype integrated_circuit_card_identifier: str
@@ -4128,16 +4436,16 @@
 
     def __init__(
         self,
         *,
         attached_data_network: Optional["_models.AttachedDataNetworkResourceId"] = None,
         slice: Optional["_models.SliceResourceId"] = None,
         static_ip: Optional["_models.SimStaticIpPropertiesStaticIp"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword attached_data_network: The attached data network on which the static IP address will
          be used. The combination of attached data network and slice defines the network scope of the IP
          address. The attached data network must be in the same location as the SIM.
         :paramtype attached_data_network:
          ~azure.mgmt.mobilenetwork.models.AttachedDataNetworkResourceId
         :keyword slice: The network slice on which the static IP address will be used. The combination
@@ -4168,15 +4476,15 @@
         },
     }
 
     _attribute_map = {
         "ipv4_address": {"key": "ipv4Address", "type": "str"},
     }
 
-    def __init__(self, *, ipv4_address: Optional[str] = None, **kwargs):
+    def __init__(self, *, ipv4_address: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword ipv4_address: The IPv4 address assigned to the SIM at this network scope. This address
          must be in the userEquipmentStaticAddressPoolPrefix defined in the attached data network.
         :paramtype ipv4_address: str
         """
         super().__init__(**kwargs)
         self.ipv4_address = ipv4_address
@@ -4195,15 +4503,15 @@
         "sims": {"required": True, "min_items": 1},
     }
 
     _attribute_map = {
         "sims": {"key": "sims", "type": "[SimNameAndProperties]"},
     }
 
-    def __init__(self, *, sims: List["_models.SimNameAndProperties"], **kwargs):
+    def __init__(self, *, sims: List["_models.SimNameAndProperties"], **kwargs: Any) -> None:
         """
         :keyword sims: A list of SIMs to upload. Required.
         :paramtype sims: list[~azure.mgmt.mobilenetwork.models.SimNameAndProperties]
         """
         super().__init__(**kwargs)
         self.sims = sims
 
@@ -4211,16 +4519,16 @@
 class Site(TrackedResource):
     """Site resource. Must be created in the same location as its parent mobile network.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -4255,26 +4563,48 @@
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "network_functions": {"key": "properties.networkFunctions", "type": "[SubResource]"},
     }
 
-    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.provisioning_state = None
         self.network_functions = None
 
 
+class SiteDeletePacketCore(_serialization.Model):
+    """The packet core to delete under a site.
+
+    :ivar packet_core: Reference to an packet core control plane resource.
+    :vartype packet_core: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlaneResourceId
+    """
+
+    _attribute_map = {
+        "packet_core": {"key": "packetCore", "type": "PacketCoreControlPlaneResourceId"},
+    }
+
+    def __init__(
+        self, *, packet_core: Optional["_models.PacketCoreControlPlaneResourceId"] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword packet_core: Reference to an packet core control plane resource.
+        :paramtype packet_core: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlaneResourceId
+        """
+        super().__init__(**kwargs)
+        self.packet_core = packet_core
+
+
 class SiteListResult(_serialization.Model):
     """Response for sites API service call.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar value: A list of sites in a mobile network.
     :vartype value: list[~azure.mgmt.mobilenetwork.models.Site]
@@ -4287,15 +4617,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Site]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.Site"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.Site"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: A list of sites in a mobile network.
         :paramtype value: list[~azure.mgmt.mobilenetwork.models.Site]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -4317,15 +4647,15 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Site resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -4333,16 +4663,16 @@
 class Slice(TrackedResource):
     """Network slice resource. Must be created in the same location as its parent mobile network.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -4387,16 +4717,16 @@
     def __init__(
         self,
         *,
         location: str,
         snssai: "_models.Snssai",
         tags: Optional[Dict[str, str]] = None,
         description: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword snssai: Single-network slice selection assistance information (S-NSSAI). Unique at the
          scope of a mobile network. Required.
@@ -4442,16 +4772,16 @@
 
     def __init__(
         self,
         *,
         slice: "_models.SliceResourceId",
         default_data_network: "_models.DataNetworkResourceId",
         data_network_configurations: List["_models.DataNetworkConfiguration"],
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword slice: A reference to the slice that these settings apply to. The slice must be in the
          same location as the SIM policy. Required.
         :paramtype slice: ~azure.mgmt.mobilenetwork.models.SliceResourceId
         :keyword default_data_network: The default data network to use if the UE does not explicitly
          specify it. Configuration for this object must exist in the ``dataNetworkConfigurations`` map.
          The data network must be in the same location as the SIM policy. Required.
@@ -4483,15 +4813,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Slice]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.Slice"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.Slice"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: A list of network slices in a mobile network.
         :paramtype value: list[~azure.mgmt.mobilenetwork.models.Slice]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -4513,15 +4843,15 @@
         },
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Slice resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -4543,15 +4873,15 @@
     }
 
     _attribute_map = {
         "sst": {"key": "sst", "type": "int"},
         "sd": {"key": "sd", "type": "str"},
     }
 
-    def __init__(self, *, sst: int, sd: Optional[str] = None, **kwargs):
+    def __init__(self, *, sst: int, sd: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword sst: Slice/service type (SST). Required.
         :paramtype sst: int
         :keyword sd: Slice differentiator (SD).
         :paramtype sd: str
         """
         super().__init__(**kwargs)
@@ -4572,15 +4902,15 @@
         "id": {"required": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: str, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Resource ID. Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -4618,16 +4948,16 @@
         *,
         created_by: Optional[str] = None,
         created_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         created_at: Optional[datetime.datetime] = None,
         last_modified_by: Optional[str] = None,
         last_modified_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         last_modified_at: Optional[datetime.datetime] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword created_by: The identity that created the resource.
         :paramtype created_by: str
         :keyword created_by_type: The type of identity that created the resource. Known values are:
          "User", "Application", "ManagedIdentity", and "Key".
         :paramtype created_by_type: str or ~azure.mgmt.mobilenetwork.models.CreatedByType
         :keyword created_at: The timestamp of resource creation (UTC).
@@ -4656,15 +4986,15 @@
     :vartype tags: dict[str, str]
     """
 
     _attribute_map = {
         "tags": {"key": "tags", "type": "{str}"},
     }
 
-    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         """
         super().__init__(**kwargs)
         self.tags = tags
 
@@ -4686,12 +5016,12 @@
     }
 
     _attribute_map = {
         "principal_id": {"key": "principalId", "type": "str"},
         "client_id": {"key": "clientId", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.principal_id = None
         self.client_id = None
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_services_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_services_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,32 +28,28 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_delete_request(
     resource_group_name: str, mobile_network_name: str, service_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/services/{serviceName}",
     )  # pylint: disable=line-too-long
@@ -67,15 +63,15 @@
         "serviceName": _SERIALIZER.url(
             "service_name",
             service_name,
             "str",
             max_length=64,
             pattern=r"^(?!(default|requested|service)$)[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -87,15 +83,15 @@
 
 def build_get_request(
     resource_group_name: str, mobile_network_name: str, service_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/services/{serviceName}",
     )  # pylint: disable=line-too-long
@@ -109,15 +105,15 @@
         "serviceName": _SERIALIZER.url(
             "service_name",
             service_name,
             "str",
             max_length=64,
             pattern=r"^(?!(default|requested|service)$)[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -129,15 +125,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, mobile_network_name: str, service_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/services/{serviceName}",
@@ -152,15 +148,15 @@
         "serviceName": _SERIALIZER.url(
             "service_name",
             service_name,
             "str",
             max_length=64,
             pattern=r"^(?!(default|requested|service)$)[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -174,25 +170,25 @@
 
 def build_update_tags_request(
     resource_group_name: str, mobile_network_name: str, service_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/services/{serviceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "serviceName": _SERIALIZER.url(
@@ -219,30 +215,30 @@
 
 def build_list_by_mobile_network_request(
     resource_group_name: str, mobile_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/services",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -281,17 +277,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             service_name=service_name,
             subscription_id=self._config.subscription_id,
@@ -299,16 +293,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -346,17 +341,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -421,17 +414,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Service] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             service_name=service_name,
             subscription_id=self._config.subscription_id,
@@ -439,16 +430,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -480,24 +472,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Service] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Service")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -510,16 +500,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -637,15 +628,15 @@
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param service_name: The name of the service. You must not use any of the following reserved
          strings - ``default``\ , ``requested`` or ``service``. Required.
         :type service_name: str
         :param parameters: Parameters supplied to the create or update service operation. Is either a
-         model type or a IO type. Required.
+         Service type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.Service or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -657,17 +648,15 @@
         :return: An instance of LROPoller that returns either Service or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.Service]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Service] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -790,16 +779,16 @@
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param service_name: The name of the service. You must not use any of the following reserved
          strings - ``default``\ , ``requested`` or ``service``. Required.
         :type service_name: str
-        :param parameters: Parameters supplied to update service tags. Is either a model type or a IO
-         type. Required.
+        :param parameters: Parameters supplied to update service tags. Is either a TagsObject type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Service or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.Service
@@ -812,24 +801,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Service] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -842,16 +829,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -883,17 +871,15 @@
         :return: An iterator like instance of either Service or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.Service]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ServiceListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -939,16 +925,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_slices_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_slices_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,41 +28,37 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_delete_request(
     resource_group_name: str, mobile_network_name: str, slice_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/slices/{sliceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "sliceName": _SERIALIZER.url(
@@ -83,24 +79,24 @@
 
 def build_get_request(
     resource_group_name: str, mobile_network_name: str, slice_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/slices/{sliceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "sliceName": _SERIALIZER.url(
@@ -121,25 +117,25 @@
 
 def build_create_or_update_request(
     resource_group_name: str, mobile_network_name: str, slice_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/slices/{sliceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "sliceName": _SERIALIZER.url(
@@ -162,25 +158,25 @@
 
 def build_update_tags_request(
     resource_group_name: str, mobile_network_name: str, slice_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/slices/{sliceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "sliceName": _SERIALIZER.url(
@@ -203,24 +199,24 @@
 
 def build_list_by_mobile_network_request(
     resource_group_name: str, mobile_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/slices",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
@@ -265,17 +261,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             slice_name=slice_name,
             subscription_id=self._config.subscription_id,
@@ -283,16 +277,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -329,17 +324,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -401,17 +394,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Slice] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             slice_name=slice_name,
             subscription_id=self._config.subscription_id,
@@ -419,16 +410,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -460,24 +452,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Slice] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Slice")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -490,16 +480,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -616,15 +607,15 @@
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param slice_name: The name of the network slice. Required.
         :type slice_name: str
         :param parameters: Parameters supplied to the create or update network slice operation. Is
-         either a model type or a IO type. Required.
+         either a Slice type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.Slice or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -636,17 +627,15 @@
         :return: An instance of LROPoller that returns either Slice or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.Slice]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Slice] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -766,16 +755,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param slice_name: The name of the network slice. Required.
         :type slice_name: str
-        :param parameters: Parameters supplied to update network slice tags. Is either a model type or
-         a IO type. Required.
+        :param parameters: Parameters supplied to update network slice tags. Is either a TagsObject
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Slice or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.Slice
@@ -788,24 +777,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Slice] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -818,16 +805,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -859,17 +847,15 @@
         :return: An iterator like instance of either Slice or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.Slice]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SliceListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -915,16 +901,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_data_networks_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_data_networks_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,41 +28,37 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_delete_request(
     resource_group_name: str, mobile_network_name: str, data_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/dataNetworks/{dataNetworkName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "dataNetworkName": _SERIALIZER.url(
@@ -87,24 +83,24 @@
 
 def build_get_request(
     resource_group_name: str, mobile_network_name: str, data_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/dataNetworks/{dataNetworkName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "dataNetworkName": _SERIALIZER.url(
@@ -129,25 +125,25 @@
 
 def build_create_or_update_request(
     resource_group_name: str, mobile_network_name: str, data_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/dataNetworks/{dataNetworkName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "dataNetworkName": _SERIALIZER.url(
@@ -174,25 +170,25 @@
 
 def build_update_tags_request(
     resource_group_name: str, mobile_network_name: str, data_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/dataNetworks/{dataNetworkName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "dataNetworkName": _SERIALIZER.url(
@@ -219,24 +215,24 @@
 
 def build_list_by_mobile_network_request(
     resource_group_name: str, mobile_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/dataNetworks",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
@@ -281,17 +277,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             data_network_name=data_network_name,
             subscription_id=self._config.subscription_id,
@@ -299,16 +293,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -345,17 +340,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -419,17 +412,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DataNetwork] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             data_network_name=data_network_name,
             subscription_id=self._config.subscription_id,
@@ -437,16 +428,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -478,24 +470,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DataNetwork] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "DataNetwork")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -508,16 +498,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -636,15 +627,15 @@
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param data_network_name: The name of the data network. Required.
         :type data_network_name: str
         :param parameters: Parameters supplied to the create or update data network operation. Is
-         either a model type or a IO type. Required.
+         either a DataNetwork type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.DataNetwork or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -657,17 +648,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.DataNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DataNetwork] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -787,16 +776,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param data_network_name: The name of the data network. Required.
         :type data_network_name: str
-        :param parameters: Parameters supplied to update data network tags. Is either a model type or a
-         IO type. Required.
+        :param parameters: Parameters supplied to update data network tags. Is either a TagsObject type
+         or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DataNetwork or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.DataNetwork
@@ -809,24 +798,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DataNetwork] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -839,16 +826,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -880,17 +868,15 @@
         :return: An iterator like instance of either DataNetwork or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.DataNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DataNetworkListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -936,16 +922,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_sim_groups_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_sim_groups_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,41 +28,37 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_delete_request(
     resource_group_name: str, sim_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/simGroups/{simGroupName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "simGroupName": _SERIALIZER.url(
             "sim_group_name", sim_group_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
@@ -80,24 +76,24 @@
 
 def build_get_request(
     resource_group_name: str, sim_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/simGroups/{simGroupName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "simGroupName": _SERIALIZER.url(
             "sim_group_name", sim_group_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
@@ -115,25 +111,25 @@
 
 def build_create_or_update_request(
     resource_group_name: str, sim_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/simGroups/{simGroupName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "simGroupName": _SERIALIZER.url(
             "sim_group_name", sim_group_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
@@ -153,25 +149,25 @@
 
 def build_update_tags_request(
     resource_group_name: str, sim_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/simGroups/{simGroupName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "simGroupName": _SERIALIZER.url(
             "sim_group_name", sim_group_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
@@ -189,21 +185,21 @@
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.MobileNetwork/simGroups")
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -213,27 +209,27 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/simGroups",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -272,33 +268,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -331,17 +326,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -400,33 +393,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SimGroup] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -453,24 +445,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SimGroup] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "SimGroup")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
@@ -482,16 +472,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -590,15 +581,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
         :param parameters: Parameters supplied to the create or update SIM group operation. Is either a
-         model type or a IO type. Required.
+         SimGroup type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.SimGroup or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -610,17 +601,15 @@
         :return: An instance of LROPoller that returns either SimGroup or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.SimGroup]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SimGroup] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -664,28 +653,28 @@
     }
 
     @overload
     def update_tags(
         self,
         resource_group_name: str,
         sim_group_name: str,
-        parameters: _models.TagsObject,
+        parameters: _models.IdentityAndTagsObject,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.SimGroup:
-        """Updates SIM group tags.
+        """Patch SIM group resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
-        :param parameters: Parameters supplied to update SIM group tags. Required.
-        :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject
+        :param parameters: Parameters supplied to patch SIM group resource. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.IdentityAndTagsObject
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SimGroup or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.SimGroup
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -697,46 +686,50 @@
         resource_group_name: str,
         sim_group_name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.SimGroup:
-        """Updates SIM group tags.
+        """Patch SIM group resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
-        :param parameters: Parameters supplied to update SIM group tags. Required.
+        :param parameters: Parameters supplied to patch SIM group resource. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SimGroup or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.SimGroup
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update_tags(
-        self, resource_group_name: str, sim_group_name: str, parameters: Union[_models.TagsObject, IO], **kwargs: Any
+        self,
+        resource_group_name: str,
+        sim_group_name: str,
+        parameters: Union[_models.IdentityAndTagsObject, IO],
+        **kwargs: Any
     ) -> _models.SimGroup:
-        """Updates SIM group tags.
+        """Patch SIM group resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
-        :param parameters: Parameters supplied to update SIM group tags. Is either a model type or a IO
-         type. Required.
-        :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
+        :param parameters: Parameters supplied to patch SIM group resource. Is either a
+         IdentityAndTagsObject type or a IO type. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.IdentityAndTagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SimGroup or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.SimGroup
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -748,27 +741,25 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SimGroup] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
-            _json = self._serialize.body(parameters, "TagsObject")
+            _json = self._serialize.body(parameters, "IdentityAndTagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
@@ -777,16 +768,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -811,17 +803,15 @@
         :return: An iterator like instance of either SimGroup or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.SimGroup]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SimGroupListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -865,16 +855,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -898,17 +889,15 @@
         :return: An iterator like instance of either SimGroup or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.SimGroup]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SimGroupListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -953,16 +942,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/__init__.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._attached_data_networks_operations import AttachedDataNetworksOperations
 from ._data_networks_operations import DataNetworksOperations
+from ._diagnostics_packages_operations import DiagnosticsPackagesOperations
 from ._mobile_networks_operations import MobileNetworksOperations
 from ._operations import Operations
+from ._packet_captures_operations import PacketCapturesOperations
 from ._packet_core_control_planes_operations import PacketCoreControlPlanesOperations
 from ._packet_core_control_plane_versions_operations import PacketCoreControlPlaneVersionsOperations
 from ._packet_core_data_planes_operations import PacketCoreDataPlanesOperations
 from ._services_operations import ServicesOperations
 from ._sims_operations import SimsOperations
 from ._sim_groups_operations import SimGroupsOperations
 from ._sim_policies_operations import SimPoliciesOperations
@@ -23,16 +25,18 @@
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AttachedDataNetworksOperations",
     "DataNetworksOperations",
+    "DiagnosticsPackagesOperations",
     "MobileNetworksOperations",
     "Operations",
+    "PacketCapturesOperations",
     "PacketCoreControlPlanesOperations",
     "PacketCoreControlPlaneVersionsOperations",
     "PacketCoreDataPlanesOperations",
     "ServicesOperations",
     "SimsOperations",
     "SimGroupsOperations",
     "SimPoliciesOperations",
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_attached_data_networks_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_attached_data_networks_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,18 +28,14 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -50,24 +46,24 @@
     attached_data_network_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/packetCoreDataPlanes/{packetCoreDataPlaneName}/attachedDataNetworks/{attachedDataNetworkName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
@@ -108,24 +104,24 @@
     attached_data_network_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/packetCoreDataPlanes/{packetCoreDataPlaneName}/attachedDataNetworks/{attachedDataNetworkName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
@@ -166,25 +162,25 @@
     attached_data_network_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/packetCoreDataPlanes/{packetCoreDataPlaneName}/attachedDataNetworks/{attachedDataNetworkName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
@@ -227,25 +223,25 @@
     attached_data_network_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/packetCoreDataPlanes/{packetCoreDataPlaneName}/attachedDataNetworks/{attachedDataNetworkName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
@@ -287,24 +283,24 @@
     packet_core_data_plane_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/packetCoreDataPlanes/{packetCoreDataPlaneName}/attachedDataNetworks",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
@@ -365,17 +361,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             packet_core_data_plane_name=packet_core_data_plane_name,
             attached_data_network_name=attached_data_network_name,
@@ -384,16 +378,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -437,17 +432,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -519,17 +512,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AttachedDataNetwork] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             packet_core_data_plane_name=packet_core_data_plane_name,
             attached_data_network_name=attached_data_network_name,
@@ -538,16 +529,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -580,24 +572,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AttachedDataNetwork] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "AttachedDataNetwork")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
@@ -611,16 +601,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -748,15 +739,15 @@
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
         :param packet_core_data_plane_name: The name of the packet core data plane. Required.
         :type packet_core_data_plane_name: str
         :param attached_data_network_name: The name of the attached data network. Required.
         :type attached_data_network_name: str
         :param parameters: Parameters supplied to the create or update attached data network operation.
-         Is either a model type or a IO type. Required.
+         Is either a AttachedDataNetwork type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.AttachedDataNetwork or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -769,17 +760,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.AttachedDataNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AttachedDataNetwork] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -909,16 +898,16 @@
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
         :param packet_core_data_plane_name: The name of the packet core data plane. Required.
         :type packet_core_data_plane_name: str
         :param attached_data_network_name: The name of the attached data network. Required.
         :type attached_data_network_name: str
-        :param parameters: Parameters supplied to update attached data network tags. Is either a model
-         type or a IO type. Required.
+        :param parameters: Parameters supplied to update attached data network tags. Is either a
+         TagsObject type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AttachedDataNetwork or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.AttachedDataNetwork
@@ -931,24 +920,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AttachedDataNetwork] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
@@ -962,16 +949,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1009,17 +997,15 @@
         :return: An iterator like instance of either AttachedDataNetwork or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.AttachedDataNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AttachedDataNetworkListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1066,16 +1052,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_sim_policies_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_sim_policies_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,32 +28,28 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_delete_request(
     resource_group_name: str, mobile_network_name: str, sim_policy_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/simPolicies/{simPolicyName}",
     )  # pylint: disable=line-too-long
@@ -63,15 +59,15 @@
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "simPolicyName": _SERIALIZER.url(
             "sim_policy_name", sim_policy_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -83,15 +79,15 @@
 
 def build_get_request(
     resource_group_name: str, mobile_network_name: str, sim_policy_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/simPolicies/{simPolicyName}",
     )  # pylint: disable=line-too-long
@@ -101,15 +97,15 @@
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "simPolicyName": _SERIALIZER.url(
             "sim_policy_name", sim_policy_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -121,15 +117,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, mobile_network_name: str, sim_policy_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/simPolicies/{simPolicyName}",
@@ -140,15 +136,15 @@
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "simPolicyName": _SERIALIZER.url(
             "sim_policy_name", sim_policy_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -162,25 +158,25 @@
 
 def build_update_tags_request(
     resource_group_name: str, mobile_network_name: str, sim_policy_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/simPolicies/{simPolicyName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "simPolicyName": _SERIALIZER.url(
@@ -203,30 +199,30 @@
 
 def build_list_by_mobile_network_request(
     resource_group_name: str, mobile_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/simPolicies",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -265,17 +261,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             sim_policy_name=sim_policy_name,
             subscription_id=self._config.subscription_id,
@@ -283,16 +277,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -329,17 +324,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -403,17 +396,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SimPolicy] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             sim_policy_name=sim_policy_name,
             subscription_id=self._config.subscription_id,
@@ -421,16 +412,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -462,24 +454,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SimPolicy] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "SimPolicy")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -492,16 +482,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -616,15 +607,15 @@
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param sim_policy_name: The name of the SIM policy. Required.
         :type sim_policy_name: str
         :param parameters: Parameters supplied to the create or update SIM policy operation. Is either
-         a model type or a IO type. Required.
+         a SimPolicy type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.SimPolicy or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -636,17 +627,15 @@
         :return: An instance of LROPoller that returns either SimPolicy or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.SimPolicy]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SimPolicy] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -766,16 +755,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param sim_policy_name: The name of the SIM policy. Required.
         :type sim_policy_name: str
-        :param parameters: Parameters supplied to update SIM policy tags. Is either a model type or a
-         IO type. Required.
+        :param parameters: Parameters supplied to update SIM policy tags. Is either a TagsObject type
+         or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SimPolicy or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.SimPolicy
@@ -788,24 +777,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SimPolicy] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -818,16 +805,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -859,17 +847,15 @@
         :return: An iterator like instance of either SimPolicy or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.SimPolicy]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SimPolicyListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -915,16 +901,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_sims_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_sims_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,41 +28,37 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_delete_request(
     resource_group_name: str, sim_group_name: str, sim_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/simGroups/{simGroupName}/sims/{simName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "simGroupName": _SERIALIZER.url(
             "sim_group_name", sim_group_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "simName": _SERIALIZER.url("sim_name", sim_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"),
@@ -81,24 +77,24 @@
 
 def build_get_request(
     resource_group_name: str, sim_group_name: str, sim_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/simGroups/{simGroupName}/sims/{simName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "simGroupName": _SERIALIZER.url(
             "sim_group_name", sim_group_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "simName": _SERIALIZER.url("sim_name", sim_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"),
@@ -117,25 +113,25 @@
 
 def build_create_or_update_request(
     resource_group_name: str, sim_group_name: str, sim_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/simGroups/{simGroupName}/sims/{simName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "simGroupName": _SERIALIZER.url(
             "sim_group_name", sim_group_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "simName": _SERIALIZER.url("sim_name", sim_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"),
@@ -156,27 +152,27 @@
 
 def build_list_by_group_request(
     resource_group_name: str, sim_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/simGroups/{simGroupName}/sims",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "simGroupName": _SERIALIZER.url(
             "sim_group_name", sim_group_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -191,28 +187,28 @@
 
 def build_bulk_upload_request(
     resource_group_name: str, sim_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/simGroups/{simGroupName}/uploadSims",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "simGroupName": _SERIALIZER.url(
             "sim_group_name", sim_group_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -229,28 +225,28 @@
 
 def build_bulk_delete_request(
     resource_group_name: str, sim_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/simGroups/{simGroupName}/deleteSims",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "simGroupName": _SERIALIZER.url(
             "sim_group_name", sim_group_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -267,28 +263,28 @@
 
 def build_bulk_upload_encrypted_request(
     resource_group_name: str, sim_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/simGroups/{simGroupName}/uploadEncryptedSims",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "simGroupName": _SERIALIZER.url(
             "sim_group_name", sim_group_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -332,17 +328,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
             sim_name=sim_name,
             subscription_id=self._config.subscription_id,
@@ -350,16 +344,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -396,17 +391,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -468,17 +461,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Sim] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
             sim_name=sim_name,
             subscription_id=self._config.subscription_id,
@@ -486,16 +477,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -527,24 +519,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Sim] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Sim")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
@@ -557,16 +547,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -677,15 +668,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
         :param sim_name: The name of the SIM. Required.
         :type sim_name: str
-        :param parameters: Parameters supplied to the create or update SIM operation. Is either a model
+        :param parameters: Parameters supplied to the create or update SIM operation. Is either a Sim
          type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.Sim or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
@@ -698,17 +689,15 @@
         :return: An instance of LROPoller that returns either Sim or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.Sim]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Sim] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -765,17 +754,15 @@
         :return: An iterator like instance of either Sim or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.Sim]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SimListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -821,16 +808,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -853,24 +841,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.AsyncOperationStatus]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "SimUploadList")
 
         request = build_bulk_upload_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
@@ -882,16 +868,17 @@
             template_url=self._bulk_upload_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -989,16 +976,16 @@
         """Bulk upload SIMs to a SIM group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
-        :param parameters: Parameters supplied to the bulk SIM upload operation. Is either a model type
-         or a IO type. Required.
+        :param parameters: Parameters supplied to the bulk SIM upload operation. Is either a
+         SimUploadList type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.SimUploadList or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1011,17 +998,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.AsyncOperationStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AsyncOperationStatus] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._bulk_upload_initial(
@@ -1074,24 +1059,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.AsyncOperationStatus]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "SimDeleteList")
 
         request = build_bulk_delete_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
@@ -1103,16 +1086,17 @@
             template_url=self._bulk_delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1210,16 +1194,16 @@
         """Bulk delete SIMs from a SIM group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
-        :param parameters: Parameters supplied to the bulk SIM delete operation. Is either a model type
-         or a IO type. Required.
+        :param parameters: Parameters supplied to the bulk SIM delete operation. Is either a
+         SimDeleteList type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.SimDeleteList or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1232,17 +1216,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.AsyncOperationStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AsyncOperationStatus] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._bulk_delete_initial(
@@ -1299,24 +1281,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.AsyncOperationStatus]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "EncryptedSimUploadList")
 
         request = build_bulk_upload_encrypted_request(
             resource_group_name=resource_group_name,
             sim_group_name=sim_group_name,
@@ -1328,16 +1308,17 @@
             template_url=self._bulk_upload_encrypted_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1440,15 +1421,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param sim_group_name: The name of the SIM Group. Required.
         :type sim_group_name: str
         :param parameters: Parameters supplied to the encrypted SIMs upload operation. Is either a
-         model type or a IO type. Required.
+         EncryptedSimUploadList type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.EncryptedSimUploadList or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1461,17 +1442,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.AsyncOperationStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AsyncOperationStatus] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._bulk_upload_encrypted_initial(
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_sites_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_sites_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,41 +28,37 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_delete_request(
     resource_group_name: str, mobile_network_name: str, site_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "siteName": _SERIALIZER.url(
@@ -83,24 +79,24 @@
 
 def build_get_request(
     resource_group_name: str, mobile_network_name: str, site_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "siteName": _SERIALIZER.url(
@@ -121,25 +117,25 @@
 
 def build_create_or_update_request(
     resource_group_name: str, mobile_network_name: str, site_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "siteName": _SERIALIZER.url(
@@ -162,25 +158,25 @@
 
 def build_update_tags_request(
     resource_group_name: str, mobile_network_name: str, site_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
         "siteName": _SERIALIZER.url(
@@ -203,24 +199,24 @@
 
 def build_list_by_mobile_network_request(
     resource_group_name: str, mobile_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
@@ -232,14 +228,55 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_delete_packet_core_request(
+    resource_group_name: str, mobile_network_name: str, site_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}/deletePacketCore",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "mobileNetworkName": _SERIALIZER.url(
+            "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
+        ),
+        "siteName": _SERIALIZER.url(
+            "site_name", site_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
+        ),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 class SitesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.mobilenetwork.MobileNetworkManagementClient`'s
@@ -265,17 +302,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             site_name=site_name,
             subscription_id=self._config.subscription_id,
@@ -283,16 +318,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -330,17 +366,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -402,17 +436,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Site] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             site_name=site_name,
             subscription_id=self._config.subscription_id,
@@ -420,16 +452,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -461,24 +494,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Site] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Site")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -491,16 +522,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -617,15 +649,15 @@
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param site_name: The name of the mobile network site. Required.
         :type site_name: str
         :param parameters: Parameters supplied to the create or update mobile network site operation.
-         Is either a model type or a IO type. Required.
+         Is either a Site type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.Site or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -637,17 +669,15 @@
         :return: An instance of LROPoller that returns either Site or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.Site]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Site] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -767,16 +797,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param site_name: The name of the mobile network site. Required.
         :type site_name: str
-        :param parameters: Parameters supplied to update network site tags. Is either a model type or a
-         IO type. Required.
+        :param parameters: Parameters supplied to update network site tags. Is either a TagsObject type
+         or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Site or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.Site
@@ -789,24 +819,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Site] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -819,16 +847,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -860,17 +889,15 @@
         :return: An iterator like instance of either Site or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.Site]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SiteListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -916,16 +943,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -933,7 +961,234 @@
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     list_by_mobile_network.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites"
     }
+
+    def _delete_packet_core_initial(  # pylint: disable=inconsistent-return-statements
+        self,
+        resource_group_name: str,
+        mobile_network_name: str,
+        site_name: str,
+        parameters: Union[_models.SiteDeletePacketCore, IO],
+        **kwargs: Any
+    ) -> None:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(parameters, (IOBase, bytes)):
+            _content = parameters
+        else:
+            _json = self._serialize.body(parameters, "SiteDeletePacketCore")
+
+        request = build_delete_packet_core_request(
+            resource_group_name=resource_group_name,
+            mobile_network_name=mobile_network_name,
+            site_name=site_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self._delete_packet_core_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    _delete_packet_core_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}/deletePacketCore"
+    }
+
+    @overload
+    def begin_delete_packet_core(
+        self,
+        resource_group_name: str,
+        mobile_network_name: str,
+        site_name: str,
+        parameters: _models.SiteDeletePacketCore,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[None]:
+        """Deletes a packet core under the specified mobile network site.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param mobile_network_name: The name of the mobile network. Required.
+        :type mobile_network_name: str
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
+        :param parameters: Parameters supplied to delete a packet core under a site. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.SiteDeletePacketCore
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def begin_delete_packet_core(
+        self,
+        resource_group_name: str,
+        mobile_network_name: str,
+        site_name: str,
+        parameters: IO,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[None]:
+        """Deletes a packet core under the specified mobile network site.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param mobile_network_name: The name of the mobile network. Required.
+        :type mobile_network_name: str
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
+        :param parameters: Parameters supplied to delete a packet core under a site. Required.
+        :type parameters: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def begin_delete_packet_core(
+        self,
+        resource_group_name: str,
+        mobile_network_name: str,
+        site_name: str,
+        parameters: Union[_models.SiteDeletePacketCore, IO],
+        **kwargs: Any
+    ) -> LROPoller[None]:
+        """Deletes a packet core under the specified mobile network site.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param mobile_network_name: The name of the mobile network. Required.
+        :type mobile_network_name: str
+        :param site_name: The name of the mobile network site. Required.
+        :type site_name: str
+        :param parameters: Parameters supplied to delete a packet core under a site. Is either a
+         SiteDeletePacketCore type or a IO type. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.SiteDeletePacketCore or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._delete_packet_core_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                mobile_network_name=mobile_network_name,
+                site_name=site_name,
+                parameters=parameters,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+            if cls:
+                return cls(pipeline_response, None, {})
+
+        if polling is True:
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_delete_packet_core.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}/sites/{siteName}/deletePacketCore"
+    }
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_control_plane_versions_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_packet_core_control_plane_versions_operations.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,113 +2,68 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
-from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
+from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
+from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
-from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpResponse
+from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from .. import models as _models
-from .._serialization import Serializer
-from .._vendor import _convert_request, _format_url_section
-
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
-T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
-
-_SERIALIZER = Serializer()
-_SERIALIZER.client_side_validation = False
-
-
-def build_get_request(version_name: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop("template_url", "/providers/Microsoft.MobileNetwork/packetCoreControlPlaneVersions/{versionName}")
-    path_format_arguments = {
-        "versionName": _SERIALIZER.url("version_name", version_name, "str"),
-    }
-
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_list_request(**kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop("template_url", "/providers/Microsoft.MobileNetwork/packetCoreControlPlaneVersions")
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+from ... import models as _models
+from ..._vendor import _convert_request
+from ...operations._packet_core_control_plane_versions_operations import (
+    build_get_by_subscription_request,
+    build_get_request,
+    build_list_by_subscription_request,
+    build_list_request,
+)
 
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+T = TypeVar("T")
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class PacketCoreControlPlaneVersionsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.mobilenetwork.MobileNetworkManagementClient`'s
+        :class:`~azure.mgmt.mobilenetwork.aio.MobileNetworkManagementClient`'s
         :attr:`packet_core_control_plane_versions` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @distributed_trace
-    def get(self, version_name: str, **kwargs: Any) -> _models.PacketCoreControlPlaneVersion:
+    @distributed_trace_async
+    async def get(self, version_name: str, **kwargs: Any) -> _models.PacketCoreControlPlaneVersion:
         """Gets information about the specified packet core control plane version.
 
         :param version_name: The name of the packet core control plane version. Required.
         :type version_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PacketCoreControlPlaneVersion or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlaneVersion
@@ -121,31 +76,30 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PacketCoreControlPlaneVersion] = kwargs.pop("cls", None)
 
         request = build_get_request(
             version_name=version_name,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -157,30 +111,28 @@
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {"url": "/providers/Microsoft.MobileNetwork/packetCoreControlPlaneVersions/{versionName}"}
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> Iterable["_models.PacketCoreControlPlaneVersion"]:
+    def list(self, **kwargs: Any) -> AsyncIterable["_models.PacketCoreControlPlaneVersion"]:
         """Lists all supported packet core control planes versions.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PacketCoreControlPlaneVersion or the result of
          cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.PacketCoreControlPlaneVersion]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.PacketCoreControlPlaneVersion]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PacketCoreControlPlaneVersionListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -213,32 +165,177 @@
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
-        def extract_data(pipeline_response):
+        async def extract_data(pipeline_response):
             deserialized = self._deserialize("PacketCoreControlPlaneVersionListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, iter(list_of_elem)
+            return deserialized.next_link or None, AsyncList(list_of_elem)
 
-        def get_next(next_link=None):
+        async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return ItemPaged(get_next, extract_data)
+        return AsyncItemPaged(get_next, extract_data)
 
     list.metadata = {"url": "/providers/Microsoft.MobileNetwork/packetCoreControlPlaneVersions"}
+
+    @distributed_trace_async
+    async def get_by_subscription(self, version_name: str, **kwargs: Any) -> _models.PacketCoreControlPlaneVersion:
+        """Gets information about the specified packet core control plane version.
+
+        :param version_name: The name of the packet core control plane version. Required.
+        :type version_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: PacketCoreControlPlaneVersion or the result of cls(response)
+        :rtype: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlaneVersion
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.PacketCoreControlPlaneVersion] = kwargs.pop("cls", None)
+
+        request = build_get_by_subscription_request(
+            version_name=version_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.get_by_subscription.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("PacketCoreControlPlaneVersion", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    get_by_subscription.metadata = {
+        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.MobileNetwork/packetCoreControlPlaneVersions/{versionName}"
+    }
+
+    @distributed_trace
+    def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.PacketCoreControlPlaneVersion"]:
+        """Lists all supported packet core control planes versions.
+
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: An iterator like instance of either PacketCoreControlPlaneVersion or the result of
+         cls(response)
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.mobilenetwork.models.PacketCoreControlPlaneVersion]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.PacketCoreControlPlaneVersionListResult] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                request = build_list_by_subscription_request(
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    template_url=self.list_by_subscription.metadata["url"],
+                    headers=_headers,
+                    params=_params,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
+            return request
+
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("PacketCoreControlPlaneVersionListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, AsyncList(list_of_elem)
+
+        async def get_next(next_link=None):
+            request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+            return pipeline_response
+
+        return AsyncItemPaged(get_next, extract_data)
+
+    list_by_subscription.metadata = {
+        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.MobileNetwork/packetCoreControlPlaneVersions"
+    }
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_mobile_networks_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_mobile_networks_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,41 +28,37 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_delete_request(
     resource_group_name: str, mobile_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
@@ -80,24 +76,24 @@
 
 def build_get_request(
     resource_group_name: str, mobile_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
@@ -115,25 +111,25 @@
 
 def build_create_or_update_request(
     resource_group_name: str, mobile_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
@@ -153,25 +149,25 @@
 
 def build_update_tags_request(
     resource_group_name: str, mobile_network_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks/{mobileNetworkName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "mobileNetworkName": _SERIALIZER.url(
             "mobile_network_name", mobile_network_name, "str", max_length=64, pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$"
         ),
     }
@@ -189,23 +185,23 @@
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.MobileNetwork/mobileNetworks"
     )
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -215,24 +211,24 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/mobileNetworks",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -274,33 +270,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -333,17 +328,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -402,33 +395,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MobileNetwork] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -459,24 +451,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.MobileNetwork] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "MobileNetwork")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -488,16 +478,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -604,15 +595,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
         :param parameters: Parameters supplied to the create or update mobile network operation. Is
-         either a model type or a IO type. Required.
+         either a MobileNetwork type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.MobileNetwork or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -625,17 +616,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.MobileNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.MobileNetwork] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -745,16 +734,16 @@
         """Updates mobile network tags.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param mobile_network_name: The name of the mobile network. Required.
         :type mobile_network_name: str
-        :param parameters: Parameters supplied to update mobile network tags. Is either a model type or
-         a IO type. Required.
+        :param parameters: Parameters supplied to update mobile network tags. Is either a TagsObject
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MobileNetwork or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.MobileNetwork
@@ -767,24 +756,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.MobileNetwork] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             mobile_network_name=mobile_network_name,
@@ -796,16 +783,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -830,17 +818,15 @@
         :return: An iterator like instance of either MobileNetwork or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.MobileNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MobileNetworkListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -884,16 +870,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -917,17 +904,15 @@
         :return: An iterator like instance of either MobileNetwork or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.MobileNetwork]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MobileNetworkListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -972,16 +957,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_data_planes_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_data_planes_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,18 +28,14 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -49,15 +45,15 @@
     packet_core_data_plane_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/packetCoreDataPlanes/{packetCoreDataPlaneName}",
     )  # pylint: disable=line-too-long
@@ -75,15 +71,15 @@
         "packetCoreDataPlaneName": _SERIALIZER.url(
             "packet_core_data_plane_name",
             packet_core_data_plane_name,
             "str",
             max_length=64,
             pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -99,15 +95,15 @@
     packet_core_data_plane_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/packetCoreDataPlanes/{packetCoreDataPlaneName}",
     )  # pylint: disable=line-too-long
@@ -125,15 +121,15 @@
         "packetCoreDataPlaneName": _SERIALIZER.url(
             "packet_core_data_plane_name",
             packet_core_data_plane_name,
             "str",
             max_length=64,
             pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -149,15 +145,15 @@
     packet_core_data_plane_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/packetCoreDataPlanes/{packetCoreDataPlaneName}",
@@ -176,15 +172,15 @@
         "packetCoreDataPlaneName": _SERIALIZER.url(
             "packet_core_data_plane_name",
             packet_core_data_plane_name,
             "str",
             max_length=64,
             pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -202,15 +198,15 @@
     packet_core_data_plane_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/packetCoreDataPlanes/{packetCoreDataPlaneName}",
@@ -229,15 +225,15 @@
         "packetCoreDataPlaneName": _SERIALIZER.url(
             "packet_core_data_plane_name",
             packet_core_data_plane_name,
             "str",
             max_length=64,
             pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -251,15 +247,15 @@
 
 def build_list_by_packet_core_control_plane_request(
     resource_group_name: str, packet_core_control_plane_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/packetCoreDataPlanes",
     )  # pylint: disable=line-too-long
@@ -270,15 +266,15 @@
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
             max_length=64,
             pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -321,17 +317,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             packet_core_data_plane_name=packet_core_data_plane_name,
             subscription_id=self._config.subscription_id,
@@ -339,16 +333,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -389,17 +384,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -467,17 +460,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PacketCoreDataPlane] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             packet_core_data_plane_name=packet_core_data_plane_name,
             subscription_id=self._config.subscription_id,
@@ -485,16 +476,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -526,24 +518,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PacketCoreDataPlane] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "PacketCoreDataPlane")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
@@ -556,16 +546,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -684,15 +675,15 @@
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
         :param packet_core_data_plane_name: The name of the packet core data plane. Required.
         :type packet_core_data_plane_name: str
         :param parameters: Parameters supplied to the create or update packet core data plane
-         operation. Is either a model type or a IO type. Required.
+         operation. Is either a PacketCoreDataPlane type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.PacketCoreDataPlane or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -705,17 +696,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.PacketCoreDataPlane]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PacketCoreDataPlane] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -835,16 +824,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
         :param packet_core_data_plane_name: The name of the packet core data plane. Required.
         :type packet_core_data_plane_name: str
-        :param parameters: Parameters supplied to update packet core data plane tags. Is either a model
-         type or a IO type. Required.
+        :param parameters: Parameters supplied to update packet core data plane tags. Is either a
+         TagsObject type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PacketCoreDataPlane or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.PacketCoreDataPlane
@@ -857,24 +846,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PacketCoreDataPlane] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
@@ -887,16 +874,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -928,17 +916,15 @@
         :return: An iterator like instance of either PacketCoreDataPlane or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.PacketCoreDataPlane]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PacketCoreDataPlaneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -984,16 +970,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_patch.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-mobilenetwork-2.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_control_planes_operations.py` & `azure-mgmt-mobilenetwork-3.0.0/azure/mgmt/mobilenetwork/operations/_packet_core_control_planes_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,32 +28,28 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_delete_request(
     resource_group_name: str, packet_core_control_plane_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}",
     )  # pylint: disable=line-too-long
@@ -64,15 +60,15 @@
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
             max_length=64,
             pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -84,15 +80,15 @@
 
 def build_get_request(
     resource_group_name: str, packet_core_control_plane_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}",
     )  # pylint: disable=line-too-long
@@ -103,15 +99,15 @@
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
             max_length=64,
             pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -123,15 +119,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, packet_core_control_plane_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}",
@@ -143,15 +139,15 @@
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
             max_length=64,
             pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -165,15 +161,15 @@
 
 def build_update_tags_request(
     resource_group_name: str, packet_core_control_plane_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}",
@@ -185,15 +181,15 @@
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
             max_length=64,
             pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -205,23 +201,23 @@
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -231,27 +227,27 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -263,15 +259,15 @@
 
 def build_rollback_request(
     resource_group_name: str, packet_core_control_plane_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/rollback",
     )  # pylint: disable=line-too-long
@@ -282,15 +278,15 @@
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
             max_length=64,
             pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -302,15 +298,15 @@
 
 def build_reinstall_request(
     resource_group_name: str, packet_core_control_plane_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/reinstall",
     )  # pylint: disable=line-too-long
@@ -321,15 +317,15 @@
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
             max_length=64,
             pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -341,15 +337,15 @@
 
 def build_collect_diagnostics_package_request(
     resource_group_name: str, packet_core_control_plane_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MobileNetwork/packetCoreControlPlanes/{packetCoreControlPlaneName}/collectDiagnosticsPackage",
@@ -361,15 +357,15 @@
         "packetCoreControlPlaneName": _SERIALIZER.url(
             "packet_core_control_plane_name",
             packet_core_control_plane_name,
             "str",
             max_length=64,
             pattern=r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -410,33 +406,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -471,17 +466,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -542,33 +535,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PacketCoreControlPlane] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -599,24 +591,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PacketCoreControlPlane] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "PacketCoreControlPlane")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
@@ -628,16 +618,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -744,15 +735,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
         :param parameters: Parameters supplied to the create or update packet core control plane
-         operation. Is either a model type or a IO type. Required.
+         operation. Is either a PacketCoreControlPlane type or a IO type. Required.
         :type parameters: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -765,17 +756,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PacketCoreControlPlane] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -819,28 +808,28 @@
     }
 
     @overload
     def update_tags(
         self,
         resource_group_name: str,
         packet_core_control_plane_name: str,
-        parameters: _models.TagsObject,
+        parameters: _models.IdentityAndTagsObject,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.PacketCoreControlPlane:
-        """Updates packet core control planes tags.
+        """Patch packet core control plane resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
-        :param parameters: Parameters supplied to update packet core control plane tags. Required.
-        :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject
+        :param parameters: Parameters supplied to patch packet core control plane resource. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.IdentityAndTagsObject
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PacketCoreControlPlane or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -852,22 +841,22 @@
         resource_group_name: str,
         packet_core_control_plane_name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.PacketCoreControlPlane:
-        """Updates packet core control planes tags.
+        """Patch packet core control plane resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
-        :param parameters: Parameters supplied to update packet core control plane tags. Required.
+        :param parameters: Parameters supplied to patch packet core control plane resource. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PacketCoreControlPlane or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane
@@ -875,27 +864,27 @@
         """
 
     @distributed_trace
     def update_tags(
         self,
         resource_group_name: str,
         packet_core_control_plane_name: str,
-        parameters: Union[_models.TagsObject, IO],
+        parameters: Union[_models.IdentityAndTagsObject, IO],
         **kwargs: Any
     ) -> _models.PacketCoreControlPlane:
-        """Updates packet core control planes tags.
+        """Patch packet core control plane resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
-        :param parameters: Parameters supplied to update packet core control plane tags. Is either a
-         model type or a IO type. Required.
-        :type parameters: ~azure.mgmt.mobilenetwork.models.TagsObject or IO
+        :param parameters: Parameters supplied to patch packet core control plane resource. Is either a
+         IdentityAndTagsObject type or a IO type. Required.
+        :type parameters: ~azure.mgmt.mobilenetwork.models.IdentityAndTagsObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PacketCoreControlPlane or the result of cls(response)
         :rtype: ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -907,27 +896,25 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PacketCoreControlPlane] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
-            _json = self._serialize.body(parameters, "TagsObject")
+            _json = self._serialize.body(parameters, "IdentityAndTagsObject")
 
         request = build_update_tags_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
@@ -936,16 +923,17 @@
             template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -971,17 +959,15 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PacketCoreControlPlaneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1025,16 +1011,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -1061,17 +1048,15 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.mobilenetwork.models.PacketCoreControlPlane]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PacketCoreControlPlaneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1116,16 +1101,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -1148,33 +1134,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.AsyncOperationStatus]] = kwargs.pop("cls", None)
 
         request = build_rollback_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._rollback_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1217,17 +1202,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.AsyncOperationStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AsyncOperationStatus] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._rollback_initial(
                 resource_group_name=resource_group_name,
@@ -1277,33 +1260,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.AsyncOperationStatus]] = kwargs.pop("cls", None)
 
         request = build_reinstall_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._reinstall_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1347,17 +1329,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.AsyncOperationStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AsyncOperationStatus] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._reinstall_initial(
                 resource_group_name=resource_group_name,
@@ -1411,24 +1391,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.AsyncOperationStatus]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "PacketCoreControlPlaneCollectDiagnosticsPackage")
 
         request = build_collect_diagnostics_package_request(
             resource_group_name=resource_group_name,
             packet_core_control_plane_name=packet_core_control_plane_name,
@@ -1440,16 +1418,17 @@
             template_url=self._collect_diagnostics_package_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1558,15 +1537,16 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param packet_core_control_plane_name: The name of the packet core control plane. Required.
         :type packet_core_control_plane_name: str
         :param parameters: Parameters supplied to the packet core control plane collect diagnostics
-         package operation. Is either a model type or a IO type. Required.
+         package operation. Is either a PacketCoreControlPlaneCollectDiagnosticsPackage type or a IO
+         type. Required.
         :type parameters:
          ~azure.mgmt.mobilenetwork.models.PacketCoreControlPlaneCollectDiagnosticsPackage or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
@@ -1580,17 +1560,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.mobilenetwork.models.AsyncOperationStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AsyncOperationStatus] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._collect_diagnostics_package_initial(
```

