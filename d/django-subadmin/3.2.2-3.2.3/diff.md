# Comparing `tmp/django-subadmin-3.2.2.tar.gz` & `tmp/django-subadmin-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-subadmin-3.2.2.tar", last modified: Thu Jul  6 09:46:00 2023, max compression
+gzip compressed data, was "django-subadmin-3.2.3.tar", last modified: Tue Jul 25 09:07:12 2023, max compression
```

## Comparing `django-subadmin-3.2.2.tar` & `django-subadmin-3.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.194272 django-subadmin-3.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.190272 django-subadmin-3.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.190272 django-subadmin-3.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-06 09:46:00.194272 django-subadmin-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.190272 django-subadmin-3.2.2/django_subadmin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-06 09:46:00.000000 django-subadmin-3.2.2/django_subadmin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-06 09:46:00.000000 django-subadmin-3.2.2/django_subadmin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:46:00.000000 django-subadmin-3.2.2/django_subadmin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 09:46:00.000000 django-subadmin-3.2.2/django_subadmin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 09:46:00.194272 django-subadmin-3.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.190272 django-subadmin-3.2.2/subadmin/
--rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.190272 django-subadmin-3.2.2/subadmin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.194272 django-subadmin-3.2.2/subadmin/templates/subadmin/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/delete_selected_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/object_history.html
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/parent_change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/submit_line.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.194272 django-subadmin-3.2.2/subadmin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templatetags/subadmin_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.881769 django-subadmin-3.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/django_subadmin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-25 09:07:12.000000 django-subadmin-3.2.3/django_subadmin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-25 09:07:12.000000 django-subadmin-3.2.3/django_subadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:07:12.000000 django-subadmin-3.2.3/django_subadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 09:07:12.000000 django-subadmin-3.2.3/django_subadmin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/subadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.881769 django-subadmin-3.2.3/subadmin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/subadmin/templates/subadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/delete_selected_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/object_history.html
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/parent_change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/submit_line.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/subadmin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templatetags/subadmin_tags.py
```

### Comparing `django-subadmin-3.2.2/.github/workflows/publish.yml` & `django-subadmin-3.2.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.2/.github/workflows/publish_test.yml` & `django-subadmin-3.2.3/.github/workflows/publish_test.yml`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.2/LICENSE` & `django-subadmin-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.2/PKG-INFO` & `django-subadmin-3.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-subadmin
-Version: 3.2.2
+Version: 3.2.3
 Summary: A special kind of ModelAdmin that allows it to be nested within another ModelAdmin
 Author-email: Mitja Pagon <mitja@inueni.com>
 License: MIT
 Project-URL: Homepage, https://github.com/inueni/django-subadmin/
 Project-URL: Bug Tracker, https://github.com/inueni/django-subadmin/issues
 Project-URL: Changelog, https://github.com/inueni/django-subadmin/releases
 Keywords: django,admin,modeladmin,foreignkey,related field
```

### Comparing `django-subadmin-3.2.2/README.md` & `django-subadmin-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.2/django_subadmin.egg-info/PKG-INFO` & `django-subadmin-3.2.3/django_subadmin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-subadmin
-Version: 3.2.2
+Version: 3.2.3
 Summary: A special kind of ModelAdmin that allows it to be nested within another ModelAdmin
 Author-email: Mitja Pagon <mitja@inueni.com>
 License: MIT
 Project-URL: Homepage, https://github.com/inueni/django-subadmin/
 Project-URL: Bug Tracker, https://github.com/inueni/django-subadmin/issues
 Project-URL: Changelog, https://github.com/inueni/django-subadmin/releases
 Keywords: django,admin,modeladmin,foreignkey,related field
```

### Comparing `django-subadmin-3.2.2/django_subadmin.egg-info/SOURCES.txt` & `django-subadmin-3.2.3/django_subadmin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.2/pyproject.toml` & `django-subadmin-3.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.2/subadmin/__init__.py` & `django-subadmin-3.2.3/subadmin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.2/subadmin/templates/subadmin/change_form.html` & `django-subadmin-3.2.3/subadmin/templates/subadmin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.2/subadmin/templates/subadmin/change_list.html` & `django-subadmin-3.2.3/subadmin/templates/subadmin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.2/subadmin/templates/subadmin/submit_line.html` & `django-subadmin-3.2.3/subadmin/templates/subadmin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.2/subadmin/templatetags/subadmin_tags.py` & `django-subadmin-3.2.3/subadmin/templatetags/subadmin_tags.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     for parent in subadmin_parents:
         adm = parent['admin']
         obj = parent['object']
 
         breadcrumbs.extend([{
             'name': obj._meta.verbose_name_plural,
             'url': adm.reverse_url('changelist', *view_args[:i]),
-            'has_change_permission': adm.has_change_permission(request),
+            'has_view_permission': adm.has_view_permission(request),
         }, {
             'name': force_str(obj),
             'url': adm.reverse_url('change', *view_args[:i + 1]),
-            'has_change_permission': adm.has_change_permission(request, obj),
+            'has_view_permission': adm.has_view_permission(request, obj),
         }])
         i += 1
 
     return {
         'root': root,
         'breadcrumbs': breadcrumbs,
         'opts': opts,
```

