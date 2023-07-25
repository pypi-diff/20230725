# Comparing `tmp/nonebot_plugin_easy_group_manager-0.3.2.tar.gz` & `tmp/nonebot_plugin_easy_group_manager-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_easy_group_manager-0.3.2.tar", last modified: Tue Jul 11 01:08:24 2023, max compression
+gzip compressed data, was "nonebot_plugin_easy_group_manager-0.4.2.tar", last modified: Tue Jul 25 11:30:49 2023, max compression
```

## Comparing `nonebot_plugin_easy_group_manager-0.3.2.tar` & `nonebot_plugin_easy_group_manager-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 01:08:24.651000 nonebot_plugin_easy_group_manager-0.3.2/
--rw-rw-rw-   0        0        0     1088 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     3468 2023-07-11 01:08:24.649997 nonebot_plugin_easy_group_manager-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2698 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 01:08:24.643487 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager/
--rw-rw-rw-   0        0        0     6946 2023-07-11 01:02:20.000000 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 01:08:24.648991 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/
--rw-rw-rw-   0        0        0     3468 2023-07-11 01:08:24.000000 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-11 01:08:24.000000 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 01:08:24.000000 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-11 01:08:24.000000 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-07-11 01:08:24.000000 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 01:08:24.651000 nonebot_plugin_easy_group_manager-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     3993 2023-07-11 01:07:47.000000 nonebot_plugin_easy_group_manager-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:30:49.768096 nonebot_plugin_easy_group_manager-0.4.2/
+-rw-rw-rw-   0        0        0     1088 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     3468 2023-07-25 11:30:49.767096 nonebot_plugin_easy_group_manager-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2698 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 11:30:49.763007 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager/
+-rw-rw-rw-   0        0        0     8004 2023-07-25 11:28:39.000000 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:30:49.767096 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/
+-rw-rw-rw-   0        0        0     3468 2023-07-25 11:30:49.000000 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-25 11:30:49.000000 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 11:30:49.000000 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-25 11:30:49.000000 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-07-25 11:30:49.000000 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:30:49.768096 nonebot_plugin_easy_group_manager-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     3993 2023-07-25 11:29:50.000000 nonebot_plugin_easy_group_manager-0.4.2/setup.py
```

### Comparing `nonebot_plugin_easy_group_manager-0.3.2/LICENSE` & `nonebot_plugin_easy_group_manager-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_easy_group_manager-0.3.2/PKG-INFO` & `nonebot_plugin_easy_group_manager-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_easy_group_manager
-Version: 0.3.2
+Version: 0.4.2
 Summary: 简易群管，管理员设置新方案
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_easy_group_manager-0.3.2/README.md` & `nonebot_plugin_easy_group_manager-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager/__init__.py` & `nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     usage=("""
 设置管理员 + @somebody: 设置一个管理员
 取消管理员 + @somebody: 取消一个管理员
 禁言/口球 + @somebody + 阿拉伯数字: 禁言某人，单位分钟，需要 BOT 为管理员
 解禁 + @somebody: 解除某人禁言，需要 BOT 为管理员
 移出 + @somebody: 移出某人，需要 BOT 为管理员
 移出并拉黑 + @somebody: 移出并拉黑，需要 BOT 为管理员
+(开启)全员禁言: 开启全员禁言
+解除/关闭全员禁言: 关闭全员禁言
 """
     ),
     extra={
         "author": "zhulinyv <zhulinyv2005@outlook.com>",
         "version": "0.3.1",
     },
 )
@@ -43,14 +45,16 @@
 """响应部分"""
 set_admin = on_command('添加管理员', aliases={'设置管理员'}, permission=SUPERUSER|GROUP_OWNER, priority=2, block=True)
 unset_admin = on_command('取消管理员', permission=SUPERUSER|GROUP_OWNER, priority=2, block=True)
 ban = on_command('禁言',aliases={"口球"}, permission=SUPERUSER|GROUP_OWNER|GROUP_ADMIN, priority=10, block=True)
 unban = on_command('解禁', permission=SUPERUSER|GROUP_OWNER|GROUP_ADMIN, priority=10, block=True)
 kick = on_command('移出', permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER, priority=10, block=True)
 kick_ban = on_command('移出并拉黑', permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER, priority=10, block=True)
+shut = on_command('全员禁言', aliases={'开启全员禁言'}, priority=50, permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER, priority=10, block=True)
+not_shut = on_command('解除全员禁言', aliases={'关闭全员禁言'}, priority=50, permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER, priority=10, block=True)
 
 
 
 """执行部分"""
 @set_admin.handle()
 async def _(bot: Bot, event: GroupMessageEvent):
     # 获取被操作群员的ID、所在群号、所在群群主ID
@@ -142,14 +146,30 @@
         try:
             # reject_add_request=True 阻止再次申请
             await bot.set_group_kick(group_id=gid, user_id=qid, reject_add_request=True)
             await kick.send(f'已移出并拉黑群员{qid}')
         except ActionFailed:
             await kick_ban.send('权限不足捏', at_sender=True)
 
+@shut.handle()
+async def the_world(bot: Bot, event: GroupMessageEvent):
+    try:
+        await bot.set_group_whole_ban(group_id=event.group_id, enable=True)
+        await bot.send_msg(message="已开启全员禁言~", at_sender=True)
+    except:
+        await bot.send_msg(message="权限不足捏~", at_sender=True)
+
+@not_shut.handle()
+async def time_flow(bot: Bot, event: GroupMessageEvent):
+    try:
+        await bot.set_group_whole_ban(group_id=event.group_id, enable=False)
+        await bot.send_msg(message="已关闭全员禁言~", at_sender=True)
+    except:
+        await bot.send_msg(message="权限不足捏~", at_sender=True)
+
 
 
 """一些工具"""
 # 获取被艾特用户 ID列表
 async def get_at(data:str) -> list[int]:
     qq_list = []
     data = json.loads(data)
```

### Comparing `nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO` & `nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-easy-group-manager
-Version: 0.3.2
+Version: 0.4.2
 Summary: 简易群管，管理员设置新方案
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_easy_group_manager-0.3.2/setup.py` & `nonebot_plugin_easy_group_manager-0.4.2/setup.py`

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
-VERSION = '0.3.2'
+VERSION = '0.4.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'nonebot2', 'nonebot-adapter-onebot', 'httpx',
 ]
 
 # What packages are optional?
```

