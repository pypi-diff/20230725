# Comparing `tmp/nonebot_plugin_gshisbanner-0.6.0.tar.gz` & `tmp/nonebot_plugin_gshisbanner-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gshisbanner-0.6.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_gshisbanner-0.6.1.tar", max compression
```

## Comparing `nonebot_plugin_gshisbanner-0.6.0.tar` & `nonebot_plugin_gshisbanner-0.6.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/LICENSE
--rw-r--r--   0        0        0     5510 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/README.md
--rw-r--r--   0        0        0      595 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/__init__.py
--rw-r--r--   0        0        0     1030 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/alias.py
--rw-r--r--   0        0        0      427 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/api.py
--rw-r--r--   0        0        0      300 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/config.py
--rw-r--r--   0        0        0     3621 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/deal.py
--rw-r--r--   0        0        0     1231 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/deal_json.py
--rw-r--r--   0        0        0     4979 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/main.py
--rw-r--r--   0        0        0     2640 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/send.py
--rw-r--r--   0        0        0      600 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6202 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-25 17:41:26.067110 nonebot_plugin_gshisbanner-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5510 2023-07-25 17:41:26.067110 nonebot_plugin_gshisbanner-0.6.1/README.md
+-rw-r--r--   0        0        0      581 2023-07-25 17:41:26.067110 nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/__init__.py
+-rw-r--r--   0        0        0     1030 2023-07-25 17:41:26.067110 nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/alias.py
+-rw-r--r--   0        0        0      427 2023-07-25 17:41:26.067110 nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/api.py
+-rw-r--r--   0        0        0      300 2023-07-25 17:41:26.067110 nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/config.py
+-rw-r--r--   0        0        0     3637 2023-07-25 17:41:26.067110 nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/deal.py
+-rw-r--r--   0        0        0     1231 2023-07-25 17:41:26.067110 nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/deal_json.py
+-rw-r--r--   0        0        0     5045 2023-07-25 17:41:26.067110 nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/main.py
+-rw-r--r--   0        0        0     2640 2023-07-25 17:41:26.071110 nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/send.py
+-rw-r--r--   0        0        0      600 2023-07-25 17:41:26.071110 nonebot_plugin_gshisbanner-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6202 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.6.1/PKG-INFO
```

### Comparing `nonebot_plugin_gshisbanner-0.6.0/LICENSE` & `nonebot_plugin_gshisbanner-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.6.0/README.md` & `nonebot_plugin_gshisbanner-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/__init__.py` & `nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from nonebot.plugin import PluginMetadata
 
-from .config import plugin_config
+from .config import Config
 from .main import *  # noqa: F403
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 __plugin_meta__ = PluginMetadata(
     name="gshisbanner",
     description="这是一个在机器人上获取原神历史卡池的插件",
     usage="XX历史卡池,XX卡池(版本)，详细查看本仓库readme",
     type="application",
     homepage="https://github.com/forchannot/nonebot-plugin-gshisbanner",
-    config=plugin_config,
+    config=Config,
     supported_adapters={"~onebot.v11"},
     extra={
         "author": "forchannot",
         "version": __version__,
     },
 )
```

### Comparing `nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/alias.py` & `nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/alias.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/deal.py` & `nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/deal.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 ) -> List[Dict[str, Union[str, List[str]]]]:
     """
     :param version: 版本号
     :param is_all: 是否获取全部卡池
     :return: 获取到的历史卡池数据
     """
     # 获取所有卡池信息
-    json = await get_info_from_url(True) + await get_info_from_url(False)
+    json = await get_info_from_url(True) + await get_info_from_url(False)  # type: ignore
     # 卡池类型列表
     type_list = [
         "five_character",
         "four_character",
         "five_weapon",
         "four_weapon",
     ]
```

### Comparing `nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/deal_json.py` & `nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/deal_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/main.py` & `nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 @old_gacha.handle()
 async def _(
     bot: Bot,
     event: Union[GroupMessageEvent, PrivateMessageEvent],
     key: str = Keyword(),  # noqa: B008
 ):
-    name, length = event.get_plaintext().split(key)
+    name, length = event.get_plaintext().split(key, 1)
     name = delete_command_start(name)
     if name in ["刷新", "更新"]:
         return
     if length and not length.isdigit():
         return
     real_name, real_type = find_name(name)
     if real_name is None or real_type not in ["角色", "武器"]:
@@ -68,15 +68,15 @@
 
 @version_gacha.handle()
 async def _(
     bot: Bot,
     event: Union[GroupMessageEvent, PrivateMessageEvent],
     key: str = Keyword(),  # noqa: B008
 ):
-    version, upordown = event.get_plaintext().split(key)
+    version, upordown = event.get_plaintext().split(key, 1)
     version = delete_command_start(version)
     if version in ["刷新", "更新"]:
         return
     if upordown and not (
         upordown.isdigit() and all(part.isdigit() for part in version.split("."))
     ):
         return
@@ -88,17 +88,17 @@
 
 
 @refresh.handle()
 async def _(
     event: Union[GroupMessageEvent, PrivateMessageEvent],
     key: str = Keyword(),  # noqa: B008
 ):
-    args = event.get_plaintext().split(key)
-    _arg = delete_command_start(args[0])
-    if _arg:
+    args = event.get_plaintext().split(key, 1)
+    if _arg := delete_command_start(args[0]):
+        # 去除掉命令开头如果仍然有内容则不处理
         return
     choose = args[1]
     if choose in ["历史卡池", "历史up", "卡池", "up"]:
         for i in ["character", "weapon"]:
             url = f"https://{plugin_config.gshisbanner_json_url}/{i}.json"
             path = gacha_info_path / f"{i}.json"
             result = await load_json_from_url(url, path, True)
```

### Comparing `nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/send.py` & `nonebot_plugin_gshisbanner-0.6.1/nonebot_plugin_gshisbanner/send.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.6.0/pyproject.toml` & `nonebot_plugin_gshisbanner-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gshisbanner"
-version = "0.6.0"
+version = "0.6.1"
 description = "Nonebot2查询原神历史卡池小插件"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_gshisbanner"}]
```

### Comparing `nonebot_plugin_gshisbanner-0.6.0/PKG-INFO` & `nonebot_plugin_gshisbanner-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gshisbanner
-Version: 0.6.0
+Version: 0.6.1
 Summary: Nonebot2查询原神历史卡池小插件
 License: MIT
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.6.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.6.1 Summary:
 Nonebot2æ¥è¯¢åç¥åå²å¡æ± å°æä»¶ License: MIT Author: forchannot
 Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-adapter-onebot
```

