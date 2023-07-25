# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.941.tar", last modified: Mon Jul 24 00:33:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.942.tar", last modified: Tue Jul 25 04:14:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.941.tar` & `tencentcloud-sdk-python-clb-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud/clb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud/clb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89989 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)   508288 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:33:40.000000 tencentcloud-sdk-python-clb-3.0.941/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud/clb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud/clb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89989 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)   508306 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:14:26.000000 tencentcloud-sdk-python-clb-3.0.942/tencentcloud_sdk_python_clb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-clb-3.0.941/setup.py` & `tencentcloud-sdk-python-clb-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.941/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.942/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.941/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.942/tencentcloud/clb/v20180317/clb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.941/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.942/tencentcloud/clb/v20180317/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -14309,15 +14309,15 @@
         :param _HealthCheck: 健康检查信息。详情请参见：[健康检查](https://cloud.tencent.com/document/product/214/6097)
         :type HealthCheck: :class:`tencentcloud.clb.v20180317.models.HealthCheck`
         :param _Certificate: 证书信息；此参数和MultiCertInfo不能同时传入。
         :type Certificate: :class:`tencentcloud.clb.v20180317.models.CertificateInput`
         :param _Scheduler: 规则的请求转发方式，可选值：WRR、LEAST_CONN、IP_HASH
 分别表示按权重轮询、最小连接数、按IP哈希， 默认为 WRR。
         :type Scheduler: str
-        :param _ForwardType: 负载均衡与后端服务之间的转发协议，目前支持 HTTP/HTTPS/TRPC，TRPC暂未对外开放。
+        :param _ForwardType: 负载均衡与后端服务之间的转发协议，目前支持 HTTP/HTTPS/GRPC/TRPC，TRPC暂未对外开放，默认HTTP。
         :type ForwardType: str
         :param _DefaultServer: 是否将该域名设为默认域名，注意，一个监听器下只能设置一个默认域名。
         :type DefaultServer: bool
         :param _Http2: 是否开启Http2，注意，只有HTTPS域名才能开启Http2。
         :type Http2: bool
         :param _TargetType: 后端目标类型，NODE表示绑定普通节点，TARGETGROUP表示绑定目标组
         :type TargetType: str
```

### Comparing `tencentcloud-sdk-python-clb-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-clb-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.942/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.941/README.rst` & `tencentcloud-sdk-python-clb-3.0.942/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.941/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.942/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

