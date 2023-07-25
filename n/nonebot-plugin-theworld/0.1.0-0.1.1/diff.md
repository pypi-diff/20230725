# Comparing `tmp/nonebot-plugin-theworld-0.1.0.tar.gz` & `tmp/nonebot-plugin-theworld-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-theworld-0.1.0.tar", last modified: Tue Jul 25 04:56:48 2023, max compression
+gzip compressed data, was "nonebot-plugin-theworld-0.1.1.tar", last modified: Tue Jul 25 05:07:26 2023, max compression
```

## Comparing `nonebot-plugin-theworld-0.1.0.tar` & `nonebot-plugin-theworld-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1064 2023-07-25 04:56:39.076553 nonebot-plugin-theworld-0.1.0/LICENSE
--rw-r--r--   0        0        0     2537 2023-07-25 04:56:39.076553 nonebot-plugin-theworld-0.1.0/README.md
--rw-r--r--   0        0        0     3205 2023-07-25 04:56:39.076553 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/__init__.py
--rw-r--r--   0        0        0   306038 2023-07-25 04:56:39.076553 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片1.png
--rw-r--r--   0        0        0   346627 2023-07-25 04:56:39.076553 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片2.png
--rw-r--r--   0        0        0   295756 2023-07-25 04:56:39.076553 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片3.png
--rw-r--r--   0        0        0   199862 2023-07-25 04:56:39.076553 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片4.png
--rw-r--r--   0        0        0   413902 2023-07-25 04:56:39.080554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片5.png
--rw-r--r--   0        0        0   327850 2023-07-25 04:56:39.080554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片6.png
--rw-r--r--   0        0        0   344069 2023-07-25 04:56:39.080554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片7.png
--rw-r--r--   0        0        0   527254 2023-07-25 04:56:39.080554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片8.png
--rw-r--r--   0        0        0   156921 2023-07-25 04:56:39.080554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片9.png
--rw-r--r--   0        0        0    97995 2023-07-25 04:56:39.080554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音1.mp3
--rw-r--r--   0        0        0    33360 2023-07-25 04:56:39.080554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音10.mp3
--rw-r--r--   0        0        0   209751 2023-07-25 04:56:39.084554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音11.mp3
--rw-r--r--   0        0        0    63384 2023-07-25 04:56:39.084554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音12.mp3
--rw-r--r--   0        0        0    85902 2023-07-25 04:56:39.084554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音2.mp3
--rw-r--r--   0        0        0    82566 2023-07-25 04:56:39.084554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音3.mp3
--rw-r--r--   0        0        0   158877 2023-07-25 04:56:39.088554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音4.mp3
--rw-r--r--   0        0        0    58797 2023-07-25 04:56:39.088554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音5.mp3
--rw-r--r--   0        0        0    79647 2023-07-25 04:56:39.088554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音6.mp3
--rw-r--r--   0        0        0    69222 2023-07-25 04:56:39.088554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音7.mp3
--rw-r--r--   0        0        0    97161 2023-07-25 04:56:39.088554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音8.mp3
--rw-r--r--   0        0        0    46287 2023-07-25 04:56:39.088554 nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音9.mp3
--rw-r--r--   0        0        0      597 2023-07-25 04:56:39.088554 nonebot-plugin-theworld-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 nonebot-plugin-theworld-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-25 05:07:15.316418 nonebot-plugin-theworld-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2537 2023-07-25 05:07:15.316418 nonebot-plugin-theworld-0.1.1/README.md
+-rw-r--r--   0        0        0     3204 2023-07-25 05:07:15.316418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/__init__.py
+-rw-r--r--   0        0        0   306038 2023-07-25 05:07:15.316418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片1.png
+-rw-r--r--   0        0        0   346627 2023-07-25 05:07:15.320418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片2.png
+-rw-r--r--   0        0        0   295756 2023-07-25 05:07:15.320418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片3.png
+-rw-r--r--   0        0        0   199862 2023-07-25 05:07:15.320418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片4.png
+-rw-r--r--   0        0        0   413902 2023-07-25 05:07:15.320418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片5.png
+-rw-r--r--   0        0        0   327850 2023-07-25 05:07:15.320418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片6.png
+-rw-r--r--   0        0        0   344069 2023-07-25 05:07:15.320418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片7.png
+-rw-r--r--   0        0        0   527254 2023-07-25 05:07:15.324418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片8.png
+-rw-r--r--   0        0        0   156921 2023-07-25 05:07:15.324418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片9.png
+-rw-r--r--   0        0        0    97995 2023-07-25 05:07:15.324418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音1.mp3
+-rw-r--r--   0        0        0    33360 2023-07-25 05:07:15.324418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音10.mp3
+-rw-r--r--   0        0        0   209751 2023-07-25 05:07:15.328418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音11.mp3
+-rw-r--r--   0        0        0    63384 2023-07-25 05:07:15.328418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音12.mp3
+-rw-r--r--   0        0        0    85902 2023-07-25 05:07:15.328418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音2.mp3
+-rw-r--r--   0        0        0    82566 2023-07-25 05:07:15.328418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音3.mp3
+-rw-r--r--   0        0        0   158877 2023-07-25 05:07:15.328418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音4.mp3
+-rw-r--r--   0        0        0    58797 2023-07-25 05:07:15.328418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音5.mp3
+-rw-r--r--   0        0        0    79647 2023-07-25 05:07:15.332418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音6.mp3
+-rw-r--r--   0        0        0    69222 2023-07-25 05:07:15.332418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音7.mp3
+-rw-r--r--   0        0        0    97161 2023-07-25 05:07:15.332418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音8.mp3
+-rw-r--r--   0        0        0    46287 2023-07-25 05:07:15.332418 nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音9.mp3
+-rw-r--r--   0        0        0      597 2023-07-25 05:07:15.332418 nonebot-plugin-theworld-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 nonebot-plugin-theworld-0.1.1/PKG-INFO
```

### Comparing `nonebot-plugin-theworld-0.1.0/LICENSE` & `nonebot-plugin-theworld-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/README.md` & `nonebot-plugin-theworld-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/__init__.py` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 |:-----:|:----:|:----:|:----:|
 | the world/世界/咋瓦鲁多/时间停止 | 否 | 群聊 | 启用全群禁言，持续9秒 |
 | 然后时间开始流动/时间流动/解除时停 | 否 | 群聊 | 关闭全群禁言 |
 | roadroller/泷泽萝拉哒/食我压路机/压路机 | 否 | 群聊 | 播放动画（ |
     """,
     type="application",
     homepage="https://github.com/A-kirami/nonebot-plugin-theworld",
-    supported_adapters={"~.onebot.v11"},
+    supported_adapters={"~onebot.v11"},
 )
 
 RES_PATH = Path(__file__).parent / "resources"
 
 config = Config.parse_obj(get_driver().config)
```

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片1.png` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片1.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片2.png` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片2.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片3.png` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片3.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片4.png` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片4.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片5.png` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片5.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片6.png` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片6.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片7.png` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片7.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片8.png` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片8.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/图片9.png` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/图片9.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音1.mp3` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音1.mp3`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音10.mp3` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音10.mp3`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音11.mp3` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音11.mp3`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音12.mp3` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音12.mp3`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音2.mp3` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音2.mp3`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音3.mp3` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音3.mp3`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音4.mp3` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音4.mp3`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音5.mp3` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音5.mp3`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音6.mp3` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音6.mp3`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音7.mp3` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音7.mp3`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音8.mp3` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音8.mp3`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/nonebot_plugin_theworld/resources/声音9.mp3` & `nonebot-plugin-theworld-0.1.1/nonebot_plugin_theworld/resources/声音9.mp3`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-theworld-0.1.0/pyproject.toml` & `nonebot-plugin-theworld-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-theworld"
-version = "0.1.0"
+version = "0.1.1"
 description = "「ザ・ワールド」ッ！ 時よ止まれ！"
 authors = [
     { name = "Akirami", email = "Akiramiaya@outlook.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.1",
     "nonebot-adapter-onebot>=2.2.3",
```

### Comparing `nonebot-plugin-theworld-0.1.0/PKG-INFO` & `nonebot-plugin-theworld-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-theworld
-Version: 0.1.0
+Version: 0.1.1
 Summary: 「ザ・ワールド」ッ！ 時よ止まれ！
 License: MIT
 Author-email: Akirami <Akiramiaya@outlook.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/A-kirami/nonebot-plugin-theworld
 Project-URL: Repository, https://github.com/A-kirami/nonebot-plugin-theworld
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-theworld Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-theworld Version: 0.1.1 Summary:
 ãã¶ã»ã¯ã¼ã«ãããï¼ æãæ­¢ã¾ãï¼ License: MIT Author-email:
 Akirami
 outlook.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 A-kirami/nonebot-plugin-theworld Project-URL: Repository, https://github.com/A-
 kirami/nonebot-plugin-theworld Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

