# Comparing `tmp/django-casdoor-auth-1.0.2.tar.gz` & `tmp/django-casdoor-auth-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-casdoor-auth-1.0.2.tar", last modified: Wed Mar  8 07:08:14 2023, max compression
+gzip compressed data, was "django-casdoor-auth-1.1.0.tar", last modified: Tue Jul 25 01:55:42 2023, max compression
```

## Comparing `django-casdoor-auth-1.0.2.tar` & `django-casdoor-auth-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 07:08:14.502164 django-casdoor-auth-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-08 07:07:45.000000 django-casdoor-auth-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-03-08 07:08:14.502164 django-casdoor-auth-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-03-08 07:07:45.000000 django-casdoor-auth-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 07:08:14.502164 django-casdoor-auth-1.0.2/casdoor_auth/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-08 07:07:45.000000 django-casdoor-auth-1.0.2/casdoor_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-08 07:07:45.000000 django-casdoor-auth-1.0.2/casdoor_auth/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-08 07:07:45.000000 django-casdoor-auth-1.0.2/casdoor_auth/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-08 07:07:45.000000 django-casdoor-auth-1.0.2/casdoor_auth/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-08 07:07:45.000000 django-casdoor-auth-1.0.2/casdoor_auth/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-08 07:07:45.000000 django-casdoor-auth-1.0.2/casdoor_auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 07:08:14.502164 django-casdoor-auth-1.0.2/django_casdoor_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-03-08 07:08:14.000000 django-casdoor-auth-1.0.2/django_casdoor_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-08 07:08:14.000000 django-casdoor-auth-1.0.2/django_casdoor_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 07:08:14.000000 django-casdoor-auth-1.0.2/django_casdoor_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-08 07:08:14.000000 django-casdoor-auth-1.0.2/django_casdoor_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-08 07:08:14.000000 django-casdoor-auth-1.0.2/django_casdoor_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-08 07:07:45.000000 django-casdoor-auth-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-08 07:08:14.502164 django-casdoor-auth-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-08 07:07:45.000000 django-casdoor-auth-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:55:42.246175 django-casdoor-auth-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 01:55:07.000000 django-casdoor-auth-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-25 01:55:42.246175 django-casdoor-auth-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-25 01:55:07.000000 django-casdoor-auth-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:55:42.246175 django-casdoor-auth-1.1.0/casdoor_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-25 01:55:07.000000 django-casdoor-auth-1.1.0/casdoor_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 01:55:07.000000 django-casdoor-auth-1.1.0/casdoor_auth/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-25 01:55:07.000000 django-casdoor-auth-1.1.0/casdoor_auth/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-25 01:55:07.000000 django-casdoor-auth-1.1.0/casdoor_auth/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-25 01:55:07.000000 django-casdoor-auth-1.1.0/casdoor_auth/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-25 01:55:07.000000 django-casdoor-auth-1.1.0/casdoor_auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:55:42.246175 django-casdoor-auth-1.1.0/django_casdoor_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-25 01:55:42.000000 django-casdoor-auth-1.1.0/django_casdoor_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-25 01:55:42.000000 django-casdoor-auth-1.1.0/django_casdoor_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:55:42.000000 django-casdoor-auth-1.1.0/django_casdoor_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 01:55:42.000000 django-casdoor-auth-1.1.0/django_casdoor_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 01:55:42.000000 django-casdoor-auth-1.1.0/django_casdoor_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 01:55:07.000000 django-casdoor-auth-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-25 01:55:42.246175 django-casdoor-auth-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-25 01:55:07.000000 django-casdoor-auth-1.1.0/setup.py
```

### Comparing `django-casdoor-auth-1.0.2/LICENSE` & `django-casdoor-auth-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-casdoor-auth-1.0.2/PKG-INFO` & `django-casdoor-auth-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-casdoor-auth
-Version: 1.0.2
+Version: 1.1.0
 Summary: An app for use Casdoor SSO
 Home-page: https://github.com/casdoor/django-auth-sso
 Author: leo220yuyaodog
 Author-email: magicwindyyd@gmail.com
 License: Apache 2.0
 Keywords: Casdoor Django
 Platform: any
@@ -28,15 +28,15 @@
 
 # django-casdoor-auth
 
 [![GitHub Action](https://github.com/casdoor/django-casdoor-auth/workflows/build/badge.svg?branch=master)](https://github.com/casdoor/django-casdoor-auth/actions)
 [![Version](https://img.shields.io/pypi/v/django-casdoor-auth.svg)](https://pypi.org/project/django-casdoor-auth/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/django-casdoor-auth.svg)](https://pypi.org/project/django-casdoor-auth/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/django-casdoor-auth.svg)](https://pypi.org/project/django-casdoor-auth/)
-[![Gitter](https://badges.gitter.im/casbin/casdoor.svg)](https://gitter.im/casbin/casdoor)
+[![Discord](https://img.shields.io/discord/1022748306096537660?logo=discord&label=discord&color=5865F2)](https://discord.gg/5rPsrAzK7S)
 
 Casdoor's SDK for Django will allow you to easily connect your application to the Casdoor authentication system without having to implement it from scratch.
 
 ## Step1. install app
 
 django-casdoor-auth is available on PyPI:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-casdoor-auth Version: 1.0.2 Summary: An app
+Metadata-Version: 2.1 Name: django-casdoor-auth Version: 1.1.0 Summary: An app
 for use Casdoor SSO Home-page: https://github.com/casdoor/django-auth-sso
 Author: leo220yuyaodog Author-email: magicwindyyd@gmail.com License: Apache 2.0
 Keywords: Casdoor Django Platform: any Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -14,31 +14,32 @@
 django-casdoor-auth [![GitHub Action](https://github.com/casdoor/django-
 casdoor-auth/workflows/build/badge.svg?branch=master)](https://github.com/
 casdoor/django-casdoor-auth/actions) [![Version](https://img.shields.io/pypi/v/
 django-casdoor-auth.svg)](https://pypi.org/project/django-casdoor-auth/) [!
 [PyPI - Wheel](https://img.shields.io/pypi/wheel/django-casdoor-auth.svg)]
 (https://pypi.org/project/django-casdoor-auth/) [![Pyversions](https://
 img.shields.io/pypi/pyversions/django-casdoor-auth.svg)](https://pypi.org/
-project/django-casdoor-auth/) [![Gitter](https://badges.gitter.im/casbin/
-casdoor.svg)](https://gitter.im/casbin/casdoor) Casdoor's SDK for Django will
-allow you to easily connect your application to the Casdoor authentication
-system without having to implement it from scratch. ## Step1. install app
-django-casdoor-auth is available on PyPI: ```shell pip install django-casdoor-
-auth ``` casdoor-auth is simple to use. We will show you the steps below. ##
-Step2. Config setting.py Add "casdoor_auth" in INSTALLED_APPS ```python
-INSTALLED_APPS = [ "django.contrib.admin", "django.contrib.auth",
-"django.contrib.contenttypes", "django.contrib.sessions",
-"django.contrib.messages", "django.contrib.staticfiles", "casdoor_auth" ] ```
-Initialization requires 6 parameters, which are all str type: | Name (in order)
-| Must | Description | | ---------------- | ---- | ----------------------------
------------------------ | | endpoint | Yes | Casdoor Server Url, such as `http:
-//localhost:8000` | | client_id | Yes | Application.client_id | | client_secret
-| Yes | Application.client_secret | | certificate | Yes | The public key for
-the Casdoor application's cert | | org_name | Yes | Application.organization |
-| application_name | Yes | Application.name | ```python CASDOOR_CONFIG =
+project/django-casdoor-auth/) [![Discord](https://img.shields.io/discord/
+1022748306096537660?logo=discord&label=discord&color=5865F2)](https://
+discord.gg/5rPsrAzK7S) Casdoor's SDK for Django will allow you to easily
+connect your application to the Casdoor authentication system without having to
+implement it from scratch. ## Step1. install app django-casdoor-auth is
+available on PyPI: ```shell pip install django-casdoor-auth ``` casdoor-auth is
+simple to use. We will show you the steps below. ## Step2. Config setting.py
+Add "casdoor_auth" in INSTALLED_APPS ```python INSTALLED_APPS =
+[ "django.contrib.admin", "django.contrib.auth", "django.contrib.contenttypes",
+"django.contrib.sessions", "django.contrib.messages",
+"django.contrib.staticfiles", "casdoor_auth" ] ``` Initialization requires 6
+parameters, which are all str type: | Name (in order) | Must | Description | |
+---------------- | ---- | --------------------------------------------------- |
+| endpoint | Yes | Casdoor Server Url, such as `http://localhost:8000` | |
+client_id | Yes | Application.client_id | | client_secret | Yes |
+Application.client_secret | | certificate | Yes | The public key for the
+Casdoor application's cert | | org_name | Yes | Application.organization | |
+application_name | Yes | Application.name | ```python CASDOOR_CONFIG =
 { 'endpoint': 'http://localhost:8000', 'client_id': '', 'client_secret': '',
 'certificate': '''''', 'org_name': 'built-in', 'application_name': 'app-built-
 in' } ``` The redirect url, is the URL that your APP is configured to listen to
 the response from Casdoor. ```python REDIRECT_URI = 'http://127.0.0.1:8000/
 casdoor/callback/' ``` The login redirect url, after login successfully, you
 will jump to this page. ```python LOGIN_REDIRECT_URL = '/' ``` ## Step3. router
 urls.py ```python urlpatterns = [ ... path('casdoor/', include
```

### Comparing `django-casdoor-auth-1.0.2/README.md` & `django-casdoor-auth-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # django-casdoor-auth
 
 [![GitHub Action](https://github.com/casdoor/django-casdoor-auth/workflows/build/badge.svg?branch=master)](https://github.com/casdoor/django-casdoor-auth/actions)
 [![Version](https://img.shields.io/pypi/v/django-casdoor-auth.svg)](https://pypi.org/project/django-casdoor-auth/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/django-casdoor-auth.svg)](https://pypi.org/project/django-casdoor-auth/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/django-casdoor-auth.svg)](https://pypi.org/project/django-casdoor-auth/)
-[![Gitter](https://badges.gitter.im/casbin/casdoor.svg)](https://gitter.im/casbin/casdoor)
+[![Discord](https://img.shields.io/discord/1022748306096537660?logo=discord&label=discord&color=5865F2)](https://discord.gg/5rPsrAzK7S)
 
 Casdoor's SDK for Django will allow you to easily connect your application to the Casdoor authentication system without having to implement it from scratch.
 
 ## Step1. install app
 
 django-casdoor-auth is available on PyPI:
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
 # django-casdoor-auth [![GitHub Action](https://github.com/casdoor/django-
 casdoor-auth/workflows/build/badge.svg?branch=master)](https://github.com/
 casdoor/django-casdoor-auth/actions) [![Version](https://img.shields.io/pypi/v/
 django-casdoor-auth.svg)](https://pypi.org/project/django-casdoor-auth/) [!
 [PyPI - Wheel](https://img.shields.io/pypi/wheel/django-casdoor-auth.svg)]
 (https://pypi.org/project/django-casdoor-auth/) [![Pyversions](https://
 img.shields.io/pypi/pyversions/django-casdoor-auth.svg)](https://pypi.org/
-project/django-casdoor-auth/) [![Gitter](https://badges.gitter.im/casbin/
-casdoor.svg)](https://gitter.im/casbin/casdoor) Casdoor's SDK for Django will
-allow you to easily connect your application to the Casdoor authentication
-system without having to implement it from scratch. ## Step1. install app
-django-casdoor-auth is available on PyPI: ```shell pip install django-casdoor-
-auth ``` casdoor-auth is simple to use. We will show you the steps below. ##
-Step2. Config setting.py Add "casdoor_auth" in INSTALLED_APPS ```python
-INSTALLED_APPS = [ "django.contrib.admin", "django.contrib.auth",
-"django.contrib.contenttypes", "django.contrib.sessions",
-"django.contrib.messages", "django.contrib.staticfiles", "casdoor_auth" ] ```
-Initialization requires 6 parameters, which are all str type: | Name (in order)
-| Must | Description | | ---------------- | ---- | ----------------------------
------------------------ | | endpoint | Yes | Casdoor Server Url, such as `http:
-//localhost:8000` | | client_id | Yes | Application.client_id | | client_secret
-| Yes | Application.client_secret | | certificate | Yes | The public key for
-the Casdoor application's cert | | org_name | Yes | Application.organization |
-| application_name | Yes | Application.name | ```python CASDOOR_CONFIG =
+project/django-casdoor-auth/) [![Discord](https://img.shields.io/discord/
+1022748306096537660?logo=discord&label=discord&color=5865F2)](https://
+discord.gg/5rPsrAzK7S) Casdoor's SDK for Django will allow you to easily
+connect your application to the Casdoor authentication system without having to
+implement it from scratch. ## Step1. install app django-casdoor-auth is
+available on PyPI: ```shell pip install django-casdoor-auth ``` casdoor-auth is
+simple to use. We will show you the steps below. ## Step2. Config setting.py
+Add "casdoor_auth" in INSTALLED_APPS ```python INSTALLED_APPS =
+[ "django.contrib.admin", "django.contrib.auth", "django.contrib.contenttypes",
+"django.contrib.sessions", "django.contrib.messages",
+"django.contrib.staticfiles", "casdoor_auth" ] ``` Initialization requires 6
+parameters, which are all str type: | Name (in order) | Must | Description | |
+---------------- | ---- | --------------------------------------------------- |
+| endpoint | Yes | Casdoor Server Url, such as `http://localhost:8000` | |
+client_id | Yes | Application.client_id | | client_secret | Yes |
+Application.client_secret | | certificate | Yes | The public key for the
+Casdoor application's cert | | org_name | Yes | Application.organization | |
+application_name | Yes | Application.name | ```python CASDOOR_CONFIG =
 { 'endpoint': 'http://localhost:8000', 'client_id': '', 'client_secret': '',
 'certificate': '''''', 'org_name': 'built-in', 'application_name': 'app-built-
 in' } ``` The redirect url, is the URL that your APP is configured to listen to
 the response from Casdoor. ```python REDIRECT_URI = 'http://127.0.0.1:8000/
 casdoor/callback/' ``` The login redirect url, after login successfully, you
 will jump to this page. ```python LOGIN_REDIRECT_URL = '/' ``` ## Step3. router
 urls.py ```python urlpatterns = [ ... path('casdoor/', include
```

### Comparing `django-casdoor-auth-1.0.2/casdoor_auth/__init__.py` & `django-casdoor-auth-1.1.0/casdoor_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `django-casdoor-auth-1.0.2/casdoor_auth/apps.py` & `django-casdoor-auth-1.1.0/casdoor_auth/apps.py`

 * *Files identical despite different names*

### Comparing `django-casdoor-auth-1.0.2/casdoor_auth/tests.py` & `django-casdoor-auth-1.1.0/casdoor_auth/tests.py`

 * *Files identical despite different names*

### Comparing `django-casdoor-auth-1.0.2/casdoor_auth/urls.py` & `django-casdoor-auth-1.1.0/casdoor_auth/urls.py`

 * *Files identical despite different names*

### Comparing `django-casdoor-auth-1.0.2/casdoor_auth/user.py` & `django-casdoor-auth-1.1.0/casdoor_auth/user.py`

 * *Files identical despite different names*

### Comparing `django-casdoor-auth-1.0.2/casdoor_auth/views.py` & `django-casdoor-auth-1.1.0/casdoor_auth/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     redirect_url = sdk.get_auth_link(redirect_uri=settings.REDIRECT_URI)
     return redirect(redirect_url)
 
 
 def callback(request):
     code = request.GET.get('code')
     token = sdk.get_oauth_token(code)
+    if isinstance(token, dict) and 'access_token' in token:
+        token = token['access_token']
     user = sdk.parse_jwt_token(token)
     request.session['user'] = user
     try:
         in_user = User.objects.get(username=user.get('name'))
     except:
         in_user = User.objects.create_user(user.get('name'), user.get('email'), user.get('password'))
         in_user.save()
```

### Comparing `django-casdoor-auth-1.0.2/django_casdoor_auth.egg-info/PKG-INFO` & `django-casdoor-auth-1.1.0/django_casdoor_auth.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-casdoor-auth
-Version: 1.0.2
+Version: 1.1.0
 Summary: An app for use Casdoor SSO
 Home-page: https://github.com/casdoor/django-auth-sso
 Author: leo220yuyaodog
 Author-email: magicwindyyd@gmail.com
 License: Apache 2.0
 Keywords: Casdoor Django
 Platform: any
@@ -28,15 +28,15 @@
 
 # django-casdoor-auth
 
 [![GitHub Action](https://github.com/casdoor/django-casdoor-auth/workflows/build/badge.svg?branch=master)](https://github.com/casdoor/django-casdoor-auth/actions)
 [![Version](https://img.shields.io/pypi/v/django-casdoor-auth.svg)](https://pypi.org/project/django-casdoor-auth/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/django-casdoor-auth.svg)](https://pypi.org/project/django-casdoor-auth/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/django-casdoor-auth.svg)](https://pypi.org/project/django-casdoor-auth/)
-[![Gitter](https://badges.gitter.im/casbin/casdoor.svg)](https://gitter.im/casbin/casdoor)
+[![Discord](https://img.shields.io/discord/1022748306096537660?logo=discord&label=discord&color=5865F2)](https://discord.gg/5rPsrAzK7S)
 
 Casdoor's SDK for Django will allow you to easily connect your application to the Casdoor authentication system without having to implement it from scratch.
 
 ## Step1. install app
 
 django-casdoor-auth is available on PyPI:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-casdoor-auth Version: 1.0.2 Summary: An app
+Metadata-Version: 2.1 Name: django-casdoor-auth Version: 1.1.0 Summary: An app
 for use Casdoor SSO Home-page: https://github.com/casdoor/django-auth-sso
 Author: leo220yuyaodog Author-email: magicwindyyd@gmail.com License: Apache 2.0
 Keywords: Casdoor Django Platform: any Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -14,31 +14,32 @@
 django-casdoor-auth [![GitHub Action](https://github.com/casdoor/django-
 casdoor-auth/workflows/build/badge.svg?branch=master)](https://github.com/
 casdoor/django-casdoor-auth/actions) [![Version](https://img.shields.io/pypi/v/
 django-casdoor-auth.svg)](https://pypi.org/project/django-casdoor-auth/) [!
 [PyPI - Wheel](https://img.shields.io/pypi/wheel/django-casdoor-auth.svg)]
 (https://pypi.org/project/django-casdoor-auth/) [![Pyversions](https://
 img.shields.io/pypi/pyversions/django-casdoor-auth.svg)](https://pypi.org/
-project/django-casdoor-auth/) [![Gitter](https://badges.gitter.im/casbin/
-casdoor.svg)](https://gitter.im/casbin/casdoor) Casdoor's SDK for Django will
-allow you to easily connect your application to the Casdoor authentication
-system without having to implement it from scratch. ## Step1. install app
-django-casdoor-auth is available on PyPI: ```shell pip install django-casdoor-
-auth ``` casdoor-auth is simple to use. We will show you the steps below. ##
-Step2. Config setting.py Add "casdoor_auth" in INSTALLED_APPS ```python
-INSTALLED_APPS = [ "django.contrib.admin", "django.contrib.auth",
-"django.contrib.contenttypes", "django.contrib.sessions",
-"django.contrib.messages", "django.contrib.staticfiles", "casdoor_auth" ] ```
-Initialization requires 6 parameters, which are all str type: | Name (in order)
-| Must | Description | | ---------------- | ---- | ----------------------------
------------------------ | | endpoint | Yes | Casdoor Server Url, such as `http:
-//localhost:8000` | | client_id | Yes | Application.client_id | | client_secret
-| Yes | Application.client_secret | | certificate | Yes | The public key for
-the Casdoor application's cert | | org_name | Yes | Application.organization |
-| application_name | Yes | Application.name | ```python CASDOOR_CONFIG =
+project/django-casdoor-auth/) [![Discord](https://img.shields.io/discord/
+1022748306096537660?logo=discord&label=discord&color=5865F2)](https://
+discord.gg/5rPsrAzK7S) Casdoor's SDK for Django will allow you to easily
+connect your application to the Casdoor authentication system without having to
+implement it from scratch. ## Step1. install app django-casdoor-auth is
+available on PyPI: ```shell pip install django-casdoor-auth ``` casdoor-auth is
+simple to use. We will show you the steps below. ## Step2. Config setting.py
+Add "casdoor_auth" in INSTALLED_APPS ```python INSTALLED_APPS =
+[ "django.contrib.admin", "django.contrib.auth", "django.contrib.contenttypes",
+"django.contrib.sessions", "django.contrib.messages",
+"django.contrib.staticfiles", "casdoor_auth" ] ``` Initialization requires 6
+parameters, which are all str type: | Name (in order) | Must | Description | |
+---------------- | ---- | --------------------------------------------------- |
+| endpoint | Yes | Casdoor Server Url, such as `http://localhost:8000` | |
+client_id | Yes | Application.client_id | | client_secret | Yes |
+Application.client_secret | | certificate | Yes | The public key for the
+Casdoor application's cert | | org_name | Yes | Application.organization | |
+application_name | Yes | Application.name | ```python CASDOOR_CONFIG =
 { 'endpoint': 'http://localhost:8000', 'client_id': '', 'client_secret': '',
 'certificate': '''''', 'org_name': 'built-in', 'application_name': 'app-built-
 in' } ``` The redirect url, is the URL that your APP is configured to listen to
 the response from Casdoor. ```python REDIRECT_URI = 'http://127.0.0.1:8000/
 casdoor/callback/' ``` The login redirect url, after login successfully, you
 will jump to this page. ```python LOGIN_REDIRECT_URL = '/' ``` ## Step3. router
 urls.py ```python urlpatterns = [ ... path('casdoor/', include
```

### Comparing `django-casdoor-auth-1.0.2/setup.cfg` & `django-casdoor-auth-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-casdoor-auth
-version = 1.0.2
+version = 1.1.0
 author = leo220yuyaodog
 author_email = magicwindyyd@gmail.com
 url = https://github.com/casdoor/django-auth-sso
 description = An app for use Casdoor SSO
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache 2.0
```

