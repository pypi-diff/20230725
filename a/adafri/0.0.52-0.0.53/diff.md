# Comparing `tmp/adafri-0.0.52.tar.gz` & `tmp/adafri-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.52.tar", last modified: Sun Jul 23 10:33:45 2023, max compression
+gzip compressed data, was "adafri-0.0.53.tar", last modified: Tue Jul 25 04:37:32 2023, max compression
```

## Comparing `adafri-0.0.52.tar` & `adafri-0.0.53.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.758704 adafri-0.0.52/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-23 10:33:45.758228 adafri-0.0.52/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.721979 adafri-0.0.52/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-23 10:33:41.000000 adafri-0.0.52/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.728660 adafri-0.0.52/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.52/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.52/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.52/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.52/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    17295 2023-07-23 10:10:20.000000 adafri-0.0.52/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.730135 adafri-0.0.52/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.52/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.730978 adafri-0.0.52/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.52/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.733562 adafri-0.0.52/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.52/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.52/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.52/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.734412 adafri-0.0.52/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.52/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.735618 adafri-0.0.52/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-23 10:31:50.000000 adafri-0.0.52/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1813 2023-07-23 10:31:46.000000 adafri-0.0.52/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.736151 adafri-0.0.52/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.52/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.736699 adafri-0.0.52/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.52/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.745501 adafri-0.0.52/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.52/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6761 2023-07-21 06:23:32.000000 adafri-0.0.52/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.52/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16078 2023-07-21 03:05:48.000000 adafri-0.0.52/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.52/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9363 2023-07-21 03:03:35.000000 adafri-0.0.52/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.52/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.749980 adafri-0.0.52/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.52/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.52/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.52/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.752689 adafri-0.0.52/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.52/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.52/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.753506 adafri-0.0.52/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.52/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.756543 adafri-0.0.52/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.52/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11424 2023-07-23 10:33:30.000000 adafri-0.0.52/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5448 2023-07-23 10:23:31.000000 adafri-0.0.52/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-23 10:33:45.724222 adafri-0.0.52/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-23 10:33:45.000000 adafri-0.0.52/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1220 2023-07-23 10:33:45.000000 adafri-0.0.52/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-23 10:33:45.000000 adafri-0.0.52/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-23 10:33:45.000000 adafri-0.0.52/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-23 10:33:45.758940 adafri-0.0.52/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.52/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.772229 adafri-0.0.53/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-25 04:37:32.771702 adafri-0.0.53/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.701239 adafri-0.0.53/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-25 04:37:28.000000 adafri-0.0.53/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.713627 adafri-0.0.53/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.53/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.53/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.53/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.53/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    17295 2023-07-23 10:10:20.000000 adafri-0.0.53/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.714859 adafri-0.0.53/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.53/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.715910 adafri-0.0.53/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.53/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.719131 adafri-0.0.53/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.53/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.53/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.53/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.720291 adafri-0.0.53/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.53/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.722156 adafri-0.0.53/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-23 10:31:50.000000 adafri-0.0.53/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1813 2023-07-23 10:31:46.000000 adafri-0.0.53/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.723257 adafri-0.0.53/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.53/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.723766 adafri-0.0.53/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.53/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.736031 adafri-0.0.53/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.53/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6761 2023-07-21 06:23:32.000000 adafri-0.0.53/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.53/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16078 2023-07-21 03:05:48.000000 adafri-0.0.53/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.53/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9367 2023-07-25 04:37:18.000000 adafri-0.0.53/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.53/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.742900 adafri-0.0.53/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.53/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.53/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.53/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.747456 adafri-0.0.53/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.53/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.53/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.753692 adafri-0.0.53/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.53/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.770396 adafri-0.0.53/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.53/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11424 2023-07-23 10:33:30.000000 adafri-0.0.53/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5448 2023-07-23 10:23:31.000000 adafri-0.0.53/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-25 04:37:32.703864 adafri-0.0.53/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-25 04:37:32.000000 adafri-0.0.53/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1220 2023-07-25 04:37:32.000000 adafri-0.0.53/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-25 04:37:32.000000 adafri-0.0.53/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-25 04:37:32.000000 adafri-0.0.53/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-25 04:37:32.772505 adafri-0.0.53/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.53/setup.py
```

### Comparing `adafri-0.0.52/adafri/utils/country.py` & `adafri-0.0.53/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/utils/phone_number.py` & `adafri-0.0.53/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/utils/response.py` & `adafri-0.0.53/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/utils/utils.py` & `adafri-0.0.53/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/account/models/account.py` & `adafri-0.0.53/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/account/models/account_fields.py` & `adafri-0.0.53/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.53/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.53/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.53/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.53/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.53/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.53/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.53/adafri/v1/auth/oauth/models/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,16 +91,16 @@
         model = {**token, "client_id": request.client.client_id, "uid": request.user.uid, "revoked": False}
         if 'type' not in model:
             model['type'] = 'app_token'
         token_generate = OAuthToken.generate(**model);
         if token_generate.status == ResponseStatus.ERROR:
             return token_generate
         docRef = OAuthToken(token_generate.data.to_json()).document_reference();
-        if docRef.get().exists:
-            return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Location with name {token_generate.data.id} already exist","INVALID_REQUEST", 1));
+        # if docRef.get().exists:
+        #     return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Location with name {token_generate.data.id} already exist","INVALID_REQUEST", 1));
         
         token_model: OAuthToken = token_generate.data;
         docRef.set({**token_model.to_json(), "createdAt": getTimestamp()}, merge=True);
         created_token = token_model.getOAuthToken()
         return ApiResponse(ResponseStatus.OK, StatusCode.status_200, created_token.to_json(), None);
     
     def update(self, data):
```

### Comparing `adafri-0.0.52/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.53/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.53/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.53/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/base/firebase_collection.py` & `adafri-0.0.53/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/user/models/user.py` & `adafri-0.0.53/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri/v1/user/models/user_fields.py` & `adafri-0.0.53/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/adafri.egg-info/SOURCES.txt` & `adafri-0.0.53/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.52/setup.py` & `adafri-0.0.53/setup.py`

 * *Files identical despite different names*

