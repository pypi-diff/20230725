# Comparing `tmp/aliyun-python-sdk-ehpc-1.8.0.tar.gz` & `tmp/aliyun-python-sdk-ehpc-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-ehpc-1.8.0.tar", last modified: Thu Sep 27 07:13:33 2018, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-ehpc-1.9.0.tar", last modified: Wed Nov 14 10:25:24 2018, max compression
```

## Comparing `aliyun-python-sdk-ehpc-1.8.0.tar` & `aliyun-python-sdk-ehpc-1.9.0.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-09-27 07:13:33.000000 aliyun-python-sdk-ehpc-1.8.0/
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-09-27 07:13:33.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/
--rw-r--r--   0 jenkins    (504) jenkins    (503)       21 2018-09-27 07:07:04.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/__init__.py
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-09-27 07:13:33.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/
--rw-r--r--   0 jenkins    (504) jenkins    (503)        0 2018-09-27 07:03:19.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/__init__.py
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-09-27 07:13:33.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2155 2018-09-27 07:03:08.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListInvocationResultsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1147 2018-09-27 07:03:18.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteJobTemplatesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1279 2018-09-27 07:03:05.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/AddLocalNodesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1301 2018-09-27 07:03:11.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListClustersRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1651 2018-09-27 07:03:06.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/PullImageRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1511 2018-09-27 07:03:14.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/SetJobUserRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1539 2018-09-27 07:03:12.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListPreferredEcsTypesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1473 2018-09-27 07:03:19.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListClusterLogsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1779 2018-09-27 07:03:04.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/RunCloudMetricProfilingRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1147 2018-09-27 07:03:12.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/GetAutoScaleConfigRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1299 2018-09-27 07:03:07.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteContainerAppsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1345 2018-09-27 07:03:15.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListCustomImagesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1327 2018-09-27 07:03:17.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/UpgradeClientRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1917 2018-09-27 07:03:04.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribeImagePriceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)        0 2018-09-27 07:03:19.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/__init__.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1163 2018-09-27 07:03:05.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribeImageGatewayConfigRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1149 2018-09-27 07:03:15.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListSoftwaresRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1131 2018-09-27 07:03:03.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListQueuesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)      965 2018-09-27 07:03:14.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListImagesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1671 2018-09-27 07:03:06.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListContainerImagesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4394 2018-09-27 07:03:13.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/SetAutoScaleConfigRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1619 2018-09-27 07:03:13.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteNodesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1445 2018-09-27 07:03:15.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListJobTemplatesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3030 2018-09-27 07:03:05.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ModifyImageGatewayConfigRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)      993 2018-09-27 07:03:16.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListCurrentClientVersionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1357 2018-09-27 07:03:06.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ModifyContainerAppAttributesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1549 2018-09-27 07:03:10.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/StopNodesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1299 2018-09-27 07:03:17.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListVolumesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1311 2018-09-27 07:03:06.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListContainerAppsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2788 2018-09-27 07:03:03.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribePriceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1909 2018-09-27 07:03:11.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListJobsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1157 2018-09-27 07:03:09.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribeAutoScaleConfigRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1811 2018-09-27 07:03:08.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/AddContainerAppRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     9218 2018-09-27 07:03:18.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/CreateClusterRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1526 2018-09-27 07:03:12.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ModifyUserGroupsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1317 2018-09-27 07:03:08.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListInvocationStatusRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1339 2018-09-27 07:03:18.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteClusterRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1133 2018-09-27 07:03:09.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/StopClusterRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1391 2018-09-27 07:03:14.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteUsersRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1267 2018-09-27 07:03:13.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteJobsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1139 2018-09-27 07:03:10.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/RecoverClusterRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1461 2018-09-27 07:03:17.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListUsersRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1625 2018-09-27 07:03:11.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListNodesNoPagingRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3311 2018-09-27 07:03:12.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/AddNodesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1541 2018-09-27 07:03:11.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ModifyUserPasswordsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1655 2018-09-27 07:03:04.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteImageRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1415 2018-09-27 07:03:14.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ResetNodesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1291 2018-09-27 07:03:07.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/GetHybridClusterConfigRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2921 2018-09-27 07:03:13.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/EditJobTemplateRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2753 2018-09-27 07:03:17.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/CreateJobTemplateRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1163 2018-09-27 07:03:07.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribeContainerAppRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1335 2018-09-27 07:03:04.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/GetCloudMetricProfilingRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1493 2018-09-27 07:03:04.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListCloudMetricProfilingsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1911 2018-09-27 07:03:09.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/InvokeShellCommandRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1757 2018-09-27 07:03:16.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListNodesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1659 2018-09-27 07:03:05.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribeImageRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1471 2018-09-27 07:03:17.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ModifyClusterAttributesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1141 2018-09-27 07:03:16.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribeClusterRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1265 2018-09-27 07:03:18.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/RerunJobsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1633 2018-09-27 07:03:08.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListCommandsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2527 2018-09-27 07:03:05.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/GetCloudMetricLogsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1135 2018-09-27 07:03:10.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/StartClusterRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3977 2018-09-27 07:03:16.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/SubmitJobRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1644 2018-09-27 07:03:15.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/AddUsersRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)      967 2018-09-27 07:03:11.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListRegionsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1263 2018-09-27 07:03:10.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/StopJobsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1551 2018-09-27 07:03:09.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/StartNodesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     6024 2018-09-27 07:03:07.000000 aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/CreateHybridClusterRequest.py
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-09-27 07:13:33.000000 aliyun-python-sdk-ehpc-1.8.0/aliyun_python_sdk_ehpc.egg-info/
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4264 2018-09-27 07:13:33.000000 aliyun-python-sdk-ehpc-1.8.0/aliyun_python_sdk_ehpc.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (504) jenkins    (503)       14 2018-09-27 07:13:33.000000 aliyun-python-sdk-ehpc-1.8.0/aliyun_python_sdk_ehpc.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (504) jenkins    (503)        1 2018-09-27 07:13:33.000000 aliyun-python-sdk-ehpc-1.8.0/aliyun_python_sdk_ehpc.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1326 2018-09-27 07:13:33.000000 aliyun-python-sdk-ehpc-1.8.0/aliyun_python_sdk_ehpc.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (504) jenkins    (503)       30 2018-09-27 07:13:33.000000 aliyun-python-sdk-ehpc-1.8.0/aliyun_python_sdk_ehpc.egg-info/requires.txt
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1326 2018-09-27 07:13:33.000000 aliyun-python-sdk-ehpc-1.8.0/PKG-INFO
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2591 2018-09-27 07:03:52.000000 aliyun-python-sdk-ehpc-1.8.0/setup.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)       38 2018-09-27 07:13:33.000000 aliyun-python-sdk-ehpc-1.8.0/setup.cfg
--rw-r--r--   0 jenkins    (504) jenkins    (503)        0 2018-09-27 07:03:19.000000 aliyun-python-sdk-ehpc-1.8.0/MANIFEST.in
--rw-r--r--   0 jenkins    (504) jenkins    (503)      353 2018-09-27 07:03:36.000000 aliyun-python-sdk-ehpc-1.8.0/README.rst
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-11-14 10:25:24.000000 aliyun-python-sdk-ehpc-1.9.0/
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-11-14 10:25:24.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/
+-rw-r--r--   0 jenkins    (504) jenkins    (503)       21 2018-11-14 10:17:40.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/__init__.py
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-11-14 10:25:24.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/
+-rw-r--r--   0 jenkins    (504) jenkins    (503)        0 2018-11-14 10:13:59.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/__init__.py
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-11-14 10:25:24.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2155 2018-11-14 10:13:48.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListInvocationResultsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1147 2018-11-14 10:13:58.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteJobTemplatesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1279 2018-11-14 10:13:44.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/AddLocalNodesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1301 2018-11-14 10:13:50.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListClustersRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1651 2018-11-14 10:13:45.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/PullImageRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1511 2018-11-14 10:13:53.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/SetJobUserRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1539 2018-11-14 10:13:52.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListPreferredEcsTypesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1473 2018-11-14 10:13:58.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListClusterLogsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1779 2018-11-14 10:13:43.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/RunCloudMetricProfilingRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1147 2018-11-14 10:13:51.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/GetAutoScaleConfigRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1299 2018-11-14 10:13:47.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteContainerAppsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1539 2018-11-14 10:13:42.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListAvailableEcsTypesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1345 2018-11-14 10:13:54.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListCustomImagesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1327 2018-11-14 10:13:57.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/UpgradeClientRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1917 2018-11-14 10:13:43.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribeImagePriceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)        0 2018-11-14 10:13:59.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/__init__.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1163 2018-11-14 10:13:45.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribeImageGatewayConfigRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1149 2018-11-14 10:13:55.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListSoftwaresRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1131 2018-11-14 10:13:42.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListQueuesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)      965 2018-11-14 10:13:53.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListImagesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1671 2018-11-14 10:13:45.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListContainerImagesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4716 2018-11-14 10:13:52.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/SetAutoScaleConfigRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1619 2018-11-14 10:13:53.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteNodesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1445 2018-11-14 10:13:55.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListJobTemplatesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3030 2018-11-14 10:13:44.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ModifyImageGatewayConfigRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)      993 2018-11-14 10:13:55.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListCurrentClientVersionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1357 2018-11-14 10:13:46.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ModifyContainerAppAttributesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1549 2018-11-14 10:13:49.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/StopNodesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1299 2018-11-14 10:13:56.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListVolumesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1311 2018-11-14 10:13:46.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListContainerAppsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2788 2018-11-14 10:13:43.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribePriceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1909 2018-11-14 10:13:51.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListJobsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1157 2018-11-14 10:13:48.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribeAutoScaleConfigRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1811 2018-11-14 10:13:47.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/AddContainerAppRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     9218 2018-11-14 10:13:58.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/CreateClusterRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1526 2018-11-14 10:13:51.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ModifyUserGroupsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1317 2018-11-14 10:13:48.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListInvocationStatusRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1339 2018-11-14 10:13:57.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteClusterRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1133 2018-11-14 10:13:49.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/StopClusterRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1391 2018-11-14 10:13:53.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteUsersRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1267 2018-11-14 10:13:53.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteJobsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1337 2018-11-14 10:13:42.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListFileSystemWithMountTargetsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1139 2018-11-14 10:13:50.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/RecoverClusterRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1461 2018-11-14 10:13:57.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListUsersRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1625 2018-11-14 10:13:50.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListNodesNoPagingRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3483 2018-11-14 10:13:52.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/AddNodesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1541 2018-11-14 10:13:51.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ModifyUserPasswordsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1655 2018-11-14 10:13:44.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteImageRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1415 2018-11-14 10:13:54.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ResetNodesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1291 2018-11-14 10:13:46.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/GetHybridClusterConfigRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2921 2018-11-14 10:13:52.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/EditJobTemplateRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2753 2018-11-14 10:13:56.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/CreateJobTemplateRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1163 2018-11-14 10:13:46.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribeContainerAppRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1335 2018-11-14 10:13:43.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/GetCloudMetricProfilingRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1493 2018-11-14 10:13:43.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListCloudMetricProfilingsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1911 2018-11-14 10:13:48.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/InvokeShellCommandRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1757 2018-11-14 10:13:56.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListNodesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1659 2018-11-14 10:13:44.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribeImageRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1471 2018-11-14 10:13:57.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ModifyClusterAttributesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1141 2018-11-14 10:13:56.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribeClusterRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1265 2018-11-14 10:13:58.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/RerunJobsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1633 2018-11-14 10:13:47.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListCommandsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2527 2018-11-14 10:13:45.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/GetCloudMetricLogsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1135 2018-11-14 10:13:49.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/StartClusterRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3977 2018-11-14 10:13:55.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/SubmitJobRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1644 2018-11-14 10:13:54.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/AddUsersRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)      967 2018-11-14 10:13:50.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListRegionsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1263 2018-11-14 10:13:50.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/StopJobsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1551 2018-11-14 10:13:49.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/StartNodesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     6704 2018-11-14 10:13:47.000000 aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/CreateHybridClusterRequest.py
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-11-14 10:25:24.000000 aliyun-python-sdk-ehpc-1.9.0/aliyun_python_sdk_ehpc.egg-info/
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4401 2018-11-14 10:25:24.000000 aliyun-python-sdk-ehpc-1.9.0/aliyun_python_sdk_ehpc.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (504) jenkins    (503)       14 2018-11-14 10:25:24.000000 aliyun-python-sdk-ehpc-1.9.0/aliyun_python_sdk_ehpc.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (504) jenkins    (503)        1 2018-11-14 10:25:24.000000 aliyun-python-sdk-ehpc-1.9.0/aliyun_python_sdk_ehpc.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1326 2018-11-14 10:25:24.000000 aliyun-python-sdk-ehpc-1.9.0/aliyun_python_sdk_ehpc.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (504) jenkins    (503)       30 2018-11-14 10:25:24.000000 aliyun-python-sdk-ehpc-1.9.0/aliyun_python_sdk_ehpc.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1326 2018-11-14 10:25:24.000000 aliyun-python-sdk-ehpc-1.9.0/PKG-INFO
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2591 2018-11-14 10:14:34.000000 aliyun-python-sdk-ehpc-1.9.0/setup.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)       38 2018-11-14 10:25:24.000000 aliyun-python-sdk-ehpc-1.9.0/setup.cfg
+-rw-r--r--   0 jenkins    (504) jenkins    (503)        0 2018-11-14 10:13:59.000000 aliyun-python-sdk-ehpc-1.9.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (504) jenkins    (503)      353 2018-11-14 10:14:16.000000 aliyun-python-sdk-ehpc-1.9.0/README.rst
```

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListInvocationResultsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListInvocationResultsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteJobTemplatesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteJobTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/AddLocalNodesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/AddLocalNodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListClustersRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/PullImageRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/PullImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/SetJobUserRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/SetJobUserRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListPreferredEcsTypesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListPreferredEcsTypesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListClusterLogsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListClusterLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/RunCloudMetricProfilingRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/RunCloudMetricProfilingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/GetAutoScaleConfigRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/GetAutoScaleConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteContainerAppsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteContainerAppsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListCustomImagesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListCustomImagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/UpgradeClientRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/UpgradeClientRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribeImagePriceRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribeImagePriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribeImageGatewayConfigRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribeImageGatewayConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListSoftwaresRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListSoftwaresRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListQueuesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListQueuesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListImagesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListImagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListContainerImagesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListContainerImagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/SetAutoScaleConfigRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/SetAutoScaleConfigRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,16 +90,20 @@
 		for i in range(len(Queuess)):	
 			if Queuess[i].get('SpotStrategy') is not None:
 				self.add_query_param('Queues.' + str(i + 1) + '.SpotStrategy' , Queuess[i].get('SpotStrategy'))
 			if Queuess[i].get('QueueName') is not None:
 				self.add_query_param('Queues.' + str(i + 1) + '.QueueName' , Queuess[i].get('QueueName'))
 			if Queuess[i].get('InstanceType') is not None:
 				self.add_query_param('Queues.' + str(i + 1) + '.InstanceType' , Queuess[i].get('InstanceType'))
+			if Queuess[i].get('EnableAutoGrow') is not None:
+				self.add_query_param('Queues.' + str(i + 1) + '.EnableAutoGrow' , Queuess[i].get('EnableAutoGrow'))
 			if Queuess[i].get('SpotPriceLimit') is not None:
 				self.add_query_param('Queues.' + str(i + 1) + '.SpotPriceLimit' , Queuess[i].get('SpotPriceLimit'))
+			if Queuess[i].get('EnableAutoShrink') is not None:
+				self.add_query_param('Queues.' + str(i + 1) + '.EnableAutoShrink' , Queuess[i].get('EnableAutoShrink'))
 
 
 	def get_ExtraNodesGrowRatio(self):
 		return self.get_query_params().get('ExtraNodesGrowRatio')
 
 	def set_ExtraNodesGrowRatio(self,ExtraNodesGrowRatio):
 		self.add_query_param('ExtraNodesGrowRatio',ExtraNodesGrowRatio)
```

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteNodesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteNodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListJobTemplatesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListJobTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ModifyImageGatewayConfigRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ModifyImageGatewayConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListCurrentClientVersionRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListCurrentClientVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ModifyContainerAppAttributesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ModifyContainerAppAttributesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/StopNodesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/StopNodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListVolumesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListVolumesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListContainerAppsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListContainerAppsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribePriceRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribePriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListJobsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribeAutoScaleConfigRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribeAutoScaleConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/AddContainerAppRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/AddContainerAppRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/CreateClusterRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/CreateClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ModifyUserGroupsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ModifyUserGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListInvocationStatusRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListInvocationStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteClusterRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/StopClusterRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/StopClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteUsersRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteUsersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteJobsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/RecoverClusterRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/RecoverClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListUsersRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListUsersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListNodesNoPagingRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListNodesNoPagingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/AddNodesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/AddNodesRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,14 +85,20 @@
 
 	def get_EcsChargeType(self):
 		return self.get_query_params().get('EcsChargeType')
 
 	def set_EcsChargeType(self,EcsChargeType):
 		self.add_query_param('EcsChargeType',EcsChargeType)
 
+	def get_CreateMode(self):
+		return self.get_query_params().get('CreateMode')
+
+	def set_CreateMode(self,CreateMode):
+		self.add_query_param('CreateMode',CreateMode)
+
 	def get_InstanceType(self):
 		return self.get_query_params().get('InstanceType')
 
 	def set_InstanceType(self,InstanceType):
 		self.add_query_param('InstanceType',InstanceType)
 
 	def get_ComputeSpotPriceLimit(self):
```

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ModifyUserPasswordsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ModifyUserPasswordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DeleteImageRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DeleteImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ResetNodesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ResetNodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/GetHybridClusterConfigRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/GetHybridClusterConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/EditJobTemplateRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/EditJobTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/CreateJobTemplateRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/CreateJobTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribeContainerAppRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribeContainerAppRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/GetCloudMetricProfilingRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/GetCloudMetricProfilingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListCloudMetricProfilingsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListCloudMetricProfilingsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/InvokeShellCommandRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/InvokeShellCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListNodesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListNodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribeImageRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribeImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ModifyClusterAttributesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ModifyClusterAttributesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/DescribeClusterRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/DescribeClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/RerunJobsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/RerunJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListCommandsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListCommandsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/GetCloudMetricLogsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/GetCloudMetricLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/StartClusterRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/StartClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/SubmitJobRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/SubmitJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/AddUsersRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/AddUsersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/ListRegionsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/ListRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/StopJobsRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/StopJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/StartNodesRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/StartNodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyunsdkehpc/request/v20180412/CreateHybridClusterRequest.py` & `aliyun-python-sdk-ehpc-1.9.0/aliyunsdkehpc/request/v20180412/CreateHybridClusterRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,20 @@
 
 	def get_OnPremiseVolumeRemotePath(self):
 		return self.get_query_params().get('OnPremiseVolumeRemotePath')
 
 	def set_OnPremiseVolumeRemotePath(self,OnPremiseVolumeRemotePath):
 		self.add_query_param('OnPremiseVolumeRemotePath',OnPremiseVolumeRemotePath)
 
+	def get_JobQueue(self):
+		return self.get_query_params().get('JobQueue')
+
+	def set_JobQueue(self,JobQueue):
+		self.add_query_param('JobQueue',JobQueue)
+
 	def get_VolumeType(self):
 		return self.get_query_params().get('VolumeType')
 
 	def set_VolumeType(self,VolumeType):
 		self.add_query_param('VolumeType',VolumeType)
 
 	def get_Password(self):
@@ -115,14 +121,25 @@
 
 	def get_RemoteDirectory(self):
 		return self.get_query_params().get('RemoteDirectory')
 
 	def set_RemoteDirectory(self,RemoteDirectory):
 		self.add_query_param('RemoteDirectory',RemoteDirectory)
 
+	def get_PostInstallScripts(self):
+		return self.get_query_params().get('PostInstallScripts')
+
+	def set_PostInstallScripts(self,PostInstallScripts):
+		for i in range(len(PostInstallScripts)):	
+			if PostInstallScripts[i].get('Args') is not None:
+				self.add_query_param('PostInstallScript.' + str(i + 1) + '.Args' , PostInstallScripts[i].get('Args'))
+			if PostInstallScripts[i].get('Url') is not None:
+				self.add_query_param('PostInstallScript.' + str(i + 1) + '.Url' , PostInstallScripts[i].get('Url'))
+
+
 	def get_VSwitchId(self):
 		return self.get_query_params().get('VSwitchId')
 
 	def set_VSwitchId(self,VSwitchId):
 		self.add_query_param('VSwitchId',VSwitchId)
 
 	def get_Nodes(self):
```

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyun_python_sdk_ehpc.egg-info/SOURCES.txt` & `aliyun-python-sdk-ehpc-1.9.0/aliyun_python_sdk_ehpc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,22 +31,24 @@
 aliyunsdkehpc/request/v20180412/DescribePriceRequest.py
 aliyunsdkehpc/request/v20180412/EditJobTemplateRequest.py
 aliyunsdkehpc/request/v20180412/GetAutoScaleConfigRequest.py
 aliyunsdkehpc/request/v20180412/GetCloudMetricLogsRequest.py
 aliyunsdkehpc/request/v20180412/GetCloudMetricProfilingRequest.py
 aliyunsdkehpc/request/v20180412/GetHybridClusterConfigRequest.py
 aliyunsdkehpc/request/v20180412/InvokeShellCommandRequest.py
+aliyunsdkehpc/request/v20180412/ListAvailableEcsTypesRequest.py
 aliyunsdkehpc/request/v20180412/ListCloudMetricProfilingsRequest.py
 aliyunsdkehpc/request/v20180412/ListClusterLogsRequest.py
 aliyunsdkehpc/request/v20180412/ListClustersRequest.py
 aliyunsdkehpc/request/v20180412/ListCommandsRequest.py
 aliyunsdkehpc/request/v20180412/ListContainerAppsRequest.py
 aliyunsdkehpc/request/v20180412/ListContainerImagesRequest.py
 aliyunsdkehpc/request/v20180412/ListCurrentClientVersionRequest.py
 aliyunsdkehpc/request/v20180412/ListCustomImagesRequest.py
+aliyunsdkehpc/request/v20180412/ListFileSystemWithMountTargetsRequest.py
 aliyunsdkehpc/request/v20180412/ListImagesRequest.py
 aliyunsdkehpc/request/v20180412/ListInvocationResultsRequest.py
 aliyunsdkehpc/request/v20180412/ListInvocationStatusRequest.py
 aliyunsdkehpc/request/v20180412/ListJobTemplatesRequest.py
 aliyunsdkehpc/request/v20180412/ListJobsRequest.py
 aliyunsdkehpc/request/v20180412/ListNodesNoPagingRequest.py
 aliyunsdkehpc/request/v20180412/ListNodesRequest.py
```

### Comparing `aliyun-python-sdk-ehpc-1.8.0/aliyun_python_sdk_ehpc.egg-info/PKG-INFO` & `aliyun-python-sdk-ehpc-1.9.0/aliyun_python_sdk_ehpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ehpc
-Version: 1.8.0
+Version: 1.9.0
 Summary: The ehpc module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: aliyun-python-sdk-ehpc
         This is the ehpc module of Aliyun Python SDK.
```

### Comparing `aliyun-python-sdk-ehpc-1.8.0/PKG-INFO` & `aliyun-python-sdk-ehpc-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ehpc
-Version: 1.8.0
+Version: 1.9.0
 Summary: The ehpc module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: aliyun-python-sdk-ehpc
         This is the ehpc module of Aliyun Python SDK.
```

### Comparing `aliyun-python-sdk-ehpc-1.8.0/setup.py` & `aliyun-python-sdk-ehpc-1.9.0/setup.py`

 * *Files identical despite different names*

