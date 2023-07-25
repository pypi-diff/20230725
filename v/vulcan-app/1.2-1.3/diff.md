# Comparing `tmp/vulcan-app-1.2.tar.gz` & `tmp/vulcan-app-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-app-1.2.tar", last modified: Fri Jul 21 10:27:14 2023, max compression
+gzip compressed data, was "vulcan-app-1.3.tar", last modified: Tue Jul 25 15:55:29 2023, max compression
```

## Comparing `vulcan-app-1.2.tar` & `vulcan-app-1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-21 10:27:14.105609 vulcan-app-1.2/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1073 2023-02-15 10:28:00.000000 vulcan-app-1.2/LICENSE
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-07-21 10:27:14.105609 vulcan-app-1.2/PKG-INFO
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       62 2023-02-15 10:28:00.000000 vulcan-app-1.2/README.md
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       38 2023-07-21 10:27:14.105609 vulcan-app-1.2/setup.cfg
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1157 2023-07-21 10:24:12.000000 vulcan-app-1.2/setup.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-21 10:27:14.105609 vulcan-app-1.2/vulcan_app/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      533 2023-07-18 13:53:23.000000 vulcan-app-1.2/vulcan_app/__init__.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      805 2023-02-23 08:06:39.000000 vulcan-app-1.2/vulcan_app/configuration.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-21 10:27:14.105609 vulcan-app-1.2/vulcan_app/database/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1520 2023-02-23 13:43:03.000000 vulcan-app-1.2/vulcan_app/database/__init__.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      251 2023-02-15 06:39:24.000000 vulcan-app-1.2/vulcan_app/database/mongo.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1257 2023-02-15 06:59:22.000000 vulcan-app-1.2/vulcan_app/database/postgre.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      686 2023-01-09 13:08:56.000000 vulcan-app-1.2/vulcan_app/database/tunnel.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     6312 2023-07-21 10:26:33.000000 vulcan-app-1.2/vulcan_app/security.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2442 2023-02-15 10:40:00.000000 vulcan-app-1.2/vulcan_app/services.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2860 2023-07-04 14:18:15.000000 vulcan-app-1.2/vulcan_app/worklog_processor.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-21 10:27:14.105609 vulcan-app-1.2/vulcan_app.egg-info/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-07-21 10:27:14.000000 vulcan-app-1.2/vulcan_app.egg-info/PKG-INFO
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      446 2023-07-21 10:27:14.000000 vulcan-app-1.2/vulcan_app.egg-info/SOURCES.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)        1 2023-07-21 10:27:14.000000 vulcan-app-1.2/vulcan_app.egg-info/dependency_links.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      161 2023-07-21 10:27:14.000000 vulcan-app-1.2/vulcan_app.egg-info/requires.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       11 2023-07-21 10:27:14.000000 vulcan-app-1.2/vulcan_app.egg-info/top_level.txt
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-25 15:55:29.689559 vulcan-app-1.3/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1073 2023-02-15 10:28:00.000000 vulcan-app-1.3/LICENSE
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-07-25 15:55:29.689559 vulcan-app-1.3/PKG-INFO
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       62 2023-02-15 10:28:00.000000 vulcan-app-1.3/README.md
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       38 2023-07-25 15:55:29.689559 vulcan-app-1.3/setup.cfg
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1157 2023-07-25 15:36:45.000000 vulcan-app-1.3/setup.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-25 15:55:29.689559 vulcan-app-1.3/vulcan_app/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      558 2023-07-25 15:37:12.000000 vulcan-app-1.3/vulcan_app/__init__.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      805 2023-02-23 08:06:39.000000 vulcan-app-1.3/vulcan_app/configuration.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-25 15:55:29.689559 vulcan-app-1.3/vulcan_app/database/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1520 2023-02-23 13:43:03.000000 vulcan-app-1.3/vulcan_app/database/__init__.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      251 2023-02-15 06:39:24.000000 vulcan-app-1.3/vulcan_app/database/mongo.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1257 2023-02-15 06:59:22.000000 vulcan-app-1.3/vulcan_app/database/postgre.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      686 2023-01-09 13:08:56.000000 vulcan-app-1.3/vulcan_app/database/tunnel.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     7283 2023-07-25 15:54:54.000000 vulcan-app-1.3/vulcan_app/security.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2442 2023-02-15 10:40:00.000000 vulcan-app-1.3/vulcan_app/services.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2860 2023-07-04 14:18:15.000000 vulcan-app-1.3/vulcan_app/worklog_processor.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-25 15:55:29.689559 vulcan-app-1.3/vulcan_app.egg-info/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-07-25 15:55:29.000000 vulcan-app-1.3/vulcan_app.egg-info/PKG-INFO
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      446 2023-07-25 15:55:29.000000 vulcan-app-1.3/vulcan_app.egg-info/SOURCES.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)        1 2023-07-25 15:55:29.000000 vulcan-app-1.3/vulcan_app.egg-info/dependency_links.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      161 2023-07-25 15:55:29.000000 vulcan-app-1.3/vulcan_app.egg-info/requires.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       11 2023-07-25 15:55:29.000000 vulcan-app-1.3/vulcan_app.egg-info/top_level.txt
```

### Comparing `vulcan-app-1.2/LICENSE` & `vulcan-app-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.2/PKG-INFO` & `vulcan-app-1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-app
-Version: 1.2
+Version: 1.3
 Summary: Vulcan's web application server.
 Home-page: https://github.com/vulcan-coalition/vulcan-app.git
 Author: Chatavut Viriyasuthee
 Author-email: chatavut@lab.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `vulcan-app-1.2/setup.py` & `vulcan-app-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from distutils.core import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="vulcan-app",
-    version="1.2",
+    version="1.3",
     author="Chatavut Viriyasuthee",
     author_email="chatavut@lab.ai",
     description="Vulcan's web application server.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vulcan-coalition/vulcan-app.git",
     packages=["vulcan_app", "vulcan_app.database"],
```

### Comparing `vulcan-app-1.2/vulcan_app/__init__.py` & `vulcan-app-1.3/vulcan_app/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .configuration import initialize as init_config, get_config
 from .security import initialize as init_security, User
 from .services import *
 from .database import initialize as init_db, terminate_connections, Base, TimeStamp
 
 
-def initialize(project_root, fast_api_app=None, security_prefix=""):
+def initialize(project_root, fast_api_app=None, security_prefix="", get_user=None):
     init_config(project_root)
     init_db(configuration.get_config_object())
     if fast_api_app is not None:
-        return init_security(fast_api_app, security_prefix)
+        return init_security(fast_api_app, security_prefix, get_user)
     return None
 
 
 def terminate():
     terminate_connections()
```

### Comparing `vulcan-app-1.2/vulcan_app/configuration.py` & `vulcan-app-1.3/vulcan_app/configuration.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.2/vulcan_app/database/__init__.py` & `vulcan-app-1.3/vulcan_app/database/__init__.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.2/vulcan_app/database/postgre.py` & `vulcan-app-1.3/vulcan_app/database/postgre.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.2/vulcan_app/database/tunnel.py` & `vulcan-app-1.3/vulcan_app/database/tunnel.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.2/vulcan_app/security.py` & `vulcan-app-1.3/vulcan_app/security.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,20 +77,23 @@
 
 class Token(BaseModel):
     access_token: str
     refresh_token: str
     token_type: str
 
 
-def initialize(app, security_prefix=""):
+def initialize(app, security_prefix="", get_user=None):
 
     router = APIRouter(prefix=security_prefix, tags=[security_prefix[1:] if security_prefix.startswith("/") else security_prefix])
 
     @router.post("/exchange", response_model=Token)
     async def exchange_access_token(token: str = Form(...)):
+        """
+            Login as a collab user
+        """
         bypass_security = get_config("test")
         if bypass_security:
             userdata = {'email': "testuser@vulcan", 'disability': 0}
         else:
             result, userdata = await login(token)
             if not result:
                 raise HTTPException(
@@ -105,30 +108,53 @@
     async def refresh_token(refresher: str = Form(...)):
 
         email, disability = decode_token(refresher)
 
         return create_tokens({"email": email, "disability": disability})
 
     @router.post("/token", response_model=Token)
+    @router.post("/admin", response_model=Token)
     async def login_for_admin_token(form_data: OAuth2PasswordRequestForm = Depends()):
+        """
+            Login as a value performanceManager
+        """
         bypass_security = get_config("test")
         if bypass_security:
-            userdata = {'email': "testuser@vulcan", 'data': True}
+            userdata = {'email': "testadmin@vulcan", 'data': True}
         else:
             result, userdata = await admin_login(form_data.username, form_data.password)
             if not result:
                 raise HTTPException(
                     status_code=status.HTTP_401_UNAUTHORIZED,
                     detail="Incorrect username or password",
                     headers={"WWW-Authenticate": "Bearer"},
                 )
             userdata["data"] = True
 
         return create_tokens(userdata)
 
+    @router.post("/login", response_model=Token)
+    async def login(form_data: OAuth2PasswordRequestForm = Depends()):
+        """
+            custom user login (required parameter get_user)
+        """
+        bypass_security = get_config("test")
+        if bypass_security:
+            userdata = {'email': "testuser@vulcan", 'data': False}
+        elif get_user is not None:
+            result, userdata = await get_user(form_data.username, form_data.password)
+            if result:
+                userdata["data"] = False
+                return create_tokens(userdata)
+        raise HTTPException(
+            status_code=status.HTTP_401_UNAUTHORIZED,
+            detail="Incorrect username or password",
+            headers={"WWW-Authenticate": "Bearer"},
+        )
+
     app.include_router(router)
 
     async def get_active_current_user(Authorization: str = Header(None)):
         bypass_security = get_config("test")
         if Authorization is None:
             raise HTTPException(
                 status_code=status.HTTP_401_UNAUTHORIZED,
```

### Comparing `vulcan-app-1.2/vulcan_app/services.py` & `vulcan-app-1.3/vulcan_app/services.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.2/vulcan_app/worklog_processor.py` & `vulcan-app-1.3/vulcan_app/worklog_processor.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.2/vulcan_app.egg-info/PKG-INFO` & `vulcan-app-1.3/vulcan_app.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-app
-Version: 1.2
+Version: 1.3
 Summary: Vulcan's web application server.
 Home-page: https://github.com/vulcan-coalition/vulcan-app.git
 Author: Chatavut Viriyasuthee
 Author-email: chatavut@lab.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

