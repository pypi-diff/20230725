# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.941.tar", last modified: Mon Jul 24 00:47:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.942.tar", last modified: Tue Jul 25 04:29:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.941.tar` & `tencentcloud-sdk-python-vpc-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/vpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/vpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   333624 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42776 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1312271 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:47:56.000000 tencentcloud-sdk-python-vpc-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/vpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/vpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   333624 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43190 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1312271 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:29:43.000000 tencentcloud-sdk-python-vpc-3.0.942/README.rst
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.941/setup.py` & `tencentcloud-sdk-python-vpc-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -814,14 +814,17 @@
 
 # 资源被锁定。
 UNSUPPORTEDOPERATION_LOCKEDRESOURCES = 'UnsupportedOperation.LockedResources'
 
 # 账户不支持修改公网IP的该属性。
 UNSUPPORTEDOPERATION_MODIFYADDRESSATTRIBUTE = 'UnsupportedOperation.ModifyAddressAttribute'
 
+# VPC实例内部有帐号纬度的IPv6白名单，不支持关联多云联网。
+UNSUPPORTEDOPERATION_MULTIPLEVPCNOTSUPPORTATTACHACCOUNTHASIPV6 = 'UnsupportedOperation.MultipleVpcNotSupportAttachAccountHasIpv6'
+
 # 资源互斥操作任务正在执行。
 UNSUPPORTEDOPERATION_MUTEXOPERATIONTASKRUNNING = 'UnsupportedOperation.MutexOperationTaskRunning'
 
 # NAT网关的公网IP不存在。
 UNSUPPORTEDOPERATION_NATGATEWAYEIPNOTEXISTS = 'UnsupportedOperation.NatGatewayEipNotExists'
 
 # NAT网关存在未解绑的IP。
@@ -916,14 +919,17 @@
 
 # 未找到相关角色，请确认角色是否授权。
 UNSUPPORTEDOPERATION_ROLENOTFOUND = 'UnsupportedOperation.RoleNotFound'
 
 # 路由表绑定了子网。
 UNSUPPORTEDOPERATION_ROUTETABLEHASSUBNETRULE = 'UnsupportedOperation.RouteTableHasSubnetRule'
 
+# SSL客户端状态不可用，不支持下载
+UNSUPPORTEDOPERATION_SSLCLIENTCERTDISABLEUNSUPPORTEDDOWNLOADSSLCLIENTCERT = 'UnsupportedOperation.SSLClientCertDisableUnsupportedDownloadSSLClientCert'
+
 # 实例已关联快照策略。
 UNSUPPORTEDOPERATION_SNAPSHOTATTACHED = 'UnsupportedOperation.SnapshotAttached'
 
 # 快照备份策略不支持修改。
 UNSUPPORTEDOPERATION_SNAPSHOTBACKUPTYPEMODIFY = 'UnsupportedOperation.SnapshotBackupTypeModify'
 
 # 快照文件生成失败。
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/vpc/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.942/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.941'
+__version__ = '3.0.942'
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.942/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.941/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.942/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.941/README.rst` & `tencentcloud-sdk-python-vpc-3.0.942/README.rst`

 * *Files identical despite different names*

