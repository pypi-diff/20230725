# Comparing `tmp/bkpaas-auth-2.0.5.tar.gz` & `tmp/bkpaas-auth-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkpaas-auth-2.0.5.tar", max compression
+gzip compressed data, was "bkpaas-auth-2.0.6.tar", max compression
```

## Comparing `bkpaas-auth-2.0.5.tar` & `bkpaas-auth-2.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     5197 2023-07-19 09:05:35.796657 bkpaas-auth-2.0.5/README.md
--rw-r--r--   0        0        0     1012 2023-07-19 09:05:35.797268 bkpaas-auth-2.0.5/bkpaas_auth/__init__.py
--rw-r--r--   0        0        0      191 2023-07-19 09:05:35.797573 bkpaas-auth-2.0.5/bkpaas_auth/apps.py
--rw-r--r--   0        0        0     8202 2023-07-19 09:05:35.797836 bkpaas-auth-2.0.5/bkpaas_auth/backends.py
--rw-r--r--   0        0        0     2526 2023-07-19 09:05:35.798113 bkpaas-auth-2.0.5/bkpaas_auth/conf.py
--rw-r--r--   0        0        0        0 2023-07-19 09:05:35.798368 bkpaas-auth-2.0.5/bkpaas_auth/core/__init__.py
--rw-r--r--   0        0        0      346 2023-07-19 09:05:35.798564 bkpaas-auth-2.0.5/bkpaas_auth/core/constants.py
--rw-r--r--   0        0        0     2302 2023-07-19 09:05:35.799097 bkpaas-auth-2.0.5/bkpaas_auth/core/encoder.py
--rw-r--r--   0        0        0      437 2023-07-19 09:05:35.799386 bkpaas-auth-2.0.5/bkpaas_auth/core/exceptions.py
--rw-r--r--   0        0        0     2167 2023-07-19 09:05:35.799655 bkpaas-auth-2.0.5/bkpaas_auth/core/http.py
--rw-r--r--   0        0        0     1173 2023-07-19 09:05:35.800113 bkpaas-auth-2.0.5/bkpaas_auth/core/plugins.py
--rw-r--r--   0        0        0     3132 2023-07-19 09:05:35.800389 bkpaas-auth-2.0.5/bkpaas_auth/core/services.py
--rw-r--r--   0        0        0     4167 2023-07-19 09:05:35.800698 bkpaas-auth-2.0.5/bkpaas_auth/core/token.py
--rw-r--r--   0        0        0     2493 2023-07-19 09:05:35.800936 bkpaas-auth-2.0.5/bkpaas_auth/core/user_info.py
--rw-r--r--   0        0        0      641 2023-07-19 09:05:35.801156 bkpaas-auth-2.0.5/bkpaas_auth/core/utils.py
--rw-r--r--   0        0        0     4041 2023-07-19 09:05:35.801399 bkpaas-auth-2.0.5/bkpaas_auth/middlewares.py
--rw-r--r--   0        0        0     3368 2023-07-19 09:05:35.801614 bkpaas-auth-2.0.5/bkpaas_auth/models.py
--rw-r--r--   0        0        0     1263 2023-07-19 09:05:35.801829 bkpaas-auth-2.0.5/bkpaas_auth/monkey.py
--rw-r--r--   0        0        0     1267 2023-07-19 09:05:35.802640 bkpaas-auth-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     6058 2023-07-19 09:06:31.625674 bkpaas-auth-2.0.5/setup.py
--rw-r--r--   0        0        0     5927 2023-07-19 09:06:31.626430 bkpaas-auth-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     5197 2023-07-25 02:38:43.140092 bkpaas-auth-2.0.6/README.md
+-rw-r--r--   0        0        0     1012 2023-07-25 02:38:43.140936 bkpaas-auth-2.0.6/bkpaas_auth/__init__.py
+-rw-r--r--   0        0        0      191 2023-07-25 02:38:43.141167 bkpaas-auth-2.0.6/bkpaas_auth/apps.py
+-rw-r--r--   0        0        0     8202 2023-07-25 02:38:43.141406 bkpaas-auth-2.0.6/bkpaas_auth/backends.py
+-rw-r--r--   0        0        0     2526 2023-07-25 02:38:43.141619 bkpaas-auth-2.0.6/bkpaas_auth/conf.py
+-rw-r--r--   0        0        0        0 2023-07-25 02:38:43.141818 bkpaas-auth-2.0.6/bkpaas_auth/core/__init__.py
+-rw-r--r--   0        0        0      346 2023-07-25 02:38:43.141991 bkpaas-auth-2.0.6/bkpaas_auth/core/constants.py
+-rw-r--r--   0        0        0     2302 2023-07-25 02:38:43.142372 bkpaas-auth-2.0.6/bkpaas_auth/core/encoder.py
+-rw-r--r--   0        0        0      437 2023-07-25 02:38:43.142577 bkpaas-auth-2.0.6/bkpaas_auth/core/exceptions.py
+-rw-r--r--   0        0        0     2167 2023-07-25 02:38:43.142779 bkpaas-auth-2.0.6/bkpaas_auth/core/http.py
+-rw-r--r--   0        0        0     1173 2023-07-25 02:38:43.142994 bkpaas-auth-2.0.6/bkpaas_auth/core/plugins.py
+-rw-r--r--   0        0        0     3132 2023-07-25 02:38:43.143207 bkpaas-auth-2.0.6/bkpaas_auth/core/services.py
+-rw-r--r--   0        0        0     4301 2023-07-25 02:38:43.143538 bkpaas-auth-2.0.6/bkpaas_auth/core/token.py
+-rw-r--r--   0        0        0     2493 2023-07-25 02:38:43.143771 bkpaas-auth-2.0.6/bkpaas_auth/core/user_info.py
+-rw-r--r--   0        0        0      641 2023-07-25 02:38:43.144249 bkpaas-auth-2.0.6/bkpaas_auth/core/utils.py
+-rw-r--r--   0        0        0     4041 2023-07-25 02:38:43.144756 bkpaas-auth-2.0.6/bkpaas_auth/middlewares.py
+-rw-r--r--   0        0        0     3368 2023-07-25 02:38:43.145038 bkpaas-auth-2.0.6/bkpaas_auth/models.py
+-rw-r--r--   0        0        0     1263 2023-07-25 02:38:43.145244 bkpaas-auth-2.0.6/bkpaas_auth/monkey.py
+-rw-r--r--   0        0        0     1267 2023-07-25 02:38:43.145914 bkpaas-auth-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6058 2023-07-25 02:39:38.211437 bkpaas-auth-2.0.6/setup.py
+-rw-r--r--   0        0        0     5927 2023-07-25 02:39:38.211945 bkpaas-auth-2.0.6/PKG-INFO
```

### Comparing `bkpaas-auth-2.0.5/README.md` & `bkpaas-auth-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/__init__.py` & `bkpaas-auth-2.0.6/bkpaas_auth/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 def get_user_by_user_id(user_id: str, username_only: bool = True):
     """Get a user object from given user_id"""
     from bkpaas_auth.core.constants import ProviderType
     from bkpaas_auth.core.encoder import user_id_encoder
     from bkpaas_auth.core.services import get_bk_user_info, get_rtx_user_info
```

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/backends.py` & `bkpaas-auth-2.0.6/bkpaas_auth/backends.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/conf.py` & `bkpaas-auth-2.0.6/bkpaas_auth/conf.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/core/encoder.py` & `bkpaas-auth-2.0.6/bkpaas_auth/core/encoder.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/core/http.py` & `bkpaas-auth-2.0.6/bkpaas_auth/core/http.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/core/plugins.py` & `bkpaas-auth-2.0.6/bkpaas_auth/core/plugins.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/core/services.py` & `bkpaas-auth-2.0.6/bkpaas_auth/core/services.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/core/token.py` & `bkpaas-auth-2.0.6/bkpaas_auth/core/token.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 """Access token for blueking
 """
 import datetime
 import logging
 
 from django.utils.timezone import now
+from django.utils.translation import get_language
 
 from bkpaas_auth.conf import bkauth_settings
-from bkpaas_auth.core.constants import ProviderType, ACCESS_PERMISSION_DENIED_CODE
-from bkpaas_auth.core.exceptions import InvalidTokenCredentialsError, ServiceError, AccessPermissionDenied
+from bkpaas_auth.core.constants import ACCESS_PERMISSION_DENIED_CODE, ProviderType
+from bkpaas_auth.core.exceptions import AccessPermissionDenied, InvalidTokenCredentialsError, ServiceError
 from bkpaas_auth.core.http import http_get
-from bkpaas_auth.core.user_info import BkUserInfo, RtxUserInfo, UserInfo
 from bkpaas_auth.core.services import get_app_credentials
+from bkpaas_auth.core.user_info import BkUserInfo, RtxUserInfo, UserInfo
 from bkpaas_auth.models import User
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractRequestBackend:
     def request_username(self, **credentials):
@@ -25,15 +26,18 @@
 class TokenRequestBackend(AbstractRequestBackend):
 
     provider_type = ProviderType.BK
 
     def request_username(self, **credentials):
         """Get username through credentials"""
         is_success, resp = http_get(
-            bkauth_settings.USER_COOKIE_VERIFY_URL, params=dict(credentials, **get_app_credentials()), timeout=10
+            bkauth_settings.USER_COOKIE_VERIFY_URL,
+            params=dict(credentials, **get_app_credentials()),
+            timeout=10,
+            headers={'blueking-language': get_language()},
         )
         if not is_success:
             raise ServiceError('unable to fetch token services')
 
         # API 返回格式为：{"result": true, "code": 0, "message": "", "data": {"bk_username": "xxx"}}
         code = resp.get('code')
         if code == 0:
```

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/core/user_info.py` & `bkpaas-auth-2.0.6/bkpaas_auth/core/user_info.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/core/utils.py` & `bkpaas-auth-2.0.6/bkpaas_auth/core/utils.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/middlewares.py` & `bkpaas-auth-2.0.6/bkpaas_auth/middlewares.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/models.py` & `bkpaas-auth-2.0.6/bkpaas_auth/models.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.5/bkpaas_auth/monkey.py` & `bkpaas-auth-2.0.6/bkpaas_auth/monkey.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.5/pyproject.toml` & `bkpaas-auth-2.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bkpaas-auth"
-version = "2.0.5"
+version = "2.0.6"
 description = "User authentication django app for blueking internal projects"
 license = "Apach License 2.0"
 readme = "README.md"
 authors = ["blueking <blueking@tencent.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.6,<4.0"
```

### Comparing `bkpaas-auth-2.0.5/setup.py` & `bkpaas-auth-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['cryptography', 'django>=1.11,<4.0', 'requests', 'six']
 
 setup_kwargs = {
     'name': 'bkpaas-auth',
-    'version': '2.0.5',
+    'version': '2.0.6',
     'description': 'User authentication django app for blueking internal projects',
     'long_description': '# bkpaas-auth\n\n蓝鲸 PaaS 平台内部服务使用的用户鉴权模块。\n\n## 版本历史\n\n详见 `CHANGES.md`。\n\n## 开发指南\n\n### 发布包\n\n- 在 `bkpaas_auth/__init__.py`  文件中更新 `__version__`\n- 在 `setup.py` 文件中更新 `version`\n- 在 `pyproject.toml` 中更新 `version`\n- 在 `CHANGES.md` 中添加对应的版本日志\n- 执行 `poetry build` 命令在 dist 目录下生成当前版本的包。然后执行 `twine upload dist/* --repository-url {pypi_address} --username {your_name} --password {your_token}` 将其上传到 pypi 服务器上。\n\n### 关于 setup.py\n\n虽然在 [PEP 517](https://python-poetry.org/docs/pyproject/#poetry-and-pep-517) 规范里，Python 包不再需要 `setup.py` 文件。但真正少了 `setup.py` 文件后，会发现有些功能就没法正常使用，比如 pip 的可编辑安装模式、tox 等（[相关文档](https://github.com/python-poetry/poetry/issues/761)）。所以我们仍然需要它。\n\n为了避免维护重复的 `pyproject.toml` 和 `setup.py` 文件，我们使用了 [dephell](https://github.com/dephell/dephell) 工具来自动生成 `setup.py` 文件。\n\n- 安装 dephell\n- 在根目录执行 `dephell deps convert --from pyproject.toml --to setup.py`\n\n## 使用指南\n1. 更新 settings：\n```python\nINSTALLED_APPS = [\n    ...\n    \'bkpaas_auth\',\n    ...\n]\n\nMIDDLEWARE = [\n    ...\n    \'bkpaas_auth.middlewares.CookieLoginMiddleware\',\n    ...\n]\n\nAUTHENTICATION_BACKENDS = [\n    # [推荐] 使用内置的虚拟用户类型，不依赖于数据库表.\n    \'bkpaas_auth.backends.UniversalAuthBackend\',\n    # 如果项目需要保留使用数据库表的方式来设计用户模型, 则需要使用 DjangoAuthUserCompatibleBackend\n    # \'bkpaas_auth.backends.DjangoAuthUserCompatibleBackend\',\n]\n\n# 使用 bkpaas_auth 内置的基于内存的用户模型\n# 如果项目需要保留使用数据库表的方式来设计用户模型, 可阅读 「关于AUTH_USER_MODEL」的部分说明\nAUTH_USER_MODEL = \'bkpaas_auth.User\'\n\n# 用户登录态认证类型\nBKAUTH_BACKEND_TYPE = "bk_token" # 可选值：bk_token/bk_ticket\n# 验证用户登录态的 API，如 蓝鲸统一登录校验登录态的 API\nBKAUTH_USER_COOKIE_VERIFY_URL = "http://bk-login-web/api/v3/is_login/"\n\n# [可选]`BKAUTH_DEFAULT_PROVIDER_TYPE` 的值用于 JWT 校验时获取默认的用户认证类型。\nBKAUTH_DEFAULT_PROVIDER_TYPE = \'RTX\'  # 可选值：RTX/UIN/BK，详见 ProviderType\n```\n\n2. 在 app config 中进行 patch：\n\n配置登录模块的 apps.py\n\n```python\nfrom bkpaas_auth.backends import DjangoAuthUserCompatibleBackend\nfrom bkpaas_auth.models import User\nfrom django.apps import AppConfig\n\n\nclass MyAppConfig(AppConfig):\n    name = \'my_app\'\n\n    def ready(self):\n        from bkpaas_auth.monkey import patch_middleware_get_user\n\n        patch_middleware_get_user()\n```\n\n更新 `__init__.py`，配置 default_app_config\n```\ndefault_app_config = \'xxx.apps.MyAppConfig\'\n```\n\n3. 配置日志（可选）\n在 django settings 的 LOGGING 中，为 sdk 配置 logger，如\n\n```python\nLOGGING = {\n    "handlers": {\n        "root": {\n            ...\n        },\n    },\n    "loggers": {\n        "bkpaas_auth": {\n            "handlers": ["root"],\n            "level": "WARNING",\n            "propagate": True,\n        },\n    },\n}\n```\n\n### 关于 AUTH_USER_MODEL\n\nbkpaas-auth 内置的基于内存的不依赖于数据库表的用户模型, 如果需要复用原有的用户模型, 则需要使用 `DjangoAuthUserCompatibleBackend` 作为用户校验后端.\n\n在默认情况下, `DjangoAuthUserCompatibleBackend` 会从 bkpaas-auth 获取到当前登录的用户信息, 并会根据用户信息尝试创建一个基于数据库的用户模型.\n如果你有以下诉求, 则应当继承 `DjangoAuthUserCompatibleBackend`, 自行实现具体的业务逻辑:\n\n1. 不希望自动创建基于数据库的用户模型:\n```python\n\n\nclass YourDjangoAuthUserCompatibleBackend(DjangoAuthUserCompatibleBackend):\n    create_unknown_user = False\n```\n\n2. 用户模型有与 django `auth.User` 不兼容的字段或其他需要初始化的字段:\n```python\n\nclass YourDjangoAuthUserCompatibleBackend(DjangoAuthUserCompatibleBackend):\n    def configure_user(self, db_user, bk_user: User):\n        """\n        Configure a user after creation and return the updated user.\n        """\n        ...\n        return db_user\n```\n\n#### 和 [apigw-manager](../apigw-manager) 集成\n该 SDK 可以和 apigw-manager 集成，完成网关 JWT 的校验，在 settings 中配置：\n```python\nINSTALLED_APPS += ["apigw_manager.apigw"]\nAUTHENTICATION_BACKENDS += ["bkpaas_auth.backends.APIGatewayAuthBackend"]\nMIDDLEWARE += [\n    "apigw_manager.apigw.authentication.ApiGatewayJWTGenericMiddleware",  # JWT 认证\n    "apigw_manager.apigw.authentication.ApiGatewayJWTAppMiddleware",  # JWT 透传的应用信息\n    "apigw_manager.apigw.authentication.ApiGatewayJWTUserMiddleware",  # JWT 透传的用户信息\n]\n```\n\n设置之后，通过 JWT 透传的用户态会验证后，会写入到 `request.user` 中。注意，配置了不认证用户的网关资源透传的请求，会生成一个有对应用户名的匿名用户对象（`is_authenticated` 为 `False`）。\n',
     'author': 'blueking',
     'author_email': 'blueking@tencent.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `bkpaas-auth-2.0.5/PKG-INFO` & `bkpaas-auth-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bkpaas-auth
-Version: 2.0.5
+Version: 2.0.6
 Summary: User authentication django app for blueking internal projects
 License: Apach License 2.0
 Author: blueking
 Author-email: blueking@tencent.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

