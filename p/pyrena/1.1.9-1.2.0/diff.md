# Comparing `tmp/pyrena-1.1.9.tar.gz` & `tmp/pyrena-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrena-1.1.9.tar", last modified: Tue Sep  6 20:01:48 2022, max compression
+gzip compressed data, was "pyrena-1.2.0.tar", last modified: Tue Jul 25 21:03:29 2023, max compression
```

## Comparing `pyrena-1.1.9.tar` & `pyrena-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-09-06 20:01:48.072085 pyrena-1.1.9/
--rw-rw-rw-   0        0        0     1077 2022-08-03 18:04:59.000000 pyrena-1.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0     1365 2022-09-06 20:01:48.071085 pyrena-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1145 2022-08-04 15:50:28.000000 pyrena-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2022-09-06 20:01:48.050462 pyrena-1.1.9/pyrena/
--rw-rw-rw-   0        0        0    17943 2022-09-06 20:01:21.000000 pyrena-1.1.9/pyrena/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 20:01:48.070084 pyrena-1.1.9/pyrena/classes/
--rw-rw-rw-   0        0        0      374 2022-08-09 14:25:32.000000 pyrena-1.1.9/pyrena/classes/__init__.py
--rw-rw-rw-   0        0        0     9272 2022-09-06 18:41:33.000000 pyrena-1.1.9/pyrena/classes/base.py
--rw-rw-rw-   0        0        0      637 2022-08-03 20:21:48.000000 pyrena-1.1.9/pyrena/classes/bom.py
--rw-rw-rw-   0        0        0     3909 2022-08-09 13:17:11.000000 pyrena-1.1.9/pyrena/classes/change.py
--rw-rw-rw-   0        0        0     2844 2022-08-03 20:21:36.000000 pyrena-1.1.9/pyrena/classes/eventqueue.py
--rw-rw-rw-   0        0        0      112 2022-07-29 17:42:48.000000 pyrena-1.1.9/pyrena/classes/extract.py
--rw-rw-rw-   0        0        0     3292 2022-09-06 18:27:13.000000 pyrena-1.1.9/pyrena/classes/file.py
--rw-rw-rw-   0        0        0     2555 2022-08-08 18:19:07.000000 pyrena-1.1.9/pyrena/classes/item.py
--rw-rw-rw-   0        0        0     7449 2022-09-06 18:51:17.000000 pyrena-1.1.9/pyrena/classes/quality.py
--rw-rw-rw-   0        0        0     1943 2022-08-08 18:21:30.000000 pyrena-1.1.9/pyrena/classes/supplier.py
--rw-rw-rw-   0        0        0     3407 2022-08-09 14:36:00.000000 pyrena-1.1.9/pyrena/classes/tickets.py
--rw-rw-rw-   0        0        0     3475 2022-08-19 14:57:46.000000 pyrena-1.1.9/pyrena/classes/training.py
--rw-rw-rw-   0        0        0      473 2022-08-03 20:22:24.000000 pyrena-1.1.9/pyrena/classes/user.py
-drwxrwxrwx   0        0        0        0 2022-09-06 20:01:48.054462 pyrena-1.1.9/pyrena.egg-info/
--rw-rw-rw-   0        0        0     1365 2022-09-06 20:01:48.000000 pyrena-1.1.9/pyrena.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2022-09-06 20:01:48.000000 pyrena-1.1.9/pyrena.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-06 20:01:48.000000 pyrena-1.1.9/pyrena.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2022-09-06 20:01:48.000000 pyrena-1.1.9/pyrena.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-09-06 20:01:48.000000 pyrena-1.1.9/pyrena.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-06 20:01:48.072085 pyrena-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      480 2022-09-06 20:01:34.000000 pyrena-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:03:29.885562 pyrena-1.2.0/
+-rw-rw-rw-   0        0        0     1077 2022-08-03 18:04:59.000000 pyrena-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1687 2023-07-25 21:03:29.884560 pyrena-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2023-07-25 21:02:45.000000 pyrena-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 21:03:29.868561 pyrena-1.2.0/pyrena/
+-rw-rw-rw-   0        0        0    15367 2023-07-25 21:00:35.000000 pyrena-1.2.0/pyrena/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:03:29.883561 pyrena-1.2.0/pyrena/classes/
+-rw-rw-rw-   0        0        0      374 2022-08-09 14:25:32.000000 pyrena-1.2.0/pyrena/classes/__init__.py
+-rw-rw-rw-   0        0        0     9349 2022-10-04 15:18:47.000000 pyrena-1.2.0/pyrena/classes/base.py
+-rw-rw-rw-   0        0        0      637 2022-08-03 20:21:48.000000 pyrena-1.2.0/pyrena/classes/bom.py
+-rw-rw-rw-   0        0        0     3909 2022-08-09 13:17:11.000000 pyrena-1.2.0/pyrena/classes/change.py
+-rw-rw-rw-   0        0        0     2844 2022-08-03 20:21:36.000000 pyrena-1.2.0/pyrena/classes/eventqueue.py
+-rw-rw-rw-   0        0        0      112 2022-07-29 17:42:48.000000 pyrena-1.2.0/pyrena/classes/extract.py
+-rw-rw-rw-   0        0        0     3292 2022-10-04 14:38:59.000000 pyrena-1.2.0/pyrena/classes/file.py
+-rw-rw-rw-   0        0        0     2668 2022-10-04 14:38:43.000000 pyrena-1.2.0/pyrena/classes/item.py
+-rw-rw-rw-   0        0        0     7449 2022-09-06 18:51:17.000000 pyrena-1.2.0/pyrena/classes/quality.py
+-rw-rw-rw-   0        0        0     1943 2022-08-08 18:21:30.000000 pyrena-1.2.0/pyrena/classes/supplier.py
+-rw-rw-rw-   0        0        0     3407 2022-08-09 14:36:00.000000 pyrena-1.2.0/pyrena/classes/tickets.py
+-rw-rw-rw-   0        0        0     3475 2022-08-19 14:57:46.000000 pyrena-1.2.0/pyrena/classes/training.py
+-rw-rw-rw-   0        0        0      473 2022-09-21 14:12:18.000000 pyrena-1.2.0/pyrena/classes/user.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:03:29.872561 pyrena-1.2.0/pyrena.egg-info/
+-rw-rw-rw-   0        0        0     1687 2023-07-25 21:03:29.000000 pyrena-1.2.0/pyrena.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2023-07-25 21:03:29.000000 pyrena-1.2.0/pyrena.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 21:03:29.000000 pyrena-1.2.0/pyrena.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-25 21:03:29.000000 pyrena-1.2.0/pyrena.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 21:03:29.000000 pyrena-1.2.0/pyrena.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 21:03:29.885562 pyrena-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      508 2023-07-25 21:01:49.000000 pyrena-1.2.0/setup.py
```

### Comparing `pyrena-1.1.9/LICENSE.txt` & `pyrena-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.9/PKG-INFO` & `pyrena-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: pyrena
-Version: 1.1.9
+Version: 1.2.0
 Summary: Python wrapper for Arena QMS API.
 Home-page: https://github.com/thecodeforge/pyrena
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # pyrena
 
 API wrapper for interacting with Arena QMS.
 
@@ -31,15 +32,17 @@
 
 ```python
 import pyrena
 
 client = pyrena.Arena("username", "password")
 ```
 
-Government users should add the parameter `base_url="https://api.arenagov.com/v1/v1"` during client creation.
+Users on the government server should add the parameter `arenagov=True` during client creation.
+
+Users on the Europe server should add the parameter `europe=True` during client creation. 
 
 ### Change users
 
 ```python
 client.logout()
 client.login("different_username", "different_password")
 ```
@@ -50,10 +53,18 @@
 
 ```python
 search_results = client.Listing(client.QualityProcess, number="NCMR-*")
 ```
 
 ### Retrieve specific object
 
+Option 1 - get object by object GUID, if known
+
 ```python
 my_change_order = client.Change("object_guid")
 ```
+
+Option 2 - get object by its "user-friendly" ID (known as `number` in the API)
+
+```python
+my_capa = client.find(client.QualityProcess, number="CAPA-000001")
+```
```

### Comparing `pyrena-1.1.9/README.md` & `pyrena-1.2.0/pyrena.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: pyrena
+Version: 1.2.0
+Summary: Python wrapper for Arena QMS API.
+Home-page: https://github.com/thecodeforge/pyrena
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # pyrena
 
 API wrapper for interacting with Arena QMS.
 
 Pyrena is not associated with or approved by Arena Solutions or PTC.
 
 ## Installation
@@ -23,15 +32,17 @@
 
 ```python
 import pyrena
 
 client = pyrena.Arena("username", "password")
 ```
 
-Government users should add the parameter `base_url="https://api.arenagov.com/v1/v1"` during client creation.
+Users on the government server should add the parameter `arenagov=True` during client creation.
+
+Users on the Europe server should add the parameter `europe=True` during client creation. 
 
 ### Change users
 
 ```python
 client.logout()
 client.login("different_username", "different_password")
 ```
@@ -42,10 +53,18 @@
 
 ```python
 search_results = client.Listing(client.QualityProcess, number="NCMR-*")
 ```
 
 ### Retrieve specific object
 
+Option 1 - get object by object GUID, if known
+
 ```python
 my_change_order = client.Change("object_guid")
-```
+```
+
+Option 2 - get object by its "user-friendly" ID (known as `number` in the API)
+
+```python
+my_capa = client.find(client.QualityProcess, number="CAPA-000001")
+```
```

### Comparing `pyrena-1.1.9/pyrena/__init__.py` & `pyrena-1.2.0/pyrena/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,56 +15,66 @@
 import pyrena.classes as classes
 
 class ArenaHTTPError(Exception):
     pass
 
 class Arena():
 
-    def __init__(self, username=None, password=None, ssl_verify=True, user_agent="Python Pyrena", verbose=False, arenagov=False):
+    def __init__(self, username=None, password=None, env=None, ssl_verify=True, user_agent="Python Pyrena", verbose=False, arenagov=False, europe=False):
 
         """
         Creates the Arena client
 
         Optional arguments:
-        - arenagov      - Set to True for accessing workspaces located on app.arenagov.com. Defaults to False for workspaces located on app.bom.com.
+        - env           - Arena Workspace ID. If omitted, will use the workspace most recently accessed by the authenticated account.
+        - arenagov      - Set to True for accessing workspaces located on app.arenagov.com. Defaults to False.
+        - europe        - Set to True for accessing workspaces located on app.europe.arenaplm.com. Defaults to False
         - ssl_verify    - Use strict SSL verification in requests. May need to be set to False when accessing Arena from a corporate-controlled network.
         - user_agent    - Set a User-Agent header.
         - verbose       - Verbosely output API requests to console
         """
 
         #set properties
-        self.base_url = "https://api.arenagov.com/v1/v1" if arenagov else "https://api.arenasolutions.com/v1"
-        self.browser_url = "https://app.arenagov.com/" if arenagov else "https://app.bom.com/"
+        if arenagov:
+            self.base_url="https://api.arenagov.com/v1"
+            self.browser_url = "https://app.arenagov.com/"
+        elif europe:
+            self.base_url="https://api.europe.arenaplm.com/v1"
+            self.browser_url = "https://app.europe.arenaplm.com/"
+        else:
+            self.base_url="https://api.arenasolutions.com/v1"
+            self.browser_url = "https://app.bom.com/"
+
         self.ssl_verify = ssl_verify
 
 
         #if ssl_verify is false, disable insecure http warnings
         if not ssl_verify:
             warnings.filterwarnings("ignore", category=urllib3.exceptions.InsecureRequestWarning)
 
         self.user_agent = user_agent
 
         self._debug=verbose
-
+ 
         self.__dict__['_username']=username
         self.__dict__['_password']=password
-
+        self.__dict__['_env']=env
 
         self.headers={
             "User-Agent": self.user_agent,
             "Content-Type": "application/json"
         }
 
-        self._reqs_remaining=25000
+        self._reqs_remaining=123456789 #arbitrary high - depends on your deal with Arena. Updates after first call.
 
         #login
         try:
             self.login()
         except ArenaHTTPError:
-            print("Unable to log in. Call `login(username, password)` on this client to authenticate with Arena.")
+            print("Unable to log in. Call `login(username, password + optional env)` on this client to authenticate with Arena.")
         except ssl.SSLCertVerificationError:
             print("Unable to establish a secure connection to Arena. Use a different internet connection or use `ssl_verify=False` to allow insecure requests.")
 
         #initialize cache
         self._cache={}
 
     def __getattr__(self, name):
@@ -85,80 +95,88 @@
             raise AttributeError
 
         obj._client=self
 
         return obj
 
     def __repr__(self):
-        return f"<Arena(user={self.__dict__['_username']})>"
+        if self.__dict__['_env']:
+            return f"<Arena(user={self.__dict__['_username']}) in env={self.__dict__['_env']}>"
+        else:
+            return f"<Arena(user={self.__dict__['_username']}) in default env>"
 
-    def login(self, username=None, password=None):
+    def login(self, username=None, password=None, env=None):
 
         """
         Log into Arena
 
         Optional arguments:
         - username    - Username. Defaults to username given at client creation if not specified.
         - password    - Password. Defaults to password given at client creation if not specified.
         """
 
         self.__dict__["_username"] = username or self.__dict__["_username"]
         self.__dict__["_password"] = password or self.__dict__["_password"]
+        self.__dict__["_env"] = env or self.__dict__["_env"]
 
-        login_data = self._post(
-            "/login",
-            data={
-                "email":self.__dict__["_username"],
-                "password":self.__dict__["_password"]
-                }
-            )
-
+        if env: #e.g to switch between several workspaces or sandboxes
+            login_data = self._post(
+                "/login",
+                data={
+                    "email":self.__dict__["_username"],
+                    "password":self.__dict__["_password"],
+                    "workspaceId":self.__dict__["_env"]
+                    }
+                )
+        else: # if no env specified, logs into to default env
+            login_data = self._post(
+                "/login",
+                data={
+                    "email":self.__dict__["_username"],
+                    "password":self.__dict__["_password"],
+                    }
+                )
 
         #set auth token
         self.headers["arena_session_id"]=login_data["arenaSessionId"]
-
-        #set workspace id and name
-        self._workspace_id=login_data["workspaceId"]
-        self._workspace_name=login_data["workspaceName"]
-
         #set time to re-auth, 1 min before expiry
-        self.reauth_utc = int(time.time())+60*60*80
+        self.reauth_utc = int(time.time())+60*60*89
+        #update reqs remaining
+        self._reqs_remaining = login_data["workspaceRequestLimit"]
 
     def logout(self):
 
         """
         Log out of Arena.
         """
-
-        self._put("/logout")
+        self._put("/logout", expect_json = False)
         self.__dict__["_username"]=None
         self.__dict__["_password"]=None
         self.__dict__["me"]=None
-        self._workspace_id=None
-        self._workspace_name=NOne
+        self.__dict__["env"]=None
         self.headers["arena_session_id"]=None
         self.reauth_utc=0
 
     def _fetch(self, method, endpoint, params={}, data={}, files={}, headers={}, expect_json=True, **kwargs):
 
         if not self._reqs_remaining:
-            raise ArenaHTTPError("Request limit of 25000/day reached.")
+            raise ArenaHTTPError("Request limit reached.") 
 
         #reauth 1 min before expiry
         if endpoint != "/login" and int(time.time())> self.reauth_utc:
             self.login()
 
         url = f"{self.base_url}{'' if endpoint.startswith('/') else '/'}{endpoint}"
 
         req_headers=self.headers
         for header in headers:
             req_headers[header]=headers[header]
 
         try:
-            req = getattr(requests, method.lower())(
+            resp = getattr(requests, method.lower())(
                 url, 
                 headers=req_headers, 
                 params=params,
                 json=data, 
                 files=files,
                 verify=self.ssl_verify,
                 )
@@ -166,33 +184,42 @@
             raise requests.exceptions.SSLError("Unable to establish a secure connection to Arena. Use a different internet connection or use `ssl_verify=False` to allow insecure requests.")
 
         if self._debug:
             print("===PAYLOAD===")
             print(f"{method.upper()} {endpoint}")
             pprint(data)
             print("===RESPONSE===")
-            print(f"status {req.status_code}")
-            pprint(req.json())
+            print(f"status {resp.status_code}")
+            pprint(resp.json())
 
-        if req.status_code >=400:
-            data=req.json()
-            raise ArenaHTTPError(f"HTTP Error {req.status_code} - {data['errors'][0]['message']} (Arena Error Code {data['errors'][0]['code']})")
+        if resp.status_code >=400:
+            data=resp.json()
+            raise ArenaHTTPError(f"HTTP Error {resp.status_code} - {data['errors'][0]['message']} (Arena Error Code {data['errors'][0]['code']})")
 
-        req.raise_for_status()
+        resp.raise_for_status()
 
 
-        #update reqs remaining
-        self._reqs_remaining = req.headers.get("X-Arena-Requests-Remaining", self._reqs_remaining)
+        #update requests remaining
+        self._reqs_remaining = int(resp.headers.get("X-Arena-Requests-Remaining", self._reqs_remaining))
+
+        # print reqs remaining at login/logout:
+        if self._reqs_remaining < 1000 and self._debug:
+            print(f"Caution: {self._reqs_remaining} requests remaining")
+        elif endpoint in ["/login", "/logout"]:
+            print(f"Number of remaining requests: {self._reqs_remaining}")
+
+        #update reauth timer - 90min from last action, not 90min from authentication
+        self.reauth_utc=int(time.time())+60*60*89
 
         if method.lower()=="delete":
             return
         elif expect_json==False:
-            return req.content
+            return resp.content
         else:
-            return req.json()
+            return resp.json()
 
     def _get(self, endpoint, params={}, **kwargs):
         return self._fetch("get", endpoint, params=params, **kwargs)
 
     #@disable
     def _post(self, endpoint, data={}, files={}, **kwargs):
         return self._fetch("post", endpoint, data=data, files=files, **kwargs)
@@ -256,15 +283,15 @@
         if not listing:
             return []
 
         for item in listing:
             item._client=self
 
 
-        if len(listing)==limit:
+        if not limit or len(listing)==limit:
             listing+=self.Listing(
                     obj, 
                     endpoint, 
                     limit=400 if limit else None,
                     offset=offset+400,
                     **kwargs
                     )
@@ -358,130 +385,22 @@
 
         if self.__dict__.get("me"):
             return self.__dict__['me']
         else:
             self.__dict__['me']=self.Listing(self.User, email=self.__dict__['_username'])[0]
             return self.__dict__['me']
 
-    def archive(self, folder_name="", exclude=[]):
-
-        """
-        WIP feature
-
-        Downloads all available data from the current Arena instance and saves it in JSON format.
-        Intended to be used as a rapid bulk export for local backup.
-
-        This may take some time, will verbosely output data, and may consume a large portion of the daily API limit.
-
-        Optional arguments:
-
-        - folder    - Path to existing archive folder, if one already exists
-        - exclude   - list of Arena classes to exclude from the backup.
-        """
-
-        d= time.strftime("%d_%B_%Y")
-
-        folder_name = folder_name or f"Arena_archive_{self._workspace_name}_{d}"
-
-        if not os.path.exists(folder_name):
-            os.mkdir(folder_name)
-
-        #Files
-        if self.File not in exclude:
-
-            print("Collecting Files...")
-            files=self.Listing(self.File, limit=None)
-            print(f"{len(files)} Files found")
-
-            with open(f"{folder_name}/Files_{time.strftime('%d_%B_%Y')}.txt", "w+") as f:
-                f.write(json.dumps([x.json for x in files], indent=2))
-                f.truncate()
-            print("File json data saved")
-
-            if not os.path.exists(f"{folder_name}/file_vault"):
-                os.mkdir(f"{folder_name}/file_vault")
-
-            i=0
-            print("Saving files...")
-            for file in files:
-                with open(f"{folder_name}/file_vault/[{file.number}] {file.title}.{file.format}", "wb+") as f:
-                    f.write(file.content)
-                    f.truncate()
-                i+=1
-                print(f"{i}/{len(files)} [{file.number}] {file.title}.{file.format}")
-
-
-        #Items
-        if self.Item not in exclude:
-            print("Collecting Items...")
-            items = self.Listing(self.Item, limit=None)
-            print(f"{len(items)} Items found")
-
-            i=0
-            print("Loading file associations and revision data")
-            for item in items:
-                item.__dict__["files"]=[x.json for x in item.file_associations]
-                item.__dict__["revisions"]=[x.json for x in item.revisions]
-                i+=1
-                print(f"{i}/{len(items)} [{item.number}] {item.name}")
-
-            with open(f"{folder_name}/Items_{time.strftime('%d_%B_%Y')}.txt", "w+") as f:
-                f.write(json.dumps([x.json for x in items], indent=2))
-                f.truncate()
-
-            print("Item JSON data saved")
-
-        #Quality
-        if self.QualityProcess not in exclude:
-            print("Collecting Quality...")
-            qps = self.Listing(self.QualityProcess, limit=None)
-            print(f"{len(qps)} Quality records found")
-
-            i=0
-            print("Loading step and attachment data")
-            for qp in qps:
-                for step in qp.steps:
-                    step.__dict__['affected']=[x.json for x in step.affected]
-                qp.__dict__["steps"]=[x.json for x in qp.steps]
-                i+=1
-                print(f"{i}/{len(qps)} [{qp.number}] {qp.name}")
-
-            with open(f"{folder_name}/Quality_{time.strftime('%d_%B_%Y')}.txt", "w+") as f:
-                f.write(json.dumps([x.json for x in qps], indent=2))
-                f.truncate()
-
-            print("Quality JSON data saved")
-
-        #Training
-        if self.TrainingPlan not in exclude:
-            print("Collecting Training...")
-            tps = self.Listing(self.TrainingPlan, limit=None)
-            print(f"{len(tps)} Training Plans found")
-
-            i=0
-            print("Loading item and user references and training record data")
-            for tp in tps:
-                tp.__dict__["records"]=[x.json for x in tp.records]
-                tp.__dict__["items"]=[x.json for x in tp.item_associations]
-                tp.__dict__["users"]=[x.json for x in tp.user_associations]
-                i+=1
-                print(f"{i}/{len(tps)} [{tp.number}] {tp.name}")
-
-            with open(f"{folder_name}/Training_{time.strftime('%d_%B_%Y')}.txt", "w+") as f:
-                f.write(json.dumps([x.json for x in tps], indent=2))
-                f.truncate()
-
-            print("Training JSON data saved")
+   
 def docs():
 
     """
     Generate and display this documentation page.
     """
 
-    classlist = {name:cls for name, cls in list(classes.__dict__.items()) if isinstance(cls, type) and name!="Object"}
+    classlist = {name:cls for name, cls in list(classes.__dict__.items()) if isinstance(cls, type) and name not in ["Object"] and "_mixin" not in name}
     classlist["Arena"]=Arena
 
     #page header
     md = "# `Pyrena Docs`\n\n"
 
     #Iterate through classes (including the Arena client class)
     for class_name in sorted(classlist.keys()):
```

### Comparing `pyrena-1.1.9/pyrena/classes/base.py` & `pyrena-1.2.0/pyrena/classes/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,17 @@
             if "number" in self.__dict__:
                 return f"<{self.__class__.__name__}(number={self.number})>"
             elif "name" in self.__dict__:
                 return f"<{self.__class__.__name__}(name={self.name})>"
             else:
                 return f"<{self.__class__.__name__}(id={self.guid})>"
 
+    def __hash__(self):
+        return hash(self.__repr__())
+
     def __str__(self):
         if "name" in self.__dict__:
             return f"<{self.__class__.__name__}(name={self.name})>"
         else:
             return self.__repr__
 
     def __eq__(self, other):
@@ -264,16 +267,16 @@
             if isinstance(x, Object):
                 return x.json
             else:
                 return x
 
         data={x: self.__dict__[x] for x in self.__dict__}
 
-        data.pop("_client")
-        data.pop("_cache")
+        data.pop("_client", None)
+        data.pop("_cache", None)
         
         data={x:process_values(data[x]) for x in data}
 
         return data
     
     
 class openable_mixin():
```

### Comparing `pyrena-1.1.9/pyrena/classes/bom.py` & `pyrena-1.2.0/pyrena/classes/bom.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.9/pyrena/classes/change.py` & `pyrena-1.2.0/pyrena/classes/change.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.9/pyrena/classes/eventqueue.py` & `pyrena-1.2.0/pyrena/classes/eventqueue.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.9/pyrena/classes/file.py` & `pyrena-1.2.0/pyrena/classes/file.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.9/pyrena/classes/item.py` & `pyrena-1.2.0/pyrena/classes/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,20 @@
         assocs = self._client.Listing(self._client.ItemFileAssociation, endpoint=f"/items/{self.guid}/files")
         for assoc in assocs:
             assoc.item=self
         return assocs
 
     @property
     @lazy
+    def files(self):
+        return [x.file for x in self.file_associations]
+    
+
+    @property
+    @lazy
     def thumbnail(self):
 
         return self._client._get(f"/items/{self.guid}/image/content")
 
     @property
     def working_revision(self):
         rev = [x for x in self.revisions if x.status==0]
```

### Comparing `pyrena-1.1.9/pyrena/classes/quality.py` & `pyrena-1.2.0/pyrena/classes/quality.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.9/pyrena/classes/supplier.py` & `pyrena-1.2.0/pyrena/classes/supplier.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.9/pyrena/classes/tickets.py` & `pyrena-1.2.0/pyrena/classes/tickets.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.9/pyrena/classes/training.py` & `pyrena-1.2.0/pyrena/classes/training.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.9/pyrena.egg-info/SOURCES.txt` & `pyrena-1.2.0/pyrena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

