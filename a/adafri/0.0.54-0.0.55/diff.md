# Comparing `tmp/adafri-0.0.54.tar.gz` & `tmp/adafri-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.54.tar", last modified: Tue Jul 25 07:03:52 2023, max compression
+gzip compressed data, was "adafri-0.0.55.tar", last modified: Tue Jul 25 07:53:10 2023, max compression
```

## Comparing `adafri-0.0.54.tar` & `adafri-0.0.55.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.416978 adafri-0.0.54/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-25 07:03:52.416578 adafri-0.0.54/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.380012 adafri-0.0.54/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-25 07:03:43.000000 adafri-0.0.54/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.391169 adafri-0.0.54/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.54/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.54/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.54/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.54/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    17295 2023-07-23 10:10:20.000000 adafri-0.0.54/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.392548 adafri-0.0.54/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.54/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.393596 adafri-0.0.54/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.54/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.396649 adafri-0.0.54/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.54/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.54/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.54/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.397267 adafri-0.0.54/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.54/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.398595 adafri-0.0.54/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      112 2023-07-25 07:03:28.000000 adafri-0.0.54/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2400 2023-07-25 07:03:20.000000 adafri-0.0.54/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.399245 adafri-0.0.54/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.54/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.399667 adafri-0.0.54/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.54/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.405759 adafri-0.0.54/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.54/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6761 2023-07-21 06:23:32.000000 adafri-0.0.54/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.54/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16078 2023-07-21 03:05:48.000000 adafri-0.0.54/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.54/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9367 2023-07-25 04:37:18.000000 adafri-0.0.54/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.54/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.409096 adafri-0.0.54/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.54/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.54/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.54/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.411285 adafri-0.0.54/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.54/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.54/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.412310 adafri-0.0.54/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.54/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.415550 adafri-0.0.54/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.54/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11424 2023-07-23 10:33:30.000000 adafri-0.0.54/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5448 2023-07-23 10:23:31.000000 adafri-0.0.54/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:03:52.383594 adafri-0.0.54/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-25 07:03:52.000000 adafri-0.0.54/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1220 2023-07-25 07:03:52.000000 adafri-0.0.54/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-25 07:03:52.000000 adafri-0.0.54/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-25 07:03:52.000000 adafri-0.0.54/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-25 07:03:52.417205 adafri-0.0.54/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.54/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.673731 adafri-0.0.55/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-25 07:53:10.673427 adafri-0.0.55/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.641818 adafri-0.0.55/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-25 07:53:05.000000 adafri-0.0.55/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.649696 adafri-0.0.55/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.55/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.55/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.55/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.55/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    17295 2023-07-23 10:10:20.000000 adafri-0.0.55/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.650873 adafri-0.0.55/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.55/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.651888 adafri-0.0.55/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.55/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.654773 adafri-0.0.55/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.55/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.55/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.55/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.655539 adafri-0.0.55/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.55/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.657245 adafri-0.0.55/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      112 2023-07-25 07:03:28.000000 adafri-0.0.55/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2400 2023-07-25 07:03:20.000000 adafri-0.0.55/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.658639 adafri-0.0.55/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.55/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.659024 adafri-0.0.55/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.55/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.664906 adafri-0.0.55/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.55/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6761 2023-07-21 06:23:32.000000 adafri-0.0.55/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.55/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16078 2023-07-21 03:05:48.000000 adafri-0.0.55/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.55/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9367 2023-07-25 04:37:18.000000 adafri-0.0.55/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.55/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.667631 adafri-0.0.55/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.55/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.55/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.55/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.669611 adafri-0.0.55/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.55/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.55/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.670117 adafri-0.0.55/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7436 2023-07-25 07:52:57.000000 adafri-0.0.55/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.670537 adafri-0.0.55/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.55/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.672668 adafri-0.0.55/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.55/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11474 2023-07-25 07:36:47.000000 adafri-0.0.55/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5919 2023-07-25 07:35:56.000000 adafri-0.0.55/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 07:53:10.644242 adafri-0.0.55/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-25 07:53:10.000000 adafri-0.0.55/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1250 2023-07-25 07:53:10.000000 adafri-0.0.55/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-25 07:53:10.000000 adafri-0.0.55/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-25 07:53:10.000000 adafri-0.0.55/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-25 07:53:10.673858 adafri-0.0.55/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.55/setup.py
```

### Comparing `adafri-0.0.54/adafri/utils/country.py` & `adafri-0.0.55/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/utils/phone_number.py` & `adafri-0.0.55/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/utils/response.py` & `adafri-0.0.55/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/utils/utils.py` & `adafri-0.0.55/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/account/models/account.py` & `adafri-0.0.55/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/account/models/account_fields.py` & `adafri-0.0.55/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.55/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.55/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.55/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.55/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.55/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.55/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.55/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.55/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.55/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.55/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/base/firebase_collection.py` & `adafri-0.0.55/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.54/adafri/v1/user/models/user.py` & `adafri-0.0.55/adafri/v1/user/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,14 +166,16 @@
     showPushToken: bool
     telephone: str
     token: List[str]
     uid: str
     user_type: str
     password: str
     provider: str
+    status: str
+    _emailValidationSendDate: str
     
     def __init__(self, user=None, **kwargs):
         (cls_object, keys, data_args) = init_class_kwargs(self, user, STANDARD_FIELDS, UserFieldProps, USERS_COLLECTION, ['id','uid'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
             setattr(self, key, cls_object[key]);
```

### Comparing `adafri-0.0.54/adafri/v1/user/models/user_fields.py` & `adafri-0.0.55/adafri/v1/user/models/user_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     token = 'token';
     deviceInfo = 'deviceInfo';
     phoneInfo = 'phoneInfo';
     country = 'country';
     showPushToken = 'showPushToken'
     authorizedPush = 'authorizedPush';
     hasApprouvedPolicy = 'hasApprouvedPolicy';
+    _emailValidationSendDate = 'emailValidationSendDate'
+    status = 'status'
 
     @staticmethod
     def keys():
         return DictUtils.get_keys(UserFieldProps);
 
     @staticmethod
     def filtered_keys(field, condition=True):
@@ -206,12 +208,31 @@
         "type": dict,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": False,
         "default_value": {},
         "pickable": True,
-    }   
+    },
+    UserFields.status:{
+    "type": str,
+    "required": False,
+    "mutable": True,
+    "editable": True,
+    "interactive": False,
+    "default_value": {},
+    "pickable": True,
+    },
+     UserFields._emailValidationSendDate:{
+    "type": str,
+    "required": False,
+    "mutable": True,
+    "editable": True,
+    "interactive": False,
+    "default_value": {},
+    "pickable": True,
+    } 
+
 
 }
 
 STANDARD_FIELDS = UserFields.filtered_keys('pickable', True)
```

### Comparing `adafri-0.0.54/adafri.egg-info/SOURCES.txt` & `adafri-0.0.55/adafri.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,11 +27,12 @@
 adafri/v1/auth/oauth/models/token.py
 adafri/v1/auth/oauth/models/token_fields.py
 adafri/v1/auth/oauth/server/__init__.py
 adafri/v1/auth/oauth/server/oidc_server.py
 adafri/v1/auth/oauth/server/server.py
 adafri/v1/base/__init__.py
 adafri/v1/base/firebase_collection.py
+adafri/v1/mailing/__init__.py
 adafri/v1/user/__init__.py
 adafri/v1/user/models/__init__.py
 adafri/v1/user/models/user.py
 adafri/v1/user/models/user_fields.py
```

### Comparing `adafri-0.0.54/setup.py` & `adafri-0.0.55/setup.py`

 * *Files identical despite different names*

