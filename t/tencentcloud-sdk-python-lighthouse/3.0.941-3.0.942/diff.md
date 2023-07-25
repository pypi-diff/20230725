# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.941.tar", last modified: Mon Jul 24 00:39:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.942.tar", last modified: Tue Jul 25 04:20:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.941.tar` & `tencentcloud-sdk-python-lighthouse-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92864 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)    26127 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   360767 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:47.000000 tencentcloud-sdk-python-lighthouse-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-25 04:20:46.000000 tencentcloud-sdk-python-lighthouse-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:47.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:20:46.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:47.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:20:46.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:47.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:20:46.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104972 2023-07-25 04:20:46.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)    27298 2023-07-25 04:20:46.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   404234 2023-07-25 04:20:46.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/lighthouse/v20200324/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:20:47.000000 tencentcloud-sdk-python-lighthouse-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-25 04:20:47.000000 tencentcloud-sdk-python-lighthouse-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-25 04:20:46.000000 tencentcloud-sdk-python-lighthouse-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:47.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:20:47.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-25 04:20:47.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-25 04:20:47.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:20:47.000000 tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.941/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -748,14 +748,106 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeDockerActivities(self, request):
+        """查询实例内的Docker活动列表。
+
+        :param request: Request instance for DescribeDockerActivities.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDockerActivitiesRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDockerActivitiesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDockerActivities", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDockerActivitiesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeDockerContainerConfiguration(self, request):
+        """查询实例内的Docker容器配置信息
+
+        :param request: Request instance for DescribeDockerContainerConfiguration.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDockerContainerConfigurationRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDockerContainerConfigurationResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDockerContainerConfiguration", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDockerContainerConfigurationResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeDockerContainerDetail(self, request):
+        """查询实例内的Docker容器详情
+
+        :param request: Request instance for DescribeDockerContainerDetail.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDockerContainerDetailRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDockerContainerDetailResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDockerContainerDetail", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDockerContainerDetailResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeDockerContainers(self, request):
+        """查询实例内的容器列表。
+
+        :param request: Request instance for DescribeDockerContainers.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDockerContainersRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDockerContainersResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDockerContainers", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDockerContainersResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeFirewallRules(self, request):
         """本接口（DescribeFirewallRules）用于查询实例的防火墙规则。
 
         :param request: Request instance for DescribeFirewallRules.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeFirewallRulesRequest`
         :rtype: :class:`tencentcloud.lighthouse.v20200324.models.DescribeFirewallRulesResponse`
 
@@ -1539,14 +1631,38 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def ModifyDockerContainer(self, request):
+        """修改实例内的Docker容器，之后可以通过返回的ActivityId调用DescribeDockerActivities接口查询重建情况。
+        请注意：本接口会重新创建并运行实例内的Docker容器。
+
+        :param request: Request instance for ModifyDockerContainer.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.ModifyDockerContainerRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.ModifyDockerContainerResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyDockerContainer", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyDockerContainerResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def ModifyFirewallRuleDescription(self, request):
         """本接口（ModifyFirewallRuleDescription）用于修改单条防火墙规则描述。
 
         * FirewallVersion 用于指定要操作的防火墙的版本。传入 FirewallVersion 版本号若不等于当前防火墙的最新版本，将返回失败；若不传 FirewallVersion 则直接修改防火墙规则备注。
 
         在 FirewallRule 参数中：
         * Protocol 字段支持输入 TCP，UDP，ICMP，ALL。
@@ -1758,14 +1874,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def RemoveDockerContainers(self, request):
+        """删除实例内的Docker容器，之后可以通过返回的ActivityId调用DescribeDockerActivities接口查询删除情况。
+
+        :param request: Request instance for RemoveDockerContainers.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.RemoveDockerContainersRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.RemoveDockerContainersResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RemoveDockerContainers", params, headers=headers)
+            response = json.loads(body)
+            model = models.RemoveDockerContainersResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def RenameDockerContainer(self, request):
+        """重命名实例内的Docker容器，之后可以通过返回的ActivityId调用DescribeDockerActivities接口查询重命名情况。
+
+        :param request: Request instance for RenameDockerContainer.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.RenameDockerContainerRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.RenameDockerContainerResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RenameDockerContainer", params, headers=headers)
+            response = json.loads(body)
+            model = models.RenameDockerContainerResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def RenewDisks(self, request):
         """本接口(RenewDisks)用于续费一个或多个轻量应用服务器云硬盘。
 
         只有状态为 ATTACHED，UNATTACHED 或 SHUTDOWN 的数据盘才可以进行此操作。
         支持批量操作。每次请求批量云硬盘的上限为 50。
         本接口为异步接口，请求发送成功后会返回一个 RequestId，此时操作并未立即完成。云硬盘操作结果可以通过调用 [DescribeDisks](https://cloud.tencent.com/document/product/1207/66093) 接口查询，如果云硬盘的最新操作状态（LatestOperationState）为“SUCCESS”，则代表操作成功。
 
@@ -1811,14 +1973,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def RerunDockerContainer(self, request):
+        """重新创建并运行实例内的Docker容器，之后可以通过返回的ActivityId调用DescribeDockerActivities接口查询重建情况。
+
+        :param request: Request instance for RerunDockerContainer.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.RerunDockerContainerRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.RerunDockerContainerResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RerunDockerContainer", params, headers=headers)
+            response = json.loads(body)
+            model = models.RerunDockerContainerResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def ResetAttachCcn(self, request):
         """本接口 (ResetAttachCcn) 用于关联云联网实例申请过期时，重新申请关联操作。
 
         :param request: Request instance for ResetAttachCcn.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.ResetAttachCcnRequest`
         :rtype: :class:`tencentcloud.lighthouse.v20200324.models.ResetAttachCcnResponse`
 
@@ -1890,14 +2075,83 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def RestartDockerContainers(self, request):
+        """重启实例内的Docker容器，之后可以通过返回的ActivityId调用DescribeDockerActivities接口查询重启情况。
+
+        :param request: Request instance for RestartDockerContainers.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.RestartDockerContainersRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.RestartDockerContainersResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RestartDockerContainers", params, headers=headers)
+            response = json.loads(body)
+            model = models.RestartDockerContainersResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def RunDockerContainers(self, request):
+        """创建并运行多个Docker容器，之后可以通过返回的ActivityIds调用DescribeDockerActivities接口查询创建情况。
+
+        :param request: Request instance for RunDockerContainers.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.RunDockerContainersRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.RunDockerContainersResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RunDockerContainers", params, headers=headers)
+            response = json.loads(body)
+            model = models.RunDockerContainersResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def StartDockerContainers(self, request):
+        """启动实例内的Docker容器，之后可以通过返回的ActivityId调用DescribeDockerActivities接口查询启动情况。
+
+        :param request: Request instance for StartDockerContainers.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.StartDockerContainersRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.StartDockerContainersResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StartDockerContainers", params, headers=headers)
+            response = json.loads(body)
+            model = models.StartDockerContainersResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def StartInstances(self, request):
         """本接口（StartInstances）用于启动一个或多个实例。
 
         * 只有状态为 STOPPED 的实例才可以进行此操作。
         * 接口调用成功时，实例会进入 STARTING 状态；启动实例成功时，实例会进入 RUNNING 状态。
         * 支持批量操作。每次请求批量实例的上限为 100。
         * 本接口为异步接口，请求发送成功后会返回一个 RequestId，此时操作并未立即完成。实例操作结果可以通过调用 DescribeInstances 接口查询，如果实例的最新操作状态（LatestOperationState）为“SUCCESS”，则代表操作成功。
@@ -1916,14 +2170,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def StopDockerContainers(self, request):
+        """停止实例内的Docker容器，之后可以通过返回的ActivityId调用DescribeDockerActivities接口查询停止情况。
+
+        :param request: Request instance for StopDockerContainers.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.StopDockerContainersRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.StopDockerContainersResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StopDockerContainers", params, headers=headers)
+            response = json.loads(body)
+            model = models.StopDockerContainersResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopInstances(self, request):
         """本接口（StopInstances）用于关闭一个或多个实例。
         * 只有状态为 RUNNING 的实例才可以进行此操作。
         * 接口调用成功时，实例会进入 STOPPING 状态；关闭实例成功时，实例会进入 STOPPED 状态。
         * 支持批量操作。每次请求批量实例的上限为 100。
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,20 @@
 
 # 查询资源返回了不符合要求内容。
 FAILEDOPERATION_DESCRIBERESOURCESRETURNABLEERROR = 'FailedOperation.DescribeResourcesReturnableError'
 
 # 销毁资源失败，请稍后重新操作。
 FAILEDOPERATION_DESTROYRESOURCESFAILED = 'FailedOperation.DestroyResourcesFailed'
 
+# 容器列表过长。
+FAILEDOPERATION_DOCKERCONTAINERSLISTTOOLARGE = 'FailedOperation.DockerContainersListTooLarge'
+
+# 指定Docker环境操作失败, 请检查Docker环境。
+FAILEDOPERATION_DOCKEROPERATIONFAILED = 'FailedOperation.DockerOperationFailed'
+
 # 对防火墙规则的操作失败。
 FAILEDOPERATION_FIREWALLRULESOPERATIONFAILED = 'FailedOperation.FirewallRulesOperationFailed'
 
 # 对密钥对的导入操作失败。
 FAILEDOPERATION_IMPORTKEYPAIRFAILED = 'FailedOperation.ImportKeyPairFailed'
 
 # 对实例的操作失败。
@@ -85,14 +91,17 @@
 
 # 请求错误。
 FAILEDOPERATION_REQUESTERROR = 'FailedOperation.RequestError'
 
 # 快照操作失败。
 FAILEDOPERATION_SNAPSHOTOPERATIONFAILED = 'FailedOperation.SnapshotOperationFailed'
 
+# TAT命令未完成。
+FAILEDOPERATION_TATINVOCATIONNOTFINISHED = 'FailedOperation.TATInvocationNotFinished'
+
 # 调用计费网关服务失败，请稍后重新操作。
 FAILEDOPERATION_TRADECALLBILLINGGATEWAYFAILED = 'FailedOperation.TradeCallBillingGatewayFailed'
 
 # 计费询价失败。
 FAILEDOPERATION_TRADEGETPRICEFAILED = 'FailedOperation.TradeGetPriceFailed'
 
 # 操作失败，不能创建自定义镜像。
@@ -235,14 +244,17 @@
 
 # 参数 `KeyName` 已经存在且重复。
 INVALIDPARAMETERVALUE_DUPLICATEPARAMETERVALUE = 'InvalidParameterValue.DuplicateParameterValue'
 
 # 参数值非法，不允许包含重复的值。
 INVALIDPARAMETERVALUE_DUPLICATED = 'InvalidParameterValue.Duplicated'
 
+# 列值不正确。
+INVALIDPARAMETERVALUE_FIELDSCOMPARE = 'InvalidParameterValue.FieldsCompare'
+
 # 防火墙规则描述长度超出限制。
 INVALIDPARAMETERVALUE_FIREWALLRULEDESCRIPTIONTOOLONG = 'InvalidParameterValue.FirewallRuleDescriptionTooLong'
 
 # 参数值非法，实例 ID 格式非法。
 INVALIDPARAMETERVALUE_INSTANCEIDMALFORMED = 'InvalidParameterValue.InstanceIdMalformed'
 
 # 参数值非法，实例名称超过允许的最大长度。
@@ -346,14 +358,17 @@
 
 # 参数值非法，快照 ID 格式非法。
 INVALIDPARAMETERVALUE_SNAPSHOTIDMALFORMED = 'InvalidParameterValue.SnapshotIdMalformed'
 
 # 参数值非法，快照名称超过允许的最大长度。
 INVALIDPARAMETERVALUE_SNAPSHOTNAMETOOLONG = 'InvalidParameterValue.SnapshotNameTooLong'
 
+# 参数值非法，大于有效值。
+INVALIDPARAMETERVALUE_TOOLARGE = 'InvalidParameterValue.TooLarge'
+
 # 参数取值过长，超过最大长度。
 INVALIDPARAMETERVALUE_TOOLONG = 'InvalidParameterValue.TooLong'
 
 # 非法的可用区。
 INVALIDPARAMETERVALUE_ZONEINVALID = 'InvalidParameterValue.ZoneInvalid'
 
 # 超过配额限制。
@@ -493,26 +508,44 @@
 
 # 快照不存在。
 RESOURCENOTFOUND_SNAPSHOTNOTFOUND = 'ResourceNotFound.SnapshotNotFound'
 
 # 资源不可用。
 RESOURCEUNAVAILABLE = 'ResourceUnavailable'
 
+# 指定实例镜像不符合要求。
+RESOURCEUNAVAILABLE_BLUEPRINTINVALID = 'ResourceUnavailable.BlueprintInvalid'
+
 # 镜像资源不可用。
 RESOURCEUNAVAILABLE_BLUEPRINTUNAVAILABLE = 'ResourceUnavailable.BlueprintUnavailable'
 
 # 套餐不可用。
 RESOURCEUNAVAILABLE_BUNDLEUNAVAILABLE = 'ResourceUnavailable.BundleUnavailable'
 
+# Docker资源不可用。
+RESOURCEUNAVAILABLE_DOCKERUNAVAILABLE = 'ResourceUnavailable.DockerUnavailable'
+
+# TAT agent不可用。
+RESOURCEUNAVAILABLE_TATAGENTUNAVAILABLE = 'ResourceUnavailable.TATAgentUnavailable'
+
+# TAT 服务错误。
+RESOURCEUNAVAILABLE_TATSERVICEERROR = 'ResourceUnavailable.TATServiceError'
+
 # 套餐无可用配置。
 RESOURCESSOLDOUT_PURCHASESOURCEHASNOBUNDLECONFIGS = 'ResourcesSoldOut.PurchaseSourceHasNoBundleConfigs'
 
 # 套餐无可用配置。
 RESOURCESSOLDOUT_ZONESHASNOBUNDLECONFIGS = 'ResourcesSoldOut.ZonesHasNoBundleConfigs'
 
+# 未授权操作。
+UNAUTHORIZEDOPERATION = 'UnauthorizedOperation'
+
+# 无效 Token。
+UNAUTHORIZEDOPERATION_INVALIDTOKEN = 'UnauthorizedOperation.InvalidToken'
+
 # MFA 已过期。
 UNAUTHORIZEDOPERATION_MFAEXPIRED = 'UnauthorizedOperation.MFAExpired'
 
 # MFA 不存在。
 UNAUTHORIZEDOPERATION_MFANOTFOUND = 'UnauthorizedOperation.MFANotFound'
 
 # 无权限。
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud/lighthouse/v20200324/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3936,14 +3936,474 @@
                 obj = DiskReturnable()
                 obj._deserialize(item)
                 self._DiskReturnableSet.append(obj)
         self._TotalCount = params.get("TotalCount")
         self._RequestId = params.get("RequestId")
 
 
+class DescribeDockerActivitiesRequest(AbstractModel):
+    """DescribeDockerActivities请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _ActivityIds: Docker活动ID列表。
+        :type ActivityIds: list of str
+        :param _Offset: 偏移量，默认为 0。
+        :type Offset: int
+        :param _Limit: 返回数量，默认为 20，最大值为 100。
+        :type Limit: int
+        :param _CreatedTimeBegin: 活动创建时间的起始值，时间戳秒数。
+        :type CreatedTimeBegin: int
+        :param _CreatedTimeEnd: 活动创建时间的结束值，时间戳秒数。
+        :type CreatedTimeEnd: int
+        """
+        self._InstanceId = None
+        self._ActivityIds = None
+        self._Offset = None
+        self._Limit = None
+        self._CreatedTimeBegin = None
+        self._CreatedTimeEnd = None
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
+    def ActivityIds(self):
+        return self._ActivityIds
+
+    @ActivityIds.setter
+    def ActivityIds(self, ActivityIds):
+        self._ActivityIds = ActivityIds
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+    @property
+    def CreatedTimeBegin(self):
+        return self._CreatedTimeBegin
+
+    @CreatedTimeBegin.setter
+    def CreatedTimeBegin(self, CreatedTimeBegin):
+        self._CreatedTimeBegin = CreatedTimeBegin
+
+    @property
+    def CreatedTimeEnd(self):
+        return self._CreatedTimeEnd
+
+    @CreatedTimeEnd.setter
+    def CreatedTimeEnd(self, CreatedTimeEnd):
+        self._CreatedTimeEnd = CreatedTimeEnd
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._ActivityIds = params.get("ActivityIds")
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
+        self._CreatedTimeBegin = params.get("CreatedTimeBegin")
+        self._CreatedTimeEnd = params.get("CreatedTimeEnd")
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
+class DescribeDockerActivitiesResponse(AbstractModel):
+    """DescribeDockerActivities返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 总数量。
+        :type TotalCount: int
+        :param _DockerActivitySet: Docker活动列表。
+        :type DockerActivitySet: list of DockerActivity
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TotalCount = None
+        self._DockerActivitySet = None
+        self._RequestId = None
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+    @property
+    def DockerActivitySet(self):
+        return self._DockerActivitySet
+
+    @DockerActivitySet.setter
+    def DockerActivitySet(self, DockerActivitySet):
+        self._DockerActivitySet = DockerActivitySet
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
+        self._TotalCount = params.get("TotalCount")
+        if params.get("DockerActivitySet") is not None:
+            self._DockerActivitySet = []
+            for item in params.get("DockerActivitySet"):
+                obj = DockerActivity()
+                obj._deserialize(item)
+                self._DockerActivitySet.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeDockerContainerConfigurationRequest(AbstractModel):
+    """DescribeDockerContainerConfiguration请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _ContainerId: 容器ID。
+        :type ContainerId: str
+        """
+        self._InstanceId = None
+        self._ContainerId = None
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
+    def ContainerId(self):
+        return self._ContainerId
+
+    @ContainerId.setter
+    def ContainerId(self, ContainerId):
+        self._ContainerId = ContainerId
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._ContainerId = params.get("ContainerId")
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
+class DescribeDockerContainerConfigurationResponse(AbstractModel):
+    """DescribeDockerContainerConfiguration返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ContainerConfiguration: Docker容器配置信息。
+        :type ContainerConfiguration: :class:`tencentcloud.lighthouse.v20200324.models.DockerContainerConfiguration`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._ContainerConfiguration = None
+        self._RequestId = None
+
+    @property
+    def ContainerConfiguration(self):
+        return self._ContainerConfiguration
+
+    @ContainerConfiguration.setter
+    def ContainerConfiguration(self, ContainerConfiguration):
+        self._ContainerConfiguration = ContainerConfiguration
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
+        if params.get("ContainerConfiguration") is not None:
+            self._ContainerConfiguration = DockerContainerConfiguration()
+            self._ContainerConfiguration._deserialize(params.get("ContainerConfiguration"))
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeDockerContainerDetailRequest(AbstractModel):
+    """DescribeDockerContainerDetail请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _ContainerId: 容器ID。
+        :type ContainerId: str
+        """
+        self._InstanceId = None
+        self._ContainerId = None
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
+    def ContainerId(self):
+        return self._ContainerId
+
+    @ContainerId.setter
+    def ContainerId(self, ContainerId):
+        self._ContainerId = ContainerId
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._ContainerId = params.get("ContainerId")
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
+class DescribeDockerContainerDetailResponse(AbstractModel):
+    """DescribeDockerContainerDetail返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ContainerDetail: Docker容器详情，json字符串base64编码。
+        :type ContainerDetail: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._ContainerDetail = None
+        self._RequestId = None
+
+    @property
+    def ContainerDetail(self):
+        return self._ContainerDetail
+
+    @ContainerDetail.setter
+    def ContainerDetail(self, ContainerDetail):
+        self._ContainerDetail = ContainerDetail
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
+        self._ContainerDetail = params.get("ContainerDetail")
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeDockerContainersRequest(AbstractModel):
+    """DescribeDockerContainers请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _ContainerIds: 容器ID列表。
+        :type ContainerIds: list of str
+        :param _Limit: 返回数量，默认为 20，最大值为 100。
+        :type Limit: int
+        :param _Offset: 偏移量，默认为 0。
+        :type Offset: int
+        :param _Filters: 过滤器列表。
+<li>container-id</li>按照【容器ID】进行过滤。
+类型：String
+必选：否
+<li>container-name</li>按照【容器名称】进行过滤。
+类型：String
+必选：否
+每次请求的 Filters 的上限为 10，Filter.Values 的上限为 5。参数不支持同时指定 ContainerIds 和 Filters。
+        :type Filters: list of Filter
+        """
+        self._InstanceId = None
+        self._ContainerIds = None
+        self._Limit = None
+        self._Offset = None
+        self._Filters = None
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
+    def ContainerIds(self):
+        return self._ContainerIds
+
+    @ContainerIds.setter
+    def ContainerIds(self, ContainerIds):
+        self._ContainerIds = ContainerIds
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Filters(self):
+        return self._Filters
+
+    @Filters.setter
+    def Filters(self, Filters):
+        self._Filters = Filters
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._ContainerIds = params.get("ContainerIds")
+        self._Limit = params.get("Limit")
+        self._Offset = params.get("Offset")
+        if params.get("Filters") is not None:
+            self._Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self._Filters.append(obj)
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
+class DescribeDockerContainersResponse(AbstractModel):
+    """DescribeDockerContainers返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 总数量。
+        :type TotalCount: int
+        :param _DockerContainerSet: 容器列表。
+        :type DockerContainerSet: list of DockerContainer
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TotalCount = None
+        self._DockerContainerSet = None
+        self._RequestId = None
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+    @property
+    def DockerContainerSet(self):
+        return self._DockerContainerSet
+
+    @DockerContainerSet.setter
+    def DockerContainerSet(self, DockerContainerSet):
+        self._DockerContainerSet = DockerContainerSet
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
+        self._TotalCount = params.get("TotalCount")
+        if params.get("DockerContainerSet") is not None:
+            self._DockerContainerSet = []
+            for item in params.get("DockerContainerSet"):
+                obj = DockerContainer()
+                obj._deserialize(item)
+                self._DockerContainerSet.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeFirewallRulesRequest(AbstractModel):
     """DescribeFirewallRules请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7014,14 +7474,263 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DockerActivity(AbstractModel):
+    """Docker活动信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ActivityId: 活动ID。
+        :type ActivityId: str
+        :param _ActivityName: 活动名称。
+        :type ActivityName: str
+        :param _ActivityState: 活动状态。取值范围： 
+<li>INIT：表示初始化，活动尚未执行</li>
+<li>OPERATING：表示活动执行中</li>
+<li>SUCCESS：表示活动执行成功</li>
+<li>FAILED：表示活动执行失败</li>
+        :type ActivityState: str
+        :param _ActivityCommandOutput: 活动执行的命令输出，以base64编码。
+        :type ActivityCommandOutput: str
+        :param _ContainerIds: 容器ID列表。
+        :type ContainerIds: list of str
+        :param _CreatedTime: 创建时间。按照 ISO8601 标准表示，并且使用 UTC 时间。
+        :type CreatedTime: str
+        :param _EndTime: 结束时间。按照 ISO8601 标准表示，并且使用 UTC 时间。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EndTime: str
+        """
+        self._ActivityId = None
+        self._ActivityName = None
+        self._ActivityState = None
+        self._ActivityCommandOutput = None
+        self._ContainerIds = None
+        self._CreatedTime = None
+        self._EndTime = None
+
+    @property
+    def ActivityId(self):
+        return self._ActivityId
+
+    @ActivityId.setter
+    def ActivityId(self, ActivityId):
+        self._ActivityId = ActivityId
+
+    @property
+    def ActivityName(self):
+        return self._ActivityName
+
+    @ActivityName.setter
+    def ActivityName(self, ActivityName):
+        self._ActivityName = ActivityName
+
+    @property
+    def ActivityState(self):
+        return self._ActivityState
+
+    @ActivityState.setter
+    def ActivityState(self, ActivityState):
+        self._ActivityState = ActivityState
+
+    @property
+    def ActivityCommandOutput(self):
+        return self._ActivityCommandOutput
+
+    @ActivityCommandOutput.setter
+    def ActivityCommandOutput(self, ActivityCommandOutput):
+        self._ActivityCommandOutput = ActivityCommandOutput
+
+    @property
+    def ContainerIds(self):
+        return self._ContainerIds
+
+    @ContainerIds.setter
+    def ContainerIds(self, ContainerIds):
+        self._ContainerIds = ContainerIds
+
+    @property
+    def CreatedTime(self):
+        return self._CreatedTime
+
+    @CreatedTime.setter
+    def CreatedTime(self, CreatedTime):
+        self._CreatedTime = CreatedTime
+
+    @property
+    def EndTime(self):
+        return self._EndTime
+
+    @EndTime.setter
+    def EndTime(self, EndTime):
+        self._EndTime = EndTime
+
+
+    def _deserialize(self, params):
+        self._ActivityId = params.get("ActivityId")
+        self._ActivityName = params.get("ActivityName")
+        self._ActivityState = params.get("ActivityState")
+        self._ActivityCommandOutput = params.get("ActivityCommandOutput")
+        self._ContainerIds = params.get("ContainerIds")
+        self._CreatedTime = params.get("CreatedTime")
+        self._EndTime = params.get("EndTime")
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
+class DockerContainer(AbstractModel):
+    """Docker容器信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ContainerId: 容器ID
+        :type ContainerId: str
+        :param _ContainerName: 容器名称
+        :type ContainerName: str
+        :param _ContainerImage: 容器镜像地址
+        :type ContainerImage: str
+        :param _Command: 容器Command
+        :type Command: str
+        :param _Status: 容器状态描述
+        :type Status: str
+        :param _State: 容器状态，和docker的容器状态保持一致，当前取值有：created, restarting, running, removing, paused, exited, or dead
+        :type State: str
+        :param _PublishPortSet: 容器端口主机端口映射列表
+        :type PublishPortSet: list of DockerContainerPublishPort
+        :param _VolumeSet: 容器挂载本地卷列表
+        :type VolumeSet: list of DockerContainerVolume
+        :param _CreatedTime: 创建时间。按照 ISO8601 标准表示，并且使用 UTC 时间。
+        :type CreatedTime: str
+        """
+        self._ContainerId = None
+        self._ContainerName = None
+        self._ContainerImage = None
+        self._Command = None
+        self._Status = None
+        self._State = None
+        self._PublishPortSet = None
+        self._VolumeSet = None
+        self._CreatedTime = None
+
+    @property
+    def ContainerId(self):
+        return self._ContainerId
+
+    @ContainerId.setter
+    def ContainerId(self, ContainerId):
+        self._ContainerId = ContainerId
+
+    @property
+    def ContainerName(self):
+        return self._ContainerName
+
+    @ContainerName.setter
+    def ContainerName(self, ContainerName):
+        self._ContainerName = ContainerName
+
+    @property
+    def ContainerImage(self):
+        return self._ContainerImage
+
+    @ContainerImage.setter
+    def ContainerImage(self, ContainerImage):
+        self._ContainerImage = ContainerImage
+
+    @property
+    def Command(self):
+        return self._Command
+
+    @Command.setter
+    def Command(self, Command):
+        self._Command = Command
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def State(self):
+        return self._State
+
+    @State.setter
+    def State(self, State):
+        self._State = State
+
+    @property
+    def PublishPortSet(self):
+        return self._PublishPortSet
+
+    @PublishPortSet.setter
+    def PublishPortSet(self, PublishPortSet):
+        self._PublishPortSet = PublishPortSet
+
+    @property
+    def VolumeSet(self):
+        return self._VolumeSet
+
+    @VolumeSet.setter
+    def VolumeSet(self, VolumeSet):
+        self._VolumeSet = VolumeSet
+
+    @property
+    def CreatedTime(self):
+        return self._CreatedTime
+
+    @CreatedTime.setter
+    def CreatedTime(self, CreatedTime):
+        self._CreatedTime = CreatedTime
+
+
+    def _deserialize(self, params):
+        self._ContainerId = params.get("ContainerId")
+        self._ContainerName = params.get("ContainerName")
+        self._ContainerImage = params.get("ContainerImage")
+        self._Command = params.get("Command")
+        self._Status = params.get("Status")
+        self._State = params.get("State")
+        if params.get("PublishPortSet") is not None:
+            self._PublishPortSet = []
+            for item in params.get("PublishPortSet"):
+                obj = DockerContainerPublishPort()
+                obj._deserialize(item)
+                self._PublishPortSet.append(obj)
+        if params.get("VolumeSet") is not None:
+            self._VolumeSet = []
+            for item in params.get("VolumeSet"):
+                obj = DockerContainerVolume()
+                obj._deserialize(item)
+                self._VolumeSet.append(obj)
+        self._CreatedTime = params.get("CreatedTime")
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
 class DockerContainerConfiguration(AbstractModel):
     """Docker容器创建时的配置
 
     """
 
     def __init__(self):
         r"""
@@ -9207,17 +9916,20 @@
         :param _AutoGeneratePassword: <li>"YES"代表选择自动生成密码，这时不指定Password字段。</li>
 <li>"NO"代表选择自定义密码，这时要指定Password字段。</li>
         :type AutoGeneratePassword: str
         :param _Password: 实例登录密码。具体按照操作系统的复杂度要求。 
 `LINUX_UNIX` 实例密码必须 8-30 位，推荐使用 12 位以上密码，不能包含空格, 不能以“/”开头，至少包含以下字符中的三种不同字符，字符种类：<br><li>小写字母：[a-z]<br><li>大写字母：[A-Z]<br><li>数字：0-9<br><li>特殊字符： ()\`\~!@#$%^&\*-+=\_|{}[]:;' <>,.?/</li>
 `WINDOWS` 实例密码必须 12-30 位，不能包含空格, 不能以“/”开头且不包括用户名，至少包含以下字符中的三种不同字符<br><li>小写字母：[a-z]<br><li>大写字母：[A-Z]<br><li>数字： 0-9<br><li>特殊字符：()\`~!@#$%^&\*-+=\_|{}[]:;' <>,.?/
         :type Password: str
+        :param _KeyIds: 密钥ID列表，最多同时指定5个密钥。关联密钥后，就可以通过对应的私钥来访问实例。密钥与密码不能同时指定，同时WINDOWS操作系统不支持指定密钥。密钥ID列表可以通过[DescribeKeyPairs](https://cloud.tencent.com/document/product/1207/55540)接口获取。
+        :type KeyIds: list of str
         """
         self._AutoGeneratePassword = None
         self._Password = None
+        self._KeyIds = None
 
     @property
     def AutoGeneratePassword(self):
         return self._AutoGeneratePassword
 
     @AutoGeneratePassword.setter
     def AutoGeneratePassword(self, AutoGeneratePassword):
@@ -9227,18 +9939,27 @@
     def Password(self):
         return self._Password
 
     @Password.setter
     def Password(self, Password):
         self._Password = Password
 
+    @property
+    def KeyIds(self):
+        return self._KeyIds
+
+    @KeyIds.setter
+    def KeyIds(self, KeyIds):
+        self._KeyIds = KeyIds
+
 
     def _deserialize(self, params):
         self._AutoGeneratePassword = params.get("AutoGeneratePassword")
         self._Password = params.get("Password")
+        self._KeyIds = params.get("KeyIds")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -9643,14 +10364,177 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class ModifyDockerContainerRequest(AbstractModel):
+    """ModifyDockerContainer请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _ContainerId: 容器ID。
+        :type ContainerId: str
+        :param _Envs: 环境变量列表
+        :type Envs: list of ContainerEnv
+        :param _PublishPorts: 容器端口主机端口映射列表
+        :type PublishPorts: list of DockerContainerPublishPort
+        :param _Volumes: 容器加载本地卷列表
+        :type Volumes: list of DockerContainerVolume
+        :param _Command: 运行的命令
+        :type Command: str
+        :param _RestartPolicy: 容器重启策略，对应docker "--restart"参数。
+
+枚举值:
+no: 不自动重启。默认策略。
+on-failure[:max-retries]: 当容器退出码非0时重启容器。使用max-retries限制重启次数，比如on-failure:10，限制最多重启10次。
+always: 只要容器退出就重启。
+unless-stopped: 始终重新启动容器，包括在守护进程启动时，除非容器在 Docker 守护进程停止之前进入停止状态。
+        :type RestartPolicy: str
+        """
+        self._InstanceId = None
+        self._ContainerId = None
+        self._Envs = None
+        self._PublishPorts = None
+        self._Volumes = None
+        self._Command = None
+        self._RestartPolicy = None
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
+    def ContainerId(self):
+        return self._ContainerId
+
+    @ContainerId.setter
+    def ContainerId(self, ContainerId):
+        self._ContainerId = ContainerId
+
+    @property
+    def Envs(self):
+        return self._Envs
+
+    @Envs.setter
+    def Envs(self, Envs):
+        self._Envs = Envs
+
+    @property
+    def PublishPorts(self):
+        return self._PublishPorts
+
+    @PublishPorts.setter
+    def PublishPorts(self, PublishPorts):
+        self._PublishPorts = PublishPorts
+
+    @property
+    def Volumes(self):
+        return self._Volumes
+
+    @Volumes.setter
+    def Volumes(self, Volumes):
+        self._Volumes = Volumes
+
+    @property
+    def Command(self):
+        return self._Command
+
+    @Command.setter
+    def Command(self, Command):
+        self._Command = Command
+
+    @property
+    def RestartPolicy(self):
+        return self._RestartPolicy
+
+    @RestartPolicy.setter
+    def RestartPolicy(self, RestartPolicy):
+        self._RestartPolicy = RestartPolicy
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._ContainerId = params.get("ContainerId")
+        if params.get("Envs") is not None:
+            self._Envs = []
+            for item in params.get("Envs"):
+                obj = ContainerEnv()
+                obj._deserialize(item)
+                self._Envs.append(obj)
+        if params.get("PublishPorts") is not None:
+            self._PublishPorts = []
+            for item in params.get("PublishPorts"):
+                obj = DockerContainerPublishPort()
+                obj._deserialize(item)
+                self._PublishPorts.append(obj)
+        if params.get("Volumes") is not None:
+            self._Volumes = []
+            for item in params.get("Volumes"):
+                obj = DockerContainerVolume()
+                obj._deserialize(item)
+                self._Volumes.append(obj)
+        self._Command = params.get("Command")
+        self._RestartPolicy = params.get("RestartPolicy")
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
+class ModifyDockerContainerResponse(AbstractModel):
+    """ModifyDockerContainer返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DockerActivityId: Docker活动ID。
+        :type DockerActivityId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._DockerActivityId = None
+        self._RequestId = None
+
+    @property
+    def DockerActivityId(self):
+        return self._DockerActivityId
+
+    @DockerActivityId.setter
+    def DockerActivityId(self, DockerActivityId):
+        self._DockerActivityId = DockerActivityId
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
+        self._DockerActivityId = params.get("DockerActivityId")
+        self._RequestId = params.get("RequestId")
+
+
 class ModifyFirewallRuleDescriptionRequest(AbstractModel):
     """ModifyFirewallRuleDescription请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10425,14 +11309,190 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RemoveDockerContainersRequest(AbstractModel):
+    """RemoveDockerContainers请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _ContainerIds: 容器ID列表。
+        :type ContainerIds: list of str
+        """
+        self._InstanceId = None
+        self._ContainerIds = None
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
+    def ContainerIds(self):
+        return self._ContainerIds
+
+    @ContainerIds.setter
+    def ContainerIds(self, ContainerIds):
+        self._ContainerIds = ContainerIds
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._ContainerIds = params.get("ContainerIds")
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
+class RemoveDockerContainersResponse(AbstractModel):
+    """RemoveDockerContainers返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DockerActivityId: Docker活动ID。
+        :type DockerActivityId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._DockerActivityId = None
+        self._RequestId = None
+
+    @property
+    def DockerActivityId(self):
+        return self._DockerActivityId
+
+    @DockerActivityId.setter
+    def DockerActivityId(self, DockerActivityId):
+        self._DockerActivityId = DockerActivityId
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
+        self._DockerActivityId = params.get("DockerActivityId")
+        self._RequestId = params.get("RequestId")
+
+
+class RenameDockerContainerRequest(AbstractModel):
+    """RenameDockerContainer请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _ContainerId: 容器ID。
+        :type ContainerId: str
+        :param _ContainerName: 容器新的名称。
+        :type ContainerName: str
+        """
+        self._InstanceId = None
+        self._ContainerId = None
+        self._ContainerName = None
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
+    def ContainerId(self):
+        return self._ContainerId
+
+    @ContainerId.setter
+    def ContainerId(self, ContainerId):
+        self._ContainerId = ContainerId
+
+    @property
+    def ContainerName(self):
+        return self._ContainerName
+
+    @ContainerName.setter
+    def ContainerName(self, ContainerName):
+        self._ContainerName = ContainerName
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._ContainerId = params.get("ContainerId")
+        self._ContainerName = params.get("ContainerName")
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
+class RenameDockerContainerResponse(AbstractModel):
+    """RenameDockerContainer返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DockerActivityId: Docker活动ID。
+        :type DockerActivityId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._DockerActivityId = None
+        self._RequestId = None
+
+    @property
+    def DockerActivityId(self):
+        return self._DockerActivityId
+
+    @DockerActivityId.setter
+    def DockerActivityId(self, DockerActivityId):
+        self._DockerActivityId = DockerActivityId
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
+        self._DockerActivityId = params.get("DockerActivityId")
+        self._RequestId = params.get("RequestId")
+
+
 class RenewDiskChargePrepaid(AbstractModel):
     """续费云硬盘包年包月相关参数设置
 
     """
 
     def __init__(self):
         r"""
@@ -10684,14 +11744,110 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class RerunDockerContainerRequest(AbstractModel):
+    """RerunDockerContainer请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _ContainerConfiguration: 重新创建的容器配置。
+        :type ContainerConfiguration: :class:`tencentcloud.lighthouse.v20200324.models.DockerContainerConfiguration`
+        :param _ContainerId: 容器ID。
+        :type ContainerId: str
+        """
+        self._InstanceId = None
+        self._ContainerConfiguration = None
+        self._ContainerId = None
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
+    def ContainerConfiguration(self):
+        return self._ContainerConfiguration
+
+    @ContainerConfiguration.setter
+    def ContainerConfiguration(self, ContainerConfiguration):
+        self._ContainerConfiguration = ContainerConfiguration
+
+    @property
+    def ContainerId(self):
+        return self._ContainerId
+
+    @ContainerId.setter
+    def ContainerId(self, ContainerId):
+        self._ContainerId = ContainerId
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        if params.get("ContainerConfiguration") is not None:
+            self._ContainerConfiguration = DockerContainerConfiguration()
+            self._ContainerConfiguration._deserialize(params.get("ContainerConfiguration"))
+        self._ContainerId = params.get("ContainerId")
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
+class RerunDockerContainerResponse(AbstractModel):
+    """RerunDockerContainer返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DockerActivityId: Docker活动ID。
+        :type DockerActivityId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._DockerActivityId = None
+        self._RequestId = None
+
+    @property
+    def DockerActivityId(self):
+        return self._DockerActivityId
+
+    @DockerActivityId.setter
+    def DockerActivityId(self, DockerActivityId):
+        self._DockerActivityId = DockerActivityId
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
+        self._DockerActivityId = params.get("DockerActivityId")
+        self._RequestId = params.get("RequestId")
+
+
 class ResetAttachCcnRequest(AbstractModel):
     """ResetAttachCcn请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10955,14 +12111,183 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class RestartDockerContainersRequest(AbstractModel):
+    """RestartDockerContainers请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _ContainerIds: 容器ID列表。
+        :type ContainerIds: list of str
+        """
+        self._InstanceId = None
+        self._ContainerIds = None
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
+    def ContainerIds(self):
+        return self._ContainerIds
+
+    @ContainerIds.setter
+    def ContainerIds(self, ContainerIds):
+        self._ContainerIds = ContainerIds
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._ContainerIds = params.get("ContainerIds")
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
+class RestartDockerContainersResponse(AbstractModel):
+    """RestartDockerContainers返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DockerActivityId: Docker活动ID。
+        :type DockerActivityId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._DockerActivityId = None
+        self._RequestId = None
+
+    @property
+    def DockerActivityId(self):
+        return self._DockerActivityId
+
+    @DockerActivityId.setter
+    def DockerActivityId(self, DockerActivityId):
+        self._DockerActivityId = DockerActivityId
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
+        self._DockerActivityId = params.get("DockerActivityId")
+        self._RequestId = params.get("RequestId")
+
+
+class RunDockerContainersRequest(AbstractModel):
+    """RunDockerContainers请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _Containers: 要创建的容器列表。
+        :type Containers: list of DockerContainerConfiguration
+        """
+        self._InstanceId = None
+        self._Containers = None
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
+    def Containers(self):
+        return self._Containers
+
+    @Containers.setter
+    def Containers(self, Containers):
+        self._Containers = Containers
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        if params.get("Containers") is not None:
+            self._Containers = []
+            for item in params.get("Containers"):
+                obj = DockerContainerConfiguration()
+                obj._deserialize(item)
+                self._Containers.append(obj)
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
+class RunDockerContainersResponse(AbstractModel):
+    """RunDockerContainers返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DockerActivitySet: Docker活动ID列表。
+        :type DockerActivitySet: list of str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._DockerActivitySet = None
+        self._RequestId = None
+
+    @property
+    def DockerActivitySet(self):
+        return self._DockerActivitySet
+
+    @DockerActivitySet.setter
+    def DockerActivitySet(self, DockerActivitySet):
+        self._DockerActivitySet = DockerActivitySet
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
+        self._DockerActivitySet = params.get("DockerActivitySet")
+        self._RequestId = params.get("RequestId")
+
+
 class Scene(AbstractModel):
     """使用场景信息
 
     """
 
     def __init__(self):
         r"""
@@ -11427,14 +12752,96 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class StartDockerContainersRequest(AbstractModel):
+    """StartDockerContainers请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _ContainerIds: 容器ID列表。
+        :type ContainerIds: list of str
+        """
+        self._InstanceId = None
+        self._ContainerIds = None
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
+    def ContainerIds(self):
+        return self._ContainerIds
+
+    @ContainerIds.setter
+    def ContainerIds(self, ContainerIds):
+        self._ContainerIds = ContainerIds
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._ContainerIds = params.get("ContainerIds")
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
+class StartDockerContainersResponse(AbstractModel):
+    """StartDockerContainers返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DockerActivityId: Docker活动ID。
+        :type DockerActivityId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._DockerActivityId = None
+        self._RequestId = None
+
+    @property
+    def DockerActivityId(self):
+        return self._DockerActivityId
+
+    @DockerActivityId.setter
+    def DockerActivityId(self, DockerActivityId):
+        self._DockerActivityId = DockerActivityId
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
+        self._DockerActivityId = params.get("DockerActivityId")
+        self._RequestId = params.get("RequestId")
+
+
 class StartInstancesRequest(AbstractModel):
     """StartInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11485,14 +12892,96 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class StopDockerContainersRequest(AbstractModel):
+    """StopDockerContainers请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _ContainerIds: 容器ID列表。
+        :type ContainerIds: list of str
+        """
+        self._InstanceId = None
+        self._ContainerIds = None
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
+    def ContainerIds(self):
+        return self._ContainerIds
+
+    @ContainerIds.setter
+    def ContainerIds(self, ContainerIds):
+        self._ContainerIds = ContainerIds
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._ContainerIds = params.get("ContainerIds")
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
+class StopDockerContainersResponse(AbstractModel):
+    """StopDockerContainers返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DockerActivityId: Docker活动ID。
+        :type DockerActivityId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._DockerActivityId = None
+        self._RequestId = None
+
+    @property
+    def DockerActivityId(self):
+        return self._DockerActivityId
+
+    @DockerActivityId.setter
+    def DockerActivityId(self, DockerActivityId):
+        self._DockerActivityId = DockerActivityId
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
+        self._DockerActivityId = params.get("DockerActivityId")
+        self._RequestId = params.get("RequestId")
+
+
 class StopInstancesRequest(AbstractModel):
     """StopInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.942/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.941/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.942/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.942/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

