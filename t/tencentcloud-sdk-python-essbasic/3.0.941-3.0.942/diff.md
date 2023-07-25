# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.941.tar", last modified: Mon Jul 24 00:37:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.942.tar", last modified: Tue Jul 25 04:18:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.941.tar` & `tencentcloud-sdk-python-essbasic-3.0.942.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    55045 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   387357 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54057 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:37:00.000000 tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    55045 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   387357 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.941/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8897,15 +8897,15 @@
         :param _ComponentId: 表单域或控件的ID，跟ComponentName二选一，不能全为空；
 CreateFlowsByTemplates 接口不使用此字段。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ComponentId: str
         :param _ComponentName: 控件的名字，跟ComponentId二选一，不能全为空
 注意：此字段可能返回 null，表示取不到有效值。
         :type ComponentName: str
-        :param _LockComponentValue: 是否锁定模版控件值，锁定后无法修改（用于嵌入式发起合同），true-锁定，false-不锁定
+        :param _LockComponentValue: 是否锁定模板控件值，锁定后无法修改（用于嵌入式发起合同），true-锁定，false-不锁定
 注意：此字段可能返回 null，表示取不到有效值。
         :type LockComponentValue: bool
         """
         self._ComponentValue = None
         self._ComponentId = None
         self._ComponentName = None
         self._LockComponentValue = None
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.942/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.941/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.942/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.941/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

