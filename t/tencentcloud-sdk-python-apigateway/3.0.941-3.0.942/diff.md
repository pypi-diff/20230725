# Comparing `tmp/tencentcloud-sdk-python-apigateway-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-apigateway-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.941.tar", last modified: Mon Jul 24 00:19:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.942.tar", last modified: Tue Jul 25 04:10:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apigateway-3.0.941.tar` & `tencentcloud-sdk-python-apigateway-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/apigateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/apigateway/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/apigateway/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21433 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/apigateway/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   648371 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/apigateway/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)    96571 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/apigateway/v20180808/apigateway_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud_sdk_python_apigateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-24 00:19:02.000000 tencentcloud-sdk-python-apigateway-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/apigateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/apigateway/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/apigateway/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21433 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/apigateway/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   648371 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/apigateway/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)    96571 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/apigateway/v20180808/apigateway_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud_sdk_python_apigateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-25 04:10:49.000000 tencentcloud-sdk-python-apigateway-3.0.942/README.rst
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.941/setup.py` & `tencentcloud-sdk-python-apigateway-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/apigateway/v20180808/errorcodes.py` & `tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/apigateway/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/apigateway/v20180808/models.py` & `tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/apigateway/v20180808/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/apigateway/v20180808/apigateway_client.py` & `tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/apigateway/v20180808/apigateway_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-apigateway-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.942/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.941/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.942/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.941/README.rst` & `tencentcloud-sdk-python-apigateway-3.0.942/README.rst`

 * *Files identical despite different names*
