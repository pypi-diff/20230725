# Comparing `tmp/tencentcloud-sdk-python-aiart-3.0.941.tar.gz` & `tmp/tencentcloud-sdk-python-aiart-3.0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-aiart-3.0.941.tar", last modified: Mon Jul 24 00:18:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-aiart-3.0.942.tar", last modified: Tue Jul 25 04:10:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-aiart-3.0.941.tar` & `tencentcloud-sdk-python-aiart-3.0.942.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/aiart/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/aiart/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/aiart/v20221229/
--rw-r--r--   0 root         (0) root         (0)     3676 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/aiart/v20221229/aiart_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/aiart/v20221229/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/aiart/v20221229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    16321 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/aiart/v20221229/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud_sdk_python_aiart.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud_sdk_python_aiart.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud_sdk_python_aiart.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:18:23.000000 tencentcloud-sdk-python-aiart-3.0.941/tencentcloud_sdk_python_aiart.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/aiart/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/aiart/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/aiart/v20221229/
+-rw-r--r--   0 root         (0) root         (0)     3676 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/aiart/v20221229/aiart_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/aiart/v20221229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/aiart/v20221229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    17082 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/aiart/v20221229/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud_sdk_python_aiart.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud_sdk_python_aiart.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud_sdk_python_aiart.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:10:03.000000 tencentcloud-sdk-python-aiart-3.0.942/tencentcloud_sdk_python_aiart.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.941/setup.py` & `tencentcloud-sdk-python-aiart-3.0.942/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/aiart/v20221229/aiart_client.py` & `tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/aiart/v20221229/aiart_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextToImage(self, request):
         """智能文生图接口将根据输入的描述文本，智能生成与之相关的结果图。
-        输入：512个字符以内的描述性文本，推荐使用中文。
+        输入：256个字符以内的描述性文本，推荐使用中文。
         输出：对应风格及分辨率的 AI 生成图。
         可支持的风格详见 [智能文生图风格列表](https://cloud.tencent.com/document/product/1668/86249)，请将列表中的“风格编号”传入 Styles 数组，建议选择一种风格。
 
         请求频率限制为1次/秒。
 
         :param request: Request instance for TextToImage.
         :type request: :class:`tencentcloud.aiart.v20221229.models.TextToImageRequest`
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/aiart/v20221229/errorcodes.py` & `tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/aiart/v20221229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/aiart/v20221229/models.py` & `tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/aiart/v20221229/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,50 +32,52 @@
         :type InputImage: str
         :param _InputUrl: 输入图 Url。
 算法将根据输入的图片，结合文本描述智能生成与之相关的图像。
 Base64 和 Url 必须提供一个，如果都提供以 Base64 为准。
 图片限制：单边分辨率小于2000，转成 Base64 字符串后小于 5MB。
         :type InputUrl: str
         :param _Prompt: 文本描述。
-用于在输入图的基础上引导生成图效果，建议详细描述画面主体、细节、场景等，文本描述越丰富，生成效果越精美。推荐使用中文。最多支持512个 utf-8 字符。
-注意：如果不输入任何文本描述，可能导致较差的效果，建议根据期望的效果输入相应的文本描述。
+用于在输入图的基础上引导生成图效果，增加生成结果中出现描述内容的可能。
+推荐使用中文。最多支持256个 utf-8 字符。
         :type Prompt: str
         :param _NegativePrompt: 反向文本描述。
 用于一定程度上从反面引导模型生成的走向，减少生成结果中出现描述内容的可能，但不能完全杜绝。
-推荐使用中文。最多可传512个 utf-8 字符。
+推荐使用中文。最多可传256个 utf-8 字符。
         :type NegativePrompt: str
         :param _Styles: 绘画风格。
 请在  [智能图生图风格列表](https://cloud.tencent.com/document/product/1668/86250) 中选择期望的风格，传入风格编号。
 推荐使用且只使用一种风格。不传默认使用201（日系动漫风格）。
-如果想要探索风格列表之外的风格，也可以尝试在 Prompt 中输入其他的风格描述。
         :type Styles: list of str
         :param _ResultConfig: 生成图结果的配置，包括输出图片分辨率和尺寸等。
         :type ResultConfig: :class:`tencentcloud.aiart.v20221229.models.ResultConfig`
         :param _LogoAdd: 为生成结果图添加标识的开关，默认为1。
 1：添加标识。
 0：不添加标识。
 其他数值：默认按1处理。
 建议您使用显著标识来提示结果图使用了 AI 绘画技术，是 AI 生成的图片。
         :type LogoAdd: int
         :param _LogoParam: 标识内容设置。
 默认在生成结果图右下角添加“图片由 AI 生成”字样，您可根据自身需要替换为其他的标识图片。
         :type LogoParam: :class:`tencentcloud.aiart.v20221229.models.LogoParam`
         :param _Strength: 生成自由度。
-Strength 值越小，生成图和原图越接近。取值范围0~1，不传默认为0.65。
+Strength 值越小，生成图和原图越接近。取值范围0~1，不传默认为0.75。
         :type Strength: float
+        :param _RspImgType: 返回图像方式（base64 或 url) ，二选一，默认为 base64。url 有效期为1小时。
+        :type RspImgType: str
         """
         self._InputImage = None
         self._InputUrl = None
         self._Prompt = None
         self._NegativePrompt = None
         self._Styles = None
         self._ResultConfig = None
         self._LogoAdd = None
         self._LogoParam = None
         self._Strength = None
+        self._RspImgType = None
 
     @property
     def InputImage(self):
         return self._InputImage
 
     @InputImage.setter
     def InputImage(self, InputImage):
@@ -141,14 +143,22 @@
     def Strength(self):
         return self._Strength
 
     @Strength.setter
     def Strength(self, Strength):
         self._Strength = Strength
 
+    @property
+    def RspImgType(self):
+        return self._RspImgType
+
+    @RspImgType.setter
+    def RspImgType(self, RspImgType):
+        self._RspImgType = RspImgType
+
 
     def _deserialize(self, params):
         self._InputImage = params.get("InputImage")
         self._InputUrl = params.get("InputUrl")
         self._Prompt = params.get("Prompt")
         self._NegativePrompt = params.get("NegativePrompt")
         self._Styles = params.get("Styles")
@@ -156,14 +166,15 @@
             self._ResultConfig = ResultConfig()
             self._ResultConfig._deserialize(params.get("ResultConfig"))
         self._LogoAdd = params.get("LogoAdd")
         if params.get("LogoParam") is not None:
             self._LogoParam = LogoParam()
             self._LogoParam._deserialize(params.get("LogoParam"))
         self._Strength = params.get("Strength")
+        self._RspImgType = params.get("RspImgType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -173,15 +184,17 @@
 class ImageToImageResponse(AbstractModel):
     """ImageToImage返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _ResultImage: 返回的生成图 Base64 编码。
+        :param _ResultImage: 根据入参 RspImgType 填入不同，返回不同的内容。
+如果传入 base64 则返回生成图 Base64 编码。
+如果传入 url 则返回的生成图 URL , 有效期1小时，请及时保存。
         :type ResultImage: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._ResultImage = None
         self._RequestId = None
 
@@ -378,43 +391,45 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Prompt: 文本描述。
 算法将根据输入的文本智能生成与之相关的图像。建议详细描述画面主体、细节、场景等，文本描述越丰富，生成效果越精美。
-不能为空，推荐使用中文。最多可传512个 utf-8 字符。
+不能为空，推荐使用中文。最多可传256个 utf-8 字符。
         :type Prompt: str
         :param _NegativePrompt: 反向文本描述。
 用于一定程度上从反面引导模型生成的走向，减少生成结果中出现描述内容的可能，但不能完全杜绝。
-推荐使用中文。最多可传512个 utf-8 字符。
+推荐使用中文。最多可传256个 utf-8 字符。
         :type NegativePrompt: str
         :param _Styles: 绘画风格。
 请在 [智能文生图风格列表](https://cloud.tencent.com/document/product/1668/86249) 中选择期望的风格，传入风格编号。
 推荐使用且只使用一种风格。不传默认使用201（日系动漫风格）。
-如果想要探索风格列表之外的风格，也可以尝试在 Prompt 中输入其他的风格描述。
         :type Styles: list of str
         :param _ResultConfig: 生成图结果的配置，包括输出图片分辨率和尺寸等。
         :type ResultConfig: :class:`tencentcloud.aiart.v20221229.models.ResultConfig`
         :param _LogoAdd: 为生成结果图添加标识的开关，默认为1。
 1：添加标识。
 0：不添加标识。
 其他数值：默认按1处理。
 建议您使用显著标识来提示结果图使用了 AI 绘画技术，是 AI 生成的图片。
         :type LogoAdd: int
         :param _LogoParam: 标识内容设置。
 默认在生成结果图右下角添加“图片由 AI 生成”字样，您可根据自身需要替换为其他的标识图片。
         :type LogoParam: :class:`tencentcloud.aiart.v20221229.models.LogoParam`
+        :param _RspImgType: 返回图像方式（base64 或 url) ，二选一，默认为 base64。url 有效期为1小时。
+        :type RspImgType: str
         """
         self._Prompt = None
         self._NegativePrompt = None
         self._Styles = None
         self._ResultConfig = None
         self._LogoAdd = None
         self._LogoParam = None
+        self._RspImgType = None
 
     @property
     def Prompt(self):
         return self._Prompt
 
     @Prompt.setter
     def Prompt(self, Prompt):
@@ -456,26 +471,35 @@
     def LogoParam(self):
         return self._LogoParam
 
     @LogoParam.setter
     def LogoParam(self, LogoParam):
         self._LogoParam = LogoParam
 
+    @property
+    def RspImgType(self):
+        return self._RspImgType
+
+    @RspImgType.setter
+    def RspImgType(self, RspImgType):
+        self._RspImgType = RspImgType
+
 
     def _deserialize(self, params):
         self._Prompt = params.get("Prompt")
         self._NegativePrompt = params.get("NegativePrompt")
         self._Styles = params.get("Styles")
         if params.get("ResultConfig") is not None:
             self._ResultConfig = ResultConfig()
             self._ResultConfig._deserialize(params.get("ResultConfig"))
         self._LogoAdd = params.get("LogoAdd")
         if params.get("LogoParam") is not None:
             self._LogoParam = LogoParam()
             self._LogoParam._deserialize(params.get("LogoParam"))
+        self._RspImgType = params.get("RspImgType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -485,15 +509,17 @@
 class TextToImageResponse(AbstractModel):
     """TextToImage返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _ResultImage: 返回的生成图 Base64 编码。
+        :param _ResultImage: 根据入参 RspImgType 填入不同，返回不同的内容。
+如果传入 base64 则返回生成图 Base64 编码。
+如果传入 url 则返回的生成图 URL , 有效期1小时，请及时保存。
         :type ResultImage: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._ResultImage = None
         self._RequestId = None
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.941/tencentcloud/__init__.py` & `tencentcloud-sdk-python-aiart-3.0.942/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-aiart-3.0.941/PKG-INFO` & `tencentcloud-sdk-python-aiart-3.0.942/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-aiart
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Aiart SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.941/README.rst` & `tencentcloud-sdk-python-aiart-3.0.942/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.941/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO` & `tencentcloud-sdk-python-aiart-3.0.942/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-aiart
-Version: 3.0.941
+Version: 3.0.942
 Summary: Tencent Cloud Aiart SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

