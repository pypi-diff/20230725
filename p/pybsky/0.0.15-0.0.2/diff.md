# Comparing `tmp/pybsky-0.0.15.tar.gz` & `tmp/pybsky-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybsky-0.0.15.tar", last modified: Tue Jul 25 19:48:43 2023, max compression
+gzip compressed data, was "pybsky-0.0.2.tar", last modified: Sun Jul 23 19:40:03 2023, max compression
```

## Comparing `pybsky-0.0.15.tar` & `pybsky-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 19:48:43.659350 pybsky-0.0.15/
--rw-rw-rw-   0        0        0     1100 2023-07-23 19:53:13.000000 pybsky-0.0.15/LICENSE
--rw-rw-rw-   0        0        0     1079 2023-07-25 19:48:43.658351 pybsky-0.0.15/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-23 19:53:13.000000 pybsky-0.0.15/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 19:48:43.633350 pybsky-0.0.15/pybsky/
--rw-rw-rw-   0        0        0       67 2023-07-23 19:53:13.000000 pybsky-0.0.15/pybsky/__init__.py
--rw-rw-rw-   0        0        0      933 2023-07-25 19:44:38.000000 pybsky-0.0.15/pybsky/client.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:48:43.654350 pybsky-0.0.15/pybsky/core/
--rw-rw-rw-   0        0        0      101 2023-07-25 18:51:39.000000 pybsky-0.0.15/pybsky/core/__init__.py
--rw-rw-rw-   0        0        0      115 2023-07-23 19:53:13.000000 pybsky-0.0.15/pybsky/core/configs.py
--rw-rw-rw-   0        0        0      266 2023-07-23 19:53:13.000000 pybsky-0.0.15/pybsky/core/exceptions.py
--rw-rw-rw-   0        0        0     5947 2023-07-23 19:53:13.000000 pybsky-0.0.15/pybsky/core/user_agents.py
--rw-rw-rw-   0        0        0     1066 2023-07-23 19:53:13.000000 pybsky-0.0.15/pybsky/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:48:43.657352 pybsky-0.0.15/pybsky/mixins/
--rw-rw-rw-   0        0        0       60 2023-07-23 19:53:13.000000 pybsky-0.0.15/pybsky/mixins/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-23 19:53:13.000000 pybsky-0.0.15/pybsky/mixins/base.py
--rw-rw-rw-   0        0        0      871 2023-07-23 19:53:13.000000 pybsky-0.0.15/pybsky/mixins/feed.py
--rw-rw-rw-   0        0        0     1396 2023-07-23 19:53:13.000000 pybsky-0.0.15/pybsky/mixins/login.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:48:43.650352 pybsky-0.0.15/pybsky.egg-info/
--rw-rw-rw-   0        0        0     1079 2023-07-25 19:48:43.000000 pybsky-0.0.15/pybsky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-07-25 19:48:43.000000 pybsky-0.0.15/pybsky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 19:48:43.000000 pybsky-0.0.15/pybsky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-25 19:48:43.000000 pybsky-0.0.15/pybsky.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-25 19:48:43.000000 pybsky-0.0.15/pybsky.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1385 2023-07-25 19:48:32.000000 pybsky-0.0.15/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 19:48:43.659350 pybsky-0.0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.421621 pybsky-0.0.2/
+-rw-rw-rw-   0        0        0     1100 2023-07-23 19:26:05.000000 pybsky-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1183 2023-07-23 19:40:03.420621 pybsky-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2023-07-23 19:38:22.000000 pybsky-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.399622 pybsky-0.0.2/pybsky/
+-rw-rw-rw-   0        0        0       68 2023-07-23 18:34:27.000000 pybsky-0.0.2/pybsky/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-07-23 18:18:34.000000 pybsky-0.0.2/pybsky/client.py
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.416622 pybsky-0.0.2/pybsky/core/
+-rw-rw-rw-   0        0        0      122 2023-07-23 18:34:23.000000 pybsky-0.0.2/pybsky/core/__init__.py
+-rw-rw-rw-   0        0        0      115 2023-07-21 12:03:54.000000 pybsky-0.0.2/pybsky/core/configs.py
+-rw-rw-rw-   0        0        0      266 2023-07-21 11:59:59.000000 pybsky-0.0.2/pybsky/core/exceptions.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 19:13:17.000000 pybsky-0.0.2/pybsky/core/log.py
+-rw-rw-rw-   0        0        0     5947 2023-07-23 18:36:54.000000 pybsky-0.0.2/pybsky/core/user_agents.py
+-rw-rw-rw-   0        0        0     1038 2023-07-23 18:38:10.000000 pybsky-0.0.2/pybsky/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.419622 pybsky-0.0.2/pybsky/mixins/
+-rw-rw-rw-   0        0        0       60 2023-07-23 18:34:35.000000 pybsky-0.0.2/pybsky/mixins/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 19:51:23.000000 pybsky-0.0.2/pybsky/mixins/base.py
+-rw-rw-rw-   0        0        0      878 2023-07-23 18:18:45.000000 pybsky-0.0.2/pybsky/mixins/feed.py
+-rw-rw-rw-   0        0        0     1399 2023-07-23 18:18:50.000000 pybsky-0.0.2/pybsky/mixins/login.py
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.411622 pybsky-0.0.2/pybsky.egg-info/
+-rw-rw-rw-   0        0        0     1183 2023-07-23 19:40:03.000000 pybsky-0.0.2/pybsky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-07-23 19:40:03.000000 pybsky-0.0.2/pybsky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-23 19:40:03.000000 pybsky-0.0.2/pybsky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-23 19:40:03.000000 pybsky-0.0.2/pybsky.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1031 2023-07-23 19:39:45.000000 pybsky-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-23 19:40:03.421621 pybsky-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-07-23 19:20:21.000000 pybsky-0.0.2/setup.py
```

### Comparing `pybsky-0.0.15/LICENSE` & `pybsky-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybsky-0.0.15/PKG-INFO` & `pybsky-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pybsky
-Version: 0.0.15
+Version: 0.0.2
 Summary: Python Client for bsky social media
+Author: softrebel, ovan
 Author-email: Mohammadreza softrebel <sh.mohammad66@yahoo.com>, Mahdi Ovan <mahdi.ovan@yahoo.com>
 Project-URL: Homepage, https://github.com/softrebel/pybsky
 Project-URL: Bug Tracker, https://github.com/softrebel/pybsky/issues
+Keywords: python,pybsky,bsky
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pybsky
 
 <div align='center'>
-
-![./a](./assets/cover.png)
+    <img src="./assets/cover.png" height="150" width="500" alt="pybsky-logo" >
 
 </div>
 
 
 ## TODO List:
 
 - [x] Create Client
```

### Comparing `pybsky-0.0.15/pybsky/client.py` & `pybsky-0.0.2/pybsky/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+
 import requests
 from .mixins import LoginMixin, FeedMixin
 from .core import USER_AGENTS, SERVER_URL
 import random
+from pydantic import BaseModel
 
 
-class Client(LoginMixin, FeedMixin):
+class Client(BaseModel, LoginMixin, FeedMixin):
     server: str = None
     proxies: str = None
     access_jwt: str = None
     refresh_jwt: str = None
     user_agent: str = None
-    session: requests.Session = None
+    session: requests.session = None
 
-    def __init__(self, proxies=None, server=None, **kwargs):
+    def __init__(
+        self,
+        proxies=None,
+        server=None,
+        **kwargs
+    ):
         super().__init__(**kwargs)
 
         self.server = server if server else SERVER_URL
         self.session = requests.Session()
         self.session.timeout = 20
         self.user_agent = random.choice(USER_AGENTS)
 
@@ -25,8 +32,8 @@
             self.proxies = proxies
             self.session.proxies = proxies
 
     def get_actor(self, username: str) -> str:
         if self.server in username:
             return username
         else:
-            return f"{username}.{self.server}"
+            return f'{username}.{self.server}'
```

### Comparing `pybsky-0.0.15/pybsky/core/user_agents.py` & `pybsky-0.0.2/pybsky/core/user_agents.py`

 * *Files identical despite different names*

### Comparing `pybsky-0.0.15/pybsky/core/utils.py` & `pybsky-0.0.2/pybsky/core/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import json
 import requests
-from .exceptions import (
-    AuthenticationRequiredException,
-    UnknownResponseException,
-    BadRequestResponseException,
-)
-
+from .exceptions import AuthenticationRequiredException,UnknownResponseException,\
+    BadRequestResponseException
 Response = requests.models.Response
 
 
 def validate_value(value, cls):
     if not isinstance(value, cls):
-        raise TypeError(f"{value} must be in type {cls}")
+        raise TypeError(f'{value} must be in type {cls}')
     return True
 
 
 def json_decode(s: str) -> list | dict:
     return json.loads(s)
 
 
@@ -24,16 +20,15 @@
 
 
 def validate_get_response(response: Response):
     content = response.json()
     if response.status_code == 200:
         return content
     elif response.status_code == 401:
-        raise AuthenticationRequiredException(content["message"])
+        raise AuthenticationRequiredException(content['message'])
     elif response.status_code == 400:
-        raise BadRequestResponseException(content["message"])
+        raise BadRequestResponseException(content['message'])
     else:
         raise UnknownResponseException(
-            f"status code => {response.status_code} , response => {response.text}"
-        )
+            f"status code => {response.status_code} , response => {response.text}")
 
     # TODO => handle all type of response
```

### Comparing `pybsky-0.0.15/pybsky/mixins/login.py` & `pybsky-0.0.2/pybsky/mixins/login.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import random
 import requests
 
 from ..core import USER_AGENTS, validate_value, validate_get_response
 
 
-class LoginMixin:
+class LoginMixin():
+
     def login(self, username: str, password: str):
         validate_value(username, str)
         validate_value(password, str)
         if len(username) == 0:
-            raise ValueError("username should not be empty")
+            raise ValueError('username should not be empty')
         if len(password) == 0:
-            raise ValueError("username should not be empty")
+            raise ValueError('username should not be empty')
 
         session = requests.Session()
         session.timeout = 30
         session.proxies = self.session.proxies
 
         self.user_agent = random.choice(USER_AGENTS)
 
         headers = {
-            "origin": "https://bsky.app",
-            "referer": "https://bsky.app/",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "cross-site",
-            "user-agent": self.user_agent,
+            'origin': 'https://bsky.app',
+            'referer': 'https://bsky.app/',
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'cross-site',
+            'user-agent': self.user_agent
         }
 
         payload = {
-            "identifier": self.get_actor(username),
-            "password": password,
+            'identifier': self.get_actor(username),
+            'password': password,
         }
-        url = "https://bsky.social/xrpc/com.atproto.server.createSession"
+        url = 'https://bsky.social/xrpc/com.atproto.server.createSession'
         response = requests.post(url, headers=headers, json=payload)
 
         validated_response = validate_get_response(response)
         self.access_jwt = validated_response["accessJwt"]
         self.refresh_jwt = validated_response["refreshJwt"]
         return validated_response
```

### Comparing `pybsky-0.0.15/pybsky.egg-info/PKG-INFO` & `pybsky-0.0.2/pybsky.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pybsky
-Version: 0.0.15
+Version: 0.0.2
 Summary: Python Client for bsky social media
+Author: softrebel, ovan
 Author-email: Mohammadreza softrebel <sh.mohammad66@yahoo.com>, Mahdi Ovan <mahdi.ovan@yahoo.com>
 Project-URL: Homepage, https://github.com/softrebel/pybsky
 Project-URL: Bug Tracker, https://github.com/softrebel/pybsky/issues
+Keywords: python,pybsky,bsky
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pybsky
 
 <div align='center'>
-
-![./a](./assets/cover.png)
+    <img src="./assets/cover.png" height="150" width="500" alt="pybsky-logo" >
 
 </div>
 
 
 ## TODO List:
 
 - [x] Create Client
```

### Comparing `pybsky-0.0.15/pyproject.toml` & `pybsky-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 [project]
 name = "pybsky"
-version = "0.0.15"
+version = "0.0.2"
 authors = [
   { name="Mohammadreza softrebel", email="sh.mohammad66@yahoo.com" },
     { name="Mahdi Ovan", email="mahdi.ovan@yahoo.com" },
 ]
 description ='Python Client for bsky social media'
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = [
-    "requests==2.31.0",
-]
 
 [project.urls]
 "Homepage" = "https://github.com/softrebel/pybsky"
 "Bug Tracker" = "https://github.com/softrebel/pybsky/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
@@ -34,13 +31,7 @@
 
 # Avoid trying to fix flake8-bugbear (`B`) violations.
 unfixable = ["B"]
 
 # Ignore `E402` (import violations) in all `__init__.py` files`.
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402","F403","F401"]
-
-[tool.setuptools.packages.find]
-where = ["."]  # list of folders that contain the packages (["."] by default)
-include = ["pybsky"]  # package names should match these glob patterns (["*"] by default)
-exclude = []  # exclude packages matching these glob patterns (empty by default)
-namespaces = false
```

