# Comparing `tmp/tencentcloud-sdk-python-cfg-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-cfg-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfg-3.0.941.tar", last modified: Mon Jul 24 00:32:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfg-3.0.942.tar", last modified: Tue Jul 25 04:13:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfg-3.0.941.tar` & `tencentcloud-sdk-python-cfg-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/cfg/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/cfg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/cfg/v20210820/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/cfg/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9735 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/cfg/v20210820/cfg_client.py
--rw-r--r--   0 root         (0) root         (0)     1933 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/cfg/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   113819 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/cfg/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud_sdk_python_cfg.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud_sdk_python_cfg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud_sdk_python_cfg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud_sdk_python_cfg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:32:57.000000 tencentcloud-sdk-python-cfg-3.0.941/tencentcloud_sdk_python_cfg.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/cfg/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/cfg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/cfg/v20210820/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/cfg/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9735 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/cfg/v20210820/cfg_client.py
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/cfg/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   115910 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/cfg/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud_sdk_python_cfg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud_sdk_python_cfg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud_sdk_python_cfg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud_sdk_python_cfg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:13:35.000000 tencentcloud-sdk-python-cfg-3.0.942/tencentcloud_sdk_python_cfg.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cfg-3.0.941/setup.py` & `tencentcloud-sdk-python-cfg-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/cfg/v20210820/cfg_client.py` & `tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/cfg/v20210820/cfg_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/cfg/v20210820/errorcodes.py` & `tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/cfg/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfg-3.0.941/tencentcloud/cfg/v20210820/models.py` & `tencentcloud-sdk-python-cfg-3.0.942/tencentcloud/cfg/v20210820/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,59 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class ActionFilter(AbstractModel):
+    """动作库筛选栏位
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Keyword: 关键字
+        :type Keyword: str
+        :param _Values: 搜索内容值
+        :type Values: list of str
+        """
+        self._Keyword = None
+        self._Values = None
+
+    @property
+    def Keyword(self):
+        return self._Keyword
+
+    @Keyword.setter
+    def Keyword(self, Keyword):
+        self._Keyword = Keyword
+
+    @property
+    def Values(self):
+        return self._Values
+
+    @Values.setter
+    def Values(self, Values):
+        self._Values = Values
+
+
+    def _deserialize(self, params):
+        self._Keyword = params.get("Keyword")
+        self._Values = params.get("Values")
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
 class CreateTaskFromTemplateRequest(AbstractModel):
     """CreateTaskFromTemplate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -343,23 +388,26 @@
         :type TaskStatus: int
         :param _TaskStartTime: 开始时间，固定格式%Y-%m-%d %H:%M:%S
         :type TaskStartTime: str
         :param _TaskEndTime: 结束时间，固定格式%Y-%m-%d %H:%M:%S
         :type TaskEndTime: str
         :param _Tags: 标签对
         :type Tags: list of TagWithDescribe
+        :param _Filters: 筛选条件
+        :type Filters: list of ActionFilter
         """
         self._Limit = None
         self._Offset = None
         self._TaskTitle = None
         self._TaskTag = None
         self._TaskStatus = None
         self._TaskStartTime = None
         self._TaskEndTime = None
         self._Tags = None
+        self._Filters = None
 
     @property
     def Limit(self):
         return self._Limit
 
     @Limit.setter
     def Limit(self, Limit):
@@ -417,14 +465,22 @@
     def Tags(self):
         return self._Tags
 
     @Tags.setter
     def Tags(self, Tags):
         self._Tags = Tags
 
+    @property
+    def Filters(self):
+        return self._Filters
+
+    @Filters.setter
+    def Filters(self, Filters):
+        self._Filters = Filters
+
 
     def _deserialize(self, params):
         self._Limit = params.get("Limit")
         self._Offset = params.get("Offset")
         self._TaskTitle = params.get("TaskTitle")
         self._TaskTag = params.get("TaskTag")
         self._TaskStatus = params.get("TaskStatus")
@@ -432,14 +488,20 @@
         self._TaskEndTime = params.get("TaskEndTime")
         if params.get("Tags") is not None:
             self._Tags = []
             for item in params.get("Tags"):
                 obj = TagWithDescribe()
                 obj._deserialize(item)
                 self._Tags.append(obj)
+        if params.get("Filters") is not None:
+            self._Filters = []
+            for item in params.get("Filters"):
+                obj = ActionFilter()
+                obj._deserialize(item)
+                self._Filters.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -606,23 +668,26 @@
         :type IsUsed: int
         :param _Tags: 标签对
         :type Tags: list of TagWithDescribe
         :param _TemplateSource: 经验来源 0-自建 1-专家推荐
         :type TemplateSource: int
         :param _TemplateIdList: 经验ID
         :type TemplateIdList: list of int
+        :param _Filters: 过滤参数
+        :type Filters: list of ActionFilter
         """
         self._Limit = None
         self._Offset = None
         self._Title = None
         self._Tag = None
         self._IsUsed = None
         self._Tags = None
         self._TemplateSource = None
         self._TemplateIdList = None
+        self._Filters = None
 
     @property
     def Limit(self):
         return self._Limit
 
     @Limit.setter
     def Limit(self, Limit):
@@ -680,14 +745,22 @@
     def TemplateIdList(self):
         return self._TemplateIdList
 
     @TemplateIdList.setter
     def TemplateIdList(self, TemplateIdList):
         self._TemplateIdList = TemplateIdList
 
+    @property
+    def Filters(self):
+        return self._Filters
+
+    @Filters.setter
+    def Filters(self, Filters):
+        self._Filters = Filters
+
 
     def _deserialize(self, params):
         self._Limit = params.get("Limit")
         self._Offset = params.get("Offset")
         self._Title = params.get("Title")
         self._Tag = params.get("Tag")
         self._IsUsed = params.get("IsUsed")
@@ -695,14 +768,20 @@
             self._Tags = []
             for item in params.get("Tags"):
                 obj = TagWithDescribe()
                 obj._deserialize(item)
                 self._Tags.append(obj)
         self._TemplateSource = params.get("TemplateSource")
         self._TemplateIdList = params.get("TemplateIdList")
+        if params.get("Filters") is not None:
+            self._Filters = []
+            for item in params.get("Filters"):
+                obj = ActionFilter()
+                obj._deserialize(item)
+                self._Filters.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cfg-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-cfg-3.0.942/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfg
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Cfg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfg-3.0.941/README.rst` & `tencentcloud-sdk-python-cfg-3.0.942/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfg-3.0.941/tencentcloud_sdk_python_cfg.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfg-3.0.942/tencentcloud_sdk_python_cfg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfg
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Cfg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

