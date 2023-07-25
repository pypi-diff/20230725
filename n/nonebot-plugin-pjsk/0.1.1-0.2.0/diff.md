# Comparing `tmp/nonebot_plugin_pjsk-0.1.1.tar.gz` & `tmp/nonebot_plugin_pjsk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pjsk-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_pjsk-0.2.0.tar", last modified: Tue Jul 25 16:07:35 2023, max compression
```

## Comparing `nonebot_plugin_pjsk-0.1.1.tar` & `nonebot_plugin_pjsk-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     2202 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/README.md
--rw-r--r--   0        0        0     1070 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/LICENSE
--rw-r--r--   0        0        0     1186 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/__init__.py
--rw-r--r--   0        0        0     1581 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/config.py
--rw-r--r--   0        0        0     5014 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/draw.py
--rw-r--r--   0        0        0      951 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/utils.py
--rw-r--r--   0        0        0     1078 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-25 16:07:15.896097 nonebot_plugin_pjsk-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3412 2023-07-25 16:07:15.896097 nonebot_plugin_pjsk-0.2.0/README.md
+-rw-r--r--   0        0        0      765 2023-07-25 16:07:15.964097 nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/__init__.py
+-rw-r--r--   0        0        0     4607 2023-07-25 16:07:15.964097 nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/__main__.py
+-rw-r--r--   0        0        0      695 2023-07-25 16:07:15.964097 nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/config.py
+-rw-r--r--   0        0        0     6410 2023-07-25 16:07:15.964097 nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/draw.py
+-rw-r--r--   0        0        0     3553 2023-07-25 16:07:15.964097 nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/resource.py
+-rw-r--r--   0        0        0     2460 2023-07-25 16:07:15.964097 nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/utils.py
+-rw-r--r--   0        0        0     1086 2023-07-25 16:07:35.972062 nonebot_plugin_pjsk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/LICENSE` & `nonebot_plugin_pjsk-0.2.0/LICENSE`

 * *Files identical despite different names*

