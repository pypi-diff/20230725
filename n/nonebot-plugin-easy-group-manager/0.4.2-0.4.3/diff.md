# Comparing `tmp/nonebot_plugin_easy_group_manager-0.4.2.tar.gz` & `tmp/nonebot_plugin_easy_group_manager-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_easy_group_manager-0.4.2.tar", last modified: Tue Jul 25 11:30:49 2023, max compression
+gzip compressed data, was "nonebot_plugin_easy_group_manager-0.4.3.tar", last modified: Tue Jul 25 11:45:02 2023, max compression
```

## Comparing `nonebot_plugin_easy_group_manager-0.4.2.tar` & `nonebot_plugin_easy_group_manager-0.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 11:30:49.768096 nonebot_plugin_easy_group_manager-0.4.2/
--rw-rw-rw-   0        0        0     1088 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     3468 2023-07-25 11:30:49.767096 nonebot_plugin_easy_group_manager-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     2698 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 11:30:49.763007 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager/
--rw-rw-rw-   0        0        0     8004 2023-07-25 11:28:39.000000 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 11:30:49.767096 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/
--rw-rw-rw-   0        0        0     3468 2023-07-25 11:30:49.000000 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-25 11:30:49.000000 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 11:30:49.000000 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-25 11:30:49.000000 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-07-25 11:30:49.000000 nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 11:30:49.768096 nonebot_plugin_easy_group_manager-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     3993 2023-07-25 11:29:50.000000 nonebot_plugin_easy_group_manager-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:45:02.544191 nonebot_plugin_easy_group_manager-0.4.3/
+-rw-rw-rw-   0        0        0     1088 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     3468 2023-07-25 11:45:02.544191 nonebot_plugin_easy_group_manager-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2698 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 11:45:02.539313 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager/
+-rw-rw-rw-   0        0        0     7978 2023-07-25 11:42:37.000000 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:45:02.543216 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/
+-rw-rw-rw-   0        0        0     3468 2023-07-25 11:45:02.000000 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-25 11:45:02.000000 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 11:45:02.000000 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-25 11:45:02.000000 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-07-25 11:45:02.000000 nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:45:02.544191 nonebot_plugin_easy_group_manager-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     3993 2023-07-25 11:44:51.000000 nonebot_plugin_easy_group_manager-0.4.3/setup.py
```

### Comparing `nonebot_plugin_easy_group_manager-0.4.2/LICENSE` & `nonebot_plugin_easy_group_manager-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_easy_group_manager-0.4.2/PKG-INFO` & `nonebot_plugin_easy_group_manager-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_easy_group_manager
-Version: 0.4.2
+Version: 0.4.3
 Summary: 简易群管，管理员设置新方案
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_easy_group_manager-0.4.2/README.md` & `nonebot_plugin_easy_group_manager-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager/__init__.py` & `nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 """响应部分"""
 set_admin = on_command('添加管理员', aliases={'设置管理员'}, permission=SUPERUSER|GROUP_OWNER, priority=2, block=True)
 unset_admin = on_command('取消管理员', permission=SUPERUSER|GROUP_OWNER, priority=2, block=True)
 ban = on_command('禁言',aliases={"口球"}, permission=SUPERUSER|GROUP_OWNER|GROUP_ADMIN, priority=10, block=True)
 unban = on_command('解禁', permission=SUPERUSER|GROUP_OWNER|GROUP_ADMIN, priority=10, block=True)
 kick = on_command('移出', permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER, priority=10, block=True)
 kick_ban = on_command('移出并拉黑', permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER, priority=10, block=True)
-shut = on_command('全员禁言', aliases={'开启全员禁言'}, priority=50, permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER, priority=10, block=True)
-not_shut = on_command('解除全员禁言', aliases={'关闭全员禁言'}, priority=50, permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER, priority=10, block=True)
+shut = on_command('全员禁言', aliases={'开启全员禁言'}, permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER, priority=10, block=True)
+not_shut = on_command('解除全员禁言', aliases={'关闭全员禁言'}, permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER, priority=10, block=True)
 
 
 
 """执行部分"""
 @set_admin.handle()
 async def _(bot: Bot, event: GroupMessageEvent):
     # 获取被操作群员的ID、所在群号、所在群群主ID
```

### Comparing `nonebot_plugin_easy_group_manager-0.4.2/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO` & `nonebot_plugin_easy_group_manager-0.4.3/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-easy-group-manager
-Version: 0.4.2
+Version: 0.4.3
 Summary: 简易群管，管理员设置新方案
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_easy_group_manager-0.4.2/setup.py` & `nonebot_plugin_easy_group_manager-0.4.3/setup.py`

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
-VERSION = '0.4.2'
+VERSION = '0.4.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'nonebot2', 'nonebot-adapter-onebot', 'httpx',
 ]
 
 # What packages are optional?
```

