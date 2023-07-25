# Comparing `tmp/nonebot-plugin-sendmsg-by-bots-0.0.1.tar.gz` & `tmp/nonebot-plugin-sendmsg-by-bots-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sendmsg-by-bots-0.0.1.tar", last modified: Tue Jul 25 13:23:22 2023, max compression
+gzip compressed data, was "nonebot-plugin-sendmsg-by-bots-0.0.1rc1.tar", last modified: Tue Jul 25 10:25:13 2023, max compression
```

## Comparing `nonebot-plugin-sendmsg-by-bots-0.0.1.tar` & `nonebot-plugin-sendmsg-by-bots-0.0.1rc1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1779 2023-07-25 13:23:10.765405 nonebot-plugin-sendmsg-by-bots-0.0.1/README.md
--rw-r--r--   0        0        0     1046 2023-07-25 13:23:10.765405 nonebot-plugin-sendmsg-by-bots-0.0.1/nonebot_plugin_sendmsg_by_bots/__init__.py
--rw-r--r--   0        0        0      336 2023-07-25 13:23:10.765405 nonebot-plugin-sendmsg-by-bots-0.0.1/nonebot_plugin_sendmsg_by_bots/config.py
--rw-r--r--   0        0        0     2284 2023-07-25 13:23:10.765405 nonebot-plugin-sendmsg-by-bots-0.0.1/nonebot_plugin_sendmsg_by_bots/tools.py
--rw-r--r--   0        0        0      575 2023-07-25 13:23:10.765405 nonebot-plugin-sendmsg-by-bots-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 nonebot-plugin-sendmsg-by-bots-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3764 2023-07-25 10:24:55.659386 nonebot-plugin-sendmsg-by-bots-0.0.1rc1/README.md
+-rw-r--r--   0        0        0        0 2023-07-25 10:24:55.659386 nonebot-plugin-sendmsg-by-bots-0.0.1rc1/nonebot_plugin_sendmsg_by_bots/__init__.py
+-rw-r--r--   0        0        0      296 2023-07-25 10:24:55.659386 nonebot-plugin-sendmsg-by-bots-0.0.1rc1/nonebot_plugin_sendmsg_by_bots/tools.py
+-rw-r--r--   0        0        0      578 2023-07-25 10:24:55.659386 nonebot-plugin-sendmsg-by-bots-0.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 nonebot-plugin-sendmsg-by-bots-0.0.1rc1/PKG-INFO
```

### Comparing `nonebot-plugin-sendmsg-by-bots-0.0.1/pyproject.toml` & `nonebot-plugin-sendmsg-by-bots-0.0.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-sendmsg-by-bots"
-version = "0.0.1"
+version = "0.0.1rc1"
 description = "a send msg tools"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

