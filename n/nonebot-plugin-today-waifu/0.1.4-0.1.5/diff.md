# Comparing `tmp/nonebot_plugin_today_waifu-0.1.4.tar.gz` & `tmp/nonebot_plugin_today_waifu-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_today_waifu-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_today_waifu-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_today_waifu-0.1.4.tar` & `nonebot_plugin_today_waifu-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1091 2023-04-01 09:24:29.297752 nonebot_plugin_today_waifu-0.1.4/LICENSE
--rw-r--r--   0        0        0    10040 2023-07-23 07:29:18.351544 nonebot_plugin_today_waifu-0.1.4/nonebot_plugin_today_waifu/__init__.py
--rw-r--r--   0        0        0     1098 2023-06-13 18:53:05.116786 nonebot_plugin_today_waifu-0.1.4/nonebot_plugin_today_waifu/config.py
--rw-r--r--   0        0        0     5072 2023-04-01 07:20:39.639921 nonebot_plugin_today_waifu-0.1.4/nonebot_plugin_today_waifu/record.py
--rw-r--r--   0        0        0      639 2023-07-23 07:29:18.346054 nonebot_plugin_today_waifu-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6297 2023-07-23 07:29:18.338081 nonebot_plugin_today_waifu-0.1.4/README.md
--rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 nonebot_plugin_today_waifu-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-01 09:24:29.297752 nonebot_plugin_today_waifu-0.1.5/LICENSE
+-rw-r--r--   0        0        0    10040 2023-07-25 14:54:49.561393 nonebot_plugin_today_waifu-0.1.5/nonebot_plugin_today_waifu/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-25 14:52:39.563410 nonebot_plugin_today_waifu-0.1.5/nonebot_plugin_today_waifu/config.py
+-rw-r--r--   0        0        0     5072 2023-04-01 07:20:39.639921 nonebot_plugin_today_waifu-0.1.5/nonebot_plugin_today_waifu/record.py
+-rw-r--r--   0        0        0      639 2023-07-25 14:54:49.564383 nonebot_plugin_today_waifu-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6377 2023-07-25 14:54:49.563387 nonebot_plugin_today_waifu-0.1.5/README.md
+-rw-r--r--   0        0        0     7100 1970-01-01 00:00:00.000000 nonebot_plugin_today_waifu-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_today_waifu-0.1.4/LICENSE` & `nonebot_plugin_today_waifu-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_today_waifu-0.1.4/nonebot_plugin_today_waifu/__init__.py` & `nonebot_plugin_today_waifu-0.1.5/nonebot_plugin_today_waifu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from nonebot.adapters.onebot.v11.permission import GROUP_OWNER, GROUP_ADMIN
 
 from .config import Config
 from .record import get_group_record, save_group_record, construct_waifu_msg, clear_group_record, \
     construct_change_waifu_msg
 
 __plugin_name__ = '今日老婆'
-__plugin_version__ = '0.1.4'
+__plugin_version__ = '0.1.5'
 __plugin_meta__ = PluginMetadata(
     __plugin_name__,
     "随机抽取群友作为老婆吧！",
     (
         "指令表：\n"
         "▶ 今日老婆\n"
         "  ▷ 范围：群聊\n"
```

### Comparing `nonebot_plugin_today_waifu-0.1.4/nonebot_plugin_today_waifu/config.py` & `nonebot_plugin_today_waifu-0.1.5/nonebot_plugin_today_waifu/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     @validator('today_waifu_record_dir', pre=True)
     def check_path(cls, v) -> Path:
         return Path(v) if v else Path(__file__).parent / 'record'
 
     @validator('today_waifu_ban_id_list', pre=True)
     def check_ban_id(cls, v: List[int]) -> Set[int]:
-        if not isinstance(v, Union[list, set]):
+        if not (isinstance(v, list) or isinstance(v, set)):
             return set()
         return set(map(int, v))
 
     @validator('today_waifu_aliases', pre=True)
     def check_aliases(cls, v: List[str]) -> List[str]:
         if not isinstance(v, list):
             return ['每日老婆', ]
```

### Comparing `nonebot_plugin_today_waifu-0.1.4/nonebot_plugin_today_waifu/record.py` & `nonebot_plugin_today_waifu-0.1.5/nonebot_plugin_today_waifu/record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_today_waifu-0.1.4/pyproject.toml` & `nonebot_plugin_today_waifu-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_today_waifu"
-version = "0.1.4"
+version = "0.1.5"
 description = "Nonebot2插件 可以随机抽取群友作为老婆"
 authors = ["glamorgan9826 <glamorgan9826@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/glamorgan9826/nonebot-plugin-today-waifu"
 repository = "https://github.com/glamorgan9826/nonebot-plugin-today-waifu"
```

### Comparing `nonebot_plugin_today_waifu-0.1.4/README.md` & `nonebot_plugin_today_waifu-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -143,8 +143,9 @@
 ## 📋版本历史
 
 - 0.1.0 初始版本
 - 0.1.1 更新metadata及修复一些bug
 - 0.1.2 修复每次关闭换老婆状态无法保存bug
 - 0.1.3 修改换老婆次数以及是否开启指令允许群主管理员执行。如果想保持原状仅允许主人执行换老婆相关执行则在配置文件中增加项
   `TODAY_WAIFU_SUPERUSER_OPT = true`
-- 0.1.4 指定换老婆次数命令与次数间可以存在空格
+- 0.1.4 指定换老婆次数命令与次数间可以存在空格
+- 0.1.5 修改TODAY_WAIFU_BAN_ID_LIST的验证条件以适应py3.8以下版本
```

#### html2text {}

```diff
@@ -57,8 +57,9 @@
 (https://github.com/SonderXiaoming/dailywife):
 æ¬é¡¹ç®ççµæåæè·¯æ¥æºã - [petpet](https://github.com/noneplugin/
 nonebot-plugin-petpet): æ¬é¡¹ç®è·åç¾¤åå¤´åçåè½ä»£ç æ¥æºã ##
 ðçæ¬åå² - 0.1.0 åå§çæ¬ - 0.1.1 æ´æ°metadataåä¿®å¤ä¸äºbug
 - 0.1.2 ä¿®å¤æ¯æ¬¡å³é­æ¢èå©ç¶ææ æ³ä¿å­bug - 0.1.3
 ä¿®æ¹æ¢èå©æ¬¡æ°ä»¥åæ¯å¦å¼å¯æä»¤åè®¸ç¾¤ä¸»ç®¡çåæ§è¡ãå¦ææ³ä¿æåç¶ä»åè®¸ä¸»äººæ§è¡æ¢èå©ç¸å³æ§è¡åå¨éç½®æä»¶ä¸­å¢å é¡¹
 `TODAY_WAIFU_SUPERUSER_OPT = true` - 0.1.4
-æå®æ¢èå©æ¬¡æ°å½ä»¤ä¸æ¬¡æ°é´å¯ä»¥å­å¨ç©ºæ ¼
+æå®æ¢èå©æ¬¡æ°å½ä»¤ä¸æ¬¡æ°é´å¯ä»¥å­å¨ç©ºæ ¼ - 0.1.5
+ä¿®æ¹TODAY_WAIFU_BAN_ID_LISTçéªè¯æ¡ä»¶ä»¥éåºpy3.8ä»¥ä¸çæ¬
```

### Comparing `nonebot_plugin_today_waifu-0.1.4/PKG-INFO` & `nonebot_plugin_today_waifu-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-today-waifu
-Version: 0.1.4
+Version: 0.1.5
 Summary: Nonebot2插件 可以随机抽取群友作为老婆
 Home-page: https://github.com/glamorgan9826/nonebot-plugin-today-waifu
 License: MIT
 Author: glamorgan9826
 Author-email: glamorgan9826@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -165,7 +165,8 @@
 
 - 0.1.0 初始版本
 - 0.1.1 更新metadata及修复一些bug
 - 0.1.2 修复每次关闭换老婆状态无法保存bug
 - 0.1.3 修改换老婆次数以及是否开启指令允许群主管理员执行。如果想保持原状仅允许主人执行换老婆相关执行则在配置文件中增加项
   `TODAY_WAIFU_SUPERUSER_OPT = true`
 - 0.1.4 指定换老婆次数命令与次数间可以存在空格
+- 0.1.5 修改TODAY_WAIFU_BAN_ID_LIST的验证条件以适应py3.8以下版本
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-today-waifu Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-today-waifu Version: 0.1.5 Summary:
 Nonebot2æä»¶ å¯ä»¥éæºæ½åç¾¤åä½ä¸ºèå© Home-page: https://
 github.com/glamorgan9826/nonebot-plugin-today-waifu License: MIT Author:
 glamorgan9826 Author-email: glamorgan9826@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -69,8 +69,9 @@
 (https://github.com/SonderXiaoming/dailywife):
 æ¬é¡¹ç®ççµæåæè·¯æ¥æºã - [petpet](https://github.com/noneplugin/
 nonebot-plugin-petpet): æ¬é¡¹ç®è·åç¾¤åå¤´åçåè½ä»£ç æ¥æºã ##
 ðçæ¬åå² - 0.1.0 åå§çæ¬ - 0.1.1 æ´æ°metadataåä¿®å¤ä¸äºbug
 - 0.1.2 ä¿®å¤æ¯æ¬¡å³é­æ¢èå©ç¶ææ æ³ä¿å­bug - 0.1.3
 ä¿®æ¹æ¢èå©æ¬¡æ°ä»¥åæ¯å¦å¼å¯æä»¤åè®¸ç¾¤ä¸»ç®¡çåæ§è¡ãå¦ææ³ä¿æåç¶ä»åè®¸ä¸»äººæ§è¡æ¢èå©ç¸å³æ§è¡åå¨éç½®æä»¶ä¸­å¢å é¡¹
 `TODAY_WAIFU_SUPERUSER_OPT = true` - 0.1.4
-æå®æ¢èå©æ¬¡æ°å½ä»¤ä¸æ¬¡æ°é´å¯ä»¥å­å¨ç©ºæ ¼
+æå®æ¢èå©æ¬¡æ°å½ä»¤ä¸æ¬¡æ°é´å¯ä»¥å­å¨ç©ºæ ¼ - 0.1.5
+ä¿®æ¹TODAY_WAIFU_BAN_ID_LISTçéªè¯æ¡ä»¶ä»¥éåºpy3.8ä»¥ä¸çæ¬
```

