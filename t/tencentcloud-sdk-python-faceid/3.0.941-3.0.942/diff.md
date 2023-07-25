# Comparing `tmp/tencentcloud-sdk-python-faceid-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-faceid-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.941.tar", last modified: Mon Jul 24 00:37:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.942.tar", last modified: Tue Jul 25 04:18:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-faceid-3.0.941.tar` & `tencentcloud-sdk-python-faceid-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud_sdk_python_faceid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/faceid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/faceid/v20180301/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/faceid/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9370 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/faceid/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    34162 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/faceid/v20180301/faceid_client.py
--rw-r--r--   0 root         (0) root         (0)   212614 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/faceid/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/faceid/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-24 00:37:09.000000 tencentcloud-sdk-python-faceid-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud_sdk_python_faceid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/faceid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/faceid/v20180301/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/faceid/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9370 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/faceid/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    34162 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/faceid/v20180301/faceid_client.py
+-rw-r--r--   0 root         (0) root         (0)   212626 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/faceid/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/faceid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-25 04:18:18.000000 tencentcloud-sdk-python-faceid-3.0.942/README.rst
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.941/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.942/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.941/setup.py` & `tencentcloud-sdk-python-faceid-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/faceid/v20180301/errorcodes.py` & `tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/faceid/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/faceid/v20180301/faceid_client.py` & `tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/faceid/v20180301/faceid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.941/tencentcloud/faceid/v20180301/models.py` & `tencentcloud-sdk-python-faceid-3.0.942/tencentcloud/faceid/v20180301/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2891,15 +2891,15 @@
         :type BestFrame: :class:`tencentcloud.faceid.v20180301.models.DetectInfoBestFrame`
         :param _VideoData: 视频信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type VideoData: :class:`tencentcloud.faceid.v20180301.models.DetectInfoVideoData`
         :param _Encryption: 敏感数据加密信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Encryption: :class:`tencentcloud.faceid.v20180301.models.Encryption`
-        :param _IntentionVerifyData: 意愿核身相关信息。若未使用意愿核身功能，该字段返回值可以不处理。
+        :param _IntentionVerifyData: 意愿核身朗读模式结果信息。若未使用意愿核身功能，该字段返回值可以不处理。
 注意：此字段可能返回 null，表示取不到有效值。
         :type IntentionVerifyData: :class:`tencentcloud.faceid.v20180301.models.IntentionVerifyData`
         :param _IntentionQuestionResult: 意愿核身问答模式结果。若未使用该意愿核身功能，该字段返回值可以不处理。
 注意：此字段可能返回 null，表示取不到有效值。
         :type IntentionQuestionResult: :class:`tencentcloud.faceid.v20180301.models.IntentionQuestionResult`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.942/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.941/README.rst` & `tencentcloud-sdk-python-faceid-3.0.942/README.rst`

 * *Files identical despite different names*

