# Comparing `tmp/tencentcloud-sdk-python-bma-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-bma-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bma-3.0.940.tar", last modified: Fri Jul 21 00:23:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bma-3.0.942.tar", last modified: Tue Jul 25 04:11:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bma-3.0.940.tar` & `tencentcloud-sdk-python-bma-3.0.942.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud_sdk_python_bma.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud_sdk_python_bma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud_sdk_python_bma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud_sdk_python_bma.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20221115/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20221115/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3348 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20221115/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10571 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20221115/bma_client.py
--rw-r--r--   0 root         (0) root         (0)    65352 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20221115/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20210624/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20210624/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20210624/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25903 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20210624/bma_client.py
--rw-r--r--   0 root         (0) root         (0)   146139 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20210624/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:23:11.000000 tencentcloud-sdk-python-bma-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud_sdk_python_bma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud_sdk_python_bma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud_sdk_python_bma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud_sdk_python_bma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20221115/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20221115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20221115/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    10571 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20221115/bma_client.py
+-rw-r--r--   0 root         (0) root         (0)    65352 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20221115/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20210624/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20210624/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20210624/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25903 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20210624/bma_client.py
+-rw-r--r--   0 root         (0) root         (0)   146139 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20210624/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:11:58.000000 tencentcloud-sdk-python-bma-3.0.942/README.rst
```

### Comparing `tencentcloud-sdk-python-bma-3.0.940/setup.py` & `tencentcloud-sdk-python-bma-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.940/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-bma-3.0.942/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.940/tencentcloud_sdk_python_bma.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bma-3.0.942/tencentcloud_sdk_python_bma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bma
-Version: 3.0.940
+Version: 3.0.942
 Summary: Tencent Cloud Bma SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bma-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bma-3.0.942/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.940'
+__version__ = '3.0.942'
```

### Comparing `tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20221115/errorcodes.py` & `tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20221115/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20221115/bma_client.py` & `tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20221115/bma_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20221115/models.py` & `tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20221115/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20210624/errorcodes.py` & `tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20210624/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20210624/bma_client.py` & `tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20210624/bma_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.940/tencentcloud/bma/v20210624/models.py` & `tencentcloud-sdk-python-bma-3.0.942/tencentcloud/bma/v20210624/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-bma-3.0.942/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bma
-Version: 3.0.940
+Version: 3.0.942
 Summary: Tencent Cloud Bma SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bma-3.0.940/README.rst` & `tencentcloud-sdk-python-bma-3.0.942/README.rst`

 * *Files identical despite different names*

