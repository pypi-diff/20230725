# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.941.tar", last modified: Mon Jul 24 00:48:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.942.tar", last modified: Tue Jul 25 04:29:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.941.tar` & `tencentcloud-sdk-python-waf-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    47662 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)   309376 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/tencentcloud_sdk_python_waf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:48:08.000000 tencentcloud-sdk-python-waf-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    47687 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)   309253 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:29:53.000000 tencentcloud-sdk-python-waf-3.0.942/README.rst
```

### Comparing `tencentcloud-sdk-python-waf-3.0.941/setup.py` & `tencentcloud-sdk-python-waf-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-waf-3.0.941/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.942/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.941/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.942/tencentcloud/waf/v20180125/waf_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,15 +414,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoDenyIP(self, request):
-        """描述WAF自动封禁IP详情,对齐自动封堵状态
+        """接口已废弃
+
+        描述WAF自动封禁IP详情,对齐自动封堵状态
 
         :param request: Request instance for DescribeAutoDenyIP.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeAutoDenyIPRequest`
         :rtype: :class:`tencentcloud.waf.v20180125.models.DescribeAutoDenyIPResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-waf-3.0.941/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.942/tencentcloud/waf/v20180125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10302,16 +10302,15 @@
         :type From: int
         :param _To: 要查询的日志的结束时间，Unix时间戳，单位ms
         :type To: int
         :param _Query: 查询语句，语句长度最大为4096
         :type Query: str
         :param _Limit: 单次查询返回的日志条数，最大值为100
         :type Limit: int
-        :param _Context: 加载更多日志时使用，透传上次返回的Context值，获取后续的日志内容。
-新版本此字段填空填
+        :param _Context: 新版本此字段失效，填空字符串，翻页使用Page
         :type Context: str
         :param _Sort: 日志接口是否按时间排序返回；可选值：asc(升序)、desc(降序)，默认为 desc
         :type Sort: str
         :param _Page: 第几页，从0开始。新版本接口字段
         :type Page: int
         """
         self._TopicId = None
@@ -10410,15 +10409,15 @@
 class SearchAccessLogResponse(AbstractModel):
     """SearchAccessLog返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Context: 加载后续内容的Context
+        :param _Context: 新接口此字段失效，默认返回空字符串
         :type Context: str
         :param _ListOver: 日志查询结果是否全部返回，其中，“true”表示结果返回，“false”表示结果为返回
         :type ListOver: bool
         :param _Analysis: 返回的是否为分析结果，其中，“true”表示返回分析结果，“false”表示未返回分析结果
         :type Analysis: bool
         :param _ColNames: 如果Analysis为True，则返回分析结果的列名，否则为空
 注意：此字段可能返回 null，表示取不到有效值。
@@ -10529,15 +10528,15 @@
         r"""
         :param _Domain: 查询的域名，所有域名使用all
         :type Domain: str
         :param _StartTime: 查询起始时间
         :type StartTime: str
         :param _EndTime: 查询结束时间
         :type EndTime: str
-        :param _Context: 查询的游标。第一次请求使用空字符串即可，后续请求使用上一次请求返回的最后一条记录的context的值即可。
+        :param _Context: 接口升级，这个字段传空字符串,翻页使用Page字段
         :type Context: str
         :param _QueryString: Lucene语法
         :type QueryString: str
         :param _Count: 查询的数量，默认10条，最多100条
         :type Count: int
         :param _Sort: 默认为desc，可以取值desc和asc
         :type Sort: str
@@ -10642,15 +10641,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Count: 当前返回的攻击日志条数
         :type Count: int
-        :param _Context: 翻页游标，如果没有下一页了，这个参数为空""
+        :param _Context: 接口升级，此字段无效，默认返回空字符串
         :type Context: str
         :param _Data: 攻击日志数组条目内容
         :type Data: list of AttackLogInfo
         :param _ListOver: CLS接口返回内容
         :type ListOver: bool
         :param _SqlFlag: CLS接口返回内容，标志是否启动新版本索引
         :type SqlFlag: bool
```

### Comparing `tencentcloud-sdk-python-waf-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.942/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.941/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.942/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.941/README.rst` & `tencentcloud-sdk-python-waf-3.0.942/README.rst`

 * *Files identical despite different names*

