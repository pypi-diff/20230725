# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.941.tar", last modified: Mon Jul 24 00:33:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.942.tar", last modified: Tue Jul 25 04:14:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.941.tar` & `tencentcloud-sdk-python-ckafka-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/ckafka/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/ckafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    71936 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)   768834 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-24 00:33:35.000000 tencentcloud-sdk-python-ckafka-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:19.000000 tencentcloud-sdk-python-ckafka-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-25 04:14:18.000000 tencentcloud-sdk-python-ckafka-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:19.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:14:19.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-25 04:14:19.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-25 04:14:19.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:14:19.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:19.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:14:18.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:19.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/ckafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:14:18.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/ckafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:19.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:14:18.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-07-25 04:14:18.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    72823 2023-07-25 04:14:18.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)   773069 2023-07-25 04:14:18.000000 tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:14:19.000000 tencentcloud-sdk-python-ckafka-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-25 04:14:19.000000 tencentcloud-sdk-python-ckafka-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-25 04:14:18.000000 tencentcloud-sdk-python-ckafka-3.0.942/README.rst
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.941/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1587,14 +1587,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def InstanceScalingDown(self, request):
+        """按量实例缩容
+
+        :param request: Request instance for InstanceScalingDown.
+        :type request: :class:`tencentcloud.ckafka.v20190819.models.InstanceScalingDownRequest`
+        :rtype: :class:`tencentcloud.ckafka.v20190819.models.InstanceScalingDownResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("InstanceScalingDown", params, headers=headers)
+            response = json.loads(body)
+            model = models.InstanceScalingDownResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def ModifyAclRule(self, request):
         """修改AC策略，目前只支持预设规则的是否应用到新增topic这一项的修改
 
         :param request: Request instance for ModifyAclRule.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.ModifyAclRuleRequest`
         :rtype: :class:`tencentcloud.ckafka.v20190819.models.ModifyAclRuleResponse`
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.941/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.942/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -17433,14 +17433,136 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class InstanceScalingDownRequest(AbstractModel):
+    """InstanceScalingDown请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例id
+        :type InstanceId: str
+        :param _UpgradeStrategy: 缩容模式  1:稳定变配 
+2.高速变配
+        :type UpgradeStrategy: int
+        :param _DiskSize: 磁盘大小 单位 GB
+        :type DiskSize: int
+        :param _BandWidth: 峰值带宽 单位 MB/s
+        :type BandWidth: int
+        :param _Partition: 分区上限
+        :type Partition: int
+        """
+        self._InstanceId = None
+        self._UpgradeStrategy = None
+        self._DiskSize = None
+        self._BandWidth = None
+        self._Partition = None
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+    @property
+    def UpgradeStrategy(self):
+        return self._UpgradeStrategy
+
+    @UpgradeStrategy.setter
+    def UpgradeStrategy(self, UpgradeStrategy):
+        self._UpgradeStrategy = UpgradeStrategy
+
+    @property
+    def DiskSize(self):
+        return self._DiskSize
+
+    @DiskSize.setter
+    def DiskSize(self, DiskSize):
+        self._DiskSize = DiskSize
+
+    @property
+    def BandWidth(self):
+        return self._BandWidth
+
+    @BandWidth.setter
+    def BandWidth(self, BandWidth):
+        self._BandWidth = BandWidth
+
+    @property
+    def Partition(self):
+        return self._Partition
+
+    @Partition.setter
+    def Partition(self, Partition):
+        self._Partition = Partition
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._UpgradeStrategy = params.get("UpgradeStrategy")
+        self._DiskSize = params.get("DiskSize")
+        self._BandWidth = params.get("BandWidth")
+        self._Partition = params.get("Partition")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class InstanceScalingDownResponse(AbstractModel):
+    """InstanceScalingDown返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Result: 缩容应答
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Result: :class:`tencentcloud.ckafka.v20190819.models.ScalingDownResp`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Result = None
+        self._RequestId = None
+
+    @property
+    def Result(self):
+        return self._Result
+
+    @Result.setter
+    def Result(self, Result):
+        self._Result = Result
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Result") is not None:
+            self._Result = ScalingDownResp()
+            self._Result._deserialize(params.get("Result"))
+        self._RequestId = params.get("RequestId")
+
+
 class JgwOperateResponse(AbstractModel):
     """操作型结果返回值
 
     """
 
     def __init__(self):
         r"""
@@ -22743,14 +22865,48 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ScalingDownResp(AbstractModel):
+    """实例缩容应答
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DealNames: 订单号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DealNames: list of str
+        """
+        self._DealNames = None
+
+    @property
+    def DealNames(self):
+        return self._DealNames
+
+    @DealNames.setter
+    def DealNames(self, DealNames):
+        self._DealNames = DealNames
+
+
+    def _deserialize(self, params):
+        self._DealNames = params.get("DealNames")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ScfParam(AbstractModel):
     """Scf类型入参
 
     """
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.942/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.941/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.942/README.rst`

 * *Files identical despite different names*

