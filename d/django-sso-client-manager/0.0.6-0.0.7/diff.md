# Comparing `tmp/django-sso-client-manager-0.0.6.tar.gz` & `tmp/django-sso-client-manager-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sso-client-manager-0.0.6.tar", last modified: Mon Jul 24 08:09:54 2023, max compression
+gzip compressed data, was "django-sso-client-manager-0.0.7.tar", last modified: Tue Jul 25 05:43:53 2023, max compression
```

## Comparing `django-sso-client-manager-0.0.6.tar` & `django-sso-client-manager-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-24 08:09:54.753338 django-sso-client-manager-0.0.6/
--rw-rw-r--   0 yil       (1000) yil       (1000)     5247 2023-07-24 08:09:54.753338 django-sso-client-manager-0.0.6/PKG-INFO
-drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-24 08:09:54.753338 django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/
--rw-rw-r--   0 yil       (1000) yil       (1000)     5247 2023-07-24 08:09:54.000000 django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/PKG-INFO
--rw-rw-r--   0 yil       (1000) yil       (1000)      399 2023-07-24 08:09:54.000000 django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)        1 2023-07-24 08:09:54.000000 django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)       37 2023-07-24 08:09:54.000000 django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/requires.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)       19 2023-07-24 08:09:54.000000 django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/top_level.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)       38 2023-07-24 08:09:54.753338 django-sso-client-manager-0.0.6/setup.cfg
--rw-rw-r--   0 yil       (1000) yil       (1000)     1657 2023-07-24 08:09:21.000000 django-sso-client-manager-0.0.6/setup.py
-drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-24 08:09:54.753338 django-sso-client-manager-0.0.6/sso_client_manager/
--rw-rw-r--   0 yil       (1000) yil       (1000)        0 2023-06-13 14:37:55.000000 django-sso-client-manager-0.0.6/sso_client_manager/__init__.py
--rw-rw-r--   0 yil       (1000) yil       (1000)      171 2023-07-07 05:33:04.000000 django-sso-client-manager-0.0.6/sso_client_manager/apps.py
--rw-rw-r--   0 yil       (1000) yil       (1000)     2548 2023-07-24 05:12:23.000000 django-sso-client-manager-0.0.6/sso_client_manager/middlewares.py
--rw-rw-r--   0 yil       (1000) yil       (1000)      353 2023-07-20 11:16:06.000000 django-sso-client-manager-0.0.6/sso_client_manager/urls.py
--rw-rw-r--   0 yil       (1000) yil       (1000)     5490 2023-07-24 04:45:43.000000 django-sso-client-manager-0.0.6/sso_client_manager/views.py
+drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-25 05:43:53.704333 django-sso-client-manager-0.0.7/
+-rw-rw-r--   0 yil       (1000) yil       (1000)     5291 2023-07-25 05:43:53.704333 django-sso-client-manager-0.0.7/PKG-INFO
+drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-25 05:43:53.704333 django-sso-client-manager-0.0.7/django_sso_client_manager.egg-info/
+-rw-rw-r--   0 yil       (1000) yil       (1000)     5291 2023-07-25 05:43:53.000000 django-sso-client-manager-0.0.7/django_sso_client_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 yil       (1000) yil       (1000)      399 2023-07-25 05:43:53.000000 django-sso-client-manager-0.0.7/django_sso_client_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)        1 2023-07-25 05:43:53.000000 django-sso-client-manager-0.0.7/django_sso_client_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)       37 2023-07-25 05:43:53.000000 django-sso-client-manager-0.0.7/django_sso_client_manager.egg-info/requires.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)       19 2023-07-25 05:43:53.000000 django-sso-client-manager-0.0.7/django_sso_client_manager.egg-info/top_level.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)       38 2023-07-25 05:43:53.704333 django-sso-client-manager-0.0.7/setup.cfg
+-rw-rw-r--   0 yil       (1000) yil       (1000)     1657 2023-07-25 05:41:02.000000 django-sso-client-manager-0.0.7/setup.py
+drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-25 05:43:53.704333 django-sso-client-manager-0.0.7/sso_client_manager/
+-rw-rw-r--   0 yil       (1000) yil       (1000)        0 2023-06-13 14:37:55.000000 django-sso-client-manager-0.0.7/sso_client_manager/__init__.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)      171 2023-07-07 05:33:04.000000 django-sso-client-manager-0.0.7/sso_client_manager/apps.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)     2548 2023-07-25 05:31:44.000000 django-sso-client-manager-0.0.7/sso_client_manager/middlewares.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)      353 2023-07-25 05:31:55.000000 django-sso-client-manager-0.0.7/sso_client_manager/urls.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)     5490 2023-07-25 05:32:30.000000 django-sso-client-manager-0.0.7/sso_client_manager/views.py
```

### Comparing `django-sso-client-manager-0.0.6/PKG-INFO` & `django-sso-client-manager-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-sso-client-manager
-Version: 0.0.6
-Summary: django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.
+Version: 0.0.7
+Summary: Django-SSO-Client-Manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.
 Home-page: https://github.com/rjnp2/django-sso-client-manager
 Author: rjnp2
 Author-email: rjnp2@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,84 +19,87 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 django-sso-client-manager
 =========================
 
-django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.
+django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. \
+It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management.\
+By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.
 
 To install the django-sso-client-manager package and integrate it into your Django project, follow these steps:
 ------------
 
 1. Use pip to install the package:
 
-        pip install django-sso-client-manager
+    ```python
+    pip install django-sso-client-manager    
+    ```
 
 2. Add sso_client_manager to the INSTALLED_APPS list in your project's settings.py file:
+    ```python
+    INSTALLED_APPS = [
+        # other apps
+        'sso_client_manager',
+    ]  
+    ```
         
-        INSTALLED_APPS = [
-            # other apps
-            'sso_client_manager',
-        ]
 
 3. Include the ParseCodeDataMiddleware in your project's middleware configuration by adding it to the MIDDLEWARE list in settings.py:
-        
-        MIDDLEWARE = [
-            # other middleware
-            'sso_client_manager.middlewares.ParseCodeDataMiddleware',
-        ]
+    ```python
+    MIDDLEWARE = [
+        # other middleware
+        'sso_client_manager.middlewares.ParseCodeDataMiddleware',
+    ]  
+    ```   
 
 4. Finally, include the sso_client_manager.urls in your project's urls.py file to set up the necessary URL routes for the SSO functionality:
-    
-        urlpatterns = [
-            # other URL patterns
-            path('', include('sso_client_manager.urls')),
-        ]
-
-Once you've completed these steps, the django-sso-client-manager package will be installed, and you'll have integrated its features into your Django project, allowing you to manage SSO clients with login, logout, and code handling functionalities.
+    ```python
+    urlpatterns = [
+        # other URL patterns
+        path('', include('sso_client_manager.urls')),
+    ]  
+    ```
+    Once you've completed these steps, the django-sso-client-manager package will be installed, and you'll have integrated its features into your Django project, allowing you to manage SSO clients with login, logout, and code handling functionalities.
 
 Explanation of the new field to need to add in User Model (if not exist).
 ------------
 
-* sso_id 
+1. sso_id 
 
     The user model needs to be extended with an additional field called sso_id. This field will be used to store the unique user ID provided by the SSO (Single Sign-On) server.
 
     sso_id: This field will store the user ID assigned by the SSO server. When a user logs in through the SSO process, the SSO server will generate a unique ID for that user, and this ID needs to be stored in the local user model to associate the local user with the SSO user. Having this field will enable seamless user synchronization and authentication between the local application and the SSO server.
 
     By adding the sso_id field to the user model, the application can easily link local user accounts with their corresponding SSO accounts, allowing users to log in using their SSO credentials and access the application without the need to create separate login credentials. This enhances user experience and streamlines authentication processes.
 
-* email
-* username
+2. username
 
 To integrate the SSO (Single Sign-On) functionality into your Django application, you will need to add the following variables to your settings:
 -----------------
 1. APPLICATION_ID:
 
     This variable should store the unique identifier for your application within the SSO system. It is typically provided by the SSO server during the registration process.
 
 2. SSO_SERVER:
 
     This variable holds the url of the SSO server.
 
 3. KEY:
 
     This variable represents a secret key or encryption key used for secure communication or token validation between your application and the SSO server.
+    ```python
+    APPLICATION_ID = env.str('APPLICATION_ID')
+    KEY = env.str('KEY')
+    SSO_SERVER = env.str('SSO_SERVER') 
+    ```
 
-        APPLICATION_ID = env.str('APPLICATION_ID')
-        KEY = env.str('KEY')
-        SSO_SERVER = env.str('SSO_SERVER')
-
-By setting these variables in your Django settings, your application will be able to communicate with the SSO server, authenticate users, and manage the login/logout processes securely.
+    By setting these variables in your Django settings, your application will be able to communicate with the SSO server, authenticate users, and manage the login/logout processes securely.
 
 Compatibility
 -------------
-The compatibility information you provided indicates that the django-sso-client-manager package is compatible with Python 3.10 and Django versions 4 and above.
+The compatibility information you provided indicates that the django-sso-client-manager package is compatible with Python 3.8 and Django versions 4 and above.
 
 To ensure proper compatibility, always check the official documentation and release notes of the django-sso-client-manager package to confirm its support for specific Python and Django versions.
 
 
-
-
-
-
```

### Comparing `django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/PKG-INFO` & `django-sso-client-manager-0.0.7/django_sso_client_manager.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-sso-client-manager
-Version: 0.0.6
-Summary: django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.
+Version: 0.0.7
+Summary: Django-SSO-Client-Manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.
 Home-page: https://github.com/rjnp2/django-sso-client-manager
 Author: rjnp2
 Author-email: rjnp2@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,84 +19,87 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 django-sso-client-manager
 =========================
 
-django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.
+django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. \
+It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management.\
+By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.
 
 To install the django-sso-client-manager package and integrate it into your Django project, follow these steps:
 ------------
 
 1. Use pip to install the package:
 
-        pip install django-sso-client-manager
+    ```python
+    pip install django-sso-client-manager    
+    ```
 
 2. Add sso_client_manager to the INSTALLED_APPS list in your project's settings.py file:
+    ```python
+    INSTALLED_APPS = [
+        # other apps
+        'sso_client_manager',
+    ]  
+    ```
         
-        INSTALLED_APPS = [
-            # other apps
-            'sso_client_manager',
-        ]
 
 3. Include the ParseCodeDataMiddleware in your project's middleware configuration by adding it to the MIDDLEWARE list in settings.py:
-        
-        MIDDLEWARE = [
-            # other middleware
-            'sso_client_manager.middlewares.ParseCodeDataMiddleware',
-        ]
+    ```python
+    MIDDLEWARE = [
+        # other middleware
+        'sso_client_manager.middlewares.ParseCodeDataMiddleware',
+    ]  
+    ```   
 
 4. Finally, include the sso_client_manager.urls in your project's urls.py file to set up the necessary URL routes for the SSO functionality:
-    
-        urlpatterns = [
-            # other URL patterns
-            path('', include('sso_client_manager.urls')),
-        ]
-
-Once you've completed these steps, the django-sso-client-manager package will be installed, and you'll have integrated its features into your Django project, allowing you to manage SSO clients with login, logout, and code handling functionalities.
+    ```python
+    urlpatterns = [
+        # other URL patterns
+        path('', include('sso_client_manager.urls')),
+    ]  
+    ```
+    Once you've completed these steps, the django-sso-client-manager package will be installed, and you'll have integrated its features into your Django project, allowing you to manage SSO clients with login, logout, and code handling functionalities.
 
 Explanation of the new field to need to add in User Model (if not exist).
 ------------
 
-* sso_id 
+1. sso_id 
 
     The user model needs to be extended with an additional field called sso_id. This field will be used to store the unique user ID provided by the SSO (Single Sign-On) server.
 
     sso_id: This field will store the user ID assigned by the SSO server. When a user logs in through the SSO process, the SSO server will generate a unique ID for that user, and this ID needs to be stored in the local user model to associate the local user with the SSO user. Having this field will enable seamless user synchronization and authentication between the local application and the SSO server.
 
     By adding the sso_id field to the user model, the application can easily link local user accounts with their corresponding SSO accounts, allowing users to log in using their SSO credentials and access the application without the need to create separate login credentials. This enhances user experience and streamlines authentication processes.
 
-* email
-* username
+2. username
 
 To integrate the SSO (Single Sign-On) functionality into your Django application, you will need to add the following variables to your settings:
 -----------------
 1. APPLICATION_ID:
 
     This variable should store the unique identifier for your application within the SSO system. It is typically provided by the SSO server during the registration process.
 
 2. SSO_SERVER:
 
     This variable holds the url of the SSO server.
 
 3. KEY:
 
     This variable represents a secret key or encryption key used for secure communication or token validation between your application and the SSO server.
+    ```python
+    APPLICATION_ID = env.str('APPLICATION_ID')
+    KEY = env.str('KEY')
+    SSO_SERVER = env.str('SSO_SERVER') 
+    ```
 
-        APPLICATION_ID = env.str('APPLICATION_ID')
-        KEY = env.str('KEY')
-        SSO_SERVER = env.str('SSO_SERVER')
-
-By setting these variables in your Django settings, your application will be able to communicate with the SSO server, authenticate users, and manage the login/logout processes securely.
+    By setting these variables in your Django settings, your application will be able to communicate with the SSO server, authenticate users, and manage the login/logout processes securely.
 
 Compatibility
 -------------
-The compatibility information you provided indicates that the django-sso-client-manager package is compatible with Python 3.10 and Django versions 4 and above.
+The compatibility information you provided indicates that the django-sso-client-manager package is compatible with Python 3.8 and Django versions 4 and above.
 
 To ensure proper compatibility, always check the official documentation and release notes of the django-sso-client-manager package to confirm its support for specific Python and Django versions.
 
 
-
-
-
-
```

### Comparing `django-sso-client-manager-0.0.6/setup.py` & `django-sso-client-manager-0.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 README = open(os.path.join(os.path.dirname(__file__), 'readme.md')).read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-sso-client-manager',
-    version='0.0.6',
+    version='0.0.7',
     packages=['sso_client_manager'],
     include_package_data=True,
     license='MIT License',
-    description='django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.',
+    description='Django-SSO-Client-Manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/rjnp2/django-sso-client-manager',
     author='rjnp2',
     author_email='rjnp2@outlook.com',
     classifiers=[
         'Environment :: Web Environment',
```

### Comparing `django-sso-client-manager-0.0.6/sso_client_manager/middlewares.py` & `django-sso-client-manager-0.0.7/sso_client_manager/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-sso-client-manager-0.0.6/sso_client_manager/views.py` & `django-sso-client-manager-0.0.7/sso_client_manager/views.py`

 * *Files identical despite different names*

