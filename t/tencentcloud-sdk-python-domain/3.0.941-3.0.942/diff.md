# Comparing `tmp/tencentcloud-sdk-python-domain-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-domain-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.941.tar", last modified: Mon Jul 24 00:35:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.942.tar", last modified: Tue Jul 25 04:16:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-domain-3.0.941.tar` & `tencentcloud-sdk-python-domain-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8876 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    26115 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/domain_client.py
--rw-r--r--   0 root         (0) root         (0)   122825 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud_sdk_python_domain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud_sdk_python_domain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:16:54.000000 tencentcloud-sdk-python-domain-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-25 04:16:53.000000 tencentcloud-sdk-python-domain-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:16:54.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:16:53.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:16:54.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:16:53.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:16:54.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud/domain/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:16:53.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud/domain/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9007 2023-07-25 04:16:53.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud/domain/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    26115 2023-07-25 04:16:53.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud/domain/v20180808/domain_client.py
+-rw-r--r--   0 root         (0) root         (0)   122825 2023-07-25 04:16:53.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud/domain/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:16:54.000000 tencentcloud-sdk-python-domain-3.0.942/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:16:54.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud_sdk_python_domain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:16:54.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-25 04:16:54.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-25 04:16:54.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:16:54.000000 tencentcloud-sdk-python-domain-3.0.942/tencentcloud_sdk_python_domain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-25 04:16:54.000000 tencentcloud-sdk-python-domain-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-25 04:16:53.000000 tencentcloud-sdk-python-domain-3.0.942/README.rst
```

### Comparing `tencentcloud-sdk-python-domain-3.0.941/setup.py` & `tencentcloud-sdk-python-domain-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-domain-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/errorcodes.py` & `tencentcloud-sdk-python-domain-3.0.942/tencentcloud/domain/v20180808/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,17 @@
 
 # 修改 DNS 失败，请输入正确的 DNS 服务器地址。
 FAILEDOPERATION_SETDOMAINDNSFAILED = 'FailedOperation.SetDomainDnsFailed'
 
 # 信息模板超过可用数量上限，建议删除已有模板后重试。
 FAILEDOPERATION_TEMPLATEMAXNUMFAILED = 'FailedOperation.TemplateMaxNumFailed'
 
+# 域名提交转入失败，请稍后重试。
+FAILEDOPERATION_TRANSFERINDOMAINFAILED = 'FailedOperation.TransferInDomainFailed'
+
 # 上传图片操作失败。
 FAILEDOPERATION_UPLOADIMAGEFAILED = 'FailedOperation.UploadImageFailed'
 
 # 当前用户未在官网进行实名操作。
 FAILEDOPERATION_VERIFYUINISREALNAME = 'FailedOperation.VerifyUinIsRealname'
 
 # 内部错误。
```

### Comparing `tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/domain_client.py` & `tencentcloud-sdk-python-domain-3.0.942/tencentcloud/domain/v20180808/domain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/models.py` & `tencentcloud-sdk-python-domain-3.0.942/tencentcloud/domain/v20180808/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.941/tencentcloud_sdk_python_domain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.942/tencentcloud_sdk_python_domain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.942/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.941/README.rst` & `tencentcloud-sdk-python-domain-3.0.942/README.rst`

 * *Files identical despite different names*

