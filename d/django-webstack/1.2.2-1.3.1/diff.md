# Comparing `tmp/django-webstack-1.2.2.tar.gz` & `tmp/django-webstack-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webstack-1.2.2.tar", last modified: Mon Jul 24 14:34:16 2023, max compression
+gzip compressed data, was "django-webstack-1.3.1.tar", last modified: Tue Jul 25 06:05:52 2023, max compression
```

## Comparing `django-webstack-1.2.2.tar` & `django-webstack-1.3.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.921580 django-webstack-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-24 14:34:01.000000 django-webstack-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-24 14:34:01.000000 django-webstack-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-24 14:34:16.921580 django-webstack-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 14:34:01.000000 django-webstack-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.909580 django-webstack-1.2.2/django_webstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-24 14:34:16.000000 django-webstack-1.2.2/django_webstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-24 14:34:16.000000 django-webstack-1.2.2/django_webstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:34:16.000000 django-webstack-1.2.2/django_webstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 14:34:16.000000 django-webstack-1.2.2/django_webstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 14:34:16.000000 django-webstack-1.2.2/django_webstack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:34:16.921580 django-webstack-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-24 14:34:01.000000 django-webstack-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.913580 django-webstack-1.2.2/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.913580 django-webstack-1.2.2/webstack/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/migrations/0002_auto_20230724_1835.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.905579 django-webstack-1.2.2/webstack/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.905579 django-webstack-1.2.2/webstack/static/webstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.905579 django-webstack-1.2.2/webstack/static/webstack/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.917580 django-webstack-1.2.2/webstack/static/webstack/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/css/nav.css
--rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-components.css
--rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-core.css
--rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-forms.css
--rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-skins.css
--rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.917580 django-webstack-1.2.2/webstack/static/webstack/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/images/favicon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/images/logo-collapsed@2x.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/images/logo@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/images/preview.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.921580 django-webstack-1.2.2/webstack/static/webstack/assets/js/
--rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/TweenMax.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/joinable.js
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/lozad.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/resizeable.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/xenon-api.js
--rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/xenon-custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/xenon-toggles.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.905579 django-webstack-1.2.2/webstack/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.921580 django-webstack-1.2.2/webstack/templates/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/templates/webstack/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/templates/webstack/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.905418 django-webstack-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-25 06:05:35.000000 django-webstack-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-25 06:05:35.000000 django-webstack-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-25 06:05:52.905418 django-webstack-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-25 06:05:35.000000 django-webstack-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.897417 django-webstack-1.3.1/django_webstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-25 06:05:52.000000 django-webstack-1.3.1/django_webstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-25 06:05:52.000000 django-webstack-1.3.1/django_webstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:05:52.000000 django-webstack-1.3.1/django_webstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 06:05:52.000000 django-webstack-1.3.1/django_webstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 06:05:52.000000 django-webstack-1.3.1/django_webstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:05:52.905418 django-webstack-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-25 06:05:35.000000 django-webstack-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.897417 django-webstack-1.3.1/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.897417 django-webstack-1.3.1/webstack/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/migrations/0002_auto_20230724_1835.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/migrations/0003_auto_20230725_1401.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.893417 django-webstack-1.3.1/webstack/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.893417 django-webstack-1.3.1/webstack/static/webstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.893417 django-webstack-1.3.1/webstack/static/webstack/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.901418 django-webstack-1.3.1/webstack/static/webstack/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/css/nav.css
+-rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-components.css
+-rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-core.css
+-rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-forms.css
+-rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-skins.css
+-rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.901418 django-webstack-1.3.1/webstack/static/webstack/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/images/favicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/images/logo-collapsed@2x.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/images/logo@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/images/preview.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.905418 django-webstack-1.3.1/webstack/static/webstack/assets/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/TweenMax.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/joinable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/lozad.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/resizeable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/xenon-api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/xenon-custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/xenon-toggles.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.893417 django-webstack-1.3.1/webstack/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.905418 django-webstack-1.3.1/webstack/templates/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/templates/webstack/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/templates/webstack/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/views.py
```

### Comparing `django-webstack-1.2.2/LICENSE` & `django-webstack-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/django_webstack.egg-info/SOURCES.txt` & `django-webstack-1.3.1/django_webstack.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 webstack/apps.py
 webstack/models.py
 webstack/tests.py
 webstack/urls.py
 webstack/views.py
 webstack/migrations/0001_initial.py
 webstack/migrations/0002_auto_20230724_1835.py
+webstack/migrations/0003_auto_20230725_1401.py
 webstack/migrations/__init__.py
 webstack/static/webstack/assets/css/nav.css
 webstack/static/webstack/assets/css/xenon-components.css
 webstack/static/webstack/assets/css/xenon-core.css
 webstack/static/webstack/assets/css/xenon-forms.css
 webstack/static/webstack/assets/css/xenon-skins.css
 webstack/static/webstack/assets/css/xenon.css
```

### Comparing `django-webstack-1.2.2/setup.py` & `django-webstack-1.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf-8 -*-
 # Author: https://github.com/Hopetree
 # Date: 2023/7/24
 from setuptools import find_packages, setup
 
-VERSION = '1.2.2'
+VERSION = '1.3.1'
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='django-webstack',
     version=VERSION,
```

### Comparing `django-webstack-1.2.2/webstack/admin.py` & `django-webstack-1.3.1/webstack/admin.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/migrations/0001_initial.py` & `django-webstack-1.3.1/webstack/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/migrations/0002_auto_20230724_1835.py` & `django-webstack-1.3.1/webstack/migrations/0002_auto_20230724_1835.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/models.py` & `django-webstack-1.3.1/webstack/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 # Create your models here.
 
 # 菜单父模型
 class BaseMenu(models.Model):
     name = models.CharField('名称', max_length=10)
-    icon = models.CharField('图标', max_length=30)
+    icon = models.CharField('图标', max_length=30, help_text='Font Awesome图标库格式，如:fa fa-star-o')
     sort_order = models.IntegerField('排序', default=99, help_text='自定义排序')
     create_date = models.DateTimeField(verbose_name='创建时间', auto_now_add=True)
     update_date = models.DateTimeField(verbose_name='修改时间', auto_now=True)
 
     class Meta:
         """这是一个元类，用来继承的"""
         abstract = True
@@ -58,15 +58,15 @@
     link = models.URLField('网站地址', max_length=150)
     sort_order = models.IntegerField('排序', default=99, help_text='自定义排序')
     create_date = models.DateTimeField(verbose_name='创建时间', auto_now_add=True)
     update_date = models.DateTimeField(verbose_name='修改时间', auto_now=True)
     logo = ProcessedImageField(upload_to='web/upload/%Y/%m/%d/',
                                default='web/default/default.png',
                                verbose_name='Logo',
-                               processors=[ResizeToFill(50, 50)],
+                               processors=[ResizeToFill(120, 120)],
                                help_text='上传图片大小建议使用1:1的宽高比，为了清晰度原始图片宽度应该超过50px'
                                )
     is_show = models.BooleanField('是否展示', blank=True, null=True, default=True)
     not_show_reason = models.CharField('禁用原因', max_length=50, blank=True, null=True)
 
     menu = models.ForeignKey(SecondMenu, verbose_name='所属二级菜单', on_delete=models.PROTECT,
                              related_name='navigation_sites')
```

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/css/nav.css` & `django-webstack-1.3.1/webstack/static/webstack/assets/css/nav.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-components.css` & `django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-components.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-core.css` & `django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-core.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-forms.css` & `django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-forms.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-skins.css` & `django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-skins.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon.css` & `django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/images/favicon.png` & `django-webstack-1.3.1/webstack/static/webstack/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/images/logo-collapsed@2x.png` & `django-webstack-1.3.1/webstack/static/webstack/assets/images/logo-collapsed@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/images/logo@2x.png` & `django-webstack-1.3.1/webstack/static/webstack/assets/images/logo@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/images/preview.gif` & `django-webstack-1.3.1/webstack/static/webstack/assets/images/preview.gif`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/js/TweenMax.min.js` & `django-webstack-1.3.1/webstack/static/webstack/assets/js/TweenMax.min.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/js/joinable.js` & `django-webstack-1.3.1/webstack/static/webstack/assets/js/joinable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/js/lozad.js` & `django-webstack-1.3.1/webstack/static/webstack/assets/js/lozad.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/js/resizeable.js` & `django-webstack-1.3.1/webstack/static/webstack/assets/js/resizeable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/js/xenon-api.js` & `django-webstack-1.3.1/webstack/static/webstack/assets/js/xenon-api.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/js/xenon-custom.js` & `django-webstack-1.3.1/webstack/static/webstack/assets/js/xenon-custom.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/static/webstack/assets/js/xenon-toggles.js` & `django-webstack-1.3.1/webstack/static/webstack/assets/js/xenon-toggles.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/templates/webstack/base.html` & `django-webstack-1.3.1/webstack/templates/webstack/base.html`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.2/webstack/templates/webstack/index.html` & `django-webstack-1.3.1/webstack/templates/webstack/index.html`

 * *Files identical despite different names*

