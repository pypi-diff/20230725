# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.941.tar", last modified: Mon Jul 24 00:45:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.942.tar", last modified: Tue Jul 25 04:27:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.941.tar` & `tencentcloud-sdk-python-teo-3.0.942.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:45:40.000000 tencentcloud-sdk-python-teo-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:45:39.000000 tencentcloud-sdk-python-teo-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:45:40.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:45:39.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:45:40.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:45:40.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:45:39.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60588 2023-07-24 00:45:39.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)    23798 2023-07-24 00:45:39.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   605317 2023-07-24 00:45:39.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:45:40.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:45:39.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5399 2023-07-24 00:45:39.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-07-24 00:45:39.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    38737 2023-07-24 00:45:39.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:45:39.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:45:40.000000 tencentcloud-sdk-python-teo-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:45:40.000000 tencentcloud-sdk-python-teo-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:45:39.000000 tencentcloud-sdk-python-teo-3.0.941/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:45:40.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:45:40.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-24 00:45:40.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:45:40.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:45:40.000000 tencentcloud-sdk-python-teo-3.0.941/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60588 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)    24008 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   605317 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5399 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    38737 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:27:07.000000 tencentcloud-sdk-python-teo-3.0.942/tencentcloud_sdk_python_teo.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-teo-3.0.941/setup.py` & `tencentcloud-sdk-python-teo-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 # 账户余额不足
 FAILEDOPERATION_INSUFFICIENTACCOUNTBALANCE = 'FailedOperation.InsufficientAccountBalance'
 
 # 站点状态不正确。
 FAILEDOPERATION_INVALIDZONESTATUS = 'FailedOperation.InvalidZoneStatus'
 
+# 操作失败。
+FAILEDOPERATION_MODIFYFAILED = 'FailedOperation.ModifyFailed'
+
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 后台处理出错。
 INTERNALERROR_BACKENDERROR = 'InternalError.BackendError'
 
 # 配置已被锁定，请解除配置锁定之后在重试。
@@ -349,14 +352,17 @@
 
 # 参数长度超过限制。
 INVALIDPARAMETER_LENGTHEXCEEDSLIMIT = 'InvalidParameter.LengthExceedsLimit'
 
 # 不支持智能路由
 INVALIDPARAMETER_MULTIPLYLAYERNOTSUPPORTSMARTROUTING = 'InvalidParameter.MultiplyLayerNotSupportSmartRouting'
 
+# 操作配置存在不支持的预设变量。
+INVALIDPARAMETER_NOTSUPPORTTHISPRESET = 'InvalidParameter.NotSupportThisPreset'
+
 # 源站是内网IP。
 INVALIDPARAMETER_ORIGINISINNERIP = 'InvalidParameter.OriginIsInnerIp'
 
 # 修改源站操作中源站组Id必填。
 INVALIDPARAMETER_ORIGINORIGINGROUPIDISREQUIRED = 'InvalidParameter.OriginOriginGroupIdIsRequired'
 
 # 参数错误: 无效 "结束时间", 不在允许的查询范围内: [开始时间, 开始+ 7天]
```

### Comparing `tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220901/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.941/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.942/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.942/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.941/README.rst` & `tencentcloud-sdk-python-teo-3.0.942/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.941/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.942/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.941/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.942/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

