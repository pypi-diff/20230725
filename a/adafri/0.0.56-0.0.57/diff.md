# Comparing `tmp/adafri-0.0.56.tar.gz` & `tmp/adafri-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.56.tar", last modified: Tue Jul 25 08:24:43 2023, max compression
+gzip compressed data, was "adafri-0.0.57.tar", last modified: Tue Jul 25 19:23:01 2023, max compression
```

## Comparing `adafri-0.0.56.tar` & `adafri-0.0.57.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.496306 adafri-0.0.56/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-25 08:24:43.495640 adafri-0.0.56/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.452807 adafri-0.0.56/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-25 08:24:34.000000 adafri-0.0.56/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.459840 adafri-0.0.56/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.56/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.56/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.56/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.56/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    17295 2023-07-23 10:10:20.000000 adafri-0.0.56/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.461547 adafri-0.0.56/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.56/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.462429 adafri-0.0.56/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.56/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.465507 adafri-0.0.56/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.56/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.56/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.56/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.466189 adafri-0.0.56/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.56/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.467564 adafri-0.0.56/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      226 2023-07-25 08:24:25.000000 adafri-0.0.56/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4421 2023-07-25 08:23:50.000000 adafri-0.0.56/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.468145 adafri-0.0.56/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.56/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.468707 adafri-0.0.56/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.56/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.475359 adafri-0.0.56/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.56/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6761 2023-07-21 06:23:32.000000 adafri-0.0.56/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.56/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16078 2023-07-21 03:05:48.000000 adafri-0.0.56/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.56/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9367 2023-07-25 04:37:18.000000 adafri-0.0.56/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.56/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.479483 adafri-0.0.56/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.56/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.56/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.56/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.482047 adafri-0.0.56/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.56/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.56/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.482840 adafri-0.0.56/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)     7436 2023-07-25 07:52:57.000000 adafri-0.0.56/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.489251 adafri-0.0.56/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.56/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.493228 adafri-0.0.56/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.56/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11474 2023-07-25 07:36:47.000000 adafri-0.0.56/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5919 2023-07-25 07:35:56.000000 adafri-0.0.56/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 08:24:43.455151 adafri-0.0.56/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-25 08:24:43.000000 adafri-0.0.56/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1250 2023-07-25 08:24:43.000000 adafri-0.0.56/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-25 08:24:43.000000 adafri-0.0.56/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-25 08:24:43.000000 adafri-0.0.56/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-25 08:24:43.496544 adafri-0.0.56/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.56/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.113885 adafri-0.0.57/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-25 19:23:01.112996 adafri-0.0.57/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.067333 adafri-0.0.57/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-25 19:22:55.000000 adafri-0.0.57/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.075437 adafri-0.0.57/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.57/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.57/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.57/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.57/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    17295 2023-07-23 10:10:20.000000 adafri-0.0.57/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.076944 adafri-0.0.57/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.57/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.078164 adafri-0.0.57/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.57/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.081760 adafri-0.0.57/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.57/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.57/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.57/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.083049 adafri-0.0.57/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.57/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.084989 adafri-0.0.57/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.57/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-25 19:22:50.000000 adafri-0.0.57/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.085821 adafri-0.0.57/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.57/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.086709 adafri-0.0.57/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.57/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.096736 adafri-0.0.57/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.57/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6761 2023-07-21 06:23:32.000000 adafri-0.0.57/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.57/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16078 2023-07-21 03:05:48.000000 adafri-0.0.57/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.57/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9367 2023-07-25 04:37:18.000000 adafri-0.0.57/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.57/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.100403 adafri-0.0.57/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.57/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.57/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.57/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.102559 adafri-0.0.57/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.57/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.57/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.103534 adafri-0.0.57/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7436 2023-07-25 07:52:57.000000 adafri-0.0.57/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.104659 adafri-0.0.57/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.57/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.111078 adafri-0.0.57/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.57/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11474 2023-07-25 07:36:47.000000 adafri-0.0.57/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5919 2023-07-25 07:35:56.000000 adafri-0.0.57/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 19:23:01.070565 adafri-0.0.57/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-25 19:23:00.000000 adafri-0.0.57/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1250 2023-07-25 19:23:00.000000 adafri-0.0.57/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-25 19:23:00.000000 adafri-0.0.57/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-25 19:23:00.000000 adafri-0.0.57/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-25 19:23:01.114202 adafri-0.0.57/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.57/setup.py
```

### Comparing `adafri-0.0.56/adafri/utils/country.py` & `adafri-0.0.57/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/utils/phone_number.py` & `adafri-0.0.57/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/utils/response.py` & `adafri-0.0.57/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/utils/utils.py` & `adafri-0.0.57/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/account/models/account.py` & `adafri-0.0.57/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/account/models/account_fields.py` & `adafri-0.0.57/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.57/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,39 @@
     try:
         return auth.generate_password_reset_link(email, action_code_settings=ActionCodeSettings(url=url))
     except ValueError as e:
         return None
     except FirebaseError as e:
         return None;  
 
+def get_user_by_uid(uid) -> 'auth.UserRecord':
+    try:
+        return auth.get_user(uid)
+    except ValueError as e:
+        return None;
+    except FirebaseError as e:
+        return None; 
+
+
+def get_user_by_email(email) -> 'auth.UserRecord':
+    try:
+        return auth.get_user_by_email(email)
+    except ValueError as e:
+        return None;
+    except FirebaseError as e:
+        return None; 
+
+def get_user_by_phone_number(phone_number) -> 'auth.UserRecord':
+    try:
+        return auth.get_user_by_phone_number(phone_number)
+    except ValueError as e:
+        return None;
+    except FirebaseError as e:
+        return None; 
+
 def update_firebase_user(uid, **kwargs) -> 'auth.UserRecord':
     """
     Keyword Args:
     display_name: The user's display name (optional). Can be removed by explicitly passing
         auth.DELETE_ATTRIBUTE.
     email: The user's primary email (optional).
     email_verified: A boolean indicating whether or not the user's primary email is
```

### Comparing `adafri-0.0.56/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.57/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.57/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.57/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.57/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.57/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.57/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.57/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.57/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.57/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/base/firebase_collection.py` & `adafri-0.0.57/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/mailing/__init__.py` & `adafri-0.0.57/adafri/v1/mailing/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/user/models/user.py` & `adafri-0.0.57/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri/v1/user/models/user_fields.py` & `adafri-0.0.57/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/adafri.egg-info/SOURCES.txt` & `adafri-0.0.57/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.56/setup.py` & `adafri-0.0.57/setup.py`

 * *Files identical despite different names*

