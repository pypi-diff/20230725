# Comparing `tmp/fastapi-sso-0.6.4.tar.gz` & `tmp/fastapi_sso-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-sso-0.6.4.tar", max compression
+gzip compressed data, was "fastapi_sso-0.7.0.tar", max compression
```

## Comparing `fastapi-sso-0.6.4.tar` & `fastapi_sso-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1093 2021-11-28 22:44:17.300080 fastapi-sso-0.6.4/LICENSE.md
--rw-r--r--   0        0        0     5551 2023-01-16 19:44:21.013975 fastapi-sso-0.6.4/README.md
--rw-r--r--   0        0        0     1110 2022-05-28 08:42:40.443198 fastapi-sso-0.6.4/fastapi_sso/__init__.py
--rw-r--r--   0        0        0        0 2021-11-28 22:44:17.304080 fastapi-sso-0.6.4/fastapi_sso/sso/__init__.py
--rw-r--r--   0        0        0    10181 2023-01-16 19:44:21.021975 fastapi-sso-0.6.4/fastapi_sso/sso/base.py
--rw-r--r--   0        0        0     1215 2022-07-03 07:21:25.017290 fastapi-sso-0.6.4/fastapi_sso/sso/facebook.py
--rw-r--r--   0        0        0     1146 2022-10-21 21:49:05.062354 fastapi-sso-0.6.4/fastapi_sso/sso/fitbit.py
--rw-r--r--   0        0        0     2506 2022-07-03 07:37:27.845664 fastapi-sso-0.6.4/fastapi_sso/sso/generic.py
--rw-r--r--   0        0        0      913 2022-10-21 21:56:07.776974 fastapi-sso-0.6.4/fastapi_sso/sso/github.py
--rw-r--r--   0        0        0     1319 2022-10-21 21:49:05.062354 fastapi-sso-0.6.4/fastapi_sso/sso/google.py
--rw-r--r--   0        0        0      753 2022-07-03 07:20:09.688009 fastapi-sso-0.6.4/fastapi_sso/sso/kakao.py
--rw-r--r--   0        0        0     1574 2023-01-16 19:44:21.021975 fastapi-sso-0.6.4/fastapi_sso/sso/microsoft.py
--rw-r--r--   0        0        0     1172 2022-07-03 07:18:58.038791 fastapi-sso-0.6.4/fastapi_sso/sso/spotify.py
--rw-r--r--   0        0        0      944 2023-01-16 19:44:12.182018 fastapi-sso-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     6594 2023-01-16 19:44:32.667579 fastapi-sso-0.6.4/setup.py
--rw-r--r--   0        0        0     6606 2023-01-16 19:44:32.668908 fastapi-sso-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-02-07 15:13:40.445140 fastapi_sso-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0     6118 2023-07-25 18:36:55.037625 fastapi_sso-0.7.0/README.md
+-rw-r--r--   0        0        0     1110 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/__init__.py
+-rw-r--r--   0        0        0    11117 2023-07-25 18:00:47.042827 fastapi_sso-0.7.0/fastapi_sso/sso/base.py
+-rw-r--r--   0        0        0     1215 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/facebook.py
+-rw-r--r--   0        0        0     1146 2023-03-25 12:01:05.759478 fastapi_sso-0.7.0/fastapi_sso/sso/fitbit.py
+-rw-r--r--   0        0        0     2506 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/generic.py
+-rw-r--r--   0        0        0      913 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/github.py
+-rw-r--r--   0        0        0      920 2023-07-25 18:02:43.979431 fastapi_sso-0.7.0/fastapi_sso/sso/gitlab.py
+-rw-r--r--   0        0        0     1319 2023-03-25 12:01:05.771478 fastapi_sso-0.7.0/fastapi_sso/sso/google.py
+-rw-r--r--   0        0        0      753 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/kakao.py
+-rw-r--r--   0        0        0     1574 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/microsoft.py
+-rw-r--r--   0        0        0      807 2023-07-25 09:20:48.153414 fastapi_sso-0.7.0/fastapi_sso/sso/naver.py
+-rw-r--r--   0        0        0     1172 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/spotify.py
+-rw-r--r--   0        0        0      944 2023-07-25 18:36:55.041625 fastapi_sso-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7224 1970-01-01 00:00:00.000000 fastapi_sso-0.7.0/PKG-INFO
```

### Comparing `fastapi-sso-0.6.4/LICENSE.md` & `fastapi_sso-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastapi-sso-0.6.4/README.md` & `fastapi_sso-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # FastAPI SSO
 
 FastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 account).
 
 This allows you to implement the famous `Login with Google/Facebook/Microsoft` buttons functionality on your backend very easily.
 
+## Security warning
+
+Please note that versions preceding `0.7.0` had a security vulnerability.
+The SSO instance could share state between requests, which could lead to security issues. **Please update to `0.7.0` or newer**.
+
+Also, the preferred way of using the SSO instances is to use `with` statement, which will ensure the state is cleared.
+See example below.
+
 ## Support this project
 
 If you'd like to support this project, consider [buying me a coffee ☕](https://www.buymeacoffee.com/tomas.votava).
 I tend to process Pull Requests faster when properly caffeinated 😉.
 
 <a href="https://www.buymeacoffee.com/tomas.votava" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
 
@@ -22,14 +30,16 @@
 - Fitbit
 - Github (credits to [Brandl](https://github.com/Brandl) for hint using `accept` header)
 - generic (see [docs](https://tomasvotava.github.io/fastapi-sso/sso/generic.html))
 
 ### Contributed
 
 - Kakao (by Jae-Baek Song - [thdwoqor](https://github.com/thdwoqor))
+- Naver (by 1tang2bang92) - [1tang2bang92](https://github.com/1tang2bang92)
+- Gitlab (by Alessandro Pischedda) - [Cereal84](https://github.com/Cereal84)
 
 See [Contributing](#contributing) for a guide on how to contribute your own login provider.
 
 ## Installation
 
 ### Install using `pip`
 
@@ -60,21 +70,23 @@
 app = FastAPI()
 
 google_sso = GoogleSSO("my-client-id", "my-client-secret", "https://my.awesome-web.com/google/callback")
 
 @app.get("/google/login")
 async def google_login():
     """Generate login url and redirect"""
-    return await google_sso.get_login_redirect()
+    with google_sso:
+        return await google_sso.get_login_redirect()
 
 
 @app.get("/google/callback")
 async def google_callback(request: Request):
     """Process login response from Google and return user info"""
-    user = await google_sso.verify_and_process(request)
+    with google_sso:
+        user = await google_sso.verify_and_process(request)
     return {
         "id": user.id,
         "picture": user.picture,
         "display_name": user.display_name,
         "email": user.email,
         "provider": user.provider,
     }
```

#### html2text {}

```diff
@@ -1,39 +1,46 @@
 # FastAPI SSO FastAPI plugin to enable SSO to most common providers (such as
 Facebook login, Google login and login via Microsoft Office 365 account). This
 allows you to implement the famous `Login with Google/Facebook/Microsoft`
-buttons functionality on your backend very easily. ## Support this project If
-you'd like to support this project, consider [buying me a coffee â](https://
-www.buymeacoffee.com/tomas.votava). I tend to process Pull Requests faster when
-properly caffeinated ð. [Buy_Me_A_Coffee] ## Supported login providers ###
-Official - Google - Microsoft - Facebook - Spotify - Fitbit - Github (credits
-to [Brandl](https://github.com/Brandl) for hint using `accept` header) -
-generic (see [docs](https://tomasvotava.github.io/fastapi-sso/sso/
-generic.html)) ### Contributed - Kakao (by Jae-Baek Song - [thdwoqor](https://
-github.com/thdwoqor)) See [Contributing](#contributing) for a guide on how to
-contribute your own login provider. ## Installation ### Install using `pip`
-```console pip install fastapi-sso ``` ### Install using `poetry` ```console
-poetry add fastapi-sso ``` ## Example For more examples, see [`examples`](/
-examples/) directory. ### `example.py` ```python """This is an example usage of
-fastapi-sso. """ from fastapi import FastAPI from starlette.requests import
-Request from fastapi_sso.sso.google import GoogleSSO app = FastAPI() google_sso
-= GoogleSSO("my-client-id", "my-client-secret", "https://my.awesome-web.com/
-google/callback") @app.get("/google/login") async def google_login():
-"""Generate login url and redirect""" return await
+buttons functionality on your backend very easily. ## Security warning Please
+note that versions preceding `0.7.0` had a security vulnerability. The SSO
+instance could share state between requests, which could lead to security
+issues. **Please update to `0.7.0` or newer**. Also, the preferred way of using
+the SSO instances is to use `with` statement, which will ensure the state is
+cleared. See example below. ## Support this project If you'd like to support
+this project, consider [buying me a coffee â](https://www.buymeacoffee.com/
+tomas.votava). I tend to process Pull Requests faster when properly caffeinated
+ð. [Buy_Me_A_Coffee] ## Supported login providers ### Official - Google -
+Microsoft - Facebook - Spotify - Fitbit - Github (credits to [Brandl](https://
+github.com/Brandl) for hint using `accept` header) - generic (see [docs](https:
+//tomasvotava.github.io/fastapi-sso/sso/generic.html)) ### Contributed - Kakao
+(by Jae-Baek Song - [thdwoqor](https://github.com/thdwoqor)) - Naver (by
+1tang2bang92) - [1tang2bang92](https://github.com/1tang2bang92) - Gitlab (by
+Alessandro Pischedda) - [Cereal84](https://github.com/Cereal84) See
+[Contributing](#contributing) for a guide on how to contribute your own login
+provider. ## Installation ### Install using `pip` ```console pip install
+fastapi-sso ``` ### Install using `poetry` ```console poetry add fastapi-sso
+``` ## Example For more examples, see [`examples`](/examples/) directory. ###
+`example.py` ```python """This is an example usage of fastapi-sso. """ from
+fastapi import FastAPI from starlette.requests import Request from
+fastapi_sso.sso.google import GoogleSSO app = FastAPI() google_sso = GoogleSSO
+("my-client-id", "my-client-secret", "https://my.awesome-web.com/google/
+callback") @app.get("/google/login") async def google_login(): """Generate
+login url and redirect""" with google_sso: return await
 google_sso.get_login_redirect() @app.get("/google/callback") async def
 google_callback(request: Request): """Process login response from Google and
-return user info""" user = await google_sso.verify_and_process(request) return
-{ "id": user.id, "picture": user.picture, "display_name": user.display_name,
-"email": user.email, "provider": user.provider, } ``` Run using `uvicorn
-example:app`. ### Specify `redirect_uri` on request time In scenarios you
-cannot provide the `redirect_uri` upon the SSO class initialization, you may
-simply omit the parameter and provide it when calling `get_login_redirect`
-method. ```python ... google_sso = GoogleSSO("my-client-id", "my-client-
-secret") @app.get("/google/login") async def google_login(request: Request):
-"""Generate login url and redirect""" return await
+return user info""" with google_sso: user = await google_sso.verify_and_process
+(request) return { "id": user.id, "picture": user.picture, "display_name":
+user.display_name, "email": user.email, "provider": user.provider, } ``` Run
+using `uvicorn example:app`. ### Specify `redirect_uri` on request time In
+scenarios you cannot provide the `redirect_uri` upon the SSO class
+initialization, you may simply omit the parameter and provide it when calling
+`get_login_redirect` method. ```python ... google_sso = GoogleSSO("my-client-
+id", "my-client-secret") @app.get("/google/login") async def google_login
+(request: Request): """Generate login url and redirect""" return await
 google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"))
 @app.get("/google/callback") async def google_callback(request: Request): ...
 ``` ### Specify scope Since `0.4.0` you may specify `scope` when initializing
 the SSO class. ```python from fastapi_sso.sso.microsoft import MicrosoftSSO sso
 = MicrosoftSSO(client_id="client-id", client_secret="client-secret", scope=
 ["openid", "email"]) ``` ### Additional query parameters Since `0.4.0` you may
 provide additional query parameters to be sent to the login screen. E.g.
```

### Comparing `fastapi-sso-0.6.4/fastapi_sso/__init__.py` & `fastapi_sso-0.7.0/fastapi_sso/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi-sso-0.6.4/fastapi_sso/sso/base.py` & `fastapi_sso-0.7.0/fastapi_sso/sso/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """SSO login base dependency
 """
 # pylint: disable=too-few-public-methods
 
 import json
 import sys
 import warnings
-from typing import Any, Dict, List, Optional
+from types import TracebackType
+from typing import Any, Dict, List, Optional, Type
 
 import httpx
 import pydantic
 from oauthlib.oauth2 import WebApplicationClient
 from starlette.exceptions import HTTPException
 from starlette.requests import Request
 from starlette.responses import RedirectResponse
@@ -24,14 +25,18 @@
 )
 
 
 class UnsetStateWarning(UserWarning):
     """Warning about unset state parameter"""
 
 
+class ReusedOauthClientWarning(UserWarning):
+    """Warning about reused oauth client instance"""
+
+
 class SSOLoginError(HTTPException):
     """Raised when any login-related error ocurrs
     (such as when user is not verified or if there was an attempt for fake login)
     """
 
 
 class OpenID(pydantic.BaseModel):  # pylint: disable=no-member
@@ -51,15 +56,14 @@
     """Base class (mixin) for all SSO providers"""
 
     provider: str = NotImplemented
     client_id: str = NotImplemented
     client_secret: str = NotImplemented
     redirect_uri: Optional[str] = NotImplemented
     scope: List[str] = NotImplemented
-    _oauth_client: Optional[WebApplicationClient] = None
     additional_headers: Optional[Dict[str, Any]] = None
 
     def __init__(
         self,
         client_id: str,
         client_secret: str,
         redirect_uri: Optional[str] = None,
@@ -68,14 +72,15 @@
         scope: Optional[List[str]] = None,
     ):
         # pylint: disable=too-many-arguments
         self.client_id = client_id
         self.client_secret = client_secret
         self.redirect_uri = redirect_uri
         self.allow_insecure_http = allow_insecure_http
+        self._oauth_client: Optional[WebApplicationClient] = None
         # TODO: Remove use_state argument and attribute
         if use_state:
             warnings.warn(
                 (
                     "Argument 'use_state' of SSOBase's constructor is deprecated and will be removed in "
                     "future releases. Use 'state' argument of individual methods instead."
                 ),
@@ -204,14 +209,27 @@
         if code is None:
             raise SSOLoginError(400, "'code' parameter was not found in callback request")
         self._state = request.query_params.get("state")
         return await self.process_login(
             code, request, params=params, additional_headers=headers, redirect_uri=redirect_uri
         )
 
+    def __enter__(self) -> "SSOBase":
+        self._oauth_client = None
+        self._refresh_token = None
+        return self
+
+    def __exit__(
+        self,
+        _exc_type: Optional[Type[BaseException]],
+        _exc_val: Optional[BaseException],
+        _exc_tb: Optional[TracebackType],
+    ) -> None:
+        return None
+
     async def process_login(
         self,
         code: str,
         request: Request,
         *,
         params: Optional[Dict[str, Any]] = None,
         additional_headers: Optional[Dict[str, Any]] = None,
@@ -221,14 +239,24 @@
         This is low level, you should use {verify_and_process} instead.
 
         Arguments:
             params {Optional[Dict[str, Any]]} -- Optional additional query parameters to pass to the provider
             additional_headers {Optional[Dict[str, Any]]} -- Optional additional headers to be added to all requests
         """
         # pylint: disable=too-many-locals
+        if self._oauth_client is not None:
+            self._oauth_client = None
+            self._refresh_token = None
+            warnings.warn(
+                (
+                    "Reusing the SSO object is not safe and caused a security issue in previous versions."
+                    "To make sure you don't see this warning, please use the SSO object as a context manager."
+                ),
+                ReusedOauthClientWarning,
+            )
         params = params or {}
         additional_headers = additional_headers or {}
         additional_headers.update(self.additional_headers or {})
         url = request.url
         scheme = url.scheme
         if not self.allow_insecure_http and scheme != "https":
             current_url = str(url).replace("http://", "https://")
```

### Comparing `fastapi-sso-0.6.4/fastapi_sso/sso/facebook.py` & `fastapi_sso-0.7.0/fastapi_sso/sso/facebook.py`

 * *Files identical despite different names*

### Comparing `fastapi-sso-0.6.4/fastapi_sso/sso/fitbit.py` & `fastapi_sso-0.7.0/fastapi_sso/sso/fitbit.py`

 * *Files identical despite different names*

### Comparing `fastapi-sso-0.6.4/fastapi_sso/sso/generic.py` & `fastapi_sso-0.7.0/fastapi_sso/sso/generic.py`

 * *Files identical despite different names*

### Comparing `fastapi-sso-0.6.4/fastapi_sso/sso/github.py` & `fastapi_sso-0.7.0/fastapi_sso/sso/github.py`

 * *Files identical despite different names*

### Comparing `fastapi-sso-0.6.4/fastapi_sso/sso/google.py` & `fastapi_sso-0.7.0/fastapi_sso/sso/google.py`

 * *Files identical despite different names*

### Comparing `fastapi-sso-0.6.4/fastapi_sso/sso/kakao.py` & `fastapi_sso-0.7.0/fastapi_sso/sso/kakao.py`

 * *Files identical despite different names*

### Comparing `fastapi-sso-0.6.4/fastapi_sso/sso/microsoft.py` & `fastapi_sso-0.7.0/fastapi_sso/sso/microsoft.py`

 * *Files identical despite different names*

### Comparing `fastapi-sso-0.6.4/fastapi_sso/sso/spotify.py` & `fastapi_sso-0.7.0/fastapi_sso/sso/spotify.py`

 * *Files identical despite different names*

### Comparing `fastapi-sso-0.6.4/pyproject.toml` & `fastapi_sso-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-sso"
-version = "0.6.4"
+version = "0.7.0"
 description = "FastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 Account)"
 authors = ["Tomas Votava <info@tomasvotava.eu>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/tomasvotava/fastapi-sso"
 homepage = "https://tomasvotava.github.io/fastapi-sso/"
 documentation = "https://tomasvotava.github.io/fastapi-sso/"
```

### Comparing `fastapi-sso-0.6.4/setup.py` & `fastapi_sso-0.7.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,219 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fastapi-sso
+Version: 0.7.0
+Summary: FastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 Account)
+Home-page: https://tomasvotava.github.io/fastapi-sso/
+License: MIT
+Keywords: fastapi,sso,oauth,google,facebook,spotify
+Author: Tomas Votava
+Author-email: info@tomasvotava.eu
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fastapi (<1)
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: oauthlib (>=3.1.0)
+Requires-Dist: pydantic (>=1.8.1)
+Requires-Dist: starlette (>=0.13.6)
+Project-URL: Documentation, https://tomasvotava.github.io/fastapi-sso/
+Project-URL: Repository, https://github.com/tomasvotava/fastapi-sso
+Description-Content-Type: text/markdown
 
-packages = \
-['fastapi_sso', 'fastapi_sso.sso']
+# FastAPI SSO
 
-package_data = \
-{'': ['*']}
+FastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 account).
 
-install_requires = \
-['fastapi<1',
- 'httpx>=0.23.0,<0.24.0',
- 'oauthlib>=3.1.0',
- 'pydantic>=1.8.1',
- 'starlette>=0.13.6']
-
-setup_kwargs = {
-    'name': 'fastapi-sso',
-    'version': '0.6.4',
-    'description': 'FastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 Account)',
-    'long_description': '# FastAPI SSO\n\nFastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 account).\n\nThis allows you to implement the famous `Login with Google/Facebook/Microsoft` buttons functionality on your backend very easily.\n\n## Support this project\n\nIf you\'d like to support this project, consider [buying me a coffee ☕](https://www.buymeacoffee.com/tomas.votava).\nI tend to process Pull Requests faster when properly caffeinated 😉.\n\n<a href="https://www.buymeacoffee.com/tomas.votava" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>\n\n## Supported login providers\n\n### Official\n\n- Google\n- Microsoft\n- Facebook\n- Spotify\n- Fitbit\n- Github (credits to [Brandl](https://github.com/Brandl) for hint using `accept` header)\n- generic (see [docs](https://tomasvotava.github.io/fastapi-sso/sso/generic.html))\n\n### Contributed\n\n- Kakao (by Jae-Baek Song - [thdwoqor](https://github.com/thdwoqor))\n\nSee [Contributing](#contributing) for a guide on how to contribute your own login provider.\n\n## Installation\n\n### Install using `pip`\n\n```console\npip install fastapi-sso\n```\n\n### Install using `poetry`\n\n```console\npoetry add fastapi-sso\n```\n\n## Example\n\nFor more examples, see [`examples`](/examples/) directory.\n\n### `example.py`\n\n```python\n"""This is an example usage of fastapi-sso.\n"""\n\nfrom fastapi import FastAPI\nfrom starlette.requests import Request\nfrom fastapi_sso.sso.google import GoogleSSO\n\napp = FastAPI()\n\ngoogle_sso = GoogleSSO("my-client-id", "my-client-secret", "https://my.awesome-web.com/google/callback")\n\n@app.get("/google/login")\nasync def google_login():\n    """Generate login url and redirect"""\n    return await google_sso.get_login_redirect()\n\n\n@app.get("/google/callback")\nasync def google_callback(request: Request):\n    """Process login response from Google and return user info"""\n    user = await google_sso.verify_and_process(request)\n    return {\n        "id": user.id,\n        "picture": user.picture,\n        "display_name": user.display_name,\n        "email": user.email,\n        "provider": user.provider,\n    }\n```\n\nRun using `uvicorn example:app`.\n\n### Specify `redirect_uri` on request time\n\nIn scenarios you cannot provide the `redirect_uri` upon the SSO class initialization, you may simply omit\nthe parameter and provide it when calling `get_login_redirect` method.\n\n```python\n...\n\ngoogle_sso = GoogleSSO("my-client-id", "my-client-secret")\n\n@app.get("/google/login")\nasync def google_login(request: Request):\n    """Generate login url and redirect"""\n    return await google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"))\n\n@app.get("/google/callback")\nasync def google_callback(request: Request):\n    ...\n```\n\n### Specify scope\n\nSince `0.4.0` you may specify `scope` when initializing the SSO class.\n\n```python\nfrom fastapi_sso.sso.microsoft import MicrosoftSSO\n\nsso = MicrosoftSSO(client_id="client-id", client_secret="client-secret", scope=["openid", "email"])\n```\n\n### Additional query parameters\n\nSince `0.4.0` you may provide additional query parameters to be\nsent to the login screen.\n\nE.g. sometimes you want to specify `access_type=offline` or `prompt=consent` in order for\nGoogle to return `refresh_token`.\n\n```python\nasync def google_login(request: Request):\n    return await google_sso.get_login_redirect(\n        redirect_uri=request.url_for("google_callback"),\n        params={"prompt": "consent", "access_type": "offline"}\n        )\n\n```\n\n## HTTP and development\n\n**You should always use `https` in production**. But in case you need to test on `localhost` and do not want to\nuse self-signed certificate, make sure you set up redirect uri within your SSO provider to `http://localhost:{port}`\nand then add this to your environment:\n\n```bash\nOAUTHLIB_INSECURE_TRANSPORT=1\n```\n\nAnd make sure you pass `allow_insecure_http = True` to SSO class\' constructor, such as:\n\n```python\ngoogle_sso = GoogleSSO("client-id", "client-secret", allow_insecure_http=True)\n```\n\nSee [this issue](https://github.com/tomasvotava/fastapi-sso/issues/2) for more information.\n\n## State\n\nState is useful if you want the server to return something back to you to help you understand in what\ncontext the authentication was initiated. It is mostly used to store the url you want your user to be redirected\nto after successful login. You may use `.state` property to get the state returned from the server.\n\nExample:\n\n```python\nfrom fastapi import Request\nfrom fastapi.responses import RedirectResponse\n\n# E.g. https://example.com/auth/login?return_url=https://example.com/welcome\nasync def google_login(return_url: str):\n    google_sso = GoogleSOO("client-id", "client-secret")\n    # Send return_url to Google as a state so that Google knows to return it back to us\n    return await google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"), state=return_url)\n\nasync def google_callback(request: Request):\n    google_sso = GoogleSOO("client-id", "client-secret")\n    user = await google_sso.verify_and_process(request)\n    # google_sso.state now holds your return_url (https://example.com/welcome)\n    return RedirectResponse(google_sso.state)\n\n```\n\n**Deprecation Warning**: legacy `use_state` argument in `SSOBase` constructor is deprecated and will be removed.\n\n## Contributing\n\nIf you\'d like to contribute and add your specific login provider, please see [CONTRIBUTING.md](CONTRIBUTING.md) file.\n',
-    'author': 'Tomas Votava',
-    'author_email': 'info@tomasvotava.eu',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://tomasvotava.github.io/fastapi-sso/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+This allows you to implement the famous `Login with Google/Facebook/Microsoft` buttons functionality on your backend very easily.
 
+## Security warning
+
+Please note that versions preceding `0.7.0` had a security vulnerability.
+The SSO instance could share state between requests, which could lead to security issues. **Please update to `0.7.0` or newer**.
+
+Also, the preferred way of using the SSO instances is to use `with` statement, which will ensure the state is cleared.
+See example below.
+
+## Support this project
+
+If you'd like to support this project, consider [buying me a coffee ☕](https://www.buymeacoffee.com/tomas.votava).
+I tend to process Pull Requests faster when properly caffeinated 😉.
+
+<a href="https://www.buymeacoffee.com/tomas.votava" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
+
+## Supported login providers
+
+### Official
+
+- Google
+- Microsoft
+- Facebook
+- Spotify
+- Fitbit
+- Github (credits to [Brandl](https://github.com/Brandl) for hint using `accept` header)
+- generic (see [docs](https://tomasvotava.github.io/fastapi-sso/sso/generic.html))
+
+### Contributed
+
+- Kakao (by Jae-Baek Song - [thdwoqor](https://github.com/thdwoqor))
+- Naver (by 1tang2bang92) - [1tang2bang92](https://github.com/1tang2bang92)
+- Gitlab (by Alessandro Pischedda) - [Cereal84](https://github.com/Cereal84)
+
+See [Contributing](#contributing) for a guide on how to contribute your own login provider.
+
+## Installation
+
+### Install using `pip`
+
+```console
+pip install fastapi-sso
+```
+
+### Install using `poetry`
+
+```console
+poetry add fastapi-sso
+```
+
+## Example
+
+For more examples, see [`examples`](/examples/) directory.
+
+### `example.py`
+
+```python
+"""This is an example usage of fastapi-sso.
+"""
+
+from fastapi import FastAPI
+from starlette.requests import Request
+from fastapi_sso.sso.google import GoogleSSO
+
+app = FastAPI()
+
+google_sso = GoogleSSO("my-client-id", "my-client-secret", "https://my.awesome-web.com/google/callback")
+
+@app.get("/google/login")
+async def google_login():
+    """Generate login url and redirect"""
+    with google_sso:
+        return await google_sso.get_login_redirect()
+
+
+@app.get("/google/callback")
+async def google_callback(request: Request):
+    """Process login response from Google and return user info"""
+    with google_sso:
+        user = await google_sso.verify_and_process(request)
+    return {
+        "id": user.id,
+        "picture": user.picture,
+        "display_name": user.display_name,
+        "email": user.email,
+        "provider": user.provider,
+    }
+```
+
+Run using `uvicorn example:app`.
+
+### Specify `redirect_uri` on request time
+
+In scenarios you cannot provide the `redirect_uri` upon the SSO class initialization, you may simply omit
+the parameter and provide it when calling `get_login_redirect` method.
+
+```python
+...
+
+google_sso = GoogleSSO("my-client-id", "my-client-secret")
+
+@app.get("/google/login")
+async def google_login(request: Request):
+    """Generate login url and redirect"""
+    return await google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"))
+
+@app.get("/google/callback")
+async def google_callback(request: Request):
+    ...
+```
+
+### Specify scope
+
+Since `0.4.0` you may specify `scope` when initializing the SSO class.
+
+```python
+from fastapi_sso.sso.microsoft import MicrosoftSSO
+
+sso = MicrosoftSSO(client_id="client-id", client_secret="client-secret", scope=["openid", "email"])
+```
+
+### Additional query parameters
+
+Since `0.4.0` you may provide additional query parameters to be
+sent to the login screen.
+
+E.g. sometimes you want to specify `access_type=offline` or `prompt=consent` in order for
+Google to return `refresh_token`.
+
+```python
+async def google_login(request: Request):
+    return await google_sso.get_login_redirect(
+        redirect_uri=request.url_for("google_callback"),
+        params={"prompt": "consent", "access_type": "offline"}
+        )
+
+```
+
+## HTTP and development
+
+**You should always use `https` in production**. But in case you need to test on `localhost` and do not want to
+use self-signed certificate, make sure you set up redirect uri within your SSO provider to `http://localhost:{port}`
+and then add this to your environment:
+
+```bash
+OAUTHLIB_INSECURE_TRANSPORT=1
+```
+
+And make sure you pass `allow_insecure_http = True` to SSO class' constructor, such as:
+
+```python
+google_sso = GoogleSSO("client-id", "client-secret", allow_insecure_http=True)
+```
+
+See [this issue](https://github.com/tomasvotava/fastapi-sso/issues/2) for more information.
+
+## State
+
+State is useful if you want the server to return something back to you to help you understand in what
+context the authentication was initiated. It is mostly used to store the url you want your user to be redirected
+to after successful login. You may use `.state` property to get the state returned from the server.
+
+Example:
+
+```python
+from fastapi import Request
+from fastapi.responses import RedirectResponse
+
+# E.g. https://example.com/auth/login?return_url=https://example.com/welcome
+async def google_login(return_url: str):
+    google_sso = GoogleSOO("client-id", "client-secret")
+    # Send return_url to Google as a state so that Google knows to return it back to us
+    return await google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"), state=return_url)
+
+async def google_callback(request: Request):
+    google_sso = GoogleSOO("client-id", "client-secret")
+    user = await google_sso.verify_and_process(request)
+    # google_sso.state now holds your return_url (https://example.com/welcome)
+    return RedirectResponse(google_sso.state)
+
+```
+
+**Deprecation Warning**: legacy `use_state` argument in `SSOBase` constructor is deprecated and will be removed.
+
+## Contributing
+
+If you'd like to contribute and add your specific login provider, please see [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,84 +1,91 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['fastapi_sso', 'fastapi_sso.sso'] package_data = \ {'': ['*']}
-install_requires = \ ['fastapi<1', 'httpx>=0.23.0,<0.24.0', 'oauthlib>=3.1.0',
-'pydantic>=1.8.1', 'starlette>=0.13.6'] setup_kwargs = { 'name': 'fastapi-sso',
-'version': '0.6.4', 'description': 'FastAPI plugin to enable SSO to most common
-providers (such as Facebook login, Google login and login via Microsoft Office
-365 Account)', 'long_description': '# FastAPI SSO\n\nFastAPI plugin to enable
-SSO to most common providers (such as Facebook login, Google login and login
-via Microsoft Office 365 account).\n\nThis allows you to implement the famous
-`Login with Google/Facebook/Microsoft` buttons functionality on your backend
-very easily.\n\n## Support this project\n\nIf you\'d like to support this
-project, consider [buying me a coffee â](https://www.buymeacoffee.com/
-tomas.votava).\nI tend to process Pull Requests faster when properly
-caffeinated ð.\n\n[Buy_Me_A_Coffee]\n\n## Supported login providers\n\n###
-Official\n\n- Google\n- Microsoft\n- Facebook\n- Spotify\n- Fitbit\n- Github
-(credits to [Brandl](https://github.com/Brandl) for hint using `accept`
-header)\n- generic (see [docs](https://tomasvotava.github.io/fastapi-sso/sso/
-generic.html))\n\n### Contributed\n\n- Kakao (by Jae-Baek Song - [thdwoqor]
-(https://github.com/thdwoqor))\n\nSee [Contributing](#contributing) for a guide
-on how to contribute your own login provider.\n\n## Installation\n\n### Install
-using `pip`\n\n```console\npip install fastapi-sso\n```\n\n### Install using
-`poetry`\n\n```console\npoetry add fastapi-sso\n```\n\n## Example\n\nFor more
-examples, see [`examples`](/examples/) directory.\n\n###
-`example.py`\n\n```python\n"""This is an example usage of fastapi-
-sso.\n"""\n\nfrom fastapi import FastAPI\nfrom starlette.requests import
-Request\nfrom fastapi_sso.sso.google import GoogleSSO\n\napp = FastAPI
-()\n\ngoogle_sso = GoogleSSO("my-client-id", "my-client-secret", "https://
-my.awesome-web.com/google/callback")\n\n@app.get("/google/login")\nasync def
-google_login():\n """Generate login url and redirect"""\n return await
-google_sso.get_login_redirect()\n\n\n@app.get("/google/callback")\nasync def
-google_callback(request: Request):\n """Process login response from Google and
-return user info"""\n user = await google_sso.verify_and_process(request)\n
-return {\n "id": user.id,\n "picture": user.picture,\n "display_name":
-user.display_name,\n "email": user.email,\n "provider": user.provider,\n
-}\n```\n\nRun using `uvicorn example:app`.\n\n### Specify `redirect_uri` on
-request time\n\nIn scenarios you cannot provide the `redirect_uri` upon the SSO
-class initialization, you may simply omit\nthe parameter and provide it when
-calling `get_login_redirect` method.\n\n```python\n...\n\ngoogle_sso =
-GoogleSSO("my-client-id", "my-client-secret")\n\n@app.get("/google/
-login")\nasync def google_login(request: Request):\n """Generate login url and
-redirect"""\n return await google_sso.get_login_redirect
-(redirect_uri=request.url_for("google_callback"))\n\n@app.get("/google/
-callback")\nasync def google_callback(request: Request):\n ...\n```\n\n###
-Specify scope\n\nSince `0.4.0` you may specify `scope` when initializing the
-SSO class.\n\n```python\nfrom fastapi_sso.sso.microsoft import
-MicrosoftSSO\n\nsso = MicrosoftSSO(client_id="client-id",
-client_secret="client-secret", scope=["openid", "email"])\n```\n\n###
-Additional query parameters\n\nSince `0.4.0` you may provide additional query
-parameters to be\nsent to the login screen.\n\nE.g. sometimes you want to
-specify `access_type=offline` or `prompt=consent` in order for\nGoogle to
-return `refresh_token`.\n\n```python\nasync def google_login(request: Request):
-\n return await google_sso.get_login_redirect(\n redirect_uri=request.url_for
-("google_callback"),\n params={"prompt": "consent", "access_type": "offline"}\n
-)\n\n```\n\n## HTTP and development\n\n**You should always use `https` in
-production**. But in case you need to test on `localhost` and do not want
-to\nuse self-signed certificate, make sure you set up redirect uri within your
-SSO provider to `http://localhost:{port}`\nand then add this to your
-environment:\n\n```bash\nOAUTHLIB_INSECURE_TRANSPORT=1\n```\n\nAnd make sure
-you pass `allow_insecure_http = True` to SSO class\' constructor, such as:
-\n\n```python\ngoogle_sso = GoogleSSO("client-id", "client-secret",
-allow_insecure_http=True)\n```\n\nSee [this issue](https://github.com/
-tomasvotava/fastapi-sso/issues/2) for more information.\n\n## State\n\nState is
-useful if you want the server to return something back to you to help you
-understand in what\ncontext the authentication was initiated. It is mostly used
-to store the url you want your user to be redirected\nto after successful
-login. You may use `.state` property to get the state returned from the
-server.\n\nExample:\n\n```python\nfrom fastapi import Request\nfrom
-fastapi.responses import RedirectResponse\n\n# E.g. https://example.com/auth/
-login?return_url=https://example.com/welcome\nasync def google_login
-(return_url: str):\n google_sso = GoogleSOO("client-id", "client-secret")\n #
-Send return_url to Google as a state so that Google knows to return it back to
-us\n return await google_sso.get_login_redirect(redirect_uri=request.url_for
-("google_callback"), state=return_url)\n\nasync def google_callback(request:
-Request):\n google_sso = GoogleSOO("client-id", "client-secret")\n user = await
-google_sso.verify_and_process(request)\n # google_sso.state now holds your
-return_url (https://example.com/welcome)\n return RedirectResponse
-(google_sso.state)\n\n```\n\n**Deprecation Warning**: legacy `use_state`
-argument in `SSOBase` constructor is deprecated and will be removed.\n\n##
-Contributing\n\nIf you\'d like to contribute and add your specific login
-provider, please see [CONTRIBUTING.md](CONTRIBUTING.md) file.\n', 'author':
-'Tomas Votava', 'author_email': 'info@tomasvotava.eu', 'maintainer': None,
-'maintainer_email': None, 'url': 'https://tomasvotava.github.io/fastapi-sso/',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: fastapi-sso Version: 0.7.0 Summary: FastAPI plugin
+to enable SSO to most common providers (such as Facebook login, Google login
+and login via Microsoft Office 365 Account) Home-page: https://
+tomasvotava.github.io/fastapi-sso/ License: MIT Keywords:
+fastapi,sso,oauth,google,facebook,spotify Author: Tomas Votava Author-email:
+info@tomasvotava.eu Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: fastapi (<1) Requires-Dist: httpx
+(>=0.23.0,<0.24.0) Requires-Dist: oauthlib (>=3.1.0) Requires-Dist: pydantic
+(>=1.8.1) Requires-Dist: starlette (>=0.13.6) Project-URL: Documentation,
+https://tomasvotava.github.io/fastapi-sso/ Project-URL: Repository, https://
+github.com/tomasvotava/fastapi-sso Description-Content-Type: text/markdown #
+FastAPI SSO FastAPI plugin to enable SSO to most common providers (such as
+Facebook login, Google login and login via Microsoft Office 365 account). This
+allows you to implement the famous `Login with Google/Facebook/Microsoft`
+buttons functionality on your backend very easily. ## Security warning Please
+note that versions preceding `0.7.0` had a security vulnerability. The SSO
+instance could share state between requests, which could lead to security
+issues. **Please update to `0.7.0` or newer**. Also, the preferred way of using
+the SSO instances is to use `with` statement, which will ensure the state is
+cleared. See example below. ## Support this project If you'd like to support
+this project, consider [buying me a coffee â](https://www.buymeacoffee.com/
+tomas.votava). I tend to process Pull Requests faster when properly caffeinated
+ð. [Buy_Me_A_Coffee] ## Supported login providers ### Official - Google -
+Microsoft - Facebook - Spotify - Fitbit - Github (credits to [Brandl](https://
+github.com/Brandl) for hint using `accept` header) - generic (see [docs](https:
+//tomasvotava.github.io/fastapi-sso/sso/generic.html)) ### Contributed - Kakao
+(by Jae-Baek Song - [thdwoqor](https://github.com/thdwoqor)) - Naver (by
+1tang2bang92) - [1tang2bang92](https://github.com/1tang2bang92) - Gitlab (by
+Alessandro Pischedda) - [Cereal84](https://github.com/Cereal84) See
+[Contributing](#contributing) for a guide on how to contribute your own login
+provider. ## Installation ### Install using `pip` ```console pip install
+fastapi-sso ``` ### Install using `poetry` ```console poetry add fastapi-sso
+``` ## Example For more examples, see [`examples`](/examples/) directory. ###
+`example.py` ```python """This is an example usage of fastapi-sso. """ from
+fastapi import FastAPI from starlette.requests import Request from
+fastapi_sso.sso.google import GoogleSSO app = FastAPI() google_sso = GoogleSSO
+("my-client-id", "my-client-secret", "https://my.awesome-web.com/google/
+callback") @app.get("/google/login") async def google_login(): """Generate
+login url and redirect""" with google_sso: return await
+google_sso.get_login_redirect() @app.get("/google/callback") async def
+google_callback(request: Request): """Process login response from Google and
+return user info""" with google_sso: user = await google_sso.verify_and_process
+(request) return { "id": user.id, "picture": user.picture, "display_name":
+user.display_name, "email": user.email, "provider": user.provider, } ``` Run
+using `uvicorn example:app`. ### Specify `redirect_uri` on request time In
+scenarios you cannot provide the `redirect_uri` upon the SSO class
+initialization, you may simply omit the parameter and provide it when calling
+`get_login_redirect` method. ```python ... google_sso = GoogleSSO("my-client-
+id", "my-client-secret") @app.get("/google/login") async def google_login
+(request: Request): """Generate login url and redirect""" return await
+google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"))
+@app.get("/google/callback") async def google_callback(request: Request): ...
+``` ### Specify scope Since `0.4.0` you may specify `scope` when initializing
+the SSO class. ```python from fastapi_sso.sso.microsoft import MicrosoftSSO sso
+= MicrosoftSSO(client_id="client-id", client_secret="client-secret", scope=
+["openid", "email"]) ``` ### Additional query parameters Since `0.4.0` you may
+provide additional query parameters to be sent to the login screen. E.g.
+sometimes you want to specify `access_type=offline` or `prompt=consent` in
+order for Google to return `refresh_token`. ```python async def google_login
+(request: Request): return await google_sso.get_login_redirect
+( redirect_uri=request.url_for("google_callback"), params={"prompt": "consent",
+"access_type": "offline"} ) ``` ## HTTP and development **You should always use
+`https` in production**. But in case you need to test on `localhost` and do not
+want to use self-signed certificate, make sure you set up redirect uri within
+your SSO provider to `http://localhost:{port}` and then add this to your
+environment: ```bash OAUTHLIB_INSECURE_TRANSPORT=1 ``` And make sure you pass
+`allow_insecure_http = True` to SSO class' constructor, such as: ```python
+google_sso = GoogleSSO("client-id", "client-secret", allow_insecure_http=True)
+``` See [this issue](https://github.com/tomasvotava/fastapi-sso/issues/2) for
+more information. ## State State is useful if you want the server to return
+something back to you to help you understand in what context the authentication
+was initiated. It is mostly used to store the url you want your user to be
+redirected to after successful login. You may use `.state` property to get the
+state returned from the server. Example: ```python from fastapi import Request
+from fastapi.responses import RedirectResponse # E.g. https://example.com/auth/
+login?return_url=https://example.com/welcome async def google_login(return_url:
+str): google_sso = GoogleSOO("client-id", "client-secret") # Send return_url to
+Google as a state so that Google knows to return it back to us return await
+google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"),
+state=return_url) async def google_callback(request: Request): google_sso =
+GoogleSOO("client-id", "client-secret") user = await
+google_sso.verify_and_process(request) # google_sso.state now holds your
+return_url (https://example.com/welcome) return RedirectResponse
+(google_sso.state) ``` **Deprecation Warning**: legacy `use_state` argument in
+`SSOBase` constructor is deprecated and will be removed. ## Contributing If
+you'd like to contribute and add your specific login provider, please see
+[CONTRIBUTING.md](CONTRIBUTING.md) file.
```

