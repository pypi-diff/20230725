# Comparing `tmp/djangocms-modules-1.0.0.tar.gz` & `tmp/djangocms-modules-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangocms-modules-1.0.0.tar", last modified: Wed Sep  2 13:58:52 2020, max compression
+gzip compressed data, was "djangocms-modules-2.0.0.tar", last modified: Tue Jul 25 13:50:18 2023, max compression
```

## Comparing `djangocms-modules-1.0.0.tar` & `djangocms-modules-2.0.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.374162 djangocms-modules-1.0.0/
--rw-r--r--   0 finalangel   (501) staff       (20)     1474 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/LICENSE
--rw-r--r--   0 finalangel   (501) staff       (20)      185 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/MANIFEST.in
--rw-r--r--   0 finalangel   (501) staff       (20)     4713 2020-09-02 13:58:52.373807 djangocms-modules-1.0.0/PKG-INFO
--rw-r--r--   0 finalangel   (501) staff       (20)     2805 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/README.rst
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.211013 djangocms-modules-1.0.0/djangocms_modules/
--rw-r--r--   0 finalangel   (501) staff       (20)       83 2020-09-02 13:58:41.000000 djangocms-modules-1.0.0/djangocms_modules/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)      264 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/admin.py
--rw-r--r--   0 finalangel   (501) staff       (20)      269 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/apps.py
--rw-r--r--   0 finalangel   (501) staff       (20)    10616 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/cms_plugins.py
--rw-r--r--   0 finalangel   (501) staff       (20)     2091 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/cms_toolbars.py
--rw-r--r--   0 finalangel   (501) staff       (20)     3812 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/forms.py
--rw-r--r--   0 finalangel   (501) staff       (20)     2306 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/handlers.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.225457 djangocms-modules-1.0.0/djangocms_modules/management/
--rw-r--r--   0 finalangel   (501) staff       (20)        0 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/management/__init__.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.226090 djangocms-modules-1.0.0/djangocms_modules/management/commands/
--rw-r--r--   0 finalangel   (501) staff       (20)        0 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/management/commands/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)      621 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/management/commands/update_modules_language.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.250001 djangocms-modules-1.0.0/djangocms_modules/migrations/
--rw-r--r--   0 finalangel   (501) staff       (20)     1851 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/migrations/0001_initial.py
--rw-r--r--   0 finalangel   (501) staff       (20)     1060 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/migrations/0002_auto_20190122_0412.py
--rw-r--r--   0 finalangel   (501) staff       (20)        0 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/migrations/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)     3603 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/models.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.138589 djangocms-modules-1.0.0/djangocms_modules/static/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.138996 djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.257502 djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/css/
--rw-r--r--   0 finalangel   (501) staff       (20)     2105 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/css/modules.css
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.264415 djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/img/
--rw-r--r--   0 finalangel   (501) staff       (20)      193 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/img/icon.png
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.289294 djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/js/
--rw-r--r--   0 finalangel   (501) staff       (20)      259 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/js/base.js
--rw-r--r--   0 finalangel   (501) staff       (20)      713 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/js/copy.js
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.291458 djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/js/dist/
--rw-r--r--   0 finalangel   (501) staff       (20)     3091 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/js/dist/bundle.modules.min.js
--rw-r--r--   0 finalangel   (501) staff       (20)     2767 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/js/plugin.js
--rw-r--r--   0 finalangel   (501) staff       (20)      818 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/js/structureboard.js
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.139766 djangocms-modules-1.0.0/djangocms_modules/templates/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.139527 djangocms-modules-1.0.0/djangocms_modules/templates/cms/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.293369 djangocms-modules-1.0.0/djangocms_modules/templates/cms/toolbar/
--rw-r--r--   0 finalangel   (501) staff       (20)     1146 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/templates/cms/toolbar/dragitem_menu.html
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.342267 djangocms-modules-1.0.0/djangocms_modules/templates/djangocms_modules/
--rw-r--r--   0 finalangel   (501) staff       (20)     1279 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/templates/djangocms_modules/add_module.html
--rw-r--r--   0 finalangel   (501) staff       (20)      272 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/templates/djangocms_modules/base.html
--rw-r--r--   0 finalangel   (501) staff       (20)     1265 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/templates/djangocms_modules/create_module.html
--rw-r--r--   0 finalangel   (501) staff       (20)     1022 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/templates/djangocms_modules/modules_list.html
--rw-r--r--   0 finalangel   (501) staff       (20)      741 2020-08-19 12:19:12.000000 djangocms-modules-1.0.0/djangocms_modules/templates/djangocms_modules/render_module.html
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.344227 djangocms-modules-1.0.0/djangocms_modules/templatetags/
--rw-r--r--   0 finalangel   (501) staff       (20)        0 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/templatetags/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)      687 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/djangocms_modules/templatetags/djangocms_modules_tags.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.224917 djangocms-modules-1.0.0/djangocms_modules.egg-info/
--rw-r--r--   0 finalangel   (501) staff       (20)     4713 2020-09-02 13:58:51.000000 djangocms-modules-1.0.0/djangocms_modules.egg-info/PKG-INFO
--rw-r--r--   0 finalangel   (501) staff       (20)     1764 2020-09-02 13:58:52.000000 djangocms-modules-1.0.0/djangocms_modules.egg-info/SOURCES.txt
--rw-r--r--   0 finalangel   (501) staff       (20)        1 2020-09-02 13:58:51.000000 djangocms-modules-1.0.0/djangocms_modules.egg-info/dependency_links.txt
--rw-r--r--   0 finalangel   (501) staff       (20)        1 2020-09-02 13:58:51.000000 djangocms-modules-1.0.0/djangocms_modules.egg-info/not-zip-safe
--rw-r--r--   0 finalangel   (501) staff       (20)       16 2020-09-02 13:58:51.000000 djangocms-modules-1.0.0/djangocms_modules.egg-info/requires.txt
--rw-r--r--   0 finalangel   (501) staff       (20)       24 2020-09-02 13:58:51.000000 djangocms-modules-1.0.0/djangocms_modules.egg-info/top_level.txt
--rw-r--r--   0 finalangel   (501) staff       (20)       38 2020-09-02 13:58:52.374260 djangocms-modules-1.0.0/setup.cfg
--rw-r--r--   0 finalangel   (501) staff       (20)     1569 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/setup.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:58:52.366991 djangocms-modules-1.0.0/tests/
--rw-r--r--   0 finalangel   (501) staff       (20)        0 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/tests/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)      367 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/tests/settings.py
--rw-r--r--   0 finalangel   (501) staff       (20)      885 2020-09-02 08:58:55.000000 djangocms-modules-1.0.0/tests/test_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.446070 djangocms-modules-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-25 13:50:18.446070 djangocms-modules-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.442070 djangocms-modules-2.0.0/djangocms_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/cms_toolbars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.442070 djangocms-modules-2.0.0/djangocms_modules/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.442070 djangocms-modules-2.0.0/djangocms_modules/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/management/commands/update_modules_language.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.446070 djangocms-modules-2.0.0/djangocms_modules/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/migrations/0002_auto_20190122_0412.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/migrations/0003_alter_moduleplugin_cmsplugin_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.438070 djangocms-modules-2.0.0/djangocms_modules/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.438070 djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.446070 djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/css/modules.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.446070 djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/img/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.446070 djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/js/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/js/copy.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.446070 djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/js/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/js/dist/bundle.modules.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/js/plugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/js/structureboard.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.442070 djangocms-modules-2.0.0/djangocms_modules/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.442070 djangocms-modules-2.0.0/djangocms_modules/templates/cms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.446070 djangocms-modules-2.0.0/djangocms_modules/templates/cms/toolbar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/templates/cms/toolbar/dragitem_menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.446070 djangocms-modules-2.0.0/djangocms_modules/templates/djangocms_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/templates/djangocms_modules/add_module.html
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/templates/djangocms_modules/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/templates/djangocms_modules/create_module.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/templates/djangocms_modules/modules_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/templates/djangocms_modules/render_module.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.446070 djangocms-modules-2.0.0/djangocms_modules/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/djangocms_modules/templatetags/djangocms_modules_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.442070 djangocms-modules-2.0.0/djangocms_modules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-25 13:50:18.000000 djangocms-modules-2.0.0/djangocms_modules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-25 13:50:18.000000 djangocms-modules-2.0.0/djangocms_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:50:18.000000 djangocms-modules-2.0.0/djangocms_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:50:18.000000 djangocms-modules-2.0.0/djangocms_modules.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 13:50:18.000000 djangocms-modules-2.0.0/djangocms_modules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 13:50:18.000000 djangocms-modules-2.0.0/djangocms_modules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-25 13:50:18.446070 djangocms-modules-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:18.446070 djangocms-modules-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-25 13:50:08.000000 djangocms-modules-2.0.0/tests/test_migrations.py
```

### Comparing `djangocms-modules-1.0.0/LICENSE` & `djangocms-modules-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/README.rst` & `djangocms-modules-2.0.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 ==================
 django CMS Modules
 ==================
 
-|pypi| |build| |coverage|
+|pypi|  |coverage| |python| |django| |djangocms|
 
 **django CMS Modules** adds copy/paste capabilities to groups of plugins.
 
-This addon is compatible with `Divio Cloud <http://divio.com>`_ and is also available on the
-`django CMS Marketplace <https://marketplace.django-cms.org/en/addons/browse/djangocms-modules/>`_
-for easy installation.
+.. note::
 
-.. image:: preview.gif
+        This project is endorsed by the `django CMS Association <https://www.django-cms.org/en/about-us/>`_.
+        That means that it is officially accepted by the dCA as being in line with our roadmap vision and development/plugin policy.
+        Join us on `Slack <https://www.django-cms.org/slack/>`_.
 
+.. image:: preview.gif
 
-Contributing
-============
+*******************************************
+Contribute to this project and win rewards
+*******************************************
+
+Because this is a an open-source project, we welcome everyone to
+`get involved in the project <https://www.django-cms.org/en/contribute/>`_ and
+`receive a reward <https://www.django-cms.org/en/bounty-program/>`_ for their contribution.
+Become part of a fantastic community and help us make django CMS the best CMS in the world.
 
-This is a an open-source project. We'll be delighted to receive your
+We'll be delighted to receive your
 feedback in the form of issues and pull requests. Before submitting your
 pull request, please review our `contribution guidelines
 <http://docs.django-cms.org/en/latest/contributing/index.html>`_.
 
 We're grateful to all contributors who have helped create and maintain this package.
-Contributors are listed at the `contributors <https://github.com/divio/djangocms-modules/graphs/contributors>`_
+Contributors are listed at the `contributors <https://github.com/django-cms/djangocms-modules/graphs/contributors>`_
 section.
 
-One of the easiest contributions you can make is helping to translate this addon on
-`Transifex <https://www.transifex.com/projects/p/djangocms-modules/>`_.
-
-
-Documentation
-=============
-
-See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-modules/blob/master/setup.py>`_
-file for additional dependencies:
-
-|python| |django| |djangocms|
-
-
 Installation
-------------
+============
 
 For a manual install:
 
 * run ``pip install djangocms-modules``
 * add ``djangocms_modules`` to your ``INSTALLED_APPS`` **before** ``cms``
 * run ``python manage.py migrate djangocms_modules``
 
@@ -62,18 +56,17 @@
     source env/bin/activate
     pip install -r tests/requirements.txt
     python setup.py test
 
 
 .. |pypi| image:: https://badge.fury.io/py/djangocms-modules.svg
     :target: http://badge.fury.io/py/djangocms-modules
-.. |build| image:: https://travis-ci.org/divio/djangocms-modules.svg?branch=master
-    :target: https://travis-ci.org/divio/djangocms-modules
-.. |coverage| image:: https://codecov.io/gh/divio/djangocms-modules/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/divio/djangocms-modules
 
-.. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
+.. |coverage| image:: https://codecov.io/gh/django-cms/djangocms-modules/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/django-cms/djangocms-modules
+
+.. |python| image:: https://img.shields.io/badge/python-3.9+-blue.svg
     :target: https://pypi.org/project/djangocms-modules/
-.. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
+.. |django| image:: https://img.shields.io/badge/django-3.2,%204.0-blue.svg
     :target: https://www.djangoproject.com/
-.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
+.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.9%2B-blue.svg
     :target: https://www.django-cms.org/
```

### Comparing `djangocms-modules-1.0.0/djangocms_modules/cms_plugins.py` & `djangocms-modules-2.0.0/djangocms_modules/cms_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 import copy
 import json
 
 from django.conf import settings
 from django.core.exceptions import PermissionDenied
-from django.http import (
-    HttpResponse, HttpResponseBadRequest, HttpResponseForbidden,
-)
+from django.http import HttpResponse, HttpResponseBadRequest, HttpResponseForbidden
 from django.shortcuts import get_object_or_404, render
-from django.urls import re_path, reverse
-from django.utils.encoding import force_text
+from django.urls import path, reverse
+from django.utils.encoding import force_str
 from django.utils.http import urlencode
 from django.utils.translation import get_language_from_request
 from django.utils.translation import gettext_lazy as _
 from django.views.generic import ListView
 
 from cms import operations
 from cms.exceptions import PluginLimitReached
 from cms.models import CMSPlugin
 from cms.plugin_base import CMSPluginBase, PluginMenuItem
 from cms.plugin_pool import plugin_pool
-from cms.utils.plugins import (
-    copy_plugins_to_placeholder, get_bound_plugins, has_reached_plugin_limit,
-    reorder_plugins,
-)
+from cms.utils.plugins import copy_plugins_to_placeholder, get_bound_plugins, has_reached_plugin_limit, reorder_plugins
 from cms.utils.urlutils import admin_reverse
 
 from .forms import AddModuleForm, CreateModuleForm, NewModuleForm
 from .models import Category, ModulePlugin
 
 
 def post_add_plugin(operation, **kwargs):
@@ -59,17 +54,17 @@
     }
 
     def has_add_permission(self, request):
         return False
 
     def get_plugin_urls(self):
         urlpatterns = [
-            re_path(r'^create-module/$', self.create_module_view, name='cms_create_module'),
-            re_path(r'^add-module/(?P<module_id>[0-9]+)/$', self.add_module_view, name='cms_add_module'),
-            re_path(r'^modules/$', self.modules_list_view, name='cms_modules_list'),
+            path('create-module/', self.create_module_view, name='cms_create_module'),
+            path('add-module/<int:module_id>/', self.add_module_view, name='cms_add_module'),
+            path('modules/', self.modules_list_view, name='cms_modules_list'),
         ]
         return urlpatterns
 
     @classmethod
     def get_extra_plugin_menu_items(cls, request, plugin):
         if plugin.plugin_type == cls.__name__:
             return
@@ -209,15 +204,15 @@
             target_plugin = None
         else:
             target_plugin = form.cleaned_data['target_plugin']
             target_placeholder = target_plugin.placeholder
 
         if not target_placeholder.has_add_plugin_permission(request.user, module_plugin.plugin_type):
             return HttpResponseForbidden(
-                force_text(_('You do not have permission to add a plugin.'))
+                force_str(_('You do not have permission to add a plugin.'))
             )
 
         pl_admin = target_placeholder._get_attached_admin()
 
         if pl_admin:
             template = pl_admin.get_placeholder_template(request, target_placeholder)
         else:
```

### Comparing `djangocms-modules-1.0.0/djangocms_modules/cms_toolbars.py` & `djangocms-modules-2.0.0/djangocms_modules/cms_toolbars.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.translation import gettext_lazy as _
 
 from cms.cms_toolbars import ADMIN_MENU_IDENTIFIER, ADMINISTRATION_BREAK
 from cms.toolbar.items import Break
 from cms.toolbar_base import CMSToolbar
 from cms.toolbar_pool import toolbar_pool
 from cms.utils.urlutils import admin_reverse
@@ -37,15 +37,15 @@
             admin_menu.add_break(SHORTCUTS_BREAK, position=end.index)
             start = admin_menu.find_first(Break, identifier=SHORTCUTS_BREAK)
         end = admin_menu.find_first(Break, identifier=ADMINISTRATION_BREAK)
 
         items = admin_menu.get_items()[start.index + 1: end.index]
         for idx, item in enumerate(items):
             try:
-                if force_text(item_name.lower()) < force_text(item.name.lower()):
+                if force_str(item_name.lower()) < force_str(item.name.lower()):
                     return idx + start.index + 1
             except AttributeError:
                 # Some item types do not have a 'name' attribute.
                 pass
         return end.index
 
     def populate(self):
```

### Comparing `djangocms-modules-1.0.0/djangocms_modules/forms.py` & `djangocms-modules-2.0.0/djangocms_modules/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from django import forms
 from django.conf import settings
 from django.contrib import admin
-from django.contrib.admin.widgets import (
-    AdminTextInputWidget, RelatedFieldWidgetWrapper,
-)
+from django.contrib.admin.widgets import AdminTextInputWidget, RelatedFieldWidgetWrapper
 from django.utils.translation import gettext_lazy as _
 
 from cms.models import CMSPlugin, Placeholder
 
 from .models import Category, ModulePlugin
```

### Comparing `djangocms-modules-1.0.0/djangocms_modules/handlers.py` & `djangocms-modules-2.0.0/djangocms_modules/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 from cms import operations
 from cms.models import CMSPlugin
 
 from .models import Category, ModulePlugin
 
 
 def sync_module_category(sender, **kwargs):
-    from djangocms_history.actions import (
-        MOVE_IN_PLUGIN,
-        MOVE_OUT_PLUGIN,
-    )
+    from djangocms_history.actions import MOVE_IN_PLUGIN, MOVE_OUT_PLUGIN
 
     operation = kwargs['operation']
     actions = kwargs['actions']
     affected_operations = (operations.MOVE_PLUGIN, operations.PASTE_PLUGIN)
 
     if operation.operation_type not in affected_operations:
         return
```

### Comparing `djangocms-modules-1.0.0/djangocms_modules/management/commands/update_modules_language.py` & `djangocms-modules-2.0.0/djangocms_modules/management/commands/update_modules_language.py`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/migrations/0001_initial.py` & `djangocms-modules-2.0.0/djangocms_modules/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/migrations/0002_auto_20190122_0412.py` & `djangocms-modules-2.0.0/djangocms_modules/migrations/0002_auto_20190122_0412.py`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/models.py` & `djangocms-modules-2.0.0/djangocms_modules/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from cms.models import CMSPlugin, Placeholder
 from cms.models.fields import PlaceholderField
 from cms.signals import pre_placeholder_operation
 from cms.utils.plugins import get_bound_plugins
 
 
 def _get_placeholder_slot(category):
-    return 'module-category-{}'.format(category.pk)
+    return f'module-category-{category.pk}'
 
 
 @receiver(pre_placeholder_operation)
 def sync_module_plugin(sender, **kwargs):
     """
     Updates the created placeholder operation record,
     based on the configured post operation handlers.
```

### Comparing `djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/css/modules.css` & `djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/css/modules.css`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/js/copy.js` & `djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/js/copy.js`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/js/dist/bundle.modules.min.js` & `djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/js/dist/bundle.modules.min.js`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/js/plugin.js` & `djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/js/plugin.js`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/static/djangocms_modules/js/structureboard.js` & `djangocms-modules-2.0.0/djangocms_modules/static/djangocms_modules/js/structureboard.js`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/templates/cms/toolbar/dragitem_menu.html` & `djangocms-modules-2.0.0/djangocms_modules/templates/cms/toolbar/dragitem_menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/templates/djangocms_modules/add_module.html` & `djangocms-modules-2.0.0/djangocms_modules/templates/djangocms_modules/add_module.html`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/templates/djangocms_modules/create_module.html` & `djangocms-modules-2.0.0/djangocms_modules/templates/djangocms_modules/create_module.html`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/templates/djangocms_modules/modules_list.html` & `djangocms-modules-2.0.0/djangocms_modules/templates/djangocms_modules/modules_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/templates/djangocms_modules/render_module.html` & `djangocms-modules-2.0.0/djangocms_modules/templates/djangocms_modules/render_module.html`

 * *Files identical despite different names*

### Comparing `djangocms-modules-1.0.0/djangocms_modules/templatetags/djangocms_modules_tags.py` & `djangocms-modules-2.0.0/djangocms_modules/templatetags/djangocms_modules_tags.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 @register.simple_tag()
 def get_module_add_url(module_):
     return admin_reverse('cms_add_module', args=[module_.pk])
 
 
 @register.simple_tag(takes_context=False)
 def get_module_url(module_):
-    return admin_reverse('cms_modules_list') + '#cms-plugin-{}'.format(module_.pk)
+    return admin_reverse('cms_modules_list') + f'#cms-plugin-{module_.pk}'
```

### Comparing `djangocms-modules-1.0.0/djangocms_modules.egg-info/SOURCES.txt` & `djangocms-modules-2.0.0/djangocms_modules.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 djangocms_modules/__init__.py
 djangocms_modules/admin.py
 djangocms_modules/apps.py
 djangocms_modules/cms_plugins.py
 djangocms_modules/cms_toolbars.py
 djangocms_modules/forms.py
@@ -17,14 +18,15 @@
 djangocms_modules.egg-info/requires.txt
 djangocms_modules.egg-info/top_level.txt
 djangocms_modules/management/__init__.py
 djangocms_modules/management/commands/__init__.py
 djangocms_modules/management/commands/update_modules_language.py
 djangocms_modules/migrations/0001_initial.py
 djangocms_modules/migrations/0002_auto_20190122_0412.py
+djangocms_modules/migrations/0003_alter_moduleplugin_cmsplugin_ptr.py
 djangocms_modules/migrations/__init__.py
 djangocms_modules/static/djangocms_modules/css/modules.css
 djangocms_modules/static/djangocms_modules/img/icon.png
 djangocms_modules/static/djangocms_modules/js/base.js
 djangocms_modules/static/djangocms_modules/js/copy.js
 djangocms_modules/static/djangocms_modules/js/plugin.js
 djangocms_modules/static/djangocms_modules/js/structureboard.js
```

### Comparing `djangocms-modules-1.0.0/setup.py` & `djangocms-modules-2.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,51 +2,54 @@
 from setuptools import find_packages, setup
 
 from djangocms_modules import __version__
 
 
 REQUIREMENTS = [
     'django-cms>=3.7',
+    'djangocms-history',
+    'django-treebeard>=4.3,<4.5',
 ]
 
 
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.5',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
     'Framework :: Django',
-    'Framework :: Django :: 2.2',
-    'Framework :: Django :: 3.0',
-    'Framework :: Django :: 3.1',
+    'Framework :: Django :: 3.2',
+    'Framework :: Django :: 4.0',
     'Framework :: Django CMS',
-    'Framework :: Django CMS :: 3.7',
-    'Framework :: Django CMS :: 3.8',
+    'Framework :: Django CMS :: 3.10',
+    'Framework :: Django CMS :: 3.11',
     'Topic :: Internet :: WWW/HTTP',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Software Development',
     'Topic :: Software Development :: Libraries',
 ]
 
 setup(
     name='djangocms-modules',
     version=__version__,
     author='Divio AG',
     author_email='info@divio.ch',
-    url='https://github.com/divio/djangocms-modules',
+    maintainer='Django CMS Association and contributors',
+    maintainer_email='info@django-cms.org',
+    url='https://github.com/django-cms/djangocms-modules',
     license='BSD-3-Clause',
     description='Adds copy/paste capabilities to groups of plugins',
     long_description=open('README.rst').read(),
-    packages=find_packages(),
+    packages=find_packages(exclude=['tests']),
     include_package_data=True,
     zip_safe=False,
     install_requires=REQUIREMENTS,
     classifiers=CLASSIFIERS,
+    python_requires='>=3.8',
     test_suite='tests.settings.run',
 )
```

### Comparing `djangocms-modules-1.0.0/tests/test_migrations.py` & `djangocms-modules-2.0.0/tests/test_migrations.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,8 +23,8 @@
         except SystemExit as e:
             status_code = str(e)
         else:
             # the "no changes" exit code is 0
             status_code = '0'
 
         if status_code == '1':
-            self.fail('There are missing migrations:\n {}'.format(output.getvalue()))
+            self.fail(f'There are missing migrations:\n {output.getvalue()}')
```

