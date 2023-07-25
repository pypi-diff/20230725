# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.941.tar", last modified: Mon Jul 24 00:19:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.942.tar", last modified: Tue Jul 25 04:10:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.941.tar` & `tencentcloud-sdk-python-asr-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud_sdk_python_asr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29417 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   111945 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:19:12.000000 tencentcloud-sdk-python-asr-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29417 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   111930 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/README.rst
```

### Comparing `tencentcloud-sdk-python-asr-3.0.941/setup.py` & `tencentcloud-sdk-python-asr-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.941/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.942/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.941/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/asr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.941/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.941/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2317,15 +2317,15 @@
         :type FilterPunc: int
         :param _ConvertNumMode: 是否进行阿拉伯数字智能转换。0：不转换，直接输出中文数字，1：根据场景智能转换为阿拉伯数字。默认值为1。
         :type ConvertNumMode: int
         :param _HotwordId: 热词id。用于调用对应的热词表，如果在调用语音识别服务时，不进行单独的热词id设置，自动生效默认热词；如果进行了单独的热词id设置，那么将生效单独设置的热词id。
         :type HotwordId: str
         :param _CustomizationId: 自学习模型 id。如设置了该参数，将生效对应的自学习模型。
         :type CustomizationId: str
-        :param _ReinforceHotword: 热词增强功能。1:开启后（仅支持8k_zh,16k_zh），将开启同音替换功能，同音字、词在热词中配置。举例：热词配置“蜜制”并开启增强功能后，与“蜜制”同拼音（mizhi）的“秘制”、“蜜汁”的识别结果会被强制替换成“蜜制”。因此建议客户根据自己的实际情况开启该功能。
+        :param _ReinforceHotword: 热词增强功能。1:开启后（仅支持8k_zh,16k_zh），将开启同音替换功能，同音字、词在热词中配置。举例：热词配置“蜜制”并开启增强功能后，与“蜜制”同拼音（mizhi）的“秘制”的识别结果会被强制替换成“蜜制”。因此建议客户根据自己的实际情况开启该功能。
         :type ReinforceHotword: int
         :param _HotwordList: 临时热词：用于提升识别准确率，临时热词规则：“热词|权重”，热词不超过30个字符（最多10个汉字），权重1-10，最多传入128个热词。举例："腾讯云|10,语音识别|5,ASR|10"。
 “临时热词”和“热词id”的区别：热词id需要先在控制台或通过接口创建热词表，得到热词表id后才可以使用热词功能，本字段可以在每次请求时直接传入热词使用，但每次请求后云端不会保留相关的热词数据，需要客户自行维护相关数据
         :type HotwordList: str
         :param _InputSampleRate: 支持pcm格式的8k音频在与引擎采样率不匹配的情况下升采样到16k后识别，能有效提升识别准确率。仅支持：8000。如：传入 8000 ，则pcm音频采样率为8k，当引擎选用16k_zh， 那么该8k采样率的pcm音频可以在16k_zh引擎下正常识别。 注：此参数仅适用于pcm格式音频，不传入值将维持默认状态，即默认调用的引擎采样率等于pcm音频采样率。
         :type InputSampleRate: int
         """
```

### Comparing `tencentcloud-sdk-python-asr-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.942/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.941/README.rst` & `tencentcloud-sdk-python-asr-3.0.942/README.rst`

 * *Files identical despite different names*

