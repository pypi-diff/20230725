# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.941.tar", last modified: Mon Jul 24 00:36:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.942.tar", last modified: Tue Jul 25 04:18:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.941.tar` & `tencentcloud-sdk-python-ess-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    62111 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   437808 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    62111 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   438303 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.941/setup.py` & `tencentcloud-sdk-python-ess-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,20 +189,20 @@
         :param _CustomApproverTag: 客户自定义签署人标识，64位长度，保证唯一，非企微场景不使用此字段
         :type CustomApproverTag: str
         :param _ApproverOption: 签署人个性化能力值
         :type ApproverOption: :class:`tencentcloud.ess.v20201111.models.ApproverOption`
         :param _ApproverVerifyTypes: 签署人查看合同时认证方式, 
 1-实名查看 2-短信验证码查看(企业签署方不支持该方式)
 如果不传默认为1
-模板发起的时候,认证方式以模版配置为主
+模板发起的时候,认证方式以模板配置为主
         :type ApproverVerifyTypes: list of int
         :param _ApproverSignTypes: 签署人签署合同时的认证方式
 1-人脸认证 2-签署密码 3-运营商三要素(默认为1,2)
 合同签署认证方式的优先级 verifyChannel>approverSignTypes
-模板发起的时候,认证方式以模版配置为主
+模板发起的时候,认证方式以模板配置为主
         :type ApproverSignTypes: list of int
         :param _ApproverNeedSignReview: 当前签署方进行签署操作是否需要企业内部审批，true 则为需要。为个人签署方时则由发起方企业审核。	
         :type ApproverNeedSignReview: bool
         """
         self._ApproverType = None
         self._ApproverName = None
         self._ApproverMobile = None
@@ -11279,18 +11279,21 @@
         r"""
         :param _Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _OperateType: 操作类型：1-新增，2-删除
         :type OperateType: int
         :param _CallbackInfo: 回调信息
         :type CallbackInfo: :class:`tencentcloud.ess.v20201111.models.CallbackInfo`
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._OperateType = None
         self._CallbackInfo = None
+        self._Agent = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
@@ -11308,23 +11311,34 @@
     def CallbackInfo(self):
         return self._CallbackInfo
 
     @CallbackInfo.setter
     def CallbackInfo(self, CallbackInfo):
         self._CallbackInfo = CallbackInfo
 
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._OperateType = params.get("OperateType")
         if params.get("CallbackInfo") is not None:
             self._CallbackInfo = CallbackInfo()
             self._CallbackInfo._deserialize(params.get("CallbackInfo"))
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.941/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.942/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.942/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.941/README.rst` & `tencentcloud-sdk-python-ess-3.0.942/README.rst`

 * *Files identical despite different names*

