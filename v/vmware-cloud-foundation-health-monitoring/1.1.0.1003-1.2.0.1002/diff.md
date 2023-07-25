# Comparing `tmp/vmware-cloud-foundation-health-monitoring-1.1.0.1003.tar.gz` & `tmp/vmware-cloud-foundation-health-monitoring-1.2.0.1002.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware-cloud-foundation-health-monitoring-1.1.0.1003.tar", last modified: Thu May 25 19:11:19 2023, max compression
+gzip compressed data, was "vmware-cloud-foundation-health-monitoring-1.2.0.1002.tar", last modified: Tue Jul 25 16:54:16 2023, max compression
```

## Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003.tar` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.266141 vmware-cloud-foundation-health-monitoring-1.1.0.1003/
--rw-rw-rw-   0        0        0    10980 2023-05-25 19:11:19.266141 vmware-cloud-foundation-health-monitoring-1.1.0.1003/PKG-INFO
--rw-rw-rw-   0        0        0    10173 2023-05-25 19:10:32.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/README.md
--rw-rw-rw-   0        0        0       86 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/pyproject.toml
--rw-rw-rw-   0        0        0     1053 2023-05-25 19:11:19.281760 vmware-cloud-foundation-health-monitoring-1.1.0.1003/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.172402 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/
-drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.172402 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.219263 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/
--rw-rw-rw-   0        0        0   150145 2023-02-28 03:47:12.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Alert_Definitions.xml
--rw-rw-rw-   0        0        0    28694 2023-02-28 20:06:20.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Dashboards.zip
--rw-rw-rw-   0        0        0    51491 2023-02-28 03:58:54.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Notifications.json
--rw-rw-rw-   0        0        0    16701 2023-02-28 03:10:32.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Supermetrics.json
--rw-rw-rw-   0        0        0    10147 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Views.zip
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.234888 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/examples/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/examples/__init__.py
--rwxrwxrwx   0        0        0       55 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/examples/run_send-data-to-vrops.bat
-drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.234888 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/__init__.py
--rw-rw-rw-   0        0        0     3199 2023-05-25 19:10:32.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/encrypt-passwords.py
-drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.234888 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/encrypted_files/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/encrypted_files/__init__.py
--rw-rw-rw-   0        0        0     1456 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/env.json
--rw-rw-rw-   0        0        0    70999 2023-05-25 19:10:32.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/send-data-to-vrops.py
-drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.250512 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/
--rw-rw-rw-   0        0        0     5862 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/FolderUtility.py
--rw-rw-rw-   0        0        0     4438 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/LogUtility.py
--rw-rw-rw-   0        0        0     3042 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/PSUtility.py
--rw-rw-rw-   0        0        0     7362 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/SosRest.py
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.266141 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/
--rw-rw-rw-   0        0        0    10980 2023-05-25 19:11:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-05-25 19:11:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 19:11:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-25 19:11:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 16:54:16.050637 vmware-cloud-foundation-health-monitoring-1.2.0.1002/
+-rw-rw-rw-   0        0        0    11051 2023-07-25 16:54:16.050637 vmware-cloud-foundation-health-monitoring-1.2.0.1002/PKG-INFO
+-rw-rw-rw-   0        0        0    10244 2023-07-18 16:38:22.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/pyproject.toml
+-rw-rw-rw-   0        0        0     1053 2023-07-25 16:54:16.050637 vmware-cloud-foundation-health-monitoring-1.2.0.1002/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 16:54:15.894384 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/
+drwxrwxrwx   0        0        0        0 2023-07-25 16:54:15.894384 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:54:15.956885 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/vSAN/
+-rw-rw-rw-   0        0        0   150145 2023-02-28 03:47:12.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/vSAN/Alert_Definitions.xml
+-rw-rw-rw-   0        0        0    28694 2023-02-28 20:06:20.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/vSAN/Dashboards.zip
+-rw-rw-rw-   0        0        0   123879 2023-07-18 16:38:22.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/vSAN/Notifications.json
+-rw-rw-rw-   0        0        0    16701 2023-02-28 03:10:32.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/vSAN/Supermetrics.json
+-rw-rw-rw-   0        0        0    10147 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/vSAN/Views.zip
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/vSAN/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:54:15.956885 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/examples/__init__.py
+-rwxrwxrwx   0        0        0       55 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/examples/run_send-data-to-vrops.bat
+drwxrwxrwx   0        0        0        0 2023-07-25 16:54:15.972512 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/__init__.py
+-rw-rw-rw-   0        0        0     3199 2023-05-25 19:10:32.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/encrypt-passwords.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:54:15.972512 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/encrypted_files/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/encrypted_files/__init__.py
+-rw-rw-rw-   0        0        0     1456 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/env.json
+-rw-rw-rw-   0        0        0    70250 2023-07-25 16:53:08.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/send-data-to-vrops.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:54:16.019390 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/utils/
+-rw-rw-rw-   0        0        0     5862 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/utils/FolderUtility.py
+-rw-rw-rw-   0        0        0     4438 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/utils/LogUtility.py
+-rw-rw-rw-   0        0        0     3042 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/utils/PSUtility.py
+-rw-rw-rw-   0        0        0     7362 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/utils/SosRest.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:54:16.050637 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/
+-rw-rw-rw-   0        0        0    11051 2023-07-25 16:54:15.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2023-07-25 16:54:15.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 16:54:15.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-25 16:54:15.000000 vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/top_level.txt
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/PKG-INFO` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-cloud-foundation-health-monitoring
-Version: 1.1.0.1003
+Version: 1.2.0.1002
 Summary: Python Module for VMware Cloud Foundation Health Monitoring in vRealize Operations
 Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
 Author: Bhumitra Nagar
 Author-email: bnagar@vmware.com
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
 Project-URL: repository, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
@@ -25,141 +25,142 @@
   - [Implementation](#implementation)
   - [vRealize Operations Dashboards Preview](#vRealize-operations-dashboards-preview)
   - [Known Issues](#known-issues)
   - [Support](#support)
 
 ## Introduction
 
-This content supports the [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation) validated solution which enables the user to monitor the operational state of your VMware Cloud Foundation environment through custom dashboards, alerts, and notifications. These custom dashboards are intended to serve as an extension to native vRealize Operations dashboards and dashboards that are enabled via the respective management packs.
+This content supports the [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation) validated solution which enables the user to monitor the operational state of your [VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation) environment through custom dashboards, alerts, and notifications. These custom dashboards are intended to serve as an extension to native vRealize Operations dashboards and dashboards that are enabled using the respective management packs.
 
 ## Requirements
 
 ### Platforms
 
-- [VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation) 4.4 or later
+- VMware Cloud Foundation 5.0
+- VMware Cloud Foundation 4.5
+- VMware Cloud Foundation 4.4
 
 ### Operating Systems
 
-- [VMware Photon OS](https://vmware.github.io/photon/) 3.0 and 4.0
 - Microsoft Windows Server 2019 and 2022
+- [VMware Photon OS](https://vmware.github.io/photon/) 3.0 and 4.0
 
 ### Python Version
+
 - [Python 3.x](https://www.python.org/downloads/)
 
 Follow the [Python Beginners Guide](https://wiki.python.org/moin/BeginnersGuide/Download) to download and install Python.
 
 ### Python Libraries
 
 Install requried Python libraries by running the following commands on the host virtual machine:
+
   ```python
   pip install requests
   pip install setuptools
   pip install paramiko
   pip install maskpass==0.3.1
-  
   ```
 
 ### PowerShell Editions and Versions
-- PowerShell Core 7.2.0 or later
-- Microsoft Windows PowerShell 5.1
 
+- Microsoft Windows PowerShell 5.1
+- PowerShell Core 7.2.0 or later
 
 ### PowerShell Modules
 
-- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 2.1.0
-
+- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) - latest version
 
-
-## Implementation 
+## Implementation
 
 Follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)
 
-
 ## vRealize Operations Dashboards Preview
- 
+
 1. VCF Health Rollup
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup2-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup3-min.png)
 
 2. VCF Backup Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Backups1-min.png)
-   
+
 3. VCF Certificate Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates2-min.png)
-   
+
 4. VCF Compute Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute2-min.png)
-   
+
 5. VCF Connectivity Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity2-min.png)
 
 6. VCF DNS Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS2-min.png)
 
 7. VCF Hardware Compatibility
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min2.png)
-   
+
 8. VCF Networking Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking3-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking4-min.png)
 
 9. VCF NTP Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP3-min.png)
-   
+
 10. VCF Password Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password2-min.png)
 
 11. VCF SDDC Manager and vCenter Services Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services2-min.png)
-    
+
 12. VCF Snapshot Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots2-min.png)
 
 13. VCF Storage Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage1-min.png)
 
 14. VCF vSAN Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN2-min.png)
 
-
 ## Known Issues
-### 1. [Remove FQDN suffix dependency in the name when configuring an NSX-T cloud account in vRealize Operations](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues/35)
 
-Please make sure that your NSX-T account name is configured as mentioned in this issue. 
+1. [Remove FQDN suffix dependency in the name when configuring an NSX-T cloud account in vRealize Operations](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues/35)
+
+    Please make sure that your NSX-T account name is configured as mentioned in this issue.
+
+2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.4.x. The filters on the vRealize Operations dashboards depend on the name.
 
-### 2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.4.x. The filters on the vReaize Operations dashboards depend on the name.
+    To set the Product Name for the vCenter Server, follow the below steps:
 
-To set the Product Name for the vCenter Server, follow the below steps - 
-1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn>/ui` as `administrator@vsphere.local`.
-2. In the `VMs and templates` inventory, expand the `management domain vCenter Server` tree and expand the management domain data center.
-3. Select the first `management domain vCenter Server virtual machine` and select `Configure` tab.
-4. In the `Settings` pane select `vApp Options`.
-5. Click the `Edit` button. The `Edit vApp Options` dialog box opens.
-6. If vApp options are disabled, select the `Enable vApp options` check box and click `OK`.
-7. Click the `Details` tab and enter `VMware vCenter Server Appliance` as product name in the `Name` field.
+    1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn>/ui` as `administrator@vsphere.local`.
+    2. In the `VMs and templates` inventory, expand the `management domain vCenter Server` tree and expand the management domain data center.
+    3. Select the first `management domain vCenter Server virtual machine` and select `Configure` tab.
+    4. In the `Settings` pane select `vApp Options`.
+    5. Click the `Edit` button. The `Edit vApp Options` dialog box opens.
+    6. If vApp options are disabled, select the `Enable vApp options` check box and click `OK`.
+    7. Click the `Details` tab and enter `VMware vCenter Server Appliance` as product name in the `Name` field.
 
-### 3. Shades of red, green, and yellow may vary on vRealize Operations widgets.
-Shades of red, green, and yellow may be different in different widgets but they represent the same thing. Ignore the shades as this is a vRealize Operations product limitation.
+3. Shades of red, green, and yellow may vary on vRealize Operations widgets
 
+    Shades of red, green, and yellow may be different in different widgets but they represent the same thing. Ignore the shades as this is a vRealize Operations product limitation.
 
 ## Support
 
-This Python module is not supported by VMware Support.
+This Python module is not supported by VMware Support Services.
 
 We welcome you to use the [GitHub Issues](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues) to report bugs or suggest enhancements.
 
 In order to have a good experience with our community, we recommend that you read the [contributing guidelines](../CONTRIBUTING.md).
 
 When filing an issue, please check existing open, or recently closed, issues to make sure someone else hasn't already
 reported the issue.
@@ -177,9 +178,7 @@
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/README.md` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,141 +9,142 @@
   - [Implementation](#implementation)
   - [vRealize Operations Dashboards Preview](#vRealize-operations-dashboards-preview)
   - [Known Issues](#known-issues)
   - [Support](#support)
 
 ## Introduction
 
-This content supports the [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation) validated solution which enables the user to monitor the operational state of your VMware Cloud Foundation environment through custom dashboards, alerts, and notifications. These custom dashboards are intended to serve as an extension to native vRealize Operations dashboards and dashboards that are enabled via the respective management packs.
+This content supports the [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation) validated solution which enables the user to monitor the operational state of your [VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation) environment through custom dashboards, alerts, and notifications. These custom dashboards are intended to serve as an extension to native vRealize Operations dashboards and dashboards that are enabled using the respective management packs.
 
 ## Requirements
 
 ### Platforms
 
-- [VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation) 4.4 or later
+- VMware Cloud Foundation 5.0
+- VMware Cloud Foundation 4.5
+- VMware Cloud Foundation 4.4
 
 ### Operating Systems
 
-- [VMware Photon OS](https://vmware.github.io/photon/) 3.0 and 4.0
 - Microsoft Windows Server 2019 and 2022
+- [VMware Photon OS](https://vmware.github.io/photon/) 3.0 and 4.0
 
 ### Python Version
+
 - [Python 3.x](https://www.python.org/downloads/)
 
 Follow the [Python Beginners Guide](https://wiki.python.org/moin/BeginnersGuide/Download) to download and install Python.
 
 ### Python Libraries
 
 Install requried Python libraries by running the following commands on the host virtual machine:
+
   ```python
   pip install requests
   pip install setuptools
   pip install paramiko
   pip install maskpass==0.3.1
-  
   ```
 
 ### PowerShell Editions and Versions
-- PowerShell Core 7.2.0 or later
-- Microsoft Windows PowerShell 5.1
 
+- Microsoft Windows PowerShell 5.1
+- PowerShell Core 7.2.0 or later
 
 ### PowerShell Modules
 
-- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 2.1.0
-
+- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) - latest version
 
-
-## Implementation 
+## Implementation
 
 Follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)
 
-
 ## vRealize Operations Dashboards Preview
- 
+
 1. VCF Health Rollup
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup2-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup3-min.png)
 
 2. VCF Backup Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Backups1-min.png)
-   
+
 3. VCF Certificate Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates2-min.png)
-   
+
 4. VCF Compute Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute2-min.png)
-   
+
 5. VCF Connectivity Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity2-min.png)
 
 6. VCF DNS Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS2-min.png)
 
 7. VCF Hardware Compatibility
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min2.png)
-   
+
 8. VCF Networking Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking3-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking4-min.png)
 
 9. VCF NTP Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP3-min.png)
-   
+
 10. VCF Password Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password2-min.png)
 
 11. VCF SDDC Manager and vCenter Services Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services2-min.png)
-    
+
 12. VCF Snapshot Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots2-min.png)
 
 13. VCF Storage Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage1-min.png)
 
 14. VCF vSAN Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN2-min.png)
 
-
 ## Known Issues
-### 1. [Remove FQDN suffix dependency in the name when configuring an NSX-T cloud account in vRealize Operations](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues/35)
 
-Please make sure that your NSX-T account name is configured as mentioned in this issue. 
+1. [Remove FQDN suffix dependency in the name when configuring an NSX-T cloud account in vRealize Operations](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues/35)
+
+    Please make sure that your NSX-T account name is configured as mentioned in this issue.
+
+2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.4.x. The filters on the vRealize Operations dashboards depend on the name.
 
-### 2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.4.x. The filters on the vReaize Operations dashboards depend on the name.
+    To set the Product Name for the vCenter Server, follow the below steps:
 
-To set the Product Name for the vCenter Server, follow the below steps - 
-1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn>/ui` as `administrator@vsphere.local`.
-2. In the `VMs and templates` inventory, expand the `management domain vCenter Server` tree and expand the management domain data center.
-3. Select the first `management domain vCenter Server virtual machine` and select `Configure` tab.
-4. In the `Settings` pane select `vApp Options`.
-5. Click the `Edit` button. The `Edit vApp Options` dialog box opens.
-6. If vApp options are disabled, select the `Enable vApp options` check box and click `OK`.
-7. Click the `Details` tab and enter `VMware vCenter Server Appliance` as product name in the `Name` field.
+    1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn>/ui` as `administrator@vsphere.local`.
+    2. In the `VMs and templates` inventory, expand the `management domain vCenter Server` tree and expand the management domain data center.
+    3. Select the first `management domain vCenter Server virtual machine` and select `Configure` tab.
+    4. In the `Settings` pane select `vApp Options`.
+    5. Click the `Edit` button. The `Edit vApp Options` dialog box opens.
+    6. If vApp options are disabled, select the `Enable vApp options` check box and click `OK`.
+    7. Click the `Details` tab and enter `VMware vCenter Server Appliance` as product name in the `Name` field.
 
-### 3. Shades of red, green, and yellow may vary on vRealize Operations widgets.
-Shades of red, green, and yellow may be different in different widgets but they represent the same thing. Ignore the shades as this is a vRealize Operations product limitation.
+3. Shades of red, green, and yellow may vary on vRealize Operations widgets
 
+    Shades of red, green, and yellow may be different in different widgets but they represent the same thing. Ignore the shades as this is a vRealize Operations product limitation.
 
 ## Support
 
-This Python module is not supported by VMware Support.
+This Python module is not supported by VMware Support Services.
 
 We welcome you to use the [GitHub Issues](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues) to report bugs or suggest enhancements.
 
 In order to have a good experience with our community, we recommend that you read the [contributing guidelines](../CONTRIBUTING.md).
 
 When filing an issue, please check existing open, or recently closed, issues to make sure someone else hasn't already
 reported the issue.
@@ -161,9 +162,7 @@
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/setup.cfg` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6d77 6172 652d 636c 6f75 642d   = vmware-cloud-
 00000020: 666f 756e 6461 7469 6f6e 2d68 6561 6c74  foundation-healt
 00000030: 682d 6d6f 6e69 746f 7269 6e67 0d0a 7665  h-monitoring..ve
-00000040: 7273 696f 6e20 3d20 312e 312e 302e 3130  rsion = 1.1.0.10
-00000050: 3033 0d0a 6175 7468 6f72 203d 2042 6875  03..author = Bhu
+00000040: 7273 696f 6e20 3d20 312e 322e 302e 3130  rsion = 1.2.0.10
+00000050: 3032 0d0a 6175 7468 6f72 203d 2042 6875  02..author = Bhu
 00000060: 6d69 7472 6120 4e61 6761 720d 0a61 7574  mitra Nagar..aut
 00000070: 686f 725f 656d 6169 6c20 3d20 626e 6167  hor_email = bnag
 00000080: 6172 4076 6d77 6172 652e 636f 6d0d 0a64  ar@vmware.com..d
 00000090: 6573 6372 6970 7469 6f6e 203d 2050 7974  escription = Pyt
 000000a0: 686f 6e20 4d6f 6475 6c65 2066 6f72 2056  hon Module for V
 000000b0: 4d77 6172 6520 436c 6f75 6420 466f 756e  Mware Cloud Foun
 000000c0: 6461 7469 6f6e 2048 6561 6c74 6820 4d6f  dation Health Mo
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Alert_Definitions.xml` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/vSAN/Alert_Definitions.xml`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Dashboards.zip` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/vSAN/Dashboards.zip`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Supermetrics.json` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/vSAN/Supermetrics.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Views.zip` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/artifacts/vSAN/Views.zip`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/encrypt-passwords.py` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/encrypt-passwords.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/env.json` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/env.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/send-data-to-vrops.py` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/send-data-to-vrops.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,34 +4,21 @@
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 # ===================================================================================================================
 # Created by:  Bhumitra Nagar - Senior Member of Technical Staff
 # Authors: Bhumitra Nagar, Sowjanya V
 # Date:   2023-05-04
-# Version: 1.1.0.1003
 # ===================================================================================================================
 #
 # Description:
 # The send-data-to-vrops.py script receives the operational health data as JSON from SOS utility and supporting
 # Powershell modules and then sends it to objects in vRealize Operations as custom metrics for use in dashboards
 # to monitor the platform's health.
 #
-# Change Log:
-# ---------------------------------------------------------------------------------------
-#    Version - Description
-# 1.1.0.1003 - docs: readme update and update version and dist files for release
-# 1.1.0.1002 - chore: code cleanup
-# 1.1.0.1001 - bug: [HRM] Date on Backups and Snapshot dashboard shown incorrectly #50
-# 1.1.0.1001 - artifacts_update: Updated views for backup and snapshots to address issue #50
-# 1.1.0.1001 - feat: [HRM] Remove SDDC Manager root password from Python module #38
-# 1.1.0.1000 - feat: [HRM] Update project structure to host module on PyPI
-# ---------------------------------------------------------------------------------------
-# 1.0.0.1002 - bug: [HRM] Exception while sending Backup status data to vROps #48
-#
 # Example:
 # python send-data-to-vrops.py [-options]
 #
 # [Options]:
 # -np : Retrieves the health data from SOS Utility and Powershell cmdlets and saves it JSON files.
 # It will not send the data to vRealize Operations
 
@@ -208,27 +195,28 @@
         modules_without_root = ['Publish-BackupStatus',
                                 'Publish-NsxtTransportNodeStatus',
                                 'Publish-NsxtTransportNodeTunnelStatus',
                                 'Publish-NsxtTier0BgpStatus',
                                 'Publish-SnapshotStatus',
                                 'Publish-ComponentConnectivityHealthNonSOS']
 
-        without_local_user_cmd = f'-server {self.sddc_manager_fqdn} -user {self.sddc_manager_user} ' \
-                                 f'-pass {self.sddc_manager_pwd} -allDomains -outputJson {self.logger.test_log_folder}'
-        request_token_cmd = f'Request-VCFToken -fqdn {self.sddc_manager_fqdn} -username {self.sddc_manager_user} ' \
-                            f'-password {self.sddc_manager_pwd}'
+        without_local_user_cmd = f"-server {self.sddc_manager_fqdn} -user {self.sddc_manager_user} " \
+                                 f"-pass '{self.sddc_manager_pwd}' -allDomains " \
+                                 f"-outputJson {self.logger.test_log_folder}"
+        request_token_cmd = f"Request-VCFToken -fqdn {self.sddc_manager_fqdn} -username {self.sddc_manager_user} " \
+                            f"-password '{self.sddc_manager_pwd}'"
         publish_nsx_cmd = 'Publish-NsxtHealthNonSOS ' + without_local_user_cmd
 
         combined_cmd = request_token_cmd + ' ; ' + publish_nsx_cmd
         psu.execute_ps_cmd(combined_cmd)
 
         # module requiring sddc local user
-        psu.execute_ps_cmd(f'Publish-StorageCapacityHealth {without_local_user_cmd} '
-                           f' -localUser {self.sddc_manager_local_user}'
-                           f' -localPass {self.sddc_manager_local_pwd}')
+        psu.execute_ps_cmd(f"Publish-StorageCapacityHealth {without_local_user_cmd} "
+                           f" -localUser {self.sddc_manager_local_user}"
+                           f" -localPass '{self.sddc_manager_local_pwd}'")
 
         for module in modules_without_root:
             psu.execute_ps_cmd(f'{module} {without_local_user_cmd}')
 
         self.logger.info(f'Generated JSON files for Publish-* cmdlets in location {self.logger.test_log_folder}')
 
     # TODO: change this function
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/FolderUtility.py` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/utils/FolderUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/LogUtility.py` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/utils/LogUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/PSUtility.py` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/utils/PSUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/SosRest.py` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/main/utils/SosRest.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-cloud-foundation-health-monitoring
-Version: 1.1.0.1003
+Version: 1.2.0.1002
 Summary: Python Module for VMware Cloud Foundation Health Monitoring in vRealize Operations
 Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
 Author: Bhumitra Nagar
 Author-email: bnagar@vmware.com
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
 Project-URL: repository, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
@@ -25,141 +25,142 @@
   - [Implementation](#implementation)
   - [vRealize Operations Dashboards Preview](#vRealize-operations-dashboards-preview)
   - [Known Issues](#known-issues)
   - [Support](#support)
 
 ## Introduction
 
-This content supports the [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation) validated solution which enables the user to monitor the operational state of your VMware Cloud Foundation environment through custom dashboards, alerts, and notifications. These custom dashboards are intended to serve as an extension to native vRealize Operations dashboards and dashboards that are enabled via the respective management packs.
+This content supports the [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation) validated solution which enables the user to monitor the operational state of your [VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation) environment through custom dashboards, alerts, and notifications. These custom dashboards are intended to serve as an extension to native vRealize Operations dashboards and dashboards that are enabled using the respective management packs.
 
 ## Requirements
 
 ### Platforms
 
-- [VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation) 4.4 or later
+- VMware Cloud Foundation 5.0
+- VMware Cloud Foundation 4.5
+- VMware Cloud Foundation 4.4
 
 ### Operating Systems
 
-- [VMware Photon OS](https://vmware.github.io/photon/) 3.0 and 4.0
 - Microsoft Windows Server 2019 and 2022
+- [VMware Photon OS](https://vmware.github.io/photon/) 3.0 and 4.0
 
 ### Python Version
+
 - [Python 3.x](https://www.python.org/downloads/)
 
 Follow the [Python Beginners Guide](https://wiki.python.org/moin/BeginnersGuide/Download) to download and install Python.
 
 ### Python Libraries
 
 Install requried Python libraries by running the following commands on the host virtual machine:
+
   ```python
   pip install requests
   pip install setuptools
   pip install paramiko
   pip install maskpass==0.3.1
-  
   ```
 
 ### PowerShell Editions and Versions
-- PowerShell Core 7.2.0 or later
-- Microsoft Windows PowerShell 5.1
 
+- Microsoft Windows PowerShell 5.1
+- PowerShell Core 7.2.0 or later
 
 ### PowerShell Modules
 
-- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 2.1.0
-
+- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) - latest version
 
-
-## Implementation 
+## Implementation
 
 Follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)
 
-
 ## vRealize Operations Dashboards Preview
- 
+
 1. VCF Health Rollup
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup2-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup3-min.png)
 
 2. VCF Backup Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Backups1-min.png)
-   
+
 3. VCF Certificate Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates2-min.png)
-   
+
 4. VCF Compute Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute2-min.png)
-   
+
 5. VCF Connectivity Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity2-min.png)
 
 6. VCF DNS Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS2-min.png)
 
 7. VCF Hardware Compatibility
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min2.png)
-   
+
 8. VCF Networking Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking3-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking4-min.png)
 
 9. VCF NTP Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP3-min.png)
-   
+
 10. VCF Password Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password2-min.png)
 
 11. VCF SDDC Manager and vCenter Services Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services2-min.png)
-    
+
 12. VCF Snapshot Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots1-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots2-min.png)
 
 13. VCF Storage Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage1-min.png)
 
 14. VCF vSAN Health
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN-min.png)
 ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN2-min.png)
 
-
 ## Known Issues
-### 1. [Remove FQDN suffix dependency in the name when configuring an NSX-T cloud account in vRealize Operations](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues/35)
 
-Please make sure that your NSX-T account name is configured as mentioned in this issue. 
+1. [Remove FQDN suffix dependency in the name when configuring an NSX-T cloud account in vRealize Operations](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues/35)
+
+    Please make sure that your NSX-T account name is configured as mentioned in this issue.
+
+2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.4.x. The filters on the vRealize Operations dashboards depend on the name.
 
-### 2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.4.x. The filters on the vReaize Operations dashboards depend on the name.
+    To set the Product Name for the vCenter Server, follow the below steps:
 
-To set the Product Name for the vCenter Server, follow the below steps - 
-1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn>/ui` as `administrator@vsphere.local`.
-2. In the `VMs and templates` inventory, expand the `management domain vCenter Server` tree and expand the management domain data center.
-3. Select the first `management domain vCenter Server virtual machine` and select `Configure` tab.
-4. In the `Settings` pane select `vApp Options`.
-5. Click the `Edit` button. The `Edit vApp Options` dialog box opens.
-6. If vApp options are disabled, select the `Enable vApp options` check box and click `OK`.
-7. Click the `Details` tab and enter `VMware vCenter Server Appliance` as product name in the `Name` field.
+    1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn>/ui` as `administrator@vsphere.local`.
+    2. In the `VMs and templates` inventory, expand the `management domain vCenter Server` tree and expand the management domain data center.
+    3. Select the first `management domain vCenter Server virtual machine` and select `Configure` tab.
+    4. In the `Settings` pane select `vApp Options`.
+    5. Click the `Edit` button. The `Edit vApp Options` dialog box opens.
+    6. If vApp options are disabled, select the `Enable vApp options` check box and click `OK`.
+    7. Click the `Details` tab and enter `VMware vCenter Server Appliance` as product name in the `Name` field.
 
-### 3. Shades of red, green, and yellow may vary on vRealize Operations widgets.
-Shades of red, green, and yellow may be different in different widgets but they represent the same thing. Ignore the shades as this is a vRealize Operations product limitation.
+3. Shades of red, green, and yellow may vary on vRealize Operations widgets
 
+    Shades of red, green, and yellow may be different in different widgets but they represent the same thing. Ignore the shades as this is a vRealize Operations product limitation.
 
 ## Support
 
-This Python module is not supported by VMware Support.
+This Python module is not supported by VMware Support Services.
 
 We welcome you to use the [GitHub Issues](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues) to report bugs or suggest enhancements.
 
 In order to have a good experience with our community, we recommend that you read the [contributing guidelines](../CONTRIBUTING.md).
 
 When filing an issue, please check existing open, or recently closed, issues to make sure someone else hasn't already
 reported the issue.
@@ -177,9 +178,7 @@
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt` & `vmware-cloud-foundation-health-monitoring-1.2.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

