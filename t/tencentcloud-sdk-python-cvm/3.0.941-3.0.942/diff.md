# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.941.tar", last modified: Mon Jul 24 00:34:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.942.tar", last modified: Tue Jul 25 04:15:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.941.tar` & `tencentcloud-sdk-python-cvm-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/cvm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/cvm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44021 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   119676 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)   624916 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:34:42.000000 tencentcloud-sdk-python-cvm-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/cvm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/cvm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44311 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   119676 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)   624916 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:15:40.000000 tencentcloud-sdk-python-cvm-3.0.942/README.rst
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.941/setup.py` & `tencentcloud-sdk-python-cvm-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.941/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.942/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -790,14 +790,17 @@
 
 # 异构机型不支持跨机型调整。
 UNSUPPORTEDOPERATION_HETEROGENEOUSCHANGEINSTANCEFAMILY = 'UnsupportedOperation.HeterogeneousChangeInstanceFamily'
 
 # 不支持未开启休眠功能的实例。
 UNSUPPORTEDOPERATION_HIBERNATIONFORNORMALINSTANCE = 'UnsupportedOperation.HibernationForNormalInstance'
 
+# 当前的镜像不支持休眠。
+UNSUPPORTEDOPERATION_HIBERNATIONOSVERSION = 'UnsupportedOperation.HibernationOsVersion'
+
 # IPv6实例不支持VPC迁移
 UNSUPPORTEDOPERATION_IPV6NOTSUPPORTVPCMIGRATE = 'UnsupportedOperation.IPv6NotSupportVpcMigrate'
 
 # 镜像大小超出限制，不支持导出。
 UNSUPPORTEDOPERATION_IMAGETOOLARGEEXPORTUNSUPPORTED = 'UnsupportedOperation.ImageTooLargeExportUnsupported'
 
 # 请求不支持该实例计费模式
@@ -994,14 +997,17 @@
 
 # 请求不支持该类型系统盘。
 UNSUPPORTEDOPERATION_SYSTEMDISKTYPE = 'UnsupportedOperation.SystemDiskType'
 
 # 该机型为包销机型，RenewFlag的值只允许设置为NOTIFY_AND_AUTO_RENEW。
 UNSUPPORTEDOPERATION_UNDERWRITINGINSTANCETYPEONLYSUPPORTAUTORENEW = 'UnsupportedOperation.UnderwritingInstanceTypeOnlySupportAutoRenew'
 
+# 当前实例不允许变配到非ARM机型。
+UNSUPPORTEDOPERATION_UNSUPPORTEDARMCHANGEINSTANCEFAMILY = 'UnsupportedOperation.UnsupportedARMChangeInstanceFamily'
+
 # 指定机型不支持跨机型调整配置。
 UNSUPPORTEDOPERATION_UNSUPPORTEDCHANGEINSTANCEFAMILY = 'UnsupportedOperation.UnsupportedChangeInstanceFamily'
 
 # 非ARM机型不支持调整到ARM机型。
 UNSUPPORTEDOPERATION_UNSUPPORTEDCHANGEINSTANCEFAMILYTOARM = 'UnsupportedOperation.UnsupportedChangeInstanceFamilyToARM'
 
 # 不支持实例变配到此类型机型。
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.941/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.942/tencentcloud/cvm/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.942/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.941/README.rst` & `tencentcloud-sdk-python-cvm-3.0.942/README.rst`

 * *Files identical despite different names*

