# Comparing `tmp/tencentcloud-sdk-python-vms-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-vms-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vms-3.0.941.tar", last modified: Mon Jul 24 00:47:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vms-3.0.942.tar", last modified: Tue Jul 25 04:29:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vms-3.0.941.tar` & `tencentcloud-sdk-python-vms-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud/vms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud/vms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud/vms/v20200902/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud/vms/v20200902/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4848 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud/vms/v20200902/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2741 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud/vms/v20200902/vms_client.py
--rw-r--r--   0 root         (0) root         (0)    10184 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud/vms/v20200902/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud_sdk_python_vms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud_sdk_python_vms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud_sdk_python_vms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud_sdk_python_vms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:47:43.000000 tencentcloud-sdk-python-vms-3.0.941/tencentcloud_sdk_python_vms.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud/vms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud/vms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud/vms/v20200902/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud/vms/v20200902/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4848 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud/vms/v20200902/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud/vms/v20200902/vms_client.py
+-rw-r--r--   0 root         (0) root         (0)    10184 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud/vms/v20200902/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud_sdk_python_vms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud_sdk_python_vms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud_sdk_python_vms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud_sdk_python_vms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:29:31.000000 tencentcloud-sdk-python-vms-3.0.942/tencentcloud_sdk_python_vms.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-vms-3.0.941/setup.py` & `tencentcloud-sdk-python-vms-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vms-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vms-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vms-3.0.941/tencentcloud/vms/v20200902/errorcodes.py` & `tencentcloud-sdk-python-vms-3.0.942/tencentcloud/vms/v20200902/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vms-3.0.941/tencentcloud/vms/v20200902/vms_client.py` & `tencentcloud-sdk-python-vms-3.0.942/tencentcloud/vms/v20200902/vms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vms-3.0.941/tencentcloud/vms/v20200902/models.py` & `tencentcloud-sdk-python-vms-3.0.942/tencentcloud/vms/v20200902/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vms-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-vms-3.0.942/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vms
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Vms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vms-3.0.941/README.rst` & `tencentcloud-sdk-python-vms-3.0.942/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vms-3.0.941/tencentcloud_sdk_python_vms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vms-3.0.942/tencentcloud_sdk_python_vms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vms
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Vms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

