# Comparing `tmp/baidu-acu-asr-2.0.3.tar.gz` & `tmp/baidu-acu-asr-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/baidu-acu-asr-2.0.3.tar", last modified: Thu Jan  9 02:40:19 2020, max compression
+gzip compressed data, was "baidu-acu-asr-2.0.4.tar", last modified: Tue Jul 25 04:14:27 2023, max compression
```

## Comparing `baidu-acu-asr-2.0.3.tar` & `baidu-acu-asr-2.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)        0 2020-01-09 02:40:19.000000 baidu-acu-asr-2.0.3/
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)      513 2020-01-09 02:40:19.000000 baidu-acu-asr-2.0.3/PKG-INFO
-drwxr-xr-x   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)        0 2020-01-09 02:40:19.000000 baidu-acu-asr-2.0.3/baidu_acu_asr.egg-info/
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)      513 2020-01-09 02:40:18.000000 baidu-acu-asr-2.0.3/baidu_acu_asr.egg-info/PKG-INFO
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)      563 2020-01-09 02:40:18.000000 baidu-acu-asr-2.0.3/baidu_acu_asr.egg-info/SOURCES.txt
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)       27 2020-01-09 02:40:18.000000 baidu-acu-asr-2.0.3/baidu_acu_asr.egg-info/requires.txt
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)       14 2020-01-09 02:40:18.000000 baidu-acu-asr-2.0.3/baidu_acu_asr.egg-info/top_level.txt
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)        1 2020-01-09 02:40:18.000000 baidu-acu-asr-2.0.3/baidu_acu_asr.egg-info/dependency_links.txt
-drwxr-xr-x   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)        0 2020-01-09 02:40:19.000000 baidu-acu-asr-2.0.3/baidu_acu_asr/
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)    18844 2019-11-20 13:13:16.000000 baidu-acu-asr-2.0.3/baidu_acu_asr/audio_streaming_pb2.py
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)      555 2019-11-13 12:27:16.000000 baidu-acu-asr-2.0.3/baidu_acu_asr/asr_client_factory.py
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)     1367 2019-11-13 12:27:16.000000 baidu-acu-asr-2.0.3/baidu_acu_asr/request_header_validator_interceptor.py
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)       22 2019-11-13 12:27:16.000000 baidu-acu-asr-2.0.3/baidu_acu_asr/__init__.py
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)     2547 2019-11-13 12:27:16.000000 baidu-acu-asr-2.0.3/baidu_acu_asr/generic_client_interceptor.py
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)     1585 2019-11-13 12:27:16.000000 baidu-acu-asr-2.0.3/baidu_acu_asr/header_manipulator_client_interceptor.py
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)     6031 2020-01-06 09:31:01.000000 baidu-acu-asr-2.0.3/baidu_acu_asr/asr_client.py
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)     1518 2019-11-13 12:42:18.000000 baidu-acu-asr-2.0.3/baidu_acu_asr/audio_streaming_pb2_grpc.py
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)     1296 2019-11-13 12:27:16.000000 baidu-acu-asr-2.0.3/baidu_acu_asr/asr_product.py
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)     2938 2019-12-26 03:23:26.000000 baidu-acu-asr-2.0.3/README.md
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)      902 2020-01-09 02:37:48.000000 baidu-acu-asr-2.0.3/setup.py
--rw-r--r--   0 xiashuai01 (2067451715) INTERNAL\Domain Users (672505530)       38 2020-01-09 02:40:19.000000 baidu-acu-asr-2.0.3/setup.cfg
+drwxr-xr-x   0 xiashuai01   (501) staff       (20)        0 2023-07-25 04:14:27.956625 baidu-acu-asr-2.0.4/
+-rw-r--r--   0 xiashuai01   (501) staff       (20)      483 2023-07-25 04:14:27.956695 baidu-acu-asr-2.0.4/PKG-INFO
+-rw-r--r--   0 xiashuai01   (501) staff       (20)     2938 2020-04-23 12:32:18.000000 baidu-acu-asr-2.0.4/README.md
+drwxr-xr-x   0 xiashuai01   (501) staff       (20)        0 2023-07-25 04:14:27.955922 baidu-acu-asr-2.0.4/baidu_acu_asr/
+-rw-r--r--   0 xiashuai01   (501) staff       (20)       22 2020-03-17 10:17:05.000000 baidu-acu-asr-2.0.4/baidu_acu_asr/__init__.py
+-rw-r--r--   0 xiashuai01   (501) staff       (20)     6158 2022-04-18 02:09:20.000000 baidu-acu-asr-2.0.4/baidu_acu_asr/asr_client.py
+-rw-r--r--   0 xiashuai01   (501) staff       (20)      555 2020-03-17 10:17:05.000000 baidu-acu-asr-2.0.4/baidu_acu_asr/asr_client_factory.py
+-rw-r--r--   0 xiashuai01   (501) staff       (20)     1296 2020-03-17 10:17:05.000000 baidu-acu-asr-2.0.4/baidu_acu_asr/asr_product.py
+-rw-r--r--   0 xiashuai01   (501) staff       (20)     3352 2023-07-25 03:55:33.000000 baidu-acu-asr-2.0.4/baidu_acu_asr/audio_streaming_pb2.py
+-rw-r--r--   0 xiashuai01   (501) staff       (20)     2556 2023-07-25 04:13:27.000000 baidu-acu-asr-2.0.4/baidu_acu_asr/audio_streaming_pb2_grpc.py
+-rw-r--r--   0 xiashuai01   (501) staff       (20)     2547 2020-03-17 10:17:05.000000 baidu-acu-asr-2.0.4/baidu_acu_asr/generic_client_interceptor.py
+-rw-r--r--   0 xiashuai01   (501) staff       (20)     1585 2020-03-17 10:17:05.000000 baidu-acu-asr-2.0.4/baidu_acu_asr/header_manipulator_client_interceptor.py
+-rw-r--r--   0 xiashuai01   (501) staff       (20)     1367 2020-03-17 10:17:05.000000 baidu-acu-asr-2.0.4/baidu_acu_asr/request_header_validator_interceptor.py
+drwxr-xr-x   0 xiashuai01   (501) staff       (20)        0 2023-07-25 04:14:27.956516 baidu-acu-asr-2.0.4/baidu_acu_asr.egg-info/
+-rw-r--r--   0 xiashuai01   (501) staff       (20)      483 2023-07-25 04:14:27.000000 baidu-acu-asr-2.0.4/baidu_acu_asr.egg-info/PKG-INFO
+-rw-r--r--   0 xiashuai01   (501) staff       (20)      563 2023-07-25 04:14:27.000000 baidu-acu-asr-2.0.4/baidu_acu_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 xiashuai01   (501) staff       (20)        1 2023-07-25 04:14:27.000000 baidu-acu-asr-2.0.4/baidu_acu_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 xiashuai01   (501) staff       (20)       27 2023-07-25 04:14:27.000000 baidu-acu-asr-2.0.4/baidu_acu_asr.egg-info/requires.txt
+-rw-r--r--   0 xiashuai01   (501) staff       (20)       14 2023-07-25 04:14:27.000000 baidu-acu-asr-2.0.4/baidu_acu_asr.egg-info/top_level.txt
+-rw-r--r--   0 xiashuai01   (501) staff       (20)       38 2023-07-25 04:14:27.956863 baidu-acu-asr-2.0.4/setup.cfg
+-rw-r--r--   0 xiashuai01   (501) staff       (20)      902 2023-07-25 02:15:00.000000 baidu-acu-asr-2.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `baidu-acu-asr-2.0.3/baidu_acu_asr.egg-info/SOURCES.txt` & `baidu-acu-asr-2.0.4/baidu_acu_asr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baidu-acu-asr-2.0.3/baidu_acu_asr/asr_client_factory.py` & `baidu-acu-asr-2.0.4/baidu_acu_asr/asr_client_factory.py`

 * *Files identical despite different names*

### Comparing `baidu-acu-asr-2.0.3/baidu_acu_asr/request_header_validator_interceptor.py` & `baidu-acu-asr-2.0.4/baidu_acu_asr/request_header_validator_interceptor.py`

 * *Files identical despite different names*

### Comparing `baidu-acu-asr-2.0.3/baidu_acu_asr/generic_client_interceptor.py` & `baidu-acu-asr-2.0.4/baidu_acu_asr/generic_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `baidu-acu-asr-2.0.3/baidu_acu_asr/header_manipulator_client_interceptor.py` & `baidu-acu-asr-2.0.4/baidu_acu_asr/header_manipulator_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `baidu-acu-asr-2.0.3/baidu_acu_asr/asr_client.py` & `baidu-acu-asr-2.0.4/baidu_acu_asr/asr_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,16 @@
         if product is not None:
             # 兼容使用product的老版本
             self.request.product_id = product.value[1]
             # 每次发送的音频字节数
             self.send_package_size = int(send_per_seconds * product.value[2] * sample_point_bytes)
         elif product_id == "" or sample_rate == 0:
             raise RuntimeError('product id and sample rate must be set in AsrClient')
+        elif sample_rate != 8000 and sample_rate != 16000:
+            raise RuntimeError('sample rate must be 8000 or 16000')
         else:
             self.request.product_id = product_id
             self.send_package_size = int(send_per_seconds * sample_rate * sample_point_bytes)
         self.request.sample_point_bytes = sample_point_bytes
         # 指定每次发送的音频数据包大小，通常不需要修改
         self.request.send_per_seconds = send_per_seconds
         self.request.sleep_ratio = sleep_ratio
```

### Comparing `baidu-acu-asr-2.0.3/baidu_acu_asr/audio_streaming_pb2_grpc.py` & `baidu-acu-asr-2.0.4/baidu_acu_asr/audio_streaming_pb2_grpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,66 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from . import audio_streaming_pb2 as audio__streaming__pb2
 
 
 class AsrServiceStub(object):
-  # missing associated documentation comment in .proto file
-  pass
+    """Missing associated documentation comment in .proto file."""
 
-  def __init__(self, channel):
-    """Constructor.
+    def __init__(self, channel):
+        """Constructor.
 
-    Args:
-      channel: A grpc.Channel.
-    """
-    self.send = channel.stream_stream(
-        '/com.baidu.acu.pie.AsrService/send',
-        request_serializer=audio__streaming__pb2.AudioFragmentRequest.SerializeToString,
-        response_deserializer=audio__streaming__pb2.AudioFragmentResponse.FromString,
-        )
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.send = channel.stream_stream(
+                '/com.baidu.acu.pie.AsrService/send',
+                request_serializer=audio__streaming__pb2.AudioFragmentRequest.SerializeToString,
+                response_deserializer=audio__streaming__pb2.AudioFragmentResponse.FromString,
+                )
 
 
 class AsrServiceServicer(object):
-  # missing associated documentation comment in .proto file
-  pass
+    """Missing associated documentation comment in .proto file."""
 
-  def send(self, request_iterator, context):
-    # missing associated documentation comment in .proto file
-    pass
-    context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-    context.set_details('Method not implemented!')
-    raise NotImplementedError('Method not implemented!')
+    def send(self, request_iterator, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_AsrServiceServicer_to_server(servicer, server):
-  rpc_method_handlers = {
-      'send': grpc.stream_stream_rpc_method_handler(
-          servicer.send,
-          request_deserializer=audio__streaming__pb2.AudioFragmentRequest.FromString,
-          response_serializer=audio__streaming__pb2.AudioFragmentResponse.SerializeToString,
-      ),
-  }
-  generic_handler = grpc.method_handlers_generic_handler(
-      'com.baidu.acu.pie.AsrService', rpc_method_handlers)
-  server.add_generic_rpc_handlers((generic_handler,))
+    rpc_method_handlers = {
+            'send': grpc.stream_stream_rpc_method_handler(
+                    servicer.send,
+                    request_deserializer=audio__streaming__pb2.AudioFragmentRequest.FromString,
+                    response_serializer=audio__streaming__pb2.AudioFragmentResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'com.baidu.acu.pie.AsrService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class AsrService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def send(request_iterator,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.stream_stream(request_iterator, target, '/com.baidu.acu.pie.AsrService/send',
+            audio__streaming__pb2.AudioFragmentRequest.SerializeToString,
+            audio__streaming__pb2.AudioFragmentResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `baidu-acu-asr-2.0.3/baidu_acu_asr/asr_product.py` & `baidu-acu-asr-2.0.4/baidu_acu_asr/asr_product.py`

 * *Files identical despite different names*

### Comparing `baidu-acu-asr-2.0.3/README.md` & `baidu-acu-asr-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `baidu-acu-asr-2.0.3/setup.py` & `baidu-acu-asr-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # here = os.path.abspath(os.path.dirname(__file__))
 # changes = open(os.path.join(here, 'CHANGES.md')).read()
 # with open('CHANGES.md') as f:
 #     changes = f.read()
 
 setup(
     name="baidu-acu-asr",
-    version="2.0.3",
+    version="2.0.4",
     description="asr grpc client",
     long_description="[https://github.com/baidubce/pie/tree/master/audio-streaming-client-python]" +
                      "(https://github.com/baidubce/pie/tree/master/audio-streaming-client-python)",
     long_description_content_type='text/markdown',
     author="Baidu",
     url="https://github.com/baidubce/pie/tree/master/audio-streaming-client-python-sdk",
     author_email="1908131339@qq.com",
```

