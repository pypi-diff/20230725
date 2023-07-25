# Comparing `tmp/homeconnect_webthing-1.0.0.tar.gz` & `tmp/homeconnect_webthing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeconnect_webthing-1.0.0.tar", last modified: Sun Jul 16 09:10:21 2023, max compression
+gzip compressed data, was "homeconnect_webthing-1.0.1.tar", last modified: Tue Jul 25 04:33:05 2023, max compression
```

## Comparing `homeconnect_webthing-1.0.0.tar` & `homeconnect_webthing-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:10:21.329148 homeconnect_webthing-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-16 09:10:21.329148 homeconnect_webthing-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:10:21.329148 homeconnect_webthing-1.0.0/homeconnect_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    35865 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/appliances.py
--rw-r--r--   0 runner    (1001) docker     (123)    26282 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/appliances_webthing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/eventstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/homeconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:10:21.329148 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-16 09:10:21.000000 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-16 09:10:21.000000 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 09:10:21.000000 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-16 09:10:21.000000 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-16 09:10:21.000000 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-16 09:10:21.000000 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-16 09:10:21.329148 homeconnect_webthing-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:33:05.050764 homeconnect_webthing-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-25 04:33:05.050764 homeconnect_webthing-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:33:05.050764 homeconnect_webthing-1.0.1/homeconnect_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35865 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/appliances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26282 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/appliances_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/auth_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/eventstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/homeconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:33:05.050764 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-25 04:33:05.000000 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-25 04:33:05.000000 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 04:33:05.000000 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 04:33:05.000000 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 04:33:05.000000 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 04:33:05.000000 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-25 04:33:05.050764 homeconnect_webthing-1.0.1/setup.cfg
```

### Comparing `homeconnect_webthing-1.0.0/LICENSE` & `homeconnect_webthing-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.0/PKG-INFO` & `homeconnect_webthing-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeconnect_webthing
-Version: 1.0.0
+Version: 1.0.1
 Summary: Homeconnect WebThing adapter
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `homeconnect_webthing-1.0.0/README.md` & `homeconnect_webthing-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.0/homeconnect_webthing/__init__.py` & `homeconnect_webthing-1.0.1/homeconnect_webthing/__init__.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.0/homeconnect_webthing/app.py` & `homeconnect_webthing-1.0.1/homeconnect_webthing/app.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.0/homeconnect_webthing/appliances.py` & `homeconnect_webthing-1.0.1/homeconnect_webthing/appliances.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.0/homeconnect_webthing/appliances_webthing.py` & `homeconnect_webthing-1.0.1/homeconnect_webthing/appliances_webthing.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.0/homeconnect_webthing/auth.py` & `homeconnect_webthing-1.0.1/homeconnect_webthing/auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import logging
 import requests
-import uuid
-import webbrowser
 from os import path
 from datetime import datetime, timedelta
-from urllib.parse import urlsplit, parse_qs
 from typing import Optional
 
 
-
-
-class FetchAccessToken:
+class AccessToken:
 
     def __init__(self, token: str = "", issue_time: datetime = datetime.strptime('1970-01-01', '%Y-%m-%d'), expires_in_sec: int = 0):
         self.token = token
         self.issue_time = issue_time
         self.expires_in_sec = expires_in_sec
 
     @property
@@ -26,61 +21,39 @@
 
     def __str__(self):
         return "issued: " + self.issue_time.strftime("%d.%b %H:%M") + ", " + \
                "expires: " + self.expiring_date.strftime("%d.%b %H:%M")
 
 
 class Auth:
-
     URI = "https://api.home-connect.com/security"
     DEFAULT_FILENAME = "homeconnect_oauth.txt"
 
-    @staticmethod
-    def create(client_id: str, client_secret:str, scope: str = "IdentifyAppliance%20Dishwasher%20Dryer%20Washer"):
-        state = str(uuid.uuid4())
-        uri = Auth.URI + "/oauth/authorize?response_type=code&client_id=" + client_id + "&scope=" + scope + "&state=" + state
-        webbrowser.open(uri)
-
-        auth_result = input("Please enter the URL redirected to: ")
-        query = urlsplit(auth_result).query
-        params = parse_qs(query)
-        authorization_code = params['code']
-        if params['state'][0] != state:
-            raise Exception("state mismatch")  # refer https://auth0.com/docs/secure/attack-protection/state-parameters
-
-        data = {"client_id": client_id,
-                "client_secret": client_secret,
-                "grant_type": "authorization_code",
-                "code": authorization_code}
-        response = requests.post(Auth.URI + '/oauth/token', data=data)
-        data = response.json()
-        return Auth(data['refresh_token'], client_secret)
-
     def __init__(self, refresh_token: str, client_secret: str):
-        self.__refresh_token = refresh_token
-        self.__client_secret = client_secret
-        self.__fetched_access_token = FetchAccessToken()
+        self.refresh_token = refresh_token
+        self.client_secret = client_secret
+        self.__fetched_access_token = AccessToken()
 
     @property
     def access_token(self) -> str:
         if self.__fetched_access_token.is_expired():
             logging.info("access token is (almost) expired (" + str(self.__fetched_access_token) + "). Requesting new access token")
-            data = {"grant_type": "refresh_token", "refresh_token": self.__refresh_token, "client_secret": self.__client_secret}
+            data = {"grant_type": "refresh_token", "refresh_token": self.refresh_token, "client_secret": self.client_secret}
             response = requests.post(Auth.URI + '/oauth/token', data=data)
             response.raise_for_status()
             data = response.json()
-            self.__fetched_access_token = FetchAccessToken(data['access_token'], datetime.now(), data['expires_in'])
+            self.__fetched_access_token = AccessToken(data['access_token'], datetime.now(), data['expires_in'])
             logging.info("new access token has been created (" + str(self.__fetched_access_token) + ")")
         return self.__fetched_access_token.token
 
     def store(self, filename : str = DEFAULT_FILENAME):
         logging.info("storing secret file " + path.abspath(filename))
         with open(filename, "w") as file:
-            file.write("refresh_token: " + self.__refresh_token + "\n")
-            file.write("client_secret: " + self.__client_secret + "\n")
+            file.write("refresh_token: " + self.refresh_token + "\n")
+            file.write("client_secret: " + self.client_secret + "\n")
 
     @staticmethod
     def load(filename : str = DEFAULT_FILENAME) -> Optional:
         if filename is None:
             logging.info("filename is required")
         else:
             if path.isfile(filename):
@@ -92,11 +65,11 @@
                     client_secret = client_secret_line[client_secret_line.index(":")+1:].strip()
                     return Auth(refresh_token, client_secret)
             else:
                 logging.info("secret file " + path.abspath(filename) + " does not exist")
                 return None
 
     def __str__(self):
-        return "refresh_token: " + self.__refresh_token + "\n" + "client_secret: " + self.__client_secret
+        return "refresh_token: " + self.refresh_token + "\n" + "client_secret: " + self.client_secret
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `homeconnect_webthing-1.0.0/homeconnect_webthing/eventstream.py` & `homeconnect_webthing-1.0.1/homeconnect_webthing/eventstream.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.0/homeconnect_webthing/homeconnect.py` & `homeconnect_webthing-1.0.1/homeconnect_webthing/homeconnect.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/PKG-INFO` & `homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeconnect-webthing
-Version: 1.0.0
+Version: 1.0.1
 Summary: Homeconnect WebThing adapter
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/SOURCES.txt` & `homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.cfg
 homeconnect_webthing/__init__.py
 homeconnect_webthing/app.py
 homeconnect_webthing/appliances.py
 homeconnect_webthing/appliances_webthing.py
 homeconnect_webthing/auth.py
+homeconnect_webthing/auth_manager.py
 homeconnect_webthing/eventstream.py
 homeconnect_webthing/homeconnect.py
 homeconnect_webthing/utils.py
 homeconnect_webthing.egg-info/PKG-INFO
 homeconnect_webthing.egg-info/SOURCES.txt
 homeconnect_webthing.egg-info/dependency_links.txt
 homeconnect_webthing.egg-info/entry_points.txt
```

