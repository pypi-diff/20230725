# Comparing `tmp/dynamicadaptor-0.4.5.tar.gz` & `tmp/dynamicadaptor-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicadaptor-0.4.5.tar", max compression
+gzip compressed data, was "dynamicadaptor-0.4.6.tar", max compression
```

## Comparing `dynamicadaptor-0.4.5.tar` & `dynamicadaptor-0.4.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    18431 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/LICENSE
--rw-r--r--   0        0        0    10010 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/README.md
--rw-r--r--   0        0        0     2136 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/AddonCard.py
--rw-r--r--   0        0        0      926 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/Content.py
--rw-r--r--   0        0        0    20217 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/DynamicConversion.py
--rw-r--r--   0        0        0      575 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/Header.py
--rw-r--r--   0        0        0     3882 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/Majors.py
--rw-r--r--   0        0        0      410 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/Message.py
--rw-r--r--   0        0        0      323 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/Repost.py
--rw-r--r--   0        0        0       10 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/__init__.py
--rw-r--r--   0        0        0      500 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/pyproject.toml
--rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 dynamicadaptor-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    18431 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/LICENSE
+-rw-r--r--   0        0        0    10010 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/README.md
+-rw-r--r--   0        0        0     2136 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/AddonCard.py
+-rw-r--r--   0        0        0      926 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/Content.py
+-rw-r--r--   0        0        0    20383 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/DynamicConversion.py
+-rw-r--r--   0        0        0      575 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/Header.py
+-rw-r--r--   0        0        0     3882 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/Majors.py
+-rw-r--r--   0        0        0      410 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/Message.py
+-rw-r--r--   0        0        0      323 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/Repost.py
+-rw-r--r--   0        0        0       10 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/__init__.py
+-rw-r--r--   0        0        0      500 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 dynamicadaptor-0.4.6/PKG-INFO
```

### Comparing `dynamicadaptor-0.4.5/LICENSE` & `dynamicadaptor-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.5/README.md` & `dynamicadaptor-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.5/dynamicadaptor/AddonCard.py` & `dynamicadaptor-0.4.6/dynamicadaptor/AddonCard.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.5/dynamicadaptor/Content.py` & `dynamicadaptor-0.4.6/dynamicadaptor/Content.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.5/dynamicadaptor/DynamicConversion.py` & `dynamicadaptor-0.4.6/dynamicadaptor/DynamicConversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,19 @@
         message: grpc动态转换成Json后的数据
 
     Returns: RenderMessage
 
     """
     message_type = message["cardType"]
     message_id = message["extend"]["dynIdStr"]
-    header = await get_grpc_header(message["modules"][0]["moduleAuthor"])
+    for i in message["modules"]:
+        if i["moduleType"] == "module_author":
+            header = await get_grpc_header(i["moduleAuthor"])
+            break
+    # header = await get_grpc_header(message["modules"][0]["moduleAuthor"])
     
     text = await get_grpc_text(message)
     # print(text)
     major = await get_grpc_major(message)
     additional = await get_grpc_additional(message)
     # print(additional)
     forward = await get_grpc_forward(message)
```

### Comparing `dynamicadaptor-0.4.5/dynamicadaptor/Header.py` & `dynamicadaptor-0.4.6/dynamicadaptor/Header.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.5/dynamicadaptor/Majors.py` & `dynamicadaptor-0.4.6/dynamicadaptor/Majors.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 #     类型          动态类型        示例动态
 #     draw         图片            741262186696933397
 #     archive      视频            739851131027456201
 #     live_rcmd    直播
 #     ugc_season    合集           755703296984875092 
 #     article      专栏            819930757423169558
 #     common     装扮 活动等        551309621391003098/743181895357956118
-#     music       音乐             692040384055869478
+#     music       音乐             819725994851041346
 #     pgc         电影/电视剧等     633983562923638785
 #     medialist   收藏列表          645144864359448578
 #     courses     课程             440646043801479846
 #     live        转发直播          727260760787386403
 #     """
```

### Comparing `dynamicadaptor-0.4.5/PKG-INFO` & `dynamicadaptor-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicadaptor
-Version: 0.4.5
+Version: 0.4.6
 Summary: 
 Author: DMC
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

