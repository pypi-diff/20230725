# Comparing `tmp/django-botmanager-0.2.14.tar.gz` & `tmp/django-botmanager-0.2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-botmanager-0.2.14.tar", last modified: Wed Jun 28 11:25:20 2023, max compression
+gzip compressed data, was "dist/django-botmanager-0.2.15.tar", last modified: Tue Jul 25 07:31:25 2023, max compression
```

## Comparing `django-botmanager-0.2.14.tar` & `django-botmanager-0.2.15.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-06-28 11:25:20.145034 django-botmanager-0.2.14/
--rw-rw-r--   0 titov     (1000) titov     (1000)     1479 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/LICENSE
--rw-rw-r--   0 titov     (1000) titov     (1000)      223 2023-06-28 11:25:20.145034 django-botmanager-0.2.14/PKG-INFO
--rw-rw-r--   0 titov     (1000) titov     (1000)      562 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/README.md
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-06-28 11:25:20.141034 django-botmanager-0.2.14/botmanager/
--rw-rw-r--   0 titov     (1000) titov     (1000)       73 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/__init__.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     1482 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/admin.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      135 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/apps.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     7829 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/basetask.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-06-28 11:25:20.141034 django-botmanager-0.2.14/botmanager/management/
--rw-rw-r--   0 titov     (1000) titov     (1000)        0 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/management/__init__.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-06-28 11:25:20.141034 django-botmanager-0.2.14/botmanager/management/commands/
--rw-rw-r--   0 titov     (1000) titov     (1000)      542 2023-06-28 11:16:25.000000 django-botmanager-0.2.14/botmanager/management/commands/__init__.py
--rw-rw-r--   0 titov     (1000) titov     (1000)    18210 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/management/commands/bot_manager.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-06-28 11:25:20.141034 django-botmanager-0.2.14/botmanager/migrations/
--rw-rw-r--   0 titov     (1000) titov     (1000)     3357 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/migrations/0001_initial.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      742 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/migrations/0002_auto_20161208_1406.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     1935 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/migrations/0003_auto_20161208_1529.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     2880 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/migrations/0004_auto_20161219_1931.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      712 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/migrations/0005_task_parent.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      448 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/migrations/0006_task_priority.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      667 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/migrations/0007_task_is_persistent.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      673 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/migrations/0008_auto_20170331_1752.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      489 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/migrations/0009_task_extra_params.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      653 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/migrations/0010_auto_20170531_1321.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      706 2023-06-28 11:19:02.000000 django-botmanager-0.2.14/botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py
--rw-rw-r--   0 titov     (1000) titov     (1000)        0 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/migrations/__init__.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     3665 2023-06-28 11:18:48.000000 django-botmanager-0.2.14/botmanager/models.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     3266 2023-06-28 11:15:43.000000 django-botmanager-0.2.14/botmanager/settings.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     1105 2023-06-28 10:28:59.000000 django-botmanager-0.2.14/botmanager/utils.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-06-28 11:25:20.145034 django-botmanager-0.2.14/django_botmanager.egg-info/
--rw-rw-r--   0 titov     (1000) titov     (1000)      223 2023-06-28 11:25:20.000000 django-botmanager-0.2.14/django_botmanager.egg-info/PKG-INFO
--rw-rw-r--   0 titov     (1000) titov     (1000)     1067 2023-06-28 11:25:20.000000 django-botmanager-0.2.14/django_botmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 titov     (1000) titov     (1000)        1 2023-06-28 11:25:20.000000 django-botmanager-0.2.14/django_botmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 titov     (1000) titov     (1000)       52 2023-06-28 11:25:20.000000 django-botmanager-0.2.14/django_botmanager.egg-info/requires.txt
--rw-rw-r--   0 titov     (1000) titov     (1000)       11 2023-06-28 11:25:20.000000 django-botmanager-0.2.14/django_botmanager.egg-info/top_level.txt
--rw-rw-r--   0 titov     (1000) titov     (1000)       38 2023-06-28 11:25:20.145034 django-botmanager-0.2.14/setup.cfg
--rw-rw-r--   0 titov     (1000) titov     (1000)      432 2023-06-28 10:59:06.000000 django-botmanager-0.2.14/setup.py
+drwxrwxr-x   0 dimoha    (1000) dimoha    (1000)        0 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      432 2023-07-25 07:07:34.000000 django-botmanager-0.2.15/setup.py
+drwxrwxr-x   0 dimoha    (1000) dimoha    (1000)        0 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/django_botmanager.egg-info/
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)     1095 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/django_botmanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)        1 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/django_botmanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)       52 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/django_botmanager.egg-info/requires.txt
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)       47 2017-06-06 13:08:15.000000 django-botmanager-0.2.15/django_botmanager.egg-info/pbr.json
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)       11 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/django_botmanager.egg-info/top_level.txt
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      257 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/django_botmanager.egg-info/PKG-INFO
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      562 2017-06-02 16:31:14.000000 django-botmanager-0.2.15/README.md
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)       38 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/setup.cfg
+drwxrwxr-x   0 dimoha    (1000) dimoha    (1000)        0 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/botmanager/
+-rw-r--r--   0 dimoha    (1000) dimoha    (1000)     7829 2021-05-13 08:03:27.000000 django-botmanager-0.2.15/botmanager/basetask.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)     3266 2023-07-25 07:05:19.000000 django-botmanager-0.2.15/botmanager/settings.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)     1105 2021-05-13 08:00:32.000000 django-botmanager-0.2.15/botmanager/utils.py
+-rw-r--r--   0 dimoha    (1000) dimoha    (1000)     1542 2023-07-25 07:07:16.000000 django-botmanager-0.2.15/botmanager/admin.py
+drwxrwxr-x   0 dimoha    (1000) dimoha    (1000)        0 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/botmanager/migrations/
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      489 2017-04-28 11:08:37.000000 django-botmanager-0.2.15/botmanager/migrations/0009_task_extra_params.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      706 2023-07-25 07:05:19.000000 django-botmanager-0.2.15/botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      673 2017-04-11 08:02:21.000000 django-botmanager-0.2.15/botmanager/migrations/0008_auto_20170331_1752.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)     1935 2016-12-08 14:04:16.000000 django-botmanager-0.2.15/botmanager/migrations/0003_auto_20161208_1529.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      712 2017-02-21 09:33:21.000000 django-botmanager-0.2.15/botmanager/migrations/0005_task_parent.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      742 2016-12-08 14:04:16.000000 django-botmanager-0.2.15/botmanager/migrations/0002_auto_20161208_1406.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)     2880 2016-12-19 16:31:31.000000 django-botmanager-0.2.15/botmanager/migrations/0004_auto_20161219_1931.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      653 2017-06-01 13:49:09.000000 django-botmanager-0.2.15/botmanager/migrations/0010_auto_20170531_1321.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)        0 2016-12-08 14:04:16.000000 django-botmanager-0.2.15/botmanager/migrations/__init__.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      667 2017-04-11 08:02:21.000000 django-botmanager-0.2.15/botmanager/migrations/0007_task_is_persistent.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      448 2017-02-21 09:33:21.000000 django-botmanager-0.2.15/botmanager/migrations/0006_task_priority.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)     3357 2016-12-08 14:04:16.000000 django-botmanager-0.2.15/botmanager/migrations/0001_initial.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)       73 2017-02-21 09:33:21.000000 django-botmanager-0.2.15/botmanager/__init__.py
+drwxrwxr-x   0 dimoha    (1000) dimoha    (1000)        0 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/botmanager/management/
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)        0 2016-12-08 14:04:16.000000 django-botmanager-0.2.15/botmanager/management/__init__.py
+drwxrwxr-x   0 dimoha    (1000) dimoha    (1000)        0 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/botmanager/management/commands/
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)    18210 2021-05-13 08:00:32.000000 django-botmanager-0.2.15/botmanager/management/commands/bot_manager.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      542 2016-12-08 14:04:16.000000 django-botmanager-0.2.15/botmanager/management/commands/__init__.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      135 2016-12-08 14:04:16.000000 django-botmanager-0.2.15/botmanager/apps.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)     3665 2023-07-25 07:05:19.000000 django-botmanager-0.2.15/botmanager/models.py
+-rw-rw-r--   0 dimoha    (1000) dimoha    (1000)      257 2023-07-25 07:31:25.000000 django-botmanager-0.2.15/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `django-botmanager-0.2.14/README.md` & `django-botmanager-0.2.15/README.md`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/admin.py` & `django-botmanager-0.2.15/botmanager/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 from django.contrib import admin
 from django.utils.html import escape
+from django.utils.translation import gettext_lazy as _
 from botmanager.models import Task
 
 
 class TaskAdmin(admin.ModelAdmin):
     list_display = ['id', 'name', 'is_complete', 'in_process', 'is_failed',
                     'create_dt', 'finish_dt', 'error_field', 'attempt_period', 'attempt_count', 'input_field']
     list_filter = ('is_complete', 'is_failed', 'in_process', 'name')
@@ -24,16 +25,16 @@
                     escape(obj.last_error['error']),
                     escape(obj.last_error['error'][0:err_max_len])
                 ) if len(obj.last_error['error']) > err_max_len else obj.last_error['error']
             )
         else:
             return None
 
-    error_field.short_description = u"Ошибка"
+    error_field.short_description = _("Ошибка")
     error_field.allow_tags = True
 
     def input_field(self, obj):
         return obj.input
 
-    input_field.short_description = "Вводные данные"
+    input_field.short_description = _("Вводные данные")
 
 admin.site.register(Task, TaskAdmin)
```

### Comparing `django-botmanager-0.2.14/botmanager/basetask.py` & `django-botmanager-0.2.15/botmanager/basetask.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/management/commands/__init__.py` & `django-botmanager-0.2.15/botmanager/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/management/commands/bot_manager.py` & `django-botmanager-0.2.15/botmanager/management/commands/bot_manager.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/migrations/0001_initial.py` & `django-botmanager-0.2.15/botmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/migrations/0002_auto_20161208_1406.py` & `django-botmanager-0.2.15/botmanager/migrations/0002_auto_20161208_1406.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/migrations/0003_auto_20161208_1529.py` & `django-botmanager-0.2.15/botmanager/migrations/0003_auto_20161208_1529.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/migrations/0004_auto_20161219_1931.py` & `django-botmanager-0.2.15/botmanager/migrations/0004_auto_20161219_1931.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/migrations/0005_task_parent.py` & `django-botmanager-0.2.15/botmanager/migrations/0005_task_parent.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/migrations/0007_task_is_persistent.py` & `django-botmanager-0.2.15/botmanager/migrations/0007_task_is_persistent.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/migrations/0008_auto_20170331_1752.py` & `django-botmanager-0.2.15/botmanager/migrations/0008_auto_20170331_1752.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/migrations/0010_auto_20170531_1321.py` & `django-botmanager-0.2.15/botmanager/migrations/0010_auto_20170531_1321.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py` & `django-botmanager-0.2.15/botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/models.py` & `django-botmanager-0.2.15/botmanager/models.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/settings.py` & `django-botmanager-0.2.15/botmanager/settings.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/botmanager/utils.py` & `django-botmanager-0.2.15/botmanager/utils.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.14/django_botmanager.egg-info/SOURCES.txt` & `django-botmanager-0.2.15/django_botmanager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 botmanager/__init__.py
 botmanager/admin.py
 botmanager/apps.py
 botmanager/basetask.py
 botmanager/models.py
@@ -22,9 +21,10 @@
 botmanager/migrations/0009_task_extra_params.py
 botmanager/migrations/0010_auto_20170531_1321.py
 botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py
 botmanager/migrations/__init__.py
 django_botmanager.egg-info/PKG-INFO
 django_botmanager.egg-info/SOURCES.txt
 django_botmanager.egg-info/dependency_links.txt
+django_botmanager.egg-info/pbr.json
 django_botmanager.egg-info/requires.txt
 django_botmanager.egg-info/top_level.txt
```

