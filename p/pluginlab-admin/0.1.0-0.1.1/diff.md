# Comparing `tmp/pluginlab_admin-0.1.0.tar.gz` & `tmp/pluginlab_admin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluginlab_admin-0.1.0.tar", last modified: Mon Jul 24 21:03:53 2023, max compression
+gzip compressed data, was "pluginlab_admin-0.1.1.tar", last modified: Tue Jul 25 15:12:46 2023, max compression
```

## Comparing `pluginlab_admin-0.1.0.tar` & `pluginlab_admin-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-24 21:03:53.163233 pluginlab_admin-0.1.0/
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       18 2023-07-23 16:14:55.000000 pluginlab_admin-0.1.0/MANIFEST.in
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      140 2023-07-24 21:03:53.163112 pluginlab_admin-0.1.0/PKG-INFO
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)     5522 2023-07-24 20:58:53.000000 pluginlab_admin-0.1.0/README.md
-drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-24 21:03:53.162342 pluginlab_admin-0.1.0/pluginlab_admin/
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       66 2023-07-23 15:50:42.000000 pluginlab_admin-0.1.0/pluginlab_admin/__init__.py
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      909 2023-07-23 14:10:44.000000 pluginlab_admin-0.1.0/pluginlab_admin/app.py
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)     6337 2023-07-23 14:10:40.000000 pluginlab_admin-0.1.0/pluginlab_admin/auth.py
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)     1646 2023-07-24 20:49:47.000000 pluginlab_admin-0.1.0/pluginlab_admin/token_verifier.py
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      894 2023-07-23 13:09:00.000000 pluginlab_admin-0.1.0/pluginlab_admin/webhook.py
-drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-24 21:03:53.162945 pluginlab_admin-0.1.0/pluginlab_admin.egg-info/
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      140 2023-07-24 21:03:53.000000 pluginlab_admin-0.1.0/pluginlab_admin.egg-info/PKG-INFO
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      360 2023-07-24 21:03:53.000000 pluginlab_admin-0.1.0/pluginlab_admin.egg-info/SOURCES.txt
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)        1 2023-07-24 21:03:53.000000 pluginlab_admin-0.1.0/pluginlab_admin.egg-info/dependency_links.txt
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       52 2023-07-24 21:03:53.000000 pluginlab_admin-0.1.0/pluginlab_admin.egg-info/requires.txt
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       16 2023-07-24 21:03:53.000000 pluginlab_admin-0.1.0/pluginlab_admin.egg-info/top_level.txt
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       38 2023-07-24 21:03:53.163280 pluginlab_admin-0.1.0/setup.cfg
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      267 2023-07-24 21:03:22.000000 pluginlab_admin-0.1.0/setup.py
+drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-25 15:12:46.872781 pluginlab_admin-0.1.1/
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       18 2023-07-23 16:14:55.000000 pluginlab_admin-0.1.1/MANIFEST.in
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      140 2023-07-25 15:12:46.872662 pluginlab_admin-0.1.1/PKG-INFO
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)     5518 2023-07-25 14:55:56.000000 pluginlab_admin-0.1.1/README.md
+drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-25 15:12:46.871899 pluginlab_admin-0.1.1/pluginlab_admin/
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       66 2023-07-23 15:50:42.000000 pluginlab_admin-0.1.1/pluginlab_admin/__init__.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      895 2023-07-25 15:12:21.000000 pluginlab_admin-0.1.1/pluginlab_admin/app.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)     6337 2023-07-25 15:11:40.000000 pluginlab_admin-0.1.1/pluginlab_admin/auth.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)     1646 2023-07-24 20:49:47.000000 pluginlab_admin-0.1.1/pluginlab_admin/token_verifier.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      894 2023-07-23 13:09:00.000000 pluginlab_admin-0.1.1/pluginlab_admin/webhook.py
+drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-25 15:12:46.872471 pluginlab_admin-0.1.1/pluginlab_admin.egg-info/
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      140 2023-07-25 15:12:46.000000 pluginlab_admin-0.1.1/pluginlab_admin.egg-info/PKG-INFO
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      360 2023-07-25 15:12:46.000000 pluginlab_admin-0.1.1/pluginlab_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)        1 2023-07-25 15:12:46.000000 pluginlab_admin-0.1.1/pluginlab_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       52 2023-07-25 15:12:46.000000 pluginlab_admin-0.1.1/pluginlab_admin.egg-info/requires.txt
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       16 2023-07-25 15:12:46.000000 pluginlab_admin-0.1.1/pluginlab_admin.egg-info/top_level.txt
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       38 2023-07-25 15:12:46.872838 pluginlab_admin-0.1.1/setup.cfg
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      267 2023-07-25 15:12:27.000000 pluginlab_admin-0.1.1/setup.py
```

### Comparing `pluginlab_admin-0.1.0/README.md` & `pluginlab_admin-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,26 @@
 
 ## Verify the user token
 
 Everytime ChatGPT will talk to your backend through the PluginLab proxy, it will send the user token in the Authorization header as a bearer token.
 You can verify the integrity of such token by using the `verify_token` method:
 
 ```python
-auth = app.get_auth();
+auth = app.get_auth()
 
 # usually you'd get the token from the Authorization header of the HTTP request, formatted as `Bearer <token>`
 token = "eyJhbGc...dQssw5c"
 
 try:
     payload = auth.verify_token(token)
     # from that point we know the information in the token hasn't been tampered with
 
     # we could, for instance, check if the user has a given plan and take specific action based on that
-    premium_plan_id = 'KWsmKyJnHBF2Dz1mETDF';
-    plan_id = payload.user.plan_id;
+    premium_plan_id = 'KWsmKyJnHBF2Dz1mETDF'
+    plan_id = payload.user.plan_id
 
     if plan_id:
         if plan_id == premium_plan_id: 
             do_something_special()
         else
             do_other_stuff()
 
@@ -140,15 +140,15 @@
 
 ### With adjustable limit and pagination
 
 You can request up to 100 members at a time and get a specific page by providing a cursor obtained from a previous call.
 
 ```python
 paginated_result1 = auth.get_members(50)
-cursor = paginated_result1.next_page_cursor;
+cursor = paginated_result1.next_page_cursor
 
 if not cursor is None:
     paginated_result2 = auth.get_members(50, cursor)
 ```
 
 ## Create a member
```

### Comparing `pluginlab_admin-0.1.0/pluginlab_admin/app.py` & `pluginlab_admin-0.1.1/pluginlab_admin/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .auth import AppAuth
 
 class App:
     def __init__(
             self,
             secret_key: str,
             plugin_id: str,
-            auth_url = "https://auth.pluginlab.ai/admin/v1/cert",
+            auth_url = "https://auth.pluginlab.ai",
             auth_cert_url = "https://auth.pluginlab.ai/admin/v1/cert"
         ):
         self.plugin_id = plugin_id
         self.secret_key = secret_key
         self.auth_url = auth_url
         self.auth_cert_url = auth_cert_url
```

### Comparing `pluginlab_admin-0.1.0/pluginlab_admin/auth.py` & `pluginlab_admin-0.1.1/pluginlab_admin/auth.py`

 * *Files identical despite different names*

### Comparing `pluginlab_admin-0.1.0/pluginlab_admin/token_verifier.py` & `pluginlab_admin-0.1.1/pluginlab_admin/token_verifier.py`

 * *Files identical despite different names*

### Comparing `pluginlab_admin-0.1.0/pluginlab_admin/webhook.py` & `pluginlab_admin-0.1.1/pluginlab_admin/webhook.py`

 * *Files identical despite different names*

