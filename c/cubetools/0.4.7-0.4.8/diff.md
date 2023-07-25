# Comparing `tmp/cubetools-0.4.7.tar.gz` & `tmp/cubetools-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubetools-0.4.7.tar", last modified: Wed Jul 12 06:51:44 2023, max compression
+gzip compressed data, was "dist/cubetools-0.4.8.tar", last modified: Tue Jul 25 10:16:38 2023, max compression
```

## Comparing `cubetools-0.4.7.tar` & `cubetools-0.4.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-07-12 06:51:44.000000 cubetools-0.4.7/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2340 2023-07-12 06:51:44.000000 cubetools-0.4.7/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1232 2023-06-19 07:55:29.000000 cubetools-0.4.7/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.4.7/cubetools/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3047 2023-06-19 07:55:29.000000 cubetools-0.4.7/cubetools/download_model.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.4.7/cubetools/image_tools.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.4.7/cubetools/mindspore_lite_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.4.7/cubetools/onnx_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.4.7/cubetools/openvino_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.4.7/cubetools/paddle_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2394 2023-05-23 12:05:30.000000 cubetools-0.4.7/cubetools/python_chat_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    15694 2023-05-25 10:46:59.000000 cubetools-0.4.7/cubetools/python_video_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2628 2023-07-12 06:51:33.000000 cubetools-0.4.7/cubetools/pytorch_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.4.7/cubetools/video_capture.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3799 2023-05-25 10:06:04.000000 cubetools-0.4.7/cubetools/video_predict.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2340 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      565 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       88 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       32 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-07-12 06:51:44.000000 cubetools-0.4.7/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2291 2023-07-12 06:51:33.000000 cubetools-0.4.7/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-07-25 10:16:38.000000 cubetools-0.4.8/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2328 2023-07-25 10:16:38.000000 cubetools-0.4.8/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1220 2023-07-25 10:16:23.000000 cubetools-0.4.8/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-07-25 10:16:38.000000 cubetools-0.4.8/cubetools/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.4.8/cubetools/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3047 2023-06-19 07:55:29.000000 cubetools-0.4.8/cubetools/download_model.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.4.8/cubetools/image_tools.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.4.8/cubetools/mindspore_lite_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.4.8/cubetools/onnx_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.4.8/cubetools/openvino_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.4.8/cubetools/paddle_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2394 2023-05-23 12:05:30.000000 cubetools-0.4.8/cubetools/python_chat_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    15694 2023-05-25 10:46:59.000000 cubetools-0.4.8/cubetools/python_video_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2628 2023-07-12 07:01:07.000000 cubetools-0.4.8/cubetools/pytorch_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.4.8/cubetools/video_capture.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3799 2023-05-25 10:06:04.000000 cubetools-0.4.8/cubetools/video_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     6213 2023-07-25 08:49:03.000000 cubetools-0.4.8/cubetools/video_predict2.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-07-25 10:16:38.000000 cubetools-0.4.8/cubetools.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2328 2023-07-25 10:16:38.000000 cubetools-0.4.8/cubetools.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      593 2023-07-25 10:16:38.000000 cubetools-0.4.8/cubetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-07-25 10:16:38.000000 cubetools-0.4.8/cubetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       88 2023-07-25 10:16:38.000000 cubetools-0.4.8/cubetools.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       32 2023-07-25 10:16:38.000000 cubetools-0.4.8/cubetools.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-07-25 10:16:38.000000 cubetools-0.4.8/cubetools.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-07-25 10:16:38.000000 cubetools-0.4.8/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2291 2023-07-25 10:16:23.000000 cubetools-0.4.8/setup.py
```

### Comparing `cubetools-0.4.7/PKG-INFO` & `cubetools-0.4.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.4.7
+Version: 0.4.8
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
         
         [CubeAI智立方](https://openi.pcl.ac.cn/OpenI/cubeai) 模型和应用开发常用工具集。
         
         目前主要包括：
         
         - 图像前处理、后处理等常用函数封装。
-        - 通用视频流媒体在线流式AI推理服务组件。
+        - 通用AI流媒体在线推理服务框架。
         - 通用OpenVino模型推理框架（基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装）。
         - 通用ONNX模型推理框架（基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装）。
         - 通用PaddlePaddle模型推理框架（基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装）。
         - 通用MindSporeLite推理框架（基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装）。
         - 通用Pytorch模型推理框架。
         - 基于Gradio的视频流媒体类Python前端服务组件。
         - 基于Gradio的聊天对话类Python前端服务组件。
```

### Comparing `cubetools-0.4.7/README.md` & `cubetools-0.4.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # CubeTools
 
 [CubeAI智立方](https://openi.pcl.ac.cn/OpenI/cubeai) 模型和应用开发常用工具集。
 
 目前主要包括：
 
 - 图像前处理、后处理等常用函数封装。
-- 通用视频流媒体在线流式AI推理服务组件。
+- 通用AI流媒体在线推理服务框架。
 - 通用OpenVino模型推理框架（基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装）。
 - 通用ONNX模型推理框架（基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装）。
 - 通用PaddlePaddle模型推理框架（基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装）。
 - 通用MindSporeLite推理框架（基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装）。
 - 通用Pytorch模型推理框架。
 - 基于Gradio的视频流媒体类Python前端服务组件。
 - 基于Gradio的聊天对话类Python前端服务组件。
```

### Comparing `cubetools-0.4.7/cubetools/download_model.py` & `cubetools-0.4.8/cubetools/download_model.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.7/cubetools/image_tools.py` & `cubetools-0.4.8/cubetools/image_tools.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.7/cubetools/mindspore_lite_predict.py` & `cubetools-0.4.8/cubetools/mindspore_lite_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.7/cubetools/onnx_predict.py` & `cubetools-0.4.8/cubetools/onnx_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.7/cubetools/openvino_predict.py` & `cubetools-0.4.8/cubetools/openvino_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.7/cubetools/paddle_predict.py` & `cubetools-0.4.8/cubetools/paddle_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.7/cubetools/python_chat_frontend.py` & `cubetools-0.4.8/cubetools/python_chat_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.7/cubetools/python_video_frontend.py` & `cubetools-0.4.8/cubetools/python_video_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.7/cubetools/pytorch_predict.py` & `cubetools-0.4.8/cubetools/pytorch_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.7/cubetools/video_capture.py` & `cubetools-0.4.8/cubetools/video_capture.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.7/cubetools/video_predict.py` & `cubetools-0.4.8/cubetools/video_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.7/cubetools.egg-info/PKG-INFO` & `cubetools-0.4.8/cubetools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.4.7
+Version: 0.4.8
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
         
         [CubeAI智立方](https://openi.pcl.ac.cn/OpenI/cubeai) 模型和应用开发常用工具集。
         
         目前主要包括：
         
         - 图像前处理、后处理等常用函数封装。
-        - 通用视频流媒体在线流式AI推理服务组件。
+        - 通用AI流媒体在线推理服务框架。
         - 通用OpenVino模型推理框架（基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装）。
         - 通用ONNX模型推理框架（基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装）。
         - 通用PaddlePaddle模型推理框架（基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装）。
         - 通用MindSporeLite推理框架（基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装）。
         - 通用Pytorch模型推理框架。
         - 基于Gradio的视频流媒体类Python前端服务组件。
         - 基于Gradio的聊天对话类Python前端服务组件。
```

### Comparing `cubetools-0.4.7/cubetools.egg-info/SOURCES.txt` & `cubetools-0.4.8/cubetools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 cubetools/openvino_predict.py
 cubetools/paddle_predict.py
 cubetools/python_chat_frontend.py
 cubetools/python_video_frontend.py
 cubetools/pytorch_predict.py
 cubetools/video_capture.py
 cubetools/video_predict.py
+cubetools/video_predict2.py
 cubetools.egg-info/PKG-INFO
 cubetools.egg-info/SOURCES.txt
 cubetools.egg-info/dependency_links.txt
 cubetools.egg-info/entry_points.txt
 cubetools.egg-info/requires.txt
 cubetools.egg-info/top_level.txt
```

### Comparing `cubetools-0.4.7/setup.py` & `cubetools-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='cubetools',
-    version='0.4.7',
+    version='0.4.8',
     author='cubeai',
     author_email='cubeai@163.com',
     description='CubeAI模型开发常用工具集',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

