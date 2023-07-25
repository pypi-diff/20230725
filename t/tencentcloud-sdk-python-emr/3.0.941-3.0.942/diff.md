# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.941.tar", last modified: Mon Jul 24 00:36:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.942.tar", last modified: Tue Jul 25 04:17:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.941.tar` & `tencentcloud-sdk-python-emr-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud/emr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30148 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)    14329 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   455464 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud/emr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/tencentcloud_sdk_python_emr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:36:45.000000 tencentcloud-sdk-python-emr-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud/emr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30148 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)    14440 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   455449 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud/emr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:17:50.000000 tencentcloud-sdk-python-emr-3.0.942/README.rst
```

### Comparing `tencentcloud-sdk-python-emr-3.0.941/setup.py` & `tencentcloud-sdk-python-emr-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.941/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.942/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.941/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.942/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,17 @@
 
 # 展示策略错误。
 INVALIDPARAMETER_DISPLAYSTRATEGYNOTMATCH = 'InvalidParameter.DisplayStrategyNotMatch'
 
 # 参数错误。
 INVALIDPARAMETER_HALESSMASTERCOUNT = 'InvalidParameter.HALessMasterCount'
 
+# impala查询参数异常。
+INVALIDPARAMETER_IMPALAQUERYEXCEPTION = 'InvalidParameter.ImpalaQueryException'
+
 # Common节点数量无效。
 INVALIDPARAMETER_INCORRECTCOMMONCOUNT = 'InvalidParameter.IncorrectCommonCount'
 
 # Master节点数量无效。
 INVALIDPARAMETER_INCORRECTMASTERCOUNT = 'InvalidParameter.IncorrectMasterCount'
 
 # 不合法的AllNodeResourceSpec参数。
```

### Comparing `tencentcloud-sdk-python-emr-3.0.941/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-emr-3.0.942/tencentcloud/emr/v20190103/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3468,15 +3468,15 @@
 
     def __init__(self):
         r"""
         :param _InstanceId: 集群ID
         :type InstanceId: str
         :param _StartTime: 起始时间秒
         :type StartTime: int
-        :param _EndTime: 结束时间秒，EndTime-StartTime不得超过31天秒数31*24*3600
+        :param _EndTime: 结束时间秒，EndTime-StartTime不得超过1天秒数86400
         :type EndTime: int
         :param _Offset: 分页起始偏移，从0开始
         :type Offset: int
         :param _Limit: 分页大小，合法范围[1,100]
         :type Limit: int
         """
         self._InstanceId = None
@@ -3603,15 +3603,15 @@
 
     def __init__(self):
         r"""
         :param _InstanceId: 集群ID
         :type InstanceId: str
         :param _StartTime: 起始时间秒
         :type StartTime: int
-        :param _EndTime: 结束时间秒，EndTime-StartTime不得超过31天秒数31243600
+        :param _EndTime: 结束时间秒，EndTime-StartTime不得超过1天秒数86400
         :type EndTime: int
         :param _Offset: 分页起始偏移，从0开始
         :type Offset: int
         :param _Limit: 分页大小，合法范围[1,100]
         :type Limit: int
         """
         self._InstanceId = None
@@ -4512,15 +4512,15 @@
 
     def __init__(self):
         r"""
         :param _InstanceId: 集群ID
         :type InstanceId: str
         :param _StartTime: 起始时间秒
         :type StartTime: int
-        :param _EndTime: 结束时间秒，EndTime-StartTime不得超过31天秒数31243600
+        :param _EndTime: 结束时间秒，EndTime-StartTime不得超过1天秒数86400
         :type EndTime: int
         :param _Offset: 分页起始偏移，从0开始
         :type Offset: int
         :param _Limit: 分页大小，合法范围[1,100]
         :type Limit: int
         """
         self._InstanceId = None
@@ -6306,15 +6306,15 @@
 class InquirePriceRenewEmrRequest(AbstractModel):
     """InquirePriceRenewEmr请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TimeSpan: 实例续费的时长。需要结合TimeUnit一起使用。1表示续费1一个月
+        :param _TimeSpan: 实例续费的时长。需要结合TimeUnit一起使用。1表示续费一个月
         :type TimeSpan: int
         :param _InstanceId: 待续费集群ID列表。
         :type InstanceId: str
         :param _Placement: 实例所在的位置。通过该参数可以指定实例所属可用区，所属项目等属性。
         :type Placement: :class:`tencentcloud.emr.v20190103.models.Placement`
         :param _PayMode: 实例计费模式。此处只支持取值为1，表示包年包月。
         :type PayMode: int
```

### Comparing `tencentcloud-sdk-python-emr-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-emr-3.0.941/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.942/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.942/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.941/README.rst` & `tencentcloud-sdk-python-emr-3.0.942/README.rst`

 * *Files identical despite different names*

