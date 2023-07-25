# Comparing `tmp/nonebot_plugin_easy_group_manager-0.4.3.tar.gz` & `tmp/nonebot_plugin_easy_group_manager-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_easy_group_manager-0.4.3.tar", last modified: Tue Jul 25 11:45:02 2023, max compression
+gzip compressed data, was "nonebot_plugin_easy_group_manager-0.4.4.tar", last modified: Tue Jul 25 12:00:08 2023, max compression
```

## Comparing `nonebot_plugin_easy_group_manager-0.4.3.tar` & `nonebot_plugin_easy_group_manager-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 11:45:02.544191 nonebot_plugin_easy_group_manager-0.4.3/
--rw-rw-rw-   0        0        0     1088 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.4.3/LICENSE
--rw-rw-rw-   0        0        0     3468 2023-07-25 11:45:02.544191 nonebot_plugin_easy_group_manager-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     2698 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 11:45:02.539313 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager/
--rw-rw-rw-   0        0        0     7978 2023-07-25 11:42:37.000000 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 11:45:02.543216 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/
--rw-rw-rw-   0        0        0     3468 2023-07-25 11:45:02.000000 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-25 11:45:02.000000 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 11:45:02.000000 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-25 11:45:02.000000 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-07-25 11:45:02.000000 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 11:45:02.544191 nonebot_plugin_easy_group_manager-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     3993 2023-07-25 11:44:51.000000 nonebot_plugin_easy_group_manager-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:00:08.604843 nonebot_plugin_easy_group_manager-0.4.4/
+-rw-rw-rw-   0        0        0     1088 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0     3468 2023-07-25 12:00:08.603837 nonebot_plugin_easy_group_manager-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2698 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 12:00:08.598957 nonebot_plugin_easy_group_manager-0.4.4/nonebot_plugin_easy_group_manager/
+-rw-rw-rw-   0        0        0     7934 2023-07-25 11:58:48.000000 nonebot_plugin_easy_group_manager-0.4.4/nonebot_plugin_easy_group_manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:00:08.602860 nonebot_plugin_easy_group_manager-0.4.4/nonebot_plugin_easy_group_manager.egg-info/
+-rw-rw-rw-   0        0        0     3468 2023-07-25 12:00:08.000000 nonebot_plugin_easy_group_manager-0.4.4/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-25 12:00:08.000000 nonebot_plugin_easy_group_manager-0.4.4/nonebot_plugin_easy_group_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 12:00:08.000000 nonebot_plugin_easy_group_manager-0.4.4/nonebot_plugin_easy_group_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-25 12:00:08.000000 nonebot_plugin_easy_group_manager-0.4.4/nonebot_plugin_easy_group_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-07-25 12:00:08.000000 nonebot_plugin_easy_group_manager-0.4.4/nonebot_plugin_easy_group_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 12:00:08.604843 nonebot_plugin_easy_group_manager-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     3993 2023-07-25 12:00:00.000000 nonebot_plugin_easy_group_manager-0.4.4/setup.py
```

### Comparing `nonebot_plugin_easy_group_manager-0.4.3/LICENSE` & `nonebot_plugin_easy_group_manager-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_easy_group_manager-0.4.3/PKG-INFO` & `nonebot_plugin_easy_group_manager-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_easy_group_manager
-Version: 0.4.3
+Version: 0.4.4
 Summary: 简易群管，管理员设置新方案
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_easy_group_manager-0.4.3/README.md` & `nonebot_plugin_easy_group_manager-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager/__init__.py` & `nonebot_plugin_easy_group_manager-0.4.4/nonebot_plugin_easy_group_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,25 +150,25 @@
         except ActionFailed:
             await kick_ban.send('权限不足捏', at_sender=True)
 
 @shut.handle()
 async def the_world(bot: Bot, event: GroupMessageEvent):
     try:
         await bot.set_group_whole_ban(group_id=event.group_id, enable=True)
-        await bot.send_msg(message="已开启全员禁言~", at_sender=True)
+        await shut.send("已开启全员禁言~", at_sender=True)
     except:
-        await bot.send_msg(message="权限不足捏~", at_sender=True)
+        await shut.send("权限不足捏~", at_sender=True)
 
 @not_shut.handle()
 async def time_flow(bot: Bot, event: GroupMessageEvent):
     try:
         await bot.set_group_whole_ban(group_id=event.group_id, enable=False)
-        await bot.send_msg(message="已关闭全员禁言~", at_sender=True)
+        await shut.send("已关闭全员禁言~", at_sender=True)
     except:
-        await bot.send_msg(message="权限不足捏~", at_sender=True)
+        await shut.send("权限不足捏~", at_sender=True)
 
 
 
 """一些工具"""
 # 获取被艾特用户 ID列表
 async def get_at(data:str) -> list[int]:
     qq_list = []
```

### Comparing `nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO` & `nonebot_plugin_easy_group_manager-0.4.4/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-easy-group-manager
-Version: 0.4.3
+Version: 0.4.4
 Summary: 简易群管，管理员设置新方案
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_easy_group_manager-0.4.3/setup.py` & `nonebot_plugin_easy_group_manager-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'nonebot_plugin_easy_group_manager'
 DESCRIPTION = '简易群管，管理员设置新方案'
 URL = 'https://github.com/zhulinyv/nonebot_plugin_ping'
 EMAIL = 'zhulinyv2005@outlook.com'
 AUTHOR = '(๑•小丫头片子•๑)'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.4.3'
+VERSION = '0.4.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'nonebot2', 'nonebot-adapter-onebot', 'httpx',
 ]
 
 # What packages are optional?
```

