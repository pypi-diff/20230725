# Comparing `tmp/crawler_studio-1.5.5.tar.gz` & `tmp/crawler_studio-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crawler_studio-1.5.5.tar", last modified: Tue Jul 25 05:59:45 2023, max compression
+gzip compressed data, was "dist/crawler_studio-1.5.6.tar", last modified: Tue Jul 25 08:34:12 2023, max compression
```

## Comparing `crawler_studio-1.5.5.tar` & `crawler_studio-1.5.6.tar`

### file list

```diff
@@ -1,339 +1,340 @@
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/
--rw-r--r--   0 arron      (502) staff       (20)      761 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/PKG-INFO
--rw-r--r--   0 arron      (502) staff       (20)     1189 2022-11-18 06:30:16.000000 crawler_studio-1.5.5/README.md
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/
--rw-r--r--   0 arron      (502) staff       (20)      120 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/__init__.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/app_logs/
--rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-20 03:33:11.000000 crawler_studio-1.5.5/crawler_studio/app_logs/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)      162 2022-09-22 16:26:25.000000 crawler_studio-1.5.5/crawler_studio/app_logs/apps.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/app_logs/migrations/
--rw-r--r--   0 arron      (502) staff       (20)     3272 2022-09-22 17:15:31.000000 crawler_studio-1.5.5/crawler_studio/app_logs/migrations/0001_initial.py
--rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-22 17:15:31.000000 crawler_studio-1.5.5/crawler_studio/app_logs/migrations/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)     2412 2022-09-22 17:06:46.000000 crawler_studio-1.5.5/crawler_studio/app_logs/models.py
--rw-r--r--   0 arron      (502) staff       (20)      593 2022-09-22 17:14:04.000000 crawler_studio-1.5.5/crawler_studio/app_logs/ser.py
--rw-r--r--   0 arron      (502) staff       (20)      454 2022-11-17 04:21:16.000000 crawler_studio-1.5.5/crawler_studio/app_logs/urls.py
--rw-r--r--   0 arron      (502) staff       (20)     8308 2022-11-17 08:09:05.000000 crawler_studio-1.5.5/crawler_studio/app_logs/views.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/app_schedule/
--rw-r--r--   0 arron      (502) staff       (20)        0 2022-11-14 01:48:08.000000 crawler_studio-1.5.5/crawler_studio/app_schedule/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)       63 2022-11-14 01:48:08.000000 crawler_studio-1.5.5/crawler_studio/app_schedule/admin.py
--rw-r--r--   0 arron      (502) staff       (20)      170 2022-11-14 03:21:39.000000 crawler_studio-1.5.5/crawler_studio/app_schedule/apps.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/app_schedule/migrations/
--rw-r--r--   0 arron      (502) staff       (20)     2596 2022-11-14 04:52:18.000000 crawler_studio-1.5.5/crawler_studio/app_schedule/migrations/0001_initial.py
--rw-r--r--   0 arron      (502) staff       (20)        0 2022-11-14 04:52:18.000000 crawler_studio-1.5.5/crawler_studio/app_schedule/migrations/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)     1998 2022-11-14 01:50:47.000000 crawler_studio-1.5.5/crawler_studio/app_schedule/models.py
--rw-r--r--   0 arron      (502) staff       (20)     2655 2022-11-14 06:30:44.000000 crawler_studio-1.5.5/crawler_studio/app_schedule/ser.py
--rw-r--r--   0 arron      (502) staff       (20)      279 2022-11-14 06:30:44.000000 crawler_studio-1.5.5/crawler_studio/app_schedule/urls.py
--rw-r--r--   0 arron      (502) staff       (20)     5470 2022-11-17 08:45:17.000000 crawler_studio-1.5.5/crawler_studio/app_schedule/views.py
--rw-r--r--   0 arron      (502) staff       (20)     2818 2022-11-14 06:40:24.000000 crawler_studio-1.5.5/crawler_studio/app_schedule/worker.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/
--rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)       63 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/admin.py
--rw-r--r--   0 arron      (502) staff       (20)      111 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/apps.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/migrations/
--rw-r--r--   0 arron      (502) staff       (20)     2196 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/migrations/0001_initial.py
--rw-r--r--   0 arron      (502) staff       (20)      454 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/migrations/0002_auto_20220624_1644.py
--rw-r--r--   0 arron      (502) staff       (20)     3742 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/migrations/0003_auto_20220812_1436.py
--rw-r--r--   0 arron      (502) staff       (20)      559 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/migrations/0004_auto_20220905_1014.py
--rw-r--r--   0 arron      (502) staff       (20)      461 2022-09-22 17:12:45.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/migrations/0005_auto_20220923_0112.py
--rw-r--r--   0 arron      (502) staff       (20)     1465 2022-11-14 03:21:42.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/migrations/0006_spiderstartparams.py
--rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/migrations/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)     2376 2022-11-15 09:54:48.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/models.py
--rw-r--r--   0 arron      (502) staff       (20)      863 2022-11-15 09:54:48.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/ser.py
--rw-r--r--   0 arron      (502) staff       (20)      475 2022-11-14 06:54:07.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/urls.py
--rw-r--r--   0 arron      (502) staff       (20)     9597 2023-07-24 16:09:50.000000 crawler_studio-1.5.5/crawler_studio/app_scrapyd/views.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/app_settings/
--rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_settings/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)       63 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_settings/admin.py
--rw-r--r--   0 arron      (502) staff       (20)      170 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_settings/apps.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/app_settings/migrations/
--rw-r--r--   0 arron      (502) staff       (20)     1358 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_settings/migrations/0001_initial.py
--rw-r--r--   0 arron      (502) staff       (20)      293 2022-09-20 06:59:24.000000 crawler_studio-1.5.5/crawler_studio/app_settings/migrations/0002_delete_logserver.py
--rw-r--r--   0 arron      (502) staff       (20)      795 2022-11-16 12:50:11.000000 crawler_studio-1.5.5/crawler_studio/app_settings/migrations/0003_mailsender.py
--rw-r--r--   0 arron      (502) staff       (20)      440 2022-11-16 13:02:09.000000 crawler_studio-1.5.5/crawler_studio/app_settings/migrations/0004_mailsender_auth_code.py
--rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_settings/migrations/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)      864 2022-11-16 13:01:35.000000 crawler_studio-1.5.5/crawler_studio/app_settings/models.py
--rw-r--r--   0 arron      (502) staff       (20)      441 2022-11-16 10:30:19.000000 crawler_studio-1.5.5/crawler_studio/app_settings/ser.py
--rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_settings/tests.py
--rw-r--r--   0 arron      (502) staff       (20)      299 2022-11-16 13:16:39.000000 crawler_studio-1.5.5/crawler_studio/app_settings/urls.py
--rw-r--r--   0 arron      (502) staff       (20)     3439 2022-11-17 08:43:56.000000 crawler_studio-1.5.5/crawler_studio/app_settings/views.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/app_user/
--rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_user/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)       63 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_user/admin.py
--rw-r--r--   0 arron      (502) staff       (20)      162 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_user/apps.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/app_user/migrations/
--rw-r--r--   0 arron      (502) staff       (20)      619 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_user/migrations/0001_initial.py
--rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_user/migrations/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)      228 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_user/models.py
--rw-r--r--   0 arron      (502) staff       (20)       60 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_user/tests.py
--rw-r--r--   0 arron      (502) staff       (20)      181 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/app_user/urls.py
--rw-r--r--   0 arron      (502) staff       (20)     1938 2022-09-21 09:54:18.000000 crawler_studio-1.5.5/crawler_studio/app_user/views.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/cmd/
--rw-r--r--   0 arron      (502) staff       (20)      233 2022-11-15 08:58:49.000000 crawler_studio-1.5.5/crawler_studio/cmd/__init__.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/cmd/__pycache__/
--rw-r--r--   0 arron      (502) staff       (20)      466 2022-11-15 09:10:05.000000 crawler_studio-1.5.5/crawler_studio/cmd/__pycache__/__init__.cpython-37.pyc
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/cmd/management/
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/cmd/management/commands/
--rw-r--r--   0 arron      (502) staff       (20)       91 2022-11-15 08:58:51.000000 crawler_studio-1.5.5/crawler_studio/cmd/management/commands/__init__.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/cmd/management/commands/__pycache__/
--rw-r--r--   0 arron      (502) staff       (20)      287 2022-11-15 09:10:07.000000 crawler_studio-1.5.5/crawler_studio/cmd/management/commands/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 arron      (502) staff       (20)     1318 2023-03-12 03:16:51.000000 crawler_studio-1.5.5/crawler_studio/cmd/management/commands/__pycache__/get_token.cpython-37.pyc
--rw-r--r--   0 arron      (502) staff       (20)     1391 2022-11-17 08:35:09.000000 crawler_studio-1.5.5/crawler_studio/cmd/management/commands/__pycache__/init.cpython-37.pyc
--rw-r--r--   0 arron      (502) staff       (20)      862 2023-07-24 16:09:50.000000 crawler_studio-1.5.5/crawler_studio/cmd/management/commands/get_token.py
--rw-r--r--   0 arron      (502) staff       (20)      790 2022-11-17 03:54:11.000000 crawler_studio-1.5.5/crawler_studio/cmd/management/commands/init.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/crawler_studio/
--rw-r--r--   0 arron      (502) staff       (20)      116 2022-11-14 04:43:28.000000 crawler_studio-1.5.5/crawler_studio/crawler_studio/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)      423 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/crawler_studio/asgi.py
--rw-r--r--   0 arron      (502) staff       (20)      750 2022-11-15 09:56:08.000000 crawler_studio-1.5.5/crawler_studio/crawler_studio/custom_field.py
--rw-r--r--   0 arron      (502) staff       (20)     4920 2023-07-25 05:32:36.000000 crawler_studio-1.5.5/crawler_studio/crawler_studio/settings.py
--rw-r--r--   0 arron      (502) staff       (20)     1575 2023-07-25 05:32:12.000000 crawler_studio-1.5.5/crawler_studio/crawler_studio/urls.py
--rw-r--r--   0 arron      (502) staff       (20)      423 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/crawler_studio/wsgi.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/dist/
--rw-r--r--   0 arron      (502) staff       (20)    21662 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/favicon.ico
--rw-r--r--   0 arron      (502) staff       (20)      860 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/index.html
--rw-r--r--   0 arron      (502) staff       (20)    38823 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/logo.jpeg
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/dist/static/
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/dist/static/fonts/
--rw-r--r--   0 arron      (502) staff       (20)    28200 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/fonts/element-icons.535877f5.woff
--rw-r--r--   0 arron      (502) staff       (20)    55956 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/fonts/element-icons.732389de.ttf
--rw-r--r--   0 arron      (502) staff       (20)    82216 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/fonts/ionicons.143146fa.woff2
--rw-r--r--   0 arron      (502) staff       (20)   197740 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/fonts/ionicons.99ac3308.woff
--rw-r--r--   0 arron      (502) staff       (20)   197664 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/fonts/ionicons.d535a25a.ttf
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/dist/static/img/
--rw-r--r--   0 arron      (502) staff       (20)    67646 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/img/favicon.37e81aa2.png
--rw-r--r--   0 arron      (502) staff       (20)   555353 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/img/ionicons.a2c4a261.svg
--rw-r--r--   0 arron      (502) staff       (20)  1169238 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/img/universe.0efde44f.jpeg
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/dist/static/js/
--rw-r--r--   0 arron      (502) staff       (20)    64548 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/js/0.js
--rw-r--r--   0 arron      (502) staff       (20)   118874 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/js/1.js
--rw-r--r--   0 arron      (502) staff       (20)    90525 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/js/2.js
--rw-r--r--   0 arron      (502) staff       (20)    79539 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/js/3.js
--rw-r--r--   0 arron      (502) staff       (20)    69314 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/js/4.js
--rw-r--r--   0 arron      (502) staff       (20)    54102 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/js/5.js
--rw-r--r--   0 arron      (502) staff       (20)    17781 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/js/6.js
--rw-r--r--   0 arron      (502) staff       (20)   328960 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/js/app.js
--rw-r--r--   0 arron      (502) staff       (20)  8841692 2023-07-24 16:20:06.000000 crawler_studio-1.5.5/crawler_studio/dist/static/js/chunk-vendors.js
--rwxr-xr-x   0 arron      (502) staff       (20)      782 2023-07-25 03:39:30.000000 crawler_studio-1.5.5/crawler_studio/manage.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/static/
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/static/admin/
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/
--rw-r--r--   0 arron      (502) staff       (20)     9114 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/autocomplete.css
--rw-r--r--   0 arron      (502) staff       (20)    19513 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/base.css
--rw-r--r--   0 arron      (502) staff       (20)     6874 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/changelists.css
--rw-r--r--   0 arron      (502) staff       (20)      380 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/dashboard.css
--rw-r--r--   0 arron      (502) staff       (20)      423 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/fonts.css
--rw-r--r--   0 arron      (502) staff       (20)     8804 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/forms.css
--rw-r--r--   0 arron      (502) staff       (20)      939 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/login.css
--rw-r--r--   0 arron      (502) staff       (20)     2271 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/nav_sidebar.css
--rw-r--r--   0 arron      (502) staff       (20)    18545 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/responsive.css
--rw-r--r--   0 arron      (502) staff       (20)     1741 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/responsive_rtl.css
--rw-r--r--   0 arron      (502) staff       (20)     3234 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/rtl.css
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/vendor/
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/vendor/select2/
--rw-r--r--   0 arron      (502) staff       (20)     1124 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/vendor/select2/LICENSE-SELECT2.md
--rw-r--r--   0 arron      (502) staff       (20)    17358 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/vendor/select2/select2.css
--rw-r--r--   0 arron      (502) staff       (20)    14966 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/vendor/select2/select2.min.css
--rw-r--r--   0 arron      (502) staff       (20)    11097 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/css/widgets.css
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/admin/fonts/
--rw-r--r--   0 arron      (502) staff       (20)    11560 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/fonts/LICENSE.txt
--rw-r--r--   0 arron      (502) staff       (20)      214 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/fonts/README.txt
--rw-r--r--   0 arron      (502) staff       (20)    86184 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/fonts/Roboto-Bold-webfont.woff
--rw-r--r--   0 arron      (502) staff       (20)    85692 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/fonts/Roboto-Light-webfont.woff
--rw-r--r--   0 arron      (502) staff       (20)    85876 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/fonts/Roboto-Regular-webfont.woff
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/
--rw-r--r--   0 arron      (502) staff       (20)     1081 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/LICENSE
--rw-r--r--   0 arron      (502) staff       (20)      319 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/README.txt
--rw-r--r--   0 arron      (502) staff       (20)     1094 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/calendar-icons.svg
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/gis/
--rw-r--r--   0 arron      (502) staff       (20)     1129 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/gis/move_vertex_off.svg
--rw-r--r--   0 arron      (502) staff       (20)     1129 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/gis/move_vertex_on.svg
--rw-r--r--   0 arron      (502) staff       (20)      331 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-addlink.svg
--rw-r--r--   0 arron      (502) staff       (20)      504 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-alert.svg
--rw-r--r--   0 arron      (502) staff       (20)     1086 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-calendar.svg
--rw-r--r--   0 arron      (502) staff       (20)      380 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-changelink.svg
--rw-r--r--   0 arron      (502) staff       (20)      677 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-clock.svg
--rw-r--r--   0 arron      (502) staff       (20)      392 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-deletelink.svg
--rw-r--r--   0 arron      (502) staff       (20)      560 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-no.svg
--rw-r--r--   0 arron      (502) staff       (20)      655 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-unknown-alt.svg
--rw-r--r--   0 arron      (502) staff       (20)      655 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-unknown.svg
--rw-r--r--   0 arron      (502) staff       (20)      581 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-viewlink.svg
--rw-r--r--   0 arron      (502) staff       (20)      436 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-yes.svg
--rw-r--r--   0 arron      (502) staff       (20)      560 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/inline-delete.svg
--rw-r--r--   0 arron      (502) staff       (20)      458 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/search.svg
--rw-r--r--   0 arron      (502) staff       (20)     3291 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/selector-icons.svg
--rw-r--r--   0 arron      (502) staff       (20)     1097 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/sorting-icons.svg
--rw-r--r--   0 arron      (502) staff       (20)      331 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/tooltag-add.svg
--rw-r--r--   0 arron      (502) staff       (20)      280 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/img/tooltag-arrowright.svg
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/
--rw-r--r--   0 arron      (502) staff       (20)     4360 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/SelectBox.js
--rw-r--r--   0 arron      (502) staff       (20)    12350 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/SelectFilter2.js
--rw-r--r--   0 arron      (502) staff       (20)     7867 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/actions.js
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/admin/
--rw-r--r--   0 arron      (502) staff       (20)    19634 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/admin/DateTimeShortcuts.js
--rw-r--r--   0 arron      (502) staff       (20)     5984 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/admin/RelatedObjectLookups.js
--rw-r--r--   0 arron      (502) staff       (20)     1320 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/autocomplete.js
--rw-r--r--   0 arron      (502) staff       (20)     8466 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/calendar.js
--rw-r--r--   0 arron      (502) staff       (20)      884 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/cancel.js
--rw-r--r--   0 arron      (502) staff       (20)      606 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/change_form.js
--rw-r--r--   0 arron      (502) staff       (20)     1803 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/collapse.js
--rw-r--r--   0 arron      (502) staff       (20)     5698 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/core.js
--rw-r--r--   0 arron      (502) staff       (20)    15225 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/inlines.js
--rw-r--r--   0 arron      (502) staff       (20)      347 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/jquery.init.js
--rw-r--r--   0 arron      (502) staff       (20)     1360 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/nav_sidebar.js
--rw-r--r--   0 arron      (502) staff       (20)      551 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/popup_response.js
--rw-r--r--   0 arron      (502) staff       (20)     1531 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/prepopulate.js
--rw-r--r--   0 arron      (502) staff       (20)      492 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/prepopulate_init.js
--rw-r--r--   0 arron      (502) staff       (20)     7902 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/urlify.js
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/jquery/
--rw-r--r--   0 arron      (502) staff       (20)     1095 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/jquery/LICENSE.txt
--rw-r--r--   0 arron      (502) staff       (20)   287630 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/jquery/jquery.js
--rw-r--r--   0 arron      (502) staff       (20)    89476 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/jquery/jquery.min.js
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/
--rw-r--r--   0 arron      (502) staff       (20)     1124 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/LICENSE.md
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/
--rw-r--r--   0 arron      (502) staff       (20)      866 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/af.js
--rw-r--r--   0 arron      (502) staff       (20)      905 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ar.js
--rw-r--r--   0 arron      (502) staff       (20)      721 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/az.js
--rw-r--r--   0 arron      (502) staff       (20)      968 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/bg.js
--rw-r--r--   0 arron      (502) staff       (20)     1291 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/bn.js
--rw-r--r--   0 arron      (502) staff       (20)      965 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/bs.js
--rw-r--r--   0 arron      (502) staff       (20)      900 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ca.js
--rw-r--r--   0 arron      (502) staff       (20)     1292 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/cs.js
--rw-r--r--   0 arron      (502) staff       (20)      828 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/da.js
--rw-r--r--   0 arron      (502) staff       (20)      866 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/de.js
--rw-r--r--   0 arron      (502) staff       (20)     1017 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/dsb.js
--rw-r--r--   0 arron      (502) staff       (20)     1182 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/el.js
--rw-r--r--   0 arron      (502) staff       (20)      844 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/en.js
--rw-r--r--   0 arron      (502) staff       (20)      922 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/es.js
--rw-r--r--   0 arron      (502) staff       (20)      801 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/et.js
--rw-r--r--   0 arron      (502) staff       (20)      868 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/eu.js
--rw-r--r--   0 arron      (502) staff       (20)     1023 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/fa.js
--rw-r--r--   0 arron      (502) staff       (20)      803 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/fi.js
--rw-r--r--   0 arron      (502) staff       (20)      924 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/fr.js
--rw-r--r--   0 arron      (502) staff       (20)      924 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/gl.js
--rw-r--r--   0 arron      (502) staff       (20)      984 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/he.js
--rw-r--r--   0 arron      (502) staff       (20)     1175 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/hi.js
--rw-r--r--   0 arron      (502) staff       (20)      852 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/hr.js
--rw-r--r--   0 arron      (502) staff       (20)     1018 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/hsb.js
--rw-r--r--   0 arron      (502) staff       (20)      831 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/hu.js
--rw-r--r--   0 arron      (502) staff       (20)     1028 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/hy.js
--rw-r--r--   0 arron      (502) staff       (20)      768 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/id.js
--rw-r--r--   0 arron      (502) staff       (20)      807 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/is.js
--rw-r--r--   0 arron      (502) staff       (20)      897 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/it.js
--rw-r--r--   0 arron      (502) staff       (20)      862 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ja.js
--rw-r--r--   0 arron      (502) staff       (20)     1195 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ka.js
--rw-r--r--   0 arron      (502) staff       (20)     1088 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/km.js
--rw-r--r--   0 arron      (502) staff       (20)      855 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ko.js
--rw-r--r--   0 arron      (502) staff       (20)      944 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/lt.js
--rw-r--r--   0 arron      (502) staff       (20)      900 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/lv.js
--rw-r--r--   0 arron      (502) staff       (20)     1038 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/mk.js
--rw-r--r--   0 arron      (502) staff       (20)      811 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ms.js
--rw-r--r--   0 arron      (502) staff       (20)      778 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/nb.js
--rw-r--r--   0 arron      (502) staff       (20)     1357 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ne.js
--rw-r--r--   0 arron      (502) staff       (20)      904 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/nl.js
--rw-r--r--   0 arron      (502) staff       (20)      947 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/pl.js
--rw-r--r--   0 arron      (502) staff       (20)     1049 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ps.js
--rw-r--r--   0 arron      (502) staff       (20)      876 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/pt-BR.js
--rw-r--r--   0 arron      (502) staff       (20)      878 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/pt.js
--rw-r--r--   0 arron      (502) staff       (20)      938 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ro.js
--rw-r--r--   0 arron      (502) staff       (20)     1171 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ru.js
--rw-r--r--   0 arron      (502) staff       (20)     1306 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/sk.js
--rw-r--r--   0 arron      (502) staff       (20)      925 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/sl.js
--rw-r--r--   0 arron      (502) staff       (20)      903 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/sq.js
--rw-r--r--   0 arron      (502) staff       (20)     1109 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/sr-Cyrl.js
--rw-r--r--   0 arron      (502) staff       (20)      980 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/sr.js
--rw-r--r--   0 arron      (502) staff       (20)      786 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/sv.js
--rw-r--r--   0 arron      (502) staff       (20)     1074 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/th.js
--rw-r--r--   0 arron      (502) staff       (20)      771 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/tk.js
--rw-r--r--   0 arron      (502) staff       (20)      775 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/tr.js
--rw-r--r--   0 arron      (502) staff       (20)     1156 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/uk.js
--rw-r--r--   0 arron      (502) staff       (20)      796 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/vi.js
--rw-r--r--   0 arron      (502) staff       (20)      768 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/zh-CN.js
--rw-r--r--   0 arron      (502) staff       (20)      707 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/zh-TW.js
--rw-r--r--   0 arron      (502) staff       (20)   173566 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/select2.full.js
--rw-r--r--   0 arron      (502) staff       (20)    79212 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/select2.full.min.js
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/xregexp/
--rw-r--r--   0 arron      (502) staff       (20)     1103 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/xregexp/LICENSE.txt
--rw-r--r--   0 arron      (502) staff       (20)   232381 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/xregexp/xregexp.js
--rw-r--r--   0 arron      (502) staff       (20)   125266 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/xregexp/xregexp.min.js
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/fonts/
--rw-r--r--   0 arron      (502) staff       (20)    28200 2023-07-25 05:32:12.000000 crawler_studio-1.5.5/crawler_studio/static/fonts/element-icons.535877f5.woff
--rw-r--r--   0 arron      (502) staff       (20)    55956 2023-07-25 05:32:12.000000 crawler_studio-1.5.5/crawler_studio/static/fonts/element-icons.732389de.ttf
--rw-r--r--   0 arron      (502) staff       (20)    82216 2023-07-25 05:32:12.000000 crawler_studio-1.5.5/crawler_studio/static/fonts/ionicons.143146fa.woff2
--rw-r--r--   0 arron      (502) staff       (20)   197740 2023-07-25 05:32:12.000000 crawler_studio-1.5.5/crawler_studio/static/fonts/ionicons.99ac3308.woff
--rw-r--r--   0 arron      (502) staff       (20)   197664 2023-07-25 05:32:12.000000 crawler_studio-1.5.5/crawler_studio/static/fonts/ionicons.d535a25a.ttf
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/img/
--rw-r--r--   0 arron      (502) staff       (20)    67646 2023-07-25 05:32:12.000000 crawler_studio-1.5.5/crawler_studio/static/img/favicon.37e81aa2.png
--rw-r--r--   0 arron      (502) staff       (20)   555353 2023-07-25 05:32:12.000000 crawler_studio-1.5.5/crawler_studio/static/img/ionicons.a2c4a261.svg
--rw-r--r--   0 arron      (502) staff       (20)  1169238 2023-07-25 05:32:12.000000 crawler_studio-1.5.5/crawler_studio/static/img/universe.0efde44f.jpeg
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/js/
--rw-r--r--   0 arron      (502) staff       (20)    64548 2023-07-25 05:32:22.000000 crawler_studio-1.5.5/crawler_studio/static/js/0.js
--rw-r--r--   0 arron      (502) staff       (20)   118874 2023-07-25 05:32:22.000000 crawler_studio-1.5.5/crawler_studio/static/js/1.js
--rw-r--r--   0 arron      (502) staff       (20)    90525 2023-07-25 05:32:22.000000 crawler_studio-1.5.5/crawler_studio/static/js/2.js
--rw-r--r--   0 arron      (502) staff       (20)    79539 2023-07-25 05:32:22.000000 crawler_studio-1.5.5/crawler_studio/static/js/3.js
--rw-r--r--   0 arron      (502) staff       (20)    69314 2023-07-25 05:32:22.000000 crawler_studio-1.5.5/crawler_studio/static/js/4.js
--rw-r--r--   0 arron      (502) staff       (20)    54102 2023-07-25 05:32:22.000000 crawler_studio-1.5.5/crawler_studio/static/js/5.js
--rw-r--r--   0 arron      (502) staff       (20)    17781 2023-07-25 05:32:22.000000 crawler_studio-1.5.5/crawler_studio/static/js/6.js
--rw-r--r--   0 arron      (502) staff       (20)   328960 2023-07-25 05:32:22.000000 crawler_studio-1.5.5/crawler_studio/static/js/app.js
--rw-r--r--   0 arron      (502) staff       (20)  8841692 2023-07-25 05:32:12.000000 crawler_studio-1.5.5/crawler_studio/static/js/chunk-vendors.js
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/
--rw-r--r--   0 arron      (502) staff       (20)    23411 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/bootstrap-theme.min.css
--rw-r--r--   0 arron      (502) staff       (20)    75600 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/bootstrap-theme.min.css.map
--rw-r--r--   0 arron      (502) staff       (20)     3385 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/bootstrap-tweaks.css
--rw-r--r--   0 arron      (502) staff       (20)   121457 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/bootstrap.min.css
--rw-r--r--   0 arron      (502) staff       (20)   540434 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/bootstrap.min.css.map
--rw-r--r--   0 arron      (502) staff       (20)     1152 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/default.css
--rw-r--r--   0 arron      (502) staff       (20)    21658 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/font-awesome-4.0.3.css
--rw-r--r--   0 arron      (502) staff       (20)      817 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/prettify.css
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/css/
--rw-r--r--   0 arron      (502) staff       (20)     6156 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/css/base.css
--rw-r--r--   0 arron      (502) staff       (20)     1682 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/css/highlight.css
--rw-r--r--   0 arron      (502) staff       (20)     1307 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/css/jquery.json-view.min.css
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/img/
--rw-r--r--   0 arron      (502) staff       (20)     5430 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/img/favicon.ico
--rw-r--r--   0 arron      (502) staff       (20)     1458 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/img/grid.png
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/js/
--rw-r--r--   0 arron      (502) staff       (20)    10391 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/js/api.js
--rw-r--r--   0 arron      (502) staff       (20)   300764 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/js/highlight.pack.js
--rw-r--r--   0 arron      (502) staff       (20)     2700 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/js/jquery.json-view.min.js
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/
--rw-r--r--   0 arron      (502) staff       (20)    38205 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.eot
--rw-r--r--   0 arron      (502) staff       (20)   202148 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.svg
--rw-r--r--   0 arron      (502) staff       (20)    80652 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 arron      (502) staff       (20)    44432 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.woff
--rw-r--r--   0 arron      (502) staff       (20)    20127 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 arron      (502) staff       (20)   108738 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 arron      (502) staff       (20)    45404 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 arron      (502) staff       (20)    23424 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 arron      (502) staff       (20)    18028 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/img/
--rw-r--r--   0 arron      (502) staff       (20)     8777 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/img/glyphicons-halflings-white.png
--rw-r--r--   0 arron      (502) staff       (20)    12762 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/img/glyphicons-halflings.png
--rw-r--r--   0 arron      (502) staff       (20)     1458 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/img/grid.png
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/
--rw-r--r--   0 arron      (502) staff       (20)     3597 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/ajax-form.js
--rw-r--r--   0 arron      (502) staff       (20)    39680 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/bootstrap.min.js
--rw-r--r--   0 arron      (502) staff       (20)   157600 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/coreapi-0.1.1.js
--rw-r--r--   0 arron      (502) staff       (20)     1719 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/csrf.js
--rw-r--r--   0 arron      (502) staff       (20)     1268 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/default.js
--rw-r--r--   0 arron      (502) staff       (20)    89476 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/jquery-3.5.1.min.js
--rw-r--r--   0 arron      (502) staff       (20)    13632 2022-11-16 17:13:28.000000 crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/prettify-min.js
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/crawler_studio/utils/
--rw-r--r--   0 arron      (502) staff       (20)      120 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/utils/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)      182 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/utils/exceptions.py
--rw-r--r--   0 arron      (502) staff       (20)     3100 2023-07-24 16:09:50.000000 crawler_studio-1.5.5/crawler_studio/utils/message_transmit.py
--rw-r--r--   0 arron      (502) staff       (20)     1637 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/utils/time.py
--rw-r--r--   0 arron      (502) staff       (20)      299 2022-09-24 09:28:56.000000 crawler_studio-1.5.5/crawler_studio/utils/timer_scheduler.py
--rw-r--r--   0 arron      (502) staff       (20)      671 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/utils/variable_rule_trans.py
--rw-r--r--   0 arron      (502) staff       (20)     1949 2022-09-19 10:57:11.000000 crawler_studio-1.5.5/crawler_studio/utils/verifycation.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio.egg-info/
--rw-r--r--   0 arron      (502) staff       (20)      761 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio.egg-info/PKG-INFO
--rw-r--r--   0 arron      (502) staff       (20)    14143 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio.egg-info/SOURCES.txt
--rw-r--r--   0 arron      (502) staff       (20)        1 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio.egg-info/dependency_links.txt
--rw-r--r--   0 arron      (502) staff       (20)       47 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio.egg-info/entry_points.txt
--rw-r--r--   0 arron      (502) staff       (20)      150 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio.egg-info/requires.txt
--rw-r--r--   0 arron      (502) staff       (20)       15 2023-07-25 05:59:44.000000 crawler_studio-1.5.5/crawler_studio.egg-info/top_level.txt
--rw-r--r--   0 arron      (502) staff       (20)       38 2023-07-25 05:59:45.000000 crawler_studio-1.5.5/setup.cfg
--rw-r--r--   0 arron      (502) staff       (20)     1957 2023-07-25 05:59:41.000000 crawler_studio-1.5.5/setup.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/
+-rw-r--r--   0 arron      (502) staff       (20)      761 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/PKG-INFO
+-rw-r--r--   0 arron      (502) staff       (20)     1189 2022-11-18 06:30:16.000000 crawler_studio-1.5.6/README.md
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/
+-rw-r--r--   0 arron      (502) staff       (20)      120 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/__init__.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/app_logs/
+-rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-20 03:33:11.000000 crawler_studio-1.5.6/crawler_studio/app_logs/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)      162 2022-09-22 16:26:25.000000 crawler_studio-1.5.6/crawler_studio/app_logs/apps.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/app_logs/migrations/
+-rw-r--r--   0 arron      (502) staff       (20)     3272 2022-09-22 17:15:31.000000 crawler_studio-1.5.6/crawler_studio/app_logs/migrations/0001_initial.py
+-rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-22 17:15:31.000000 crawler_studio-1.5.6/crawler_studio/app_logs/migrations/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)     2412 2022-09-22 17:06:46.000000 crawler_studio-1.5.6/crawler_studio/app_logs/models.py
+-rw-r--r--   0 arron      (502) staff       (20)      593 2022-09-22 17:14:04.000000 crawler_studio-1.5.6/crawler_studio/app_logs/ser.py
+-rw-r--r--   0 arron      (502) staff       (20)      454 2022-11-17 04:21:16.000000 crawler_studio-1.5.6/crawler_studio/app_logs/urls.py
+-rw-r--r--   0 arron      (502) staff       (20)     8308 2022-11-17 08:09:05.000000 crawler_studio-1.5.6/crawler_studio/app_logs/views.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/
+-rw-r--r--   0 arron      (502) staff       (20)        0 2022-11-14 01:48:08.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)       63 2022-11-14 01:48:08.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/admin.py
+-rw-r--r--   0 arron      (502) staff       (20)      170 2022-11-14 03:21:39.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/apps.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/migrations/
+-rw-r--r--   0 arron      (502) staff       (20)     2596 2022-11-14 04:52:18.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/migrations/0001_initial.py
+-rw-r--r--   0 arron      (502) staff       (20)      433 2023-07-25 08:02:29.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/migrations/0002_monitorrules_start_params.py
+-rw-r--r--   0 arron      (502) staff       (20)        0 2022-11-14 04:52:18.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/migrations/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)     2091 2023-07-25 07:56:37.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/models.py
+-rw-r--r--   0 arron      (502) staff       (20)     2655 2022-11-14 06:30:44.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/ser.py
+-rw-r--r--   0 arron      (502) staff       (20)      279 2022-11-14 06:30:44.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/urls.py
+-rw-r--r--   0 arron      (502) staff       (20)     5470 2022-11-17 08:45:17.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/views.py
+-rw-r--r--   0 arron      (502) staff       (20)     2818 2022-11-14 06:40:24.000000 crawler_studio-1.5.6/crawler_studio/app_schedule/worker.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/
+-rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)       63 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/admin.py
+-rw-r--r--   0 arron      (502) staff       (20)      111 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/apps.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/migrations/
+-rw-r--r--   0 arron      (502) staff       (20)     2196 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/migrations/0001_initial.py
+-rw-r--r--   0 arron      (502) staff       (20)      454 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/migrations/0002_auto_20220624_1644.py
+-rw-r--r--   0 arron      (502) staff       (20)     3742 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/migrations/0003_auto_20220812_1436.py
+-rw-r--r--   0 arron      (502) staff       (20)      559 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/migrations/0004_auto_20220905_1014.py
+-rw-r--r--   0 arron      (502) staff       (20)      461 2022-09-22 17:12:45.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/migrations/0005_auto_20220923_0112.py
+-rw-r--r--   0 arron      (502) staff       (20)     1465 2022-11-14 03:21:42.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/migrations/0006_spiderstartparams.py
+-rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/migrations/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)     2376 2022-11-15 09:54:48.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/models.py
+-rw-r--r--   0 arron      (502) staff       (20)      863 2022-11-15 09:54:48.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/ser.py
+-rw-r--r--   0 arron      (502) staff       (20)      475 2022-11-14 06:54:07.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/urls.py
+-rw-r--r--   0 arron      (502) staff       (20)     9701 2023-07-25 08:06:51.000000 crawler_studio-1.5.6/crawler_studio/app_scrapyd/views.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/app_settings/
+-rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_settings/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)       63 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_settings/admin.py
+-rw-r--r--   0 arron      (502) staff       (20)      170 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_settings/apps.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/app_settings/migrations/
+-rw-r--r--   0 arron      (502) staff       (20)     1358 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_settings/migrations/0001_initial.py
+-rw-r--r--   0 arron      (502) staff       (20)      293 2022-09-20 06:59:24.000000 crawler_studio-1.5.6/crawler_studio/app_settings/migrations/0002_delete_logserver.py
+-rw-r--r--   0 arron      (502) staff       (20)      795 2022-11-16 12:50:11.000000 crawler_studio-1.5.6/crawler_studio/app_settings/migrations/0003_mailsender.py
+-rw-r--r--   0 arron      (502) staff       (20)      440 2022-11-16 13:02:09.000000 crawler_studio-1.5.6/crawler_studio/app_settings/migrations/0004_mailsender_auth_code.py
+-rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_settings/migrations/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)      864 2022-11-16 13:01:35.000000 crawler_studio-1.5.6/crawler_studio/app_settings/models.py
+-rw-r--r--   0 arron      (502) staff       (20)      441 2022-11-16 10:30:19.000000 crawler_studio-1.5.6/crawler_studio/app_settings/ser.py
+-rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_settings/tests.py
+-rw-r--r--   0 arron      (502) staff       (20)      299 2022-11-16 13:16:39.000000 crawler_studio-1.5.6/crawler_studio/app_settings/urls.py
+-rw-r--r--   0 arron      (502) staff       (20)     3439 2022-11-17 08:43:56.000000 crawler_studio-1.5.6/crawler_studio/app_settings/views.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/app_user/
+-rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_user/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)       63 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_user/admin.py
+-rw-r--r--   0 arron      (502) staff       (20)      162 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_user/apps.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/app_user/migrations/
+-rw-r--r--   0 arron      (502) staff       (20)      619 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_user/migrations/0001_initial.py
+-rw-r--r--   0 arron      (502) staff       (20)        0 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_user/migrations/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)      228 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_user/models.py
+-rw-r--r--   0 arron      (502) staff       (20)       60 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_user/tests.py
+-rw-r--r--   0 arron      (502) staff       (20)      181 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/app_user/urls.py
+-rw-r--r--   0 arron      (502) staff       (20)     1938 2022-09-21 09:54:18.000000 crawler_studio-1.5.6/crawler_studio/app_user/views.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/cmd/
+-rw-r--r--   0 arron      (502) staff       (20)      233 2022-11-15 08:58:49.000000 crawler_studio-1.5.6/crawler_studio/cmd/__init__.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/cmd/__pycache__/
+-rw-r--r--   0 arron      (502) staff       (20)      466 2022-11-15 09:10:05.000000 crawler_studio-1.5.6/crawler_studio/cmd/__pycache__/__init__.cpython-37.pyc
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/cmd/management/
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/cmd/management/commands/
+-rw-r--r--   0 arron      (502) staff       (20)       91 2022-11-15 08:58:51.000000 crawler_studio-1.5.6/crawler_studio/cmd/management/commands/__init__.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/cmd/management/commands/__pycache__/
+-rw-r--r--   0 arron      (502) staff       (20)      287 2022-11-15 09:10:07.000000 crawler_studio-1.5.6/crawler_studio/cmd/management/commands/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 arron      (502) staff       (20)     1318 2023-03-12 03:16:51.000000 crawler_studio-1.5.6/crawler_studio/cmd/management/commands/__pycache__/get_token.cpython-37.pyc
+-rw-r--r--   0 arron      (502) staff       (20)     1391 2022-11-17 08:35:09.000000 crawler_studio-1.5.6/crawler_studio/cmd/management/commands/__pycache__/init.cpython-37.pyc
+-rw-r--r--   0 arron      (502) staff       (20)      862 2023-07-24 16:09:50.000000 crawler_studio-1.5.6/crawler_studio/cmd/management/commands/get_token.py
+-rw-r--r--   0 arron      (502) staff       (20)      790 2022-11-17 03:54:11.000000 crawler_studio-1.5.6/crawler_studio/cmd/management/commands/init.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/crawler_studio/
+-rw-r--r--   0 arron      (502) staff       (20)      116 2022-11-14 04:43:28.000000 crawler_studio-1.5.6/crawler_studio/crawler_studio/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)      423 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/crawler_studio/asgi.py
+-rw-r--r--   0 arron      (502) staff       (20)      750 2022-11-15 09:56:08.000000 crawler_studio-1.5.6/crawler_studio/crawler_studio/custom_field.py
+-rw-r--r--   0 arron      (502) staff       (20)     4920 2023-07-25 05:32:36.000000 crawler_studio-1.5.6/crawler_studio/crawler_studio/settings.py
+-rw-r--r--   0 arron      (502) staff       (20)     1575 2023-07-25 05:32:12.000000 crawler_studio-1.5.6/crawler_studio/crawler_studio/urls.py
+-rw-r--r--   0 arron      (502) staff       (20)      423 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/crawler_studio/wsgi.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/dist/
+-rw-r--r--   0 arron      (502) staff       (20)    21662 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/favicon.ico
+-rw-r--r--   0 arron      (502) staff       (20)      860 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/index.html
+-rw-r--r--   0 arron      (502) staff       (20)    38823 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/logo.jpeg
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/dist/static/
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/dist/static/fonts/
+-rw-r--r--   0 arron      (502) staff       (20)    28200 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/fonts/element-icons.535877f5.woff
+-rw-r--r--   0 arron      (502) staff       (20)    55956 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/fonts/element-icons.732389de.ttf
+-rw-r--r--   0 arron      (502) staff       (20)    82216 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/fonts/ionicons.143146fa.woff2
+-rw-r--r--   0 arron      (502) staff       (20)   197740 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/fonts/ionicons.99ac3308.woff
+-rw-r--r--   0 arron      (502) staff       (20)   197664 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/fonts/ionicons.d535a25a.ttf
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/dist/static/img/
+-rw-r--r--   0 arron      (502) staff       (20)    67646 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/img/favicon.37e81aa2.png
+-rw-r--r--   0 arron      (502) staff       (20)   555353 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/img/ionicons.a2c4a261.svg
+-rw-r--r--   0 arron      (502) staff       (20)  1169238 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/img/universe.0efde44f.jpeg
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/dist/static/js/
+-rw-r--r--   0 arron      (502) staff       (20)    64548 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/js/0.js
+-rw-r--r--   0 arron      (502) staff       (20)   118909 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/js/1.js
+-rw-r--r--   0 arron      (502) staff       (20)    90525 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/js/2.js
+-rw-r--r--   0 arron      (502) staff       (20)    79539 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/js/3.js
+-rw-r--r--   0 arron      (502) staff       (20)    69592 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/js/4.js
+-rw-r--r--   0 arron      (502) staff       (20)    54102 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/js/5.js
+-rw-r--r--   0 arron      (502) staff       (20)    17781 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/js/6.js
+-rw-r--r--   0 arron      (502) staff       (20)   328960 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/js/app.js
+-rw-r--r--   0 arron      (502) staff       (20)  8841692 2023-07-25 08:30:47.000000 crawler_studio-1.5.6/crawler_studio/dist/static/js/chunk-vendors.js
+-rwxr-xr-x   0 arron      (502) staff       (20)      782 2023-07-25 03:39:30.000000 crawler_studio-1.5.6/crawler_studio/manage.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/
+-rw-r--r--   0 arron      (502) staff       (20)     9114 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/autocomplete.css
+-rw-r--r--   0 arron      (502) staff       (20)    19513 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/base.css
+-rw-r--r--   0 arron      (502) staff       (20)     6874 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/changelists.css
+-rw-r--r--   0 arron      (502) staff       (20)      380 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/dashboard.css
+-rw-r--r--   0 arron      (502) staff       (20)      423 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/fonts.css
+-rw-r--r--   0 arron      (502) staff       (20)     8804 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/forms.css
+-rw-r--r--   0 arron      (502) staff       (20)      939 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/login.css
+-rw-r--r--   0 arron      (502) staff       (20)     2271 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/nav_sidebar.css
+-rw-r--r--   0 arron      (502) staff       (20)    18545 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/responsive.css
+-rw-r--r--   0 arron      (502) staff       (20)     1741 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/responsive_rtl.css
+-rw-r--r--   0 arron      (502) staff       (20)     3234 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/rtl.css
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/vendor/
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/vendor/select2/
+-rw-r--r--   0 arron      (502) staff       (20)     1124 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/vendor/select2/LICENSE-SELECT2.md
+-rw-r--r--   0 arron      (502) staff       (20)    17358 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/vendor/select2/select2.css
+-rw-r--r--   0 arron      (502) staff       (20)    14966 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/vendor/select2/select2.min.css
+-rw-r--r--   0 arron      (502) staff       (20)    11097 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/css/widgets.css
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/fonts/
+-rw-r--r--   0 arron      (502) staff       (20)    11560 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/fonts/LICENSE.txt
+-rw-r--r--   0 arron      (502) staff       (20)      214 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/fonts/README.txt
+-rw-r--r--   0 arron      (502) staff       (20)    86184 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/fonts/Roboto-Bold-webfont.woff
+-rw-r--r--   0 arron      (502) staff       (20)    85692 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/fonts/Roboto-Light-webfont.woff
+-rw-r--r--   0 arron      (502) staff       (20)    85876 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/fonts/Roboto-Regular-webfont.woff
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/
+-rw-r--r--   0 arron      (502) staff       (20)     1081 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/LICENSE
+-rw-r--r--   0 arron      (502) staff       (20)      319 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/README.txt
+-rw-r--r--   0 arron      (502) staff       (20)     1094 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/calendar-icons.svg
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/gis/
+-rw-r--r--   0 arron      (502) staff       (20)     1129 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/gis/move_vertex_off.svg
+-rw-r--r--   0 arron      (502) staff       (20)     1129 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/gis/move_vertex_on.svg
+-rw-r--r--   0 arron      (502) staff       (20)      331 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-addlink.svg
+-rw-r--r--   0 arron      (502) staff       (20)      504 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-alert.svg
+-rw-r--r--   0 arron      (502) staff       (20)     1086 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-calendar.svg
+-rw-r--r--   0 arron      (502) staff       (20)      380 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-changelink.svg
+-rw-r--r--   0 arron      (502) staff       (20)      677 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-clock.svg
+-rw-r--r--   0 arron      (502) staff       (20)      392 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-deletelink.svg
+-rw-r--r--   0 arron      (502) staff       (20)      560 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-no.svg
+-rw-r--r--   0 arron      (502) staff       (20)      655 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-unknown-alt.svg
+-rw-r--r--   0 arron      (502) staff       (20)      655 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-unknown.svg
+-rw-r--r--   0 arron      (502) staff       (20)      581 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-viewlink.svg
+-rw-r--r--   0 arron      (502) staff       (20)      436 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-yes.svg
+-rw-r--r--   0 arron      (502) staff       (20)      560 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/inline-delete.svg
+-rw-r--r--   0 arron      (502) staff       (20)      458 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/search.svg
+-rw-r--r--   0 arron      (502) staff       (20)     3291 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/selector-icons.svg
+-rw-r--r--   0 arron      (502) staff       (20)     1097 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/sorting-icons.svg
+-rw-r--r--   0 arron      (502) staff       (20)      331 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/tooltag-add.svg
+-rw-r--r--   0 arron      (502) staff       (20)      280 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/img/tooltag-arrowright.svg
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/
+-rw-r--r--   0 arron      (502) staff       (20)     4360 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/SelectBox.js
+-rw-r--r--   0 arron      (502) staff       (20)    12350 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/SelectFilter2.js
+-rw-r--r--   0 arron      (502) staff       (20)     7867 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/actions.js
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/admin/
+-rw-r--r--   0 arron      (502) staff       (20)    19634 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/admin/DateTimeShortcuts.js
+-rw-r--r--   0 arron      (502) staff       (20)     5984 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/admin/RelatedObjectLookups.js
+-rw-r--r--   0 arron      (502) staff       (20)     1320 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/autocomplete.js
+-rw-r--r--   0 arron      (502) staff       (20)     8466 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/calendar.js
+-rw-r--r--   0 arron      (502) staff       (20)      884 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/cancel.js
+-rw-r--r--   0 arron      (502) staff       (20)      606 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/change_form.js
+-rw-r--r--   0 arron      (502) staff       (20)     1803 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/collapse.js
+-rw-r--r--   0 arron      (502) staff       (20)     5698 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/core.js
+-rw-r--r--   0 arron      (502) staff       (20)    15225 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/inlines.js
+-rw-r--r--   0 arron      (502) staff       (20)      347 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/jquery.init.js
+-rw-r--r--   0 arron      (502) staff       (20)     1360 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/nav_sidebar.js
+-rw-r--r--   0 arron      (502) staff       (20)      551 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/popup_response.js
+-rw-r--r--   0 arron      (502) staff       (20)     1531 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/prepopulate.js
+-rw-r--r--   0 arron      (502) staff       (20)      492 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/prepopulate_init.js
+-rw-r--r--   0 arron      (502) staff       (20)     7902 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/urlify.js
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/jquery/
+-rw-r--r--   0 arron      (502) staff       (20)     1095 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/jquery/LICENSE.txt
+-rw-r--r--   0 arron      (502) staff       (20)   287630 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/jquery/jquery.js
+-rw-r--r--   0 arron      (502) staff       (20)    89476 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/jquery/jquery.min.js
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/
+-rw-r--r--   0 arron      (502) staff       (20)     1124 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/LICENSE.md
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/
+-rw-r--r--   0 arron      (502) staff       (20)      866 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/af.js
+-rw-r--r--   0 arron      (502) staff       (20)      905 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ar.js
+-rw-r--r--   0 arron      (502) staff       (20)      721 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/az.js
+-rw-r--r--   0 arron      (502) staff       (20)      968 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/bg.js
+-rw-r--r--   0 arron      (502) staff       (20)     1291 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/bn.js
+-rw-r--r--   0 arron      (502) staff       (20)      965 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/bs.js
+-rw-r--r--   0 arron      (502) staff       (20)      900 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ca.js
+-rw-r--r--   0 arron      (502) staff       (20)     1292 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/cs.js
+-rw-r--r--   0 arron      (502) staff       (20)      828 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/da.js
+-rw-r--r--   0 arron      (502) staff       (20)      866 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/de.js
+-rw-r--r--   0 arron      (502) staff       (20)     1017 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/dsb.js
+-rw-r--r--   0 arron      (502) staff       (20)     1182 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/el.js
+-rw-r--r--   0 arron      (502) staff       (20)      844 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/en.js
+-rw-r--r--   0 arron      (502) staff       (20)      922 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/es.js
+-rw-r--r--   0 arron      (502) staff       (20)      801 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/et.js
+-rw-r--r--   0 arron      (502) staff       (20)      868 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/eu.js
+-rw-r--r--   0 arron      (502) staff       (20)     1023 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/fa.js
+-rw-r--r--   0 arron      (502) staff       (20)      803 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/fi.js
+-rw-r--r--   0 arron      (502) staff       (20)      924 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/fr.js
+-rw-r--r--   0 arron      (502) staff       (20)      924 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/gl.js
+-rw-r--r--   0 arron      (502) staff       (20)      984 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/he.js
+-rw-r--r--   0 arron      (502) staff       (20)     1175 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/hi.js
+-rw-r--r--   0 arron      (502) staff       (20)      852 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/hr.js
+-rw-r--r--   0 arron      (502) staff       (20)     1018 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/hsb.js
+-rw-r--r--   0 arron      (502) staff       (20)      831 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/hu.js
+-rw-r--r--   0 arron      (502) staff       (20)     1028 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/hy.js
+-rw-r--r--   0 arron      (502) staff       (20)      768 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/id.js
+-rw-r--r--   0 arron      (502) staff       (20)      807 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/is.js
+-rw-r--r--   0 arron      (502) staff       (20)      897 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/it.js
+-rw-r--r--   0 arron      (502) staff       (20)      862 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ja.js
+-rw-r--r--   0 arron      (502) staff       (20)     1195 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ka.js
+-rw-r--r--   0 arron      (502) staff       (20)     1088 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/km.js
+-rw-r--r--   0 arron      (502) staff       (20)      855 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ko.js
+-rw-r--r--   0 arron      (502) staff       (20)      944 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/lt.js
+-rw-r--r--   0 arron      (502) staff       (20)      900 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/lv.js
+-rw-r--r--   0 arron      (502) staff       (20)     1038 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/mk.js
+-rw-r--r--   0 arron      (502) staff       (20)      811 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ms.js
+-rw-r--r--   0 arron      (502) staff       (20)      778 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/nb.js
+-rw-r--r--   0 arron      (502) staff       (20)     1357 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ne.js
+-rw-r--r--   0 arron      (502) staff       (20)      904 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/nl.js
+-rw-r--r--   0 arron      (502) staff       (20)      947 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/pl.js
+-rw-r--r--   0 arron      (502) staff       (20)     1049 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ps.js
+-rw-r--r--   0 arron      (502) staff       (20)      876 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/pt-BR.js
+-rw-r--r--   0 arron      (502) staff       (20)      878 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/pt.js
+-rw-r--r--   0 arron      (502) staff       (20)      938 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ro.js
+-rw-r--r--   0 arron      (502) staff       (20)     1171 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ru.js
+-rw-r--r--   0 arron      (502) staff       (20)     1306 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/sk.js
+-rw-r--r--   0 arron      (502) staff       (20)      925 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/sl.js
+-rw-r--r--   0 arron      (502) staff       (20)      903 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/sq.js
+-rw-r--r--   0 arron      (502) staff       (20)     1109 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/sr-Cyrl.js
+-rw-r--r--   0 arron      (502) staff       (20)      980 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/sr.js
+-rw-r--r--   0 arron      (502) staff       (20)      786 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/sv.js
+-rw-r--r--   0 arron      (502) staff       (20)     1074 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/th.js
+-rw-r--r--   0 arron      (502) staff       (20)      771 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/tk.js
+-rw-r--r--   0 arron      (502) staff       (20)      775 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/tr.js
+-rw-r--r--   0 arron      (502) staff       (20)     1156 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/uk.js
+-rw-r--r--   0 arron      (502) staff       (20)      796 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/vi.js
+-rw-r--r--   0 arron      (502) staff       (20)      768 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/zh-CN.js
+-rw-r--r--   0 arron      (502) staff       (20)      707 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/zh-TW.js
+-rw-r--r--   0 arron      (502) staff       (20)   173566 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/select2.full.js
+-rw-r--r--   0 arron      (502) staff       (20)    79212 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/select2.full.min.js
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/xregexp/
+-rw-r--r--   0 arron      (502) staff       (20)     1103 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/xregexp/LICENSE.txt
+-rw-r--r--   0 arron      (502) staff       (20)   232381 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/xregexp/xregexp.js
+-rw-r--r--   0 arron      (502) staff       (20)   125266 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/xregexp/xregexp.min.js
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/fonts/
+-rw-r--r--   0 arron      (502) staff       (20)    28200 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/fonts/element-icons.535877f5.woff
+-rw-r--r--   0 arron      (502) staff       (20)    55956 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/fonts/element-icons.732389de.ttf
+-rw-r--r--   0 arron      (502) staff       (20)    82216 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/fonts/ionicons.143146fa.woff2
+-rw-r--r--   0 arron      (502) staff       (20)   197740 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/fonts/ionicons.99ac3308.woff
+-rw-r--r--   0 arron      (502) staff       (20)   197664 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/fonts/ionicons.d535a25a.ttf
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/img/
+-rw-r--r--   0 arron      (502) staff       (20)    67646 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/img/favicon.37e81aa2.png
+-rw-r--r--   0 arron      (502) staff       (20)   555353 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/img/ionicons.a2c4a261.svg
+-rw-r--r--   0 arron      (502) staff       (20)  1169238 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/img/universe.0efde44f.jpeg
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/js/
+-rw-r--r--   0 arron      (502) staff       (20)    64548 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/js/0.js
+-rw-r--r--   0 arron      (502) staff       (20)   118909 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/js/1.js
+-rw-r--r--   0 arron      (502) staff       (20)    90525 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/js/2.js
+-rw-r--r--   0 arron      (502) staff       (20)    79539 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/js/3.js
+-rw-r--r--   0 arron      (502) staff       (20)    69592 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/js/4.js
+-rw-r--r--   0 arron      (502) staff       (20)    54102 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/js/5.js
+-rw-r--r--   0 arron      (502) staff       (20)    17781 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/js/6.js
+-rw-r--r--   0 arron      (502) staff       (20)   328960 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/js/app.js
+-rw-r--r--   0 arron      (502) staff       (20)  8841692 2023-07-25 08:32:19.000000 crawler_studio-1.5.6/crawler_studio/static/js/chunk-vendors.js
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/
+-rw-r--r--   0 arron      (502) staff       (20)    23411 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/bootstrap-theme.min.css
+-rw-r--r--   0 arron      (502) staff       (20)    75600 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 arron      (502) staff       (20)     3385 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/bootstrap-tweaks.css
+-rw-r--r--   0 arron      (502) staff       (20)   121457 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/bootstrap.min.css
+-rw-r--r--   0 arron      (502) staff       (20)   540434 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/bootstrap.min.css.map
+-rw-r--r--   0 arron      (502) staff       (20)     1152 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/default.css
+-rw-r--r--   0 arron      (502) staff       (20)    21658 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/font-awesome-4.0.3.css
+-rw-r--r--   0 arron      (502) staff       (20)      817 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/prettify.css
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/css/
+-rw-r--r--   0 arron      (502) staff       (20)     6156 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/css/base.css
+-rw-r--r--   0 arron      (502) staff       (20)     1682 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/css/highlight.css
+-rw-r--r--   0 arron      (502) staff       (20)     1307 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/css/jquery.json-view.min.css
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/img/
+-rw-r--r--   0 arron      (502) staff       (20)     5430 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/img/favicon.ico
+-rw-r--r--   0 arron      (502) staff       (20)     1458 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/img/grid.png
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/js/
+-rw-r--r--   0 arron      (502) staff       (20)    10391 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/js/api.js
+-rw-r--r--   0 arron      (502) staff       (20)   300764 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/js/highlight.pack.js
+-rw-r--r--   0 arron      (502) staff       (20)     2700 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/js/jquery.json-view.min.js
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/
+-rw-r--r--   0 arron      (502) staff       (20)    38205 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 arron      (502) staff       (20)   202148 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 arron      (502) staff       (20)    80652 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 arron      (502) staff       (20)    44432 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 arron      (502) staff       (20)    20127 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 arron      (502) staff       (20)   108738 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 arron      (502) staff       (20)    45404 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 arron      (502) staff       (20)    23424 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 arron      (502) staff       (20)    18028 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/img/
+-rw-r--r--   0 arron      (502) staff       (20)     8777 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/img/glyphicons-halflings-white.png
+-rw-r--r--   0 arron      (502) staff       (20)    12762 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/img/glyphicons-halflings.png
+-rw-r--r--   0 arron      (502) staff       (20)     1458 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/img/grid.png
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/
+-rw-r--r--   0 arron      (502) staff       (20)     3597 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/ajax-form.js
+-rw-r--r--   0 arron      (502) staff       (20)    39680 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/bootstrap.min.js
+-rw-r--r--   0 arron      (502) staff       (20)   157600 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/coreapi-0.1.1.js
+-rw-r--r--   0 arron      (502) staff       (20)     1719 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/csrf.js
+-rw-r--r--   0 arron      (502) staff       (20)     1268 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/default.js
+-rw-r--r--   0 arron      (502) staff       (20)    89476 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/jquery-3.5.1.min.js
+-rw-r--r--   0 arron      (502) staff       (20)    13632 2022-11-16 17:13:28.000000 crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/prettify-min.js
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio/utils/
+-rw-r--r--   0 arron      (502) staff       (20)      120 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/utils/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)      182 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/utils/exceptions.py
+-rw-r--r--   0 arron      (502) staff       (20)     3100 2023-07-25 08:24:32.000000 crawler_studio-1.5.6/crawler_studio/utils/message_transmit.py
+-rw-r--r--   0 arron      (502) staff       (20)     1637 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/utils/time.py
+-rw-r--r--   0 arron      (502) staff       (20)      299 2022-09-24 09:28:56.000000 crawler_studio-1.5.6/crawler_studio/utils/timer_scheduler.py
+-rw-r--r--   0 arron      (502) staff       (20)      671 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/utils/variable_rule_trans.py
+-rw-r--r--   0 arron      (502) staff       (20)     1949 2022-09-19 10:57:11.000000 crawler_studio-1.5.6/crawler_studio/utils/verifycation.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio.egg-info/
+-rw-r--r--   0 arron      (502) staff       (20)      761 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio.egg-info/PKG-INFO
+-rw-r--r--   0 arron      (502) staff       (20)    14216 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 arron      (502) staff       (20)        1 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 arron      (502) staff       (20)       47 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio.egg-info/entry_points.txt
+-rw-r--r--   0 arron      (502) staff       (20)      150 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio.egg-info/requires.txt
+-rw-r--r--   0 arron      (502) staff       (20)       15 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/crawler_studio.egg-info/top_level.txt
+-rw-r--r--   0 arron      (502) staff       (20)       38 2023-07-25 08:34:12.000000 crawler_studio-1.5.6/setup.cfg
+-rw-r--r--   0 arron      (502) staff       (20)     1957 2023-07-25 08:33:58.000000 crawler_studio-1.5.6/setup.py
```

### Comparing `crawler_studio-1.5.5/PKG-INFO` & `crawler_studio-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: crawler_studio
-Version: 1.5.5
+Version: 1.5.6
 Summary: crawler_studio
 Home-page: UNKNOWN
 Author: liuxianglong
 Author-email: 862187570@qq.com
 Maintainer: liuxianglong
 Maintainer-email: 862187570@qq.com
 License: BSD License
```

### Comparing `crawler_studio-1.5.5/README.md` & `crawler_studio-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_logs/migrations/0001_initial.py` & `crawler_studio-1.5.6/crawler_studio/app_logs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_logs/models.py` & `crawler_studio-1.5.6/crawler_studio/app_logs/models.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_logs/ser.py` & `crawler_studio-1.5.6/crawler_studio/app_logs/ser.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_logs/views.py` & `crawler_studio-1.5.6/crawler_studio/app_logs/views.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_schedule/migrations/0001_initial.py` & `crawler_studio-1.5.6/crawler_studio/app_schedule/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_schedule/models.py` & `crawler_studio-1.5.6/crawler_studio/app_schedule/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 class MonitorRules(models.Model):
     id = models.AutoField(primary_key=True)
     timer_task = models.OneToOneField(DjangoJob, null=True, on_delete=models.CASCADE)
     spider_host = models.CharField(max_length=50, verbose_name='爬虫所在主机')
     spider_project = models.CharField(null=True, max_length=100, verbose_name='爬虫项目')
     spider_name = models.CharField(null=True, max_length=100, verbose_name='爬虫名称')
     spider_job_id = models.CharField(null=True, max_length=100, db_index=True)
+    start_params = models.CharField(null=True, max_length=1000, verbose_name='启动参数')
     # monitor_type = models.CharField(max_length=50, null=True, verbose_name='预警方式，1:日志存活时间，2:日志错误率, 3:日志错误数量')
     monitor_freq = models.IntegerField(verbose_name='监控频率，秒为单位', default=1800)
     log_alive_limit = models.IntegerField(default=80, verbose_name='日志存活时间上限, 默认80sec')
     errlog_rate_limit = models.FloatField(default=0.005, verbose_name='1小时日志错误率上限，默认0.5%')
     memory_use_limit = models.IntegerField(default=500, verbose_name='占用最大内存，默认500MB')
     recipients = models.ManyToManyField(MonitorRecipients, verbose_name='收件人')
     create_time = models.DateTimeField(auto_now=True)
```

### Comparing `crawler_studio-1.5.5/crawler_studio/app_schedule/ser.py` & `crawler_studio-1.5.6/crawler_studio/app_schedule/ser.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_schedule/views.py` & `crawler_studio-1.5.6/crawler_studio/app_schedule/views.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_schedule/worker.py` & `crawler_studio-1.5.6/crawler_studio/app_schedule/worker.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_scrapyd/migrations/0001_initial.py` & `crawler_studio-1.5.6/crawler_studio/app_scrapyd/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_scrapyd/migrations/0003_auto_20220812_1436.py` & `crawler_studio-1.5.6/crawler_studio/app_scrapyd/migrations/0003_auto_20220812_1436.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_scrapyd/migrations/0004_auto_20220905_1014.py` & `crawler_studio-1.5.6/crawler_studio/app_scrapyd/migrations/0004_auto_20220905_1014.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_scrapyd/migrations/0006_spiderstartparams.py` & `crawler_studio-1.5.6/crawler_studio/app_scrapyd/migrations/0006_spiderstartparams.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_scrapyd/models.py` & `crawler_studio-1.5.6/crawler_studio/app_scrapyd/models.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_scrapyd/ser.py` & `crawler_studio-1.5.6/crawler_studio/app_scrapyd/ser.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_scrapyd/views.py` & `crawler_studio-1.5.6/crawler_studio/app_scrapyd/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
                 monitor_rule = MonitorRules.objects.filter(spider_job_id=running['id']).first()
                 item = dict()
                 item['project'] = p
                 item['job_id'] = running['id']
                 item['spider'] = running['spider']
                 item['pid'] = running['pid']
                 item['start_time'] = running['start_time'].split('.')[0]
+                item['start_params'] = 'Unknown' if monitor_rule is None else monitor_rule.start_params
                 # item['schedule_type'] = 'Unknown' if stats is None else stats.run_type
                 # item['trigger'] = 'Unknown' if stats is None else stats.trigger
                 # item['last_run'] = 'Unknown' if stats is None else stats.last_run
                 item['memory_use'] = 0 if stats is None else stats.memory_use
                 item['memory_use_limit'] = 'Unknown' if monitor_rule is None else monitor_rule.memory_use_limit
                 item['log_hourly_error_rate'] = 'Unknown' if stats is None else stats.log_hourly_error_rate
                 item['log_hourly_error_limit'] = 'Unknown' if monitor_rule is None else monitor_rule.errlog_rate_limit
```

### Comparing `crawler_studio-1.5.5/crawler_studio/app_settings/migrations/0001_initial.py` & `crawler_studio-1.5.6/crawler_studio/app_settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_settings/migrations/0003_mailsender.py` & `crawler_studio-1.5.6/crawler_studio/app_settings/migrations/0003_mailsender.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_settings/models.py` & `crawler_studio-1.5.6/crawler_studio/app_settings/models.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_settings/views.py` & `crawler_studio-1.5.6/crawler_studio/app_settings/views.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_user/migrations/0001_initial.py` & `crawler_studio-1.5.6/crawler_studio/app_user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/app_user/views.py` & `crawler_studio-1.5.6/crawler_studio/app_user/views.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/cmd/management/commands/__pycache__/get_token.cpython-37.pyc` & `crawler_studio-1.5.6/crawler_studio/cmd/management/commands/__pycache__/get_token.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/cmd/management/commands/__pycache__/init.cpython-37.pyc` & `crawler_studio-1.5.6/crawler_studio/cmd/management/commands/__pycache__/init.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/cmd/management/commands/get_token.py` & `crawler_studio-1.5.6/crawler_studio/cmd/management/commands/get_token.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/cmd/management/commands/init.py` & `crawler_studio-1.5.6/crawler_studio/cmd/management/commands/init.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/crawler_studio/custom_field.py` & `crawler_studio-1.5.6/crawler_studio/crawler_studio/custom_field.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/crawler_studio/settings.py` & `crawler_studio-1.5.6/crawler_studio/crawler_studio/settings.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/crawler_studio/urls.py` & `crawler_studio-1.5.6/crawler_studio/crawler_studio/urls.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/favicon.ico` & `crawler_studio-1.5.6/crawler_studio/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/index.html` & `crawler_studio-1.5.6/crawler_studio/dist/index.html`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/logo.jpeg` & `crawler_studio-1.5.6/crawler_studio/dist/logo.jpeg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/fonts/element-icons.535877f5.woff` & `crawler_studio-1.5.6/crawler_studio/dist/static/fonts/element-icons.535877f5.woff`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/fonts/element-icons.732389de.ttf` & `crawler_studio-1.5.6/crawler_studio/dist/static/fonts/element-icons.732389de.ttf`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/fonts/ionicons.143146fa.woff2` & `crawler_studio-1.5.6/crawler_studio/dist/static/fonts/ionicons.143146fa.woff2`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/fonts/ionicons.99ac3308.woff` & `crawler_studio-1.5.6/crawler_studio/dist/static/fonts/ionicons.99ac3308.woff`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/fonts/ionicons.d535a25a.ttf` & `crawler_studio-1.5.6/crawler_studio/dist/static/fonts/ionicons.d535a25a.ttf`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/img/favicon.37e81aa2.png` & `crawler_studio-1.5.6/crawler_studio/dist/static/img/favicon.37e81aa2.png`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/img/ionicons.a2c4a261.svg` & `crawler_studio-1.5.6/crawler_studio/dist/static/img/ionicons.a2c4a261.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/img/universe.0efde44f.jpeg` & `crawler_studio-1.5.6/crawler_studio/dist/static/img/universe.0efde44f.jpeg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/js/0.js` & `crawler_studio-1.5.6/crawler_studio/dist/static/js/0.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/js/1.js` & `crawler_studio-1.5.6/crawler_studio/dist/static/js/1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -82,45 +82,45 @@
               !*** ./node_modules/cache-loader/dist/cjs.js?{"cacheDirectory":"node_modules/.cache/vue-loader","cacheIdentifier":"023ef482-vue-loader-template"}!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options!./src/components/Settings/components/ModalMailSender.vue?vue&type=template&id=17a57dac&scoped=true& ***!
               \****************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /*! exports provided: render, staticRenderFns */
             /***/
             (function(module, __webpack_exports__, __webpack_require__) {
 
                 "use strict";
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"Modal\",\n    _vm._g(\n      _vm._b(\n        {\n          attrs: { title: \"系统邮件发件人\", width: 450, \"footer-hide\": false },\n          on: { \"on-ok\": _vm.onOK },\n          model: {\n            value: _vm.showDialog,\n            callback: function ($$v) {\n              _vm.showDialog = $$v\n            },\n            expression: \"showDialog\",\n          },\n        },\n        \"Modal\",\n        _vm.$attrs,\n        false\n      ),\n      _vm.$listeners\n    ),\n    [\n      _c(\n        \"el-form\",\n        {\n          ref: \"form\",\n          attrs: {\n            size: \"mini\",\n            rules: _vm.rules,\n            \"label-width\": \"100px\",\n            model: _vm.formData,\n          },\n        },\n        [\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"发件人地址\", prop: \"mailAddr\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.mailAddr,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"mailAddr\", $$v)\n                  },\n                  expression: \"formData.mailAddr\",\n                },\n              }),\n            ],\n            1\n          ),\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"服务器地址\", prop: \"serverAddr\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.serverAddr,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"serverAddr\", $$v)\n                  },\n                  expression: \"formData.serverAddr\",\n                },\n              }),\n            ],\n            1\n          ),\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"服务器端口\", prop: \"mailPort\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.mailPort,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"mailPort\", $$v)\n                  },\n                  expression: \"formData.mailPort\",\n                },\n              }),\n            ],\n            1\n          ),\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"邮件授权码\", prop: \"authCode\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.authCode,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"authCode\", $$v)\n                  },\n                  expression: \"formData.authCode\",\n                },\n              }),\n            ],\n            1\n          ),\n        ],\n        1\n      ),\n      _c(\n        \"div\",\n        { attrs: { slot: \"footer\" }, slot: \"footer\" },\n        [\n          _c(\n            \"Button\",\n            {\n              attrs: { type: \"text\" },\n              on: {\n                click: function ($event) {\n                  _vm.showDialog = false\n                },\n              },\n            },\n            [_vm._v(\"取消\")]\n          ),\n          _c(\n            \"Button\",\n            { attrs: { type: \"primary\" }, on: { click: _vm.onOK } },\n            [_vm._v(\"确定\")]\n          ),\n        ],\n        1\n      ),\n    ],\n    1\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Settings/components/ModalMailSender.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"Modal\",\n    _vm._g(\n      _vm._b(\n        {\n          attrs: { title: \"系统邮件发件人\", width: 450, \"footer-hide\": false },\n          on: { \"on-ok\": _vm.onOK },\n          model: {\n            value: _vm.showDialog,\n            callback: function ($$v) {\n              _vm.showDialog = $$v\n            },\n            expression: \"showDialog\",\n          },\n        },\n        \"Modal\",\n        _vm.$attrs,\n        false\n      ),\n      _vm.$listeners\n    ),\n    [\n      _c(\n        \"el-form\",\n        {\n          ref: \"form\",\n          attrs: {\n            size: \"mini\",\n            rules: _vm.rules,\n            \"label-width\": \"100px\",\n            model: _vm.formData,\n          },\n        },\n        [\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"发件人地址\", prop: \"mailAddr\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.mailAddr,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"mailAddr\", $$v)\n                  },\n                  expression: \"formData.mailAddr\",\n                },\n              }),\n            ],\n            1\n          ),\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"服务器地址\", prop: \"serverAddr\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.serverAddr,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"serverAddr\", $$v)\n                  },\n                  expression: \"formData.serverAddr\",\n                },\n              }),\n            ],\n            1\n          ),\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"服务器端口\", prop: \"mailPort\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.mailPort,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"mailPort\", $$v)\n                  },\n                  expression: \"formData.mailPort\",\n                },\n              }),\n            ],\n            1\n          ),\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"邮件授权码\", prop: \"authCode\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\", type: \"password\" },\n                model: {\n                  value: _vm.formData.authCode,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"authCode\", $$v)\n                  },\n                  expression: \"formData.authCode\",\n                },\n              }),\n            ],\n            1\n          ),\n        ],\n        1\n      ),\n      _c(\n        \"div\",\n        { attrs: { slot: \"footer\" }, slot: \"footer\" },\n        [\n          _c(\n            \"Button\",\n            {\n              attrs: { type: \"text\" },\n              on: {\n                click: function ($event) {\n                  _vm.showDialog = false\n                },\n              },\n            },\n            [_vm._v(\"取消\")]\n          ),\n          _c(\n            \"Button\",\n            { attrs: { type: \"primary\" }, on: { click: _vm.onOK } },\n            [_vm._v(\"确定\")]\n          ),\n        ],\n        1\n      ),\n    ],\n    1\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Settings/components/ModalMailSender.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
 
                 /***/
             }),
 
         /***/
         "./node_modules/cache-loader/dist/cjs.js?{\"cacheDirectory\":\"node_modules/.cache/vue-loader\",\"cacheIdentifier\":\"023ef482-vue-loader-template\"}!./node_modules/vue-loader/lib/loaders/templateLoader.js?!./node_modules/cache-loader/dist/cjs.js?!./node_modules/vue-loader/lib/index.js?!./src/components/Settings/components/ModalMonitorRev.vue?vue&type=template&id=8b6a656e&scoped=true&":
             /*!****************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
               !*** ./node_modules/cache-loader/dist/cjs.js?{"cacheDirectory":"node_modules/.cache/vue-loader","cacheIdentifier":"023ef482-vue-loader-template"}!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options!./src/components/Settings/components/ModalMonitorRev.vue?vue&type=template&id=8b6a656e&scoped=true& ***!
               \****************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /*! exports provided: render, staticRenderFns */
             /***/
             (function(module, __webpack_exports__, __webpack_require__) {
 
                 "use strict";
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"Modal\",\n    _vm._g(\n      _vm._b(\n        {\n          attrs: { title: \"监控收件人\", width: 700, \"footer-hide\": true },\n          model: {\n            value: _vm.showDialog,\n            callback: function ($$v) {\n              _vm.showDialog = $$v\n            },\n            expression: \"showDialog\",\n          },\n        },\n        \"Modal\",\n        _vm.$attrs,\n        false\n      ),\n      _vm.$listeners\n    ),\n    [\n      _c(\n        \"div\",\n        { staticClass: \"alert-page\" },\n        [\n          _c(\n            \"el-form\",\n            { attrs: { inline: true, size: \"mini\" } },\n            [\n              _c(\n                \"el-form-item\",\n                { attrs: { label: \"\" } },\n                [\n                  _c(\n                    \"el-select\",\n                    {\n                      attrs: { placeholder: \"收件方式\" },\n                      model: {\n                        value: _vm.formData.method,\n                        callback: function ($$v) {\n                          _vm.$set(_vm.formData, \"method\", $$v)\n                        },\n                        expression: \"formData.method\",\n                      },\n                    },\n                    [\n                      _c(\"el-option\", {\n                        attrs: { value: \"钉钉\", label: \"钉钉\" },\n                      }),\n                      _c(\"el-option\", {\n                        attrs: { value: \"邮件\", label: \"邮件\" },\n                      }),\n                    ],\n                    1\n                  ),\n                ],\n                1\n              ),\n              _c(\n                \"el-form-item\",\n                { attrs: { label: \"\" } },\n                [\n                  _c(\"el-input\", {\n                    attrs: { placeholder: \"收件人名称\" },\n                    model: {\n                      value: _vm.formData.revName,\n                      callback: function ($$v) {\n                        _vm.$set(_vm.formData, \"revName\", $$v)\n                      },\n                      expression: \"formData.revName\",\n                    },\n                  }),\n                ],\n                1\n              ),\n              _c(\n                \"el-form-item\",\n                { attrs: { label: \"\" } },\n                [\n                  _c(\"el-input\", {\n                    attrs: { placeholder: \"收件人地址\" },\n                    model: {\n                      value: _vm.formData.revAddr,\n                      callback: function ($$v) {\n                        _vm.$set(_vm.formData, \"revAddr\", $$v)\n                      },\n                      expression: \"formData.revAddr\",\n                    },\n                  }),\n                ],\n                1\n              ),\n              _c(\n                \"el-button\",\n                {\n                  attrs: { type: \"primary\", size: \"mini\" },\n                  on: { click: _vm.apiAdd },\n                },\n                [_vm._v(\"新增\")]\n              ),\n            ],\n            1\n          ),\n          _c(\n            \"el-table\",\n            {\n              ref: \"table\",\n              staticStyle: { width: \"100%\", \"margin-top\": \"20px\" },\n              attrs: {\n                data: _vm.tableData,\n                height: \"300\",\n                stripe: \"\",\n                fit: \"\",\n                size: \"mini\",\n                \"row-class-name\": _vm.rowClassName,\n              },\n            },\n            [\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  prop: \"id\",\n                  width: \"70\",\n                  label: \"ID\",\n                },\n              }),\n              _c(\"el-table-column\", {\n                attrs: { align: \"center\", prop: \"method\", label: \"收件方式\" },\n              }),\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  prop: \"revName\",\n                  label: \"收件人名称\",\n                },\n              }),\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  prop: \"revAddr\",\n                  label: \"收件人地址\",\n                },\n              }),\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  label: \"操作\",\n                  \"show-overflow-tooltip\": \"\",\n                },\n                scopedSlots: _vm._u([\n                  {\n                    key: \"default\",\n                    fn: function (scope) {\n                      return [\n                        _c(\n                          \"el-button-group\",\n                          [\n                            _c(\"el-button\", {\n                              attrs: {\n                                size: \"mini\",\n                                type: \"danger\",\n                                icon: \"el-icon-delete\",\n                              },\n                              on: {\n                                click: function ($event) {\n                                  return _vm.apiDelete(scope.row.revAddr)\n                                },\n                              },\n                            }),\n                          ],\n                          1\n                        ),\n                      ]\n                    },\n                  },\n                ]),\n              }),\n            ],\n            1\n          ),\n        ],\n        1\n      ),\n    ]\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Settings/components/ModalMonitorRev.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"Modal\",\n    _vm._g(\n      _vm._b(\n        {\n          attrs: { title: \"监控收件人\", width: 700, \"footer-hide\": true },\n          model: {\n            value: _vm.showDialog,\n            callback: function ($$v) {\n              _vm.showDialog = $$v\n            },\n            expression: \"showDialog\",\n          },\n        },\n        \"Modal\",\n        _vm.$attrs,\n        false\n      ),\n      _vm.$listeners\n    ),\n    [\n      _c(\n        \"div\",\n        { staticClass: \"alert-page\" },\n        [\n          _c(\n            \"el-form\",\n            { attrs: { inline: true, size: \"mini\" } },\n            [\n              _c(\n                \"el-form-item\",\n                { attrs: { label: \"\" } },\n                [\n                  _c(\n                    \"el-select\",\n                    {\n                      attrs: { placeholder: \"收件方式\" },\n                      model: {\n                        value: _vm.formData.method,\n                        callback: function ($$v) {\n                          _vm.$set(_vm.formData, \"method\", $$v)\n                        },\n                        expression: \"formData.method\",\n                      },\n                    },\n                    [\n                      _c(\"el-option\", {\n                        attrs: { value: \"钉钉\", label: \"钉钉机器人\" },\n                      }),\n                      _c(\"el-option\", {\n                        attrs: { value: \"邮件\", label: \"邮件\" },\n                      }),\n                    ],\n                    1\n                  ),\n                ],\n                1\n              ),\n              _c(\n                \"el-form-item\",\n                { attrs: { label: \"\" } },\n                [\n                  _c(\"el-input\", {\n                    attrs: { placeholder: \"收件人名称\" },\n                    model: {\n                      value: _vm.formData.revName,\n                      callback: function ($$v) {\n                        _vm.$set(_vm.formData, \"revName\", $$v)\n                      },\n                      expression: \"formData.revName\",\n                    },\n                  }),\n                ],\n                1\n              ),\n              _c(\n                \"el-form-item\",\n                { attrs: { label: \"\" } },\n                [\n                  _c(\"el-input\", {\n                    attrs: { placeholder: \"收件人地址\" },\n                    model: {\n                      value: _vm.formData.revAddr,\n                      callback: function ($$v) {\n                        _vm.$set(_vm.formData, \"revAddr\", $$v)\n                      },\n                      expression: \"formData.revAddr\",\n                    },\n                  }),\n                ],\n                1\n              ),\n              _c(\n                \"el-button\",\n                {\n                  attrs: { type: \"primary\", size: \"mini\" },\n                  on: { click: _vm.apiAdd },\n                },\n                [_vm._v(\"新增\")]\n              ),\n            ],\n            1\n          ),\n          _c(\n            \"el-table\",\n            {\n              ref: \"table\",\n              staticStyle: { width: \"100%\", \"margin-top\": \"20px\" },\n              attrs: {\n                data: _vm.tableData,\n                height: \"300\",\n                stripe: \"\",\n                fit: \"\",\n                size: \"mini\",\n                \"row-class-name\": _vm.rowClassName,\n              },\n            },\n            [\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  prop: \"id\",\n                  width: \"70\",\n                  label: \"ID\",\n                },\n              }),\n              _c(\"el-table-column\", {\n                attrs: { align: \"center\", prop: \"method\", label: \"收件方式\" },\n              }),\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  prop: \"revName\",\n                  label: \"收件人名称\",\n                },\n              }),\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  prop: \"revAddr\",\n                  label: \"收件人地址\",\n                },\n              }),\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  label: \"操作\",\n                  \"show-overflow-tooltip\": \"\",\n                },\n                scopedSlots: _vm._u([\n                  {\n                    key: \"default\",\n                    fn: function (scope) {\n                      return [\n                        _c(\n                          \"el-button-group\",\n                          [\n                            _c(\"el-button\", {\n                              attrs: {\n                                size: \"mini\",\n                                type: \"danger\",\n                                icon: \"el-icon-delete\",\n                              },\n                              on: {\n                                click: function ($event) {\n                                  return _vm.apiDelete(scope.row.revAddr)\n                                },\n                              },\n                            }),\n                          ],\n                          1\n                        ),\n                      ]\n                    },\n                  },\n                ]),\n              }),\n            ],\n            1\n          ),\n        ],\n        1\n      ),\n    ]\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Settings/components/ModalMonitorRev.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
 
                 /***/
             }),
 
         /***/
         "./node_modules/cache-loader/dist/cjs.js?{\"cacheDirectory\":\"node_modules/.cache/vue-loader\",\"cacheIdentifier\":\"023ef482-vue-loader-template\"}!./node_modules/vue-loader/lib/loaders/templateLoader.js?!./node_modules/cache-loader/dist/cjs.js?!./node_modules/vue-loader/lib/index.js?!./src/components/Settings/components/ModalScrapydServer.vue?vue&type=template&id=370f88cf&scoped=true&":
             /*!*******************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
               !*** ./node_modules/cache-loader/dist/cjs.js?{"cacheDirectory":"node_modules/.cache/vue-loader","cacheIdentifier":"023ef482-vue-loader-template"}!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options!./src/components/Settings/components/ModalScrapydServer.vue?vue&type=template&id=370f88cf&scoped=true& ***!
               \*******************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /*! exports provided: render, staticRenderFns */
             /***/
             (function(module, __webpack_exports__, __webpack_require__) {
 
                 "use strict";
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"Modal\",\n    _vm._g(\n      _vm._b(\n        { attrs: { title: \"Scrapyd Server\", width: 600, \"footer-hide\": true } },\n        \"Modal\",\n        _vm.$attrs,\n        false\n      ),\n      _vm.$listeners\n    ),\n    [\n      _c(\n        \"div\",\n        { staticClass: \"alert-page\" },\n        [\n          _c(\n            \"el-row\",\n            [\n              _c(\n                \"el-form\",\n                {\n                  staticClass: \"demo-form-inline\",\n                  attrs: { inline: true, model: _vm.server, size: \"mini\" },\n                },\n                [\n                  _c(\n                    \"el-form-item\",\n                    { attrs: { label: \"\" } },\n                    [\n                      _c(\"el-input\", {\n                        attrs: { placeholder: \"服务器地址\" },\n                        model: {\n                          value: _vm.server.addr,\n                          callback: function ($$v) {\n                            _vm.$set(_vm.server, \"addr\", $$v)\n                          },\n                          expression: \"server.addr\",\n                        },\n                      }),\n                    ],\n                    1\n                  ),\n                  _c(\n                    \"el-form-item\",\n                    { attrs: { label: \"\" } },\n                    [\n                      _c(\"el-input\", {\n                        attrs: { placeholder: \"服务器名称\" },\n                        model: {\n                          value: _vm.server.alias,\n                          callback: function ($$v) {\n                            _vm.$set(_vm.server, \"alias\", $$v)\n                          },\n                          expression: \"server.alias\",\n                        },\n                      }),\n                    ],\n                    1\n                  ),\n                  _c(\n                    \"el-form-item\",\n                    [\n                      _c(\n                        \"el-button\",\n                        {\n                          attrs: { type: \"primary\" },\n                          on: {\n                            click: function ($event) {\n                              return _vm.apiAdd(\n                                _vm.server.addr,\n                                _vm.server.alias\n                              )\n                            },\n                          },\n                        },\n                        [_vm._v(\"新增\")]\n                      ),\n                    ],\n                    1\n                  ),\n                ],\n                1\n              ),\n            ],\n            1\n          ),\n          _c(\n            \"el-row\",\n            [\n              _c(\n                \"el-table\",\n                {\n                  staticStyle: { width: \"100%\" },\n                  attrs: {\n                    data: _vm.serverData,\n                    height: \"500\",\n                    stripe: \"\",\n                    fit: \"\",\n                    \"row-class-name\": _vm.rowClassName,\n                  },\n                },\n                [\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      prop: \"xh\",\n                      width: \"70\",\n                      label: \"ID\",\n                    },\n                  }),\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      prop: \"addr\",\n                      label: \"服务器地址\",\n                    },\n                  }),\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      prop: \"alias\",\n                      label: \"服务器名称\",\n                    },\n                  }),\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      label: \"操作\",\n                      \"show-overflow-tooltip\": \"\",\n                    },\n                    scopedSlots: _vm._u([\n                      {\n                        key: \"default\",\n                        fn: function (scope) {\n                          return [\n                            _c(\n                              \"el-button-group\",\n                              [\n                                _c(\"el-button\", {\n                                  attrs: {\n                                    size: \"mini\",\n                                    type: \"danger\",\n                                    icon: \"el-icon-delete\",\n                                    disabled: scope.row.isDefault === 1,\n                                  },\n                                  on: {\n                                    click: function ($event) {\n                                      return _vm.apiDelete(scope.row.addr)\n                                    },\n                                  },\n                                }),\n                                scope.row.isDefault\n                                  ? _c(\"el-button\", {\n                                      attrs: {\n                                        size: \"mini\",\n                                        type: \"primary\",\n                                        icon: \"el-icon-circle-check\",\n                                      },\n                                    })\n                                  : _c(\"el-button\", {\n                                      attrs: {\n                                        size: \"mini\",\n                                        type: \"info\",\n                                        plain: \"\",\n                                        icon: \"el-icon-circle-plus-outline\",\n                                      },\n                                      on: {\n                                        click: function ($event) {\n                                          return _vm.apiPut(scope.row.addr)\n                                        },\n                                      },\n                                    }),\n                              ],\n                              1\n                            ),\n                          ]\n                        },\n                      },\n                    ]),\n                  }),\n                ],\n                1\n              ),\n            ],\n            1\n          ),\n        ],\n        1\n      ),\n    ]\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Settings/components/ModalScrapydServer.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"Modal\",\n    _vm._g(\n      _vm._b(\n        { attrs: { title: \"Scrapyd Server\", width: 600, \"footer-hide\": true } },\n        \"Modal\",\n        _vm.$attrs,\n        false\n      ),\n      _vm.$listeners\n    ),\n    [\n      _c(\n        \"div\",\n        { staticClass: \"alert-page\" },\n        [\n          _c(\n            \"el-row\",\n            [\n              _c(\n                \"el-form\",\n                {\n                  staticClass: \"demo-form-inline\",\n                  attrs: { inline: true, model: _vm.server, size: \"mini\" },\n                },\n                [\n                  _c(\n                    \"el-form-item\",\n                    { attrs: { label: \"\" } },\n                    [\n                      _c(\"el-input\", {\n                        attrs: { placeholder: \"http://localhost:6800\" },\n                        model: {\n                          value: _vm.server.addr,\n                          callback: function ($$v) {\n                            _vm.$set(_vm.server, \"addr\", $$v)\n                          },\n                          expression: \"server.addr\",\n                        },\n                      }),\n                    ],\n                    1\n                  ),\n                  _c(\n                    \"el-form-item\",\n                    { attrs: { label: \"\" } },\n                    [\n                      _c(\"el-input\", {\n                        attrs: { placeholder: \"服务器名称\" },\n                        model: {\n                          value: _vm.server.alias,\n                          callback: function ($$v) {\n                            _vm.$set(_vm.server, \"alias\", $$v)\n                          },\n                          expression: \"server.alias\",\n                        },\n                      }),\n                    ],\n                    1\n                  ),\n                  _c(\n                    \"el-form-item\",\n                    [\n                      _c(\n                        \"el-button\",\n                        {\n                          attrs: { type: \"primary\" },\n                          on: {\n                            click: function ($event) {\n                              return _vm.apiAdd(\n                                _vm.server.addr,\n                                _vm.server.alias\n                              )\n                            },\n                          },\n                        },\n                        [_vm._v(\"新增\")]\n                      ),\n                    ],\n                    1\n                  ),\n                ],\n                1\n              ),\n            ],\n            1\n          ),\n          _c(\n            \"el-row\",\n            [\n              _c(\n                \"el-table\",\n                {\n                  staticStyle: { width: \"100%\" },\n                  attrs: {\n                    data: _vm.serverData,\n                    height: \"500\",\n                    stripe: \"\",\n                    fit: \"\",\n                    \"row-class-name\": _vm.rowClassName,\n                  },\n                },\n                [\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      prop: \"xh\",\n                      width: \"70\",\n                      label: \"ID\",\n                    },\n                  }),\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      prop: \"addr\",\n                      label: \"服务器地址\",\n                    },\n                  }),\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      prop: \"alias\",\n                      label: \"服务器名称\",\n                    },\n                  }),\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      label: \"操作\",\n                      \"show-overflow-tooltip\": \"\",\n                    },\n                    scopedSlots: _vm._u([\n                      {\n                        key: \"default\",\n                        fn: function (scope) {\n                          return [\n                            _c(\n                              \"el-button-group\",\n                              [\n                                _c(\"el-button\", {\n                                  attrs: {\n                                    size: \"mini\",\n                                    type: \"danger\",\n                                    icon: \"el-icon-delete\",\n                                    disabled: scope.row.isDefault === 1,\n                                  },\n                                  on: {\n                                    click: function ($event) {\n                                      return _vm.apiDelete(scope.row.addr)\n                                    },\n                                  },\n                                }),\n                                scope.row.isDefault\n                                  ? _c(\"el-button\", {\n                                      attrs: {\n                                        size: \"mini\",\n                                        type: \"primary\",\n                                        icon: \"el-icon-circle-check\",\n                                      },\n                                    })\n                                  : _c(\"el-button\", {\n                                      attrs: {\n                                        size: \"mini\",\n                                        type: \"info\",\n                                        plain: \"\",\n                                        icon: \"el-icon-circle-plus-outline\",\n                                      },\n                                      on: {\n                                        click: function ($event) {\n                                          return _vm.apiPut(scope.row.addr)\n                                        },\n                                      },\n                                    }),\n                              ],\n                              1\n                            ),\n                          ]\n                        },\n                      },\n                    ]),\n                  }),\n                ],\n                1\n              ),\n            ],\n            1\n          ),\n        ],\n        1\n      ),\n    ]\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Settings/components/ModalScrapydServer.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
 
                 /***/
             }),
 
         /***/
         "./node_modules/css-loader/dist/cjs.js?!./node_modules/vue-loader/lib/loaders/stylePostLoader.js!./node_modules/postcss-loader/src/index.js?!./node_modules/less-loader/dist/cjs.js?!./node_modules/cache-loader/dist/cjs.js?!./node_modules/vue-loader/lib/index.js?!./src/components/Settings/components/ModalMailSender.vue?vue&type=style&index=0&id=17a57dac&lang=less&scoped=true&":
             /*!***************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
```

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/js/2.js` & `crawler_studio-1.5.6/crawler_studio/dist/static/js/2.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/js/3.js` & `crawler_studio-1.5.6/crawler_studio/dist/static/js/3.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/js/4.js` & `crawler_studio-1.5.6/crawler_studio/dist/static/js/4.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -7,30 +7,30 @@
               !*** ./node_modules/cache-loader/dist/cjs.js??ref--13-0!./node_modules/babel-loader/lib!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options!./src/components/Scrapyd/SpiderRunning.vue?vue&type=script&lang=js& ***!
               \******************************************************************************************************************************************************************************************************************************************************************/
             /*! exports provided: default */
             /***/
             (function(module, __webpack_exports__, __webpack_require__) {
 
                 "use strict";
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var core_js_modules_es_object_to_string_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! core-js/modules/es.object.to-string.js */ \"./node_modules/core-js/modules/es.object.to-string.js\");\n/* harmony import */ var core_js_modules_es_object_to_string_js__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_object_to_string_js__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var core_js_modules_es_regexp_to_string_js__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! core-js/modules/es.regexp.to-string.js */ \"./node_modules/core-js/modules/es.regexp.to-string.js\");\n/* harmony import */ var core_js_modules_es_regexp_to_string_js__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_regexp_to_string_js__WEBPACK_IMPORTED_MODULE_1__);\n/* harmony import */ var core_js_modules_es_array_concat_js__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! core-js/modules/es.array.concat.js */ \"./node_modules/core-js/modules/es.array.concat.js\");\n/* harmony import */ var core_js_modules_es_array_concat_js__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_array_concat_js__WEBPACK_IMPORTED_MODULE_2__);\n/* harmony import */ var _SpiderRunningHeader__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! ./SpiderRunningHeader */ \"./src/components/Scrapyd/SpiderRunningHeader.vue\");\n/* harmony import */ var _ModalMonitor__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! ./ModalMonitor */ \"./src/components/Scrapyd/ModalMonitor.vue\");\n/* harmony import */ var _utils_date__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/date */ \"./src/utils/date.js\");\n\n\n\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n\n\n\n\nfunction timer(span) {\n  return new Promise(function (r) {\n    setTimeout(function () {\n      r(undefined);\n    }, span);\n  });\n}\n\n/* harmony default export */ __webpack_exports__[\"default\"] = ({\n  name: \"spider_running\",\n  props: {\n    city: String\n  },\n  components: {\n    RunningHeader: _SpiderRunningHeader__WEBPACK_IMPORTED_MODULE_3__[\"default\"],\n    monitorModal: _ModalMonitor__WEBPACK_IMPORTED_MODULE_4__[\"default\"]\n  },\n  mounted: function mounted() {\n    if (this.currentServer) this.reloadPage();\n  },\n  data: function data() {\n    return {\n      showRecentLogsModal: false,\n      showMonitorModal: false,\n      tableData: [],\n      checkedData: [],\n      loading: true,\n      statsData: null,\n      spiderParams: {\n        project: '',\n        spider: '',\n        jobId: ''\n      },\n      timeoutID: 0\n    };\n  },\n  computed: {\n    currentServer: function currentServer() {\n      return this.$main.currentServer;\n    }\n  },\n  watch: {\n    currentServer: function currentServer(newVal, oldVal) {\n      this.reloadPage();\n    }\n  },\n  methods: {\n    cellStyle: function cellStyle(_ref) {\n      var row = _ref.row,\n          column = _ref.column,\n          rowIndex = _ref.rowIndex,\n          columnIndex = _ref.columnIndex;\n      var cellStyle;\n\n      if (row.last_run) {\n        var rowTime = new Date(row.last_run); // 开始时间\n\n        var curTime = new Date();\n        var days = Math.floor((curTime - rowTime) / 1000 / 60 / 60 / 24);\n\n        if (days === 0) {\n          cellStyle = 'background-color: #67C23A; color: white;';\n        } else if (days < 10) {\n          cellStyle = 'background-color: #fdf6ec; color: white;';\n        } else {\n          cellStyle = 'background: #F56C6C; color: white;';\n        }\n      }\n\n      if (column.label === '上次运行') return cellStyle;\n    },\n    formatStartRun: function formatStartRun(row, col) {\n      if (row.startTime) {\n        return Object(_utils_date__WEBPACK_IMPORTED_MODULE_5__[\"diffDate\"])(row.startTime);\n      } else {\n        return '';\n      }\n    },\n    formatLastRun: function formatLastRun(row, col) {\n      if (row.lastRun) {\n        return Object(_utils_date__WEBPACK_IMPORTED_MODULE_5__[\"diffDate\"])(row.lastRun);\n      } else {\n        return '';\n      }\n    },\n    openMonitorModal: function openMonitorModal(jobId) {\n      var _this = this;\n\n      this.$api.scrapyd.getSpiderStats({\n        jobId: jobId\n      }).then(function (response) {\n        _this.statsData = response.data.data;\n        _this.showMonitorModal = true;\n      });\n    },\n    rowClassName: function rowClassName(_ref2) {\n      var row = _ref2.row,\n          rowIndex = _ref2.rowIndex;\n      row.xh = rowIndex + 1;\n    },\n    reloadPage: function reloadPage() {\n      var _this2 = this;\n\n      this.tableData = [];\n      this.loading = true;\n      this.$api.scrapyd.getRunningSpider({\n        host: this.currentServer\n      }).then(function (response) {\n        _this2.tableData = response.data.data;\n        _this2.loading = false;\n      }).catch(function (error) {\n        return console.log(error);\n      });\n    },\n    closeSpider: function closeSpider(row) {\n      var _this3 = this;\n\n      var project = row.project;\n      var jobId = row.jobId;\n      var body = {\n        host: this.currentServer,\n        checkedData: [{\n          project: project,\n          jobId: jobId\n        }]\n      };\n      this.$api.scrapyd.delRunningSpider(body).then(function (response) {\n        _this3.$message.success(\"\\u5173\\u95ED\\u722C\\u866B\\u4EFB\\u52A1\\u6210\\u529F\");\n      }).catch(function (error) {\n        return _this3.$message.error(error.toString());\n      });\n    },\n    redirectLog: function redirectLog(project, spider, jobId) {\n      window.open(\"\".concat(this.currentServer, \"/logs/\").concat(project, \"/\").concat(spider, \"/\").concat(jobId, \".log\"));\n    } // handleSelectionChange(data) {\n    //   this.checkedData = data\n    // },\n\n  }\n});\n\n//# sourceURL=webpack:///./src/components/Scrapyd/SpiderRunning.vue?./node_modules/cache-loader/dist/cjs.js??ref--13-0!./node_modules/babel-loader/lib!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var core_js_modules_es_object_to_string_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! core-js/modules/es.object.to-string.js */ \"./node_modules/core-js/modules/es.object.to-string.js\");\n/* harmony import */ var core_js_modules_es_object_to_string_js__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_object_to_string_js__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var core_js_modules_es_regexp_to_string_js__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! core-js/modules/es.regexp.to-string.js */ \"./node_modules/core-js/modules/es.regexp.to-string.js\");\n/* harmony import */ var core_js_modules_es_regexp_to_string_js__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_regexp_to_string_js__WEBPACK_IMPORTED_MODULE_1__);\n/* harmony import */ var core_js_modules_es_array_concat_js__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! core-js/modules/es.array.concat.js */ \"./node_modules/core-js/modules/es.array.concat.js\");\n/* harmony import */ var core_js_modules_es_array_concat_js__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_array_concat_js__WEBPACK_IMPORTED_MODULE_2__);\n/* harmony import */ var _SpiderRunningHeader__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! ./SpiderRunningHeader */ \"./src/components/Scrapyd/SpiderRunningHeader.vue\");\n/* harmony import */ var _ModalMonitor__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! ./ModalMonitor */ \"./src/components/Scrapyd/ModalMonitor.vue\");\n/* harmony import */ var _utils_date__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/date */ \"./src/utils/date.js\");\n\n\n\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n\n\n\n\nfunction timer(span) {\n  return new Promise(function (r) {\n    setTimeout(function () {\n      r(undefined);\n    }, span);\n  });\n}\n\n/* harmony default export */ __webpack_exports__[\"default\"] = ({\n  name: \"spider_running\",\n  props: {\n    city: String\n  },\n  components: {\n    RunningHeader: _SpiderRunningHeader__WEBPACK_IMPORTED_MODULE_3__[\"default\"],\n    monitorModal: _ModalMonitor__WEBPACK_IMPORTED_MODULE_4__[\"default\"]\n  },\n  mounted: function mounted() {\n    if (this.currentServer) this.reloadPage();\n  },\n  data: function data() {\n    return {\n      showRecentLogsModal: false,\n      showMonitorModal: false,\n      tableData: [],\n      checkedData: [],\n      loading: true,\n      statsData: null,\n      spiderParams: {\n        project: '',\n        spider: '',\n        jobId: ''\n      },\n      timeoutID: 0\n    };\n  },\n  computed: {\n    currentServer: function currentServer() {\n      return this.$main.currentServer;\n    }\n  },\n  watch: {\n    currentServer: function currentServer(newVal, oldVal) {\n      this.reloadPage();\n    }\n  },\n  methods: {\n    cellStyle: function cellStyle(_ref) {\n      var row = _ref.row,\n          column = _ref.column,\n          rowIndex = _ref.rowIndex,\n          columnIndex = _ref.columnIndex;\n      var cellStyle;\n\n      if (row.last_run) {\n        var rowTime = new Date(row.last_run); // 开始时间\n\n        var curTime = new Date();\n        var days = Math.floor((curTime - rowTime) / 1000 / 60 / 60 / 24);\n\n        if (days === 0) {\n          cellStyle = 'background-color: #67C23A; color: white;';\n        } else if (days < 10) {\n          cellStyle = 'background-color: #fdf6ec; color: white;';\n        } else {\n          cellStyle = 'background: #F56C6C; color: white;';\n        }\n      }\n\n      if (column.label === '上次运行') return cellStyle;\n    },\n    formatStartRun: function formatStartRun(row, col) {\n      if (row.startTime) {\n        return Object(_utils_date__WEBPACK_IMPORTED_MODULE_5__[\"diffDate\"])(row.startTime);\n      } else {\n        return '';\n      }\n    },\n    formatLastRun: function formatLastRun(row, col) {\n      if (row.lastRun) {\n        return Object(_utils_date__WEBPACK_IMPORTED_MODULE_5__[\"diffDate\"])(row.lastRun);\n      } else {\n        return '';\n      }\n    },\n    openMonitorModal: function openMonitorModal(jobId) {\n      var _this = this;\n\n      this.$api.scrapyd.getSpiderStats({\n        jobId: jobId\n      }).then(function (response) {\n        _this.statsData = response.data.data;\n        _this.showMonitorModal = true;\n      });\n    },\n    rowClassName: function rowClassName(_ref2) {\n      var row = _ref2.row,\n          rowIndex = _ref2.rowIndex;\n      row.xh = rowIndex + 1;\n    },\n    reloadPage: function reloadPage() {\n      var _this2 = this;\n\n      this.tableData = [];\n      this.loading = true;\n      this.$api.scrapyd.getRunningSpider({\n        host: this.currentServer\n      }).then(function (response) {\n        _this2.tableData = response.data.data;\n        _this2.loading = false;\n      }).catch(function (error) {\n        return console.log(error);\n      });\n    },\n    closeSpider: function closeSpider(row) {\n      var _this3 = this;\n\n      var project = row.project;\n      var jobId = row.jobId;\n      var body = {\n        host: this.currentServer,\n        checkedData: [{\n          project: project,\n          jobId: jobId\n        }]\n      };\n      this.$api.scrapyd.delRunningSpider(body).then(function (response) {\n        _this3.$message.success(\"\\u5173\\u95ED\\u722C\\u866B\\u4EFB\\u52A1\\u6210\\u529F\");\n      }).catch(function (error) {\n        return _this3.$message.error(error.toString());\n      });\n    },\n    redirectLog: function redirectLog(project, spider, jobId) {\n      window.open(\"\".concat(this.currentServer, \"/logs/\").concat(project, \"/\").concat(spider, \"/\").concat(jobId, \".log\"));\n    } // handleSelectionChange(data) {\n    //   this.checkedData = data\n    // },\n\n  }\n});\n\n//# sourceURL=webpack:///./src/components/Scrapyd/SpiderRunning.vue?./node_modules/cache-loader/dist/cjs.js??ref--13-0!./node_modules/babel-loader/lib!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
 
                 /***/
             }),
 
         /***/
         "./node_modules/cache-loader/dist/cjs.js?{\"cacheDirectory\":\"node_modules/.cache/vue-loader\",\"cacheIdentifier\":\"023ef482-vue-loader-template\"}!./node_modules/vue-loader/lib/loaders/templateLoader.js?!./node_modules/cache-loader/dist/cjs.js?!./node_modules/vue-loader/lib/index.js?!./src/components/Scrapyd/SpiderRunning.vue?vue&type=template&id=596c9572&scoped=true&":
             /*!**************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
               !*** ./node_modules/cache-loader/dist/cjs.js?{"cacheDirectory":"node_modules/.cache/vue-loader","cacheIdentifier":"023ef482-vue-loader-template"}!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options!./src/components/Scrapyd/SpiderRunning.vue?vue&type=template&id=596c9572&scoped=true& ***!
               \**************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /*! exports provided: render, staticRenderFns */
             /***/
             (function(module, __webpack_exports__, __webpack_require__) {
 
                 "use strict";
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"div\",\n    [\n      _c(\"running-header\", {\n        attrs: { title: \"运行中的爬虫\", \"checked-data\": _vm.checkedData },\n        on: { reload: _vm.reloadPage },\n      }),\n      _c(\n        \"el-table\",\n        {\n          directives: [\n            {\n              name: \"loading\",\n              rawName: \"v-loading\",\n              value: _vm.loading,\n              expression: \"loading\",\n            },\n          ],\n          staticStyle: { width: \"100%\" },\n          attrs: {\n            data: _vm.tableData,\n            height: \"75vh\",\n            stripe: \"\",\n            fit: \"\",\n            size: \"mini\",\n            \"row-class-name\": _vm.rowClassName,\n          },\n        },\n        [\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"xh\", width: \"70\", label: \"ID\" },\n          }),\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"project\", label: \"项目\" },\n          }),\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"spider\", label: \"爬虫\" },\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              \"show-overflow-tooltip\": \"\",\n              align: \"center\",\n              prop: \"jobId\",\n              label: \"Job ID\",\n            },\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              align: \"center\",\n              prop: \"startTime\",\n              formatter: _vm.formatStartRun,\n              label: \"开始时间\",\n            },\n          }),\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"memoryUse\", label: \"占用内存\" },\n            scopedSlots: _vm._u([\n              {\n                key: \"default\",\n                fn: function (scope) {\n                  return [\n                    _c(\n                      \"el-tooltip\",\n                      {\n                        staticClass: \"item\",\n                        attrs: {\n                          effect: \"dark\",\n                          content: \"Limit \" + scope.row.memoryUseLimit + \"MB\",\n                          placement: \"top\",\n                        },\n                      },\n                      [\n                        _c(\n                          \"span\",\n                          {\n                            class: {\n                              \"cell-error\":\n                                scope.row.memoryUse > scope.row.memoryUseLimit,\n                              \"cell-ok\":\n                                scope.row.memoryUse < scope.row.memoryUseLimit,\n                              \"cell-unset\":\n                                scope.row.memoryUseLimit === \"Unknown\",\n                            },\n                          },\n                          [\n                            _vm._v(\n                              \" \" + _vm._s(scope.row.memoryUse + \"MB\") + \" \"\n                            ),\n                          ]\n                        ),\n                      ]\n                    ),\n                  ]\n                },\n              },\n            ]),\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              align: \"center\",\n              prop: \"logHourlyErrorRate\",\n              label: \"日志错误率\",\n            },\n            scopedSlots: _vm._u([\n              {\n                key: \"default\",\n                fn: function (scope) {\n                  return [\n                    _c(\n                      \"el-tooltip\",\n                      {\n                        staticClass: \"item\",\n                        attrs: {\n                          effect: \"dark\",\n                          content:\n                            \"Limit \" +\n                            ((scope.row.logHourlyErrorLimit * 100).toFixed(2) +\n                              \"%\"),\n                          placement: \"top\",\n                        },\n                      },\n                      [\n                        _c(\n                          \"span\",\n                          {\n                            class: {\n                              \"cell-error\":\n                                scope.row.logHourlyErrorRate >\n                                scope.row.logHourlyErrorLimit,\n                              \"cell-ok\":\n                                scope.row.logHourlyErrorRate <\n                                scope.row.logHourlyErrorLimit,\n                              \"cell-unset\":\n                                scope.row.logHourlyErrorLimit === \"Unknown\",\n                            },\n                          },\n                          [\n                            _vm._v(\n                              \" \" +\n                                _vm._s(\n                                  (scope.row.logHourlyErrorRate * 100).toFixed(\n                                    2\n                                  ) + \"%\"\n                                ) +\n                                \" \"\n                            ),\n                          ]\n                        ),\n                      ]\n                    ),\n                  ]\n                },\n              },\n            ]),\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              width: \"300\",\n              align: \"center\",\n              fixed: \"right\",\n              label: \"操作\",\n            },\n            scopedSlots: _vm._u([\n              {\n                key: \"default\",\n                fn: function (scope) {\n                  return [\n                    _c(\n                      \"el-button-group\",\n                      [\n                        _c(\n                          \"el-button\",\n                          {\n                            attrs: { size: \"mini\", plain: \"\", type: \"success\" },\n                            on: {\n                              click: function ($event) {\n                                return _vm.redirectLog(\n                                  scope.row.project,\n                                  scope.row.spider,\n                                  scope.row.jobId\n                                )\n                              },\n                            },\n                          },\n                          [_vm._v(\"Log\")]\n                        ),\n                        _c(\n                          \"el-button\",\n                          {\n                            attrs: { size: \"mini\", plain: \"\", type: \"success\" },\n                            on: {\n                              click: function ($event) {\n                                return _vm.openMonitorModal(scope.row.jobId)\n                              },\n                            },\n                          },\n                          [_vm._v(\"Stats\")]\n                        ),\n                        _c(\n                          \"el-popconfirm\",\n                          {\n                            attrs: { title: \"确定关闭吗？\" },\n                            on: {\n                              confirm: function ($event) {\n                                return _vm.closeSpider(scope.row)\n                              },\n                            },\n                          },\n                          [\n                            _c(\n                              \"el-button\",\n                              {\n                                attrs: {\n                                  slot: \"reference\",\n                                  size: \"mini\",\n                                  plain: \"\",\n                                  type: \"danger\",\n                                },\n                                slot: \"reference\",\n                              },\n                              [_vm._v(\"Close\")]\n                            ),\n                          ],\n                          1\n                        ),\n                      ],\n                      1\n                    ),\n                  ]\n                },\n              },\n            ]),\n          }),\n        ],\n        1\n      ),\n      _c(\"monitor-modal\", {\n        attrs: { \"stats-data\": _vm.statsData, width: 500 },\n        model: {\n          value: _vm.showMonitorModal,\n          callback: function ($$v) {\n            _vm.showMonitorModal = $$v\n          },\n          expression: \"showMonitorModal\",\n        },\n      }),\n    ],\n    1\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Scrapyd/SpiderRunning.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"div\",\n    [\n      _c(\"running-header\", {\n        attrs: { title: \"运行中的爬虫\", \"checked-data\": _vm.checkedData },\n        on: { reload: _vm.reloadPage },\n      }),\n      _c(\n        \"el-table\",\n        {\n          directives: [\n            {\n              name: \"loading\",\n              rawName: \"v-loading\",\n              value: _vm.loading,\n              expression: \"loading\",\n            },\n          ],\n          staticStyle: { width: \"100%\" },\n          attrs: {\n            data: _vm.tableData,\n            height: \"75vh\",\n            stripe: \"\",\n            fit: \"\",\n            size: \"mini\",\n            \"row-class-name\": _vm.rowClassName,\n          },\n        },\n        [\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"xh\", width: \"70\", label: \"ID\" },\n          }),\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"project\", label: \"项目\" },\n          }),\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"spider\", label: \"爬虫\" },\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              \"show-overflow-tooltip\": \"\",\n              align: \"center\",\n              prop: \"jobId\",\n              label: \"Job ID\",\n            },\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              \"show-overflow-tooltip\": \"\",\n              align: \"center\",\n              prop: \"startParams\",\n              label: \"启动参数\",\n            },\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              align: \"center\",\n              prop: \"startTime\",\n              formatter: _vm.formatStartRun,\n              label: \"开始时间\",\n            },\n          }),\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"memoryUse\", label: \"占用内存\" },\n            scopedSlots: _vm._u([\n              {\n                key: \"default\",\n                fn: function (scope) {\n                  return [\n                    _c(\n                      \"el-tooltip\",\n                      {\n                        staticClass: \"item\",\n                        attrs: {\n                          effect: \"dark\",\n                          content: \"Limit \" + scope.row.memoryUseLimit + \"MB\",\n                          placement: \"top\",\n                        },\n                      },\n                      [\n                        _c(\n                          \"span\",\n                          {\n                            class: {\n                              \"cell-error\":\n                                scope.row.memoryUse > scope.row.memoryUseLimit,\n                              \"cell-ok\":\n                                scope.row.memoryUse < scope.row.memoryUseLimit,\n                              \"cell-unset\":\n                                scope.row.memoryUseLimit === \"Unknown\",\n                            },\n                          },\n                          [\n                            _vm._v(\n                              \" \" + _vm._s(scope.row.memoryUse + \"MB\") + \" \"\n                            ),\n                          ]\n                        ),\n                      ]\n                    ),\n                  ]\n                },\n              },\n            ]),\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              align: \"center\",\n              prop: \"logHourlyErrorRate\",\n              label: \"日志错误率\",\n            },\n            scopedSlots: _vm._u([\n              {\n                key: \"default\",\n                fn: function (scope) {\n                  return [\n                    _c(\n                      \"el-tooltip\",\n                      {\n                        staticClass: \"item\",\n                        attrs: {\n                          effect: \"dark\",\n                          content:\n                            \"Limit \" +\n                            ((scope.row.logHourlyErrorLimit * 100).toFixed(2) +\n                              \"%\"),\n                          placement: \"top\",\n                        },\n                      },\n                      [\n                        _c(\n                          \"span\",\n                          {\n                            class: {\n                              \"cell-error\":\n                                scope.row.logHourlyErrorRate >\n                                scope.row.logHourlyErrorLimit,\n                              \"cell-ok\":\n                                scope.row.logHourlyErrorRate <\n                                scope.row.logHourlyErrorLimit,\n                              \"cell-unset\":\n                                scope.row.logHourlyErrorLimit === \"Unknown\",\n                            },\n                          },\n                          [\n                            _vm._v(\n                              \" \" +\n                                _vm._s(\n                                  (scope.row.logHourlyErrorRate * 100).toFixed(\n                                    2\n                                  ) + \"%\"\n                                ) +\n                                \" \"\n                            ),\n                          ]\n                        ),\n                      ]\n                    ),\n                  ]\n                },\n              },\n            ]),\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              width: \"300\",\n              align: \"center\",\n              fixed: \"right\",\n              label: \"操作\",\n            },\n            scopedSlots: _vm._u([\n              {\n                key: \"default\",\n                fn: function (scope) {\n                  return [\n                    _c(\n                      \"el-button-group\",\n                      [\n                        _c(\n                          \"el-button\",\n                          {\n                            attrs: { size: \"mini\", plain: \"\", type: \"success\" },\n                            on: {\n                              click: function ($event) {\n                                return _vm.redirectLog(\n                                  scope.row.project,\n                                  scope.row.spider,\n                                  scope.row.jobId\n                                )\n                              },\n                            },\n                          },\n                          [_vm._v(\"Log\")]\n                        ),\n                        _c(\n                          \"el-button\",\n                          {\n                            attrs: { size: \"mini\", plain: \"\", type: \"success\" },\n                            on: {\n                              click: function ($event) {\n                                return _vm.openMonitorModal(scope.row.jobId)\n                              },\n                            },\n                          },\n                          [_vm._v(\"Stats\")]\n                        ),\n                        _c(\n                          \"el-popconfirm\",\n                          {\n                            attrs: { title: \"确定关闭吗？\" },\n                            on: {\n                              confirm: function ($event) {\n                                return _vm.closeSpider(scope.row)\n                              },\n                            },\n                          },\n                          [\n                            _c(\n                              \"el-button\",\n                              {\n                                attrs: {\n                                  slot: \"reference\",\n                                  size: \"mini\",\n                                  plain: \"\",\n                                  type: \"danger\",\n                                },\n                                slot: \"reference\",\n                              },\n                              [_vm._v(\"Close\")]\n                            ),\n                          ],\n                          1\n                        ),\n                      ],\n                      1\n                    ),\n                  ]\n                },\n              },\n            ]),\n          }),\n        ],\n        1\n      ),\n      _c(\"monitor-modal\", {\n        attrs: { \"stats-data\": _vm.statsData, width: 500 },\n        model: {\n          value: _vm.showMonitorModal,\n          callback: function ($$v) {\n            _vm.showMonitorModal = $$v\n          },\n          expression: \"showMonitorModal\",\n        },\n      }),\n    ],\n    1\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Scrapyd/SpiderRunning.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
 
                 /***/
             }),
 
         /***/
         "./node_modules/core-js/internals/array-fill.js":
             /*!******************************************************!*\
```

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/js/5.js` & `crawler_studio-1.5.6/crawler_studio/dist/static/js/5.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/js/6.js` & `crawler_studio-1.5.6/crawler_studio/dist/static/js/6.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/js/app.js` & `crawler_studio-1.5.6/crawler_studio/dist/static/js/app.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/dist/static/js/chunk-vendors.js` & `crawler_studio-1.5.6/crawler_studio/dist/static/js/chunk-vendors.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/manage.py` & `crawler_studio-1.5.6/crawler_studio/manage.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/autocomplete.css` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/base.css` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/changelists.css` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/changelists.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/forms.css` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/forms.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/login.css` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/login.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/nav_sidebar.css` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/nav_sidebar.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/responsive.css` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/responsive.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/responsive_rtl.css` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/responsive_rtl.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/rtl.css` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/rtl.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/vendor/select2/LICENSE-SELECT2.md` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/vendor/select2/LICENSE-SELECT2.md`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/vendor/select2/select2.css` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/vendor/select2/select2.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/vendor/select2/select2.min.css` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/vendor/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/css/widgets.css` & `crawler_studio-1.5.6/crawler_studio/static/admin/css/widgets.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/fonts/LICENSE.txt` & `crawler_studio-1.5.6/crawler_studio/static/admin/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/fonts/Roboto-Bold-webfont.woff` & `crawler_studio-1.5.6/crawler_studio/static/admin/fonts/Roboto-Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/fonts/Roboto-Light-webfont.woff` & `crawler_studio-1.5.6/crawler_studio/static/admin/fonts/Roboto-Light-webfont.woff`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/fonts/Roboto-Regular-webfont.woff` & `crawler_studio-1.5.6/crawler_studio/static/admin/fonts/Roboto-Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/LICENSE` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/LICENSE`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/calendar-icons.svg` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/calendar-icons.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/gis/move_vertex_off.svg` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/gis/move_vertex_off.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/gis/move_vertex_on.svg` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/gis/move_vertex_on.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-calendar.svg` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-calendar.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-clock.svg` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-clock.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-no.svg` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-no.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-unknown-alt.svg` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-unknown-alt.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-unknown.svg` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-unknown.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/icon-viewlink.svg` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/icon-viewlink.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/inline-delete.svg` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/inline-delete.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/selector-icons.svg` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/img/sorting-icons.svg` & `crawler_studio-1.5.6/crawler_studio/static/admin/img/sorting-icons.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/SelectBox.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/SelectBox.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/SelectFilter2.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/SelectFilter2.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/actions.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/actions.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/admin/DateTimeShortcuts.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/admin/DateTimeShortcuts.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/admin/RelatedObjectLookups.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/admin/RelatedObjectLookups.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/autocomplete.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/autocomplete.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/calendar.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/calendar.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/cancel.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/cancel.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/change_form.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/change_form.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/collapse.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/collapse.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/core.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/core.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/inlines.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/inlines.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/nav_sidebar.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/nav_sidebar.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/popup_response.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/popup_response.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/prepopulate.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/prepopulate.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/urlify.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/urlify.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/jquery/LICENSE.txt` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/jquery/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/jquery/jquery.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/jquery/jquery.min.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/LICENSE.md` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/af.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/af.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ar.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/az.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/az.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/bg.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/bn.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/bs.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ca.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/cs.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/da.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/da.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/de.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/de.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/dsb.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/el.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/el.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/en.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/en.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/es.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/es.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/et.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/et.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/eu.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/fa.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/fi.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/fr.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/gl.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/he.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/he.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/hi.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/hr.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/hsb.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/hu.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/hy.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/id.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/id.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/is.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/is.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/it.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/it.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ja.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ka.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/km.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/km.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ko.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/lt.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/lv.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/mk.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ms.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/nb.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ne.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/nl.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/pl.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ps.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/pt-BR.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/pt.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ro.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/ru.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/sk.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/sl.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/sq.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/sr-Cyrl.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/sr.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/sv.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/th.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/th.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/tk.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/tr.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/uk.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/vi.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/zh-CN.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/i18n/zh-TW.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/select2.full.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/select2.full.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/select2/select2.full.min.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/select2/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/xregexp/LICENSE.txt` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/xregexp/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/xregexp/xregexp.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/xregexp/xregexp.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/admin/js/vendor/xregexp/xregexp.min.js` & `crawler_studio-1.5.6/crawler_studio/static/admin/js/vendor/xregexp/xregexp.min.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/fonts/element-icons.535877f5.woff` & `crawler_studio-1.5.6/crawler_studio/static/fonts/element-icons.535877f5.woff`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/fonts/element-icons.732389de.ttf` & `crawler_studio-1.5.6/crawler_studio/static/fonts/element-icons.732389de.ttf`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/fonts/ionicons.143146fa.woff2` & `crawler_studio-1.5.6/crawler_studio/static/fonts/ionicons.143146fa.woff2`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/fonts/ionicons.99ac3308.woff` & `crawler_studio-1.5.6/crawler_studio/static/fonts/ionicons.99ac3308.woff`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/fonts/ionicons.d535a25a.ttf` & `crawler_studio-1.5.6/crawler_studio/static/fonts/ionicons.d535a25a.ttf`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/img/favicon.37e81aa2.png` & `crawler_studio-1.5.6/crawler_studio/static/img/favicon.37e81aa2.png`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/img/ionicons.a2c4a261.svg` & `crawler_studio-1.5.6/crawler_studio/static/img/ionicons.a2c4a261.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/img/universe.0efde44f.jpeg` & `crawler_studio-1.5.6/crawler_studio/static/img/universe.0efde44f.jpeg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/js/0.js` & `crawler_studio-1.5.6/crawler_studio/static/js/0.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/js/1.js` & `crawler_studio-1.5.6/crawler_studio/static/js/1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -82,45 +82,45 @@
               !*** ./node_modules/cache-loader/dist/cjs.js?{"cacheDirectory":"node_modules/.cache/vue-loader","cacheIdentifier":"023ef482-vue-loader-template"}!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options!./src/components/Settings/components/ModalMailSender.vue?vue&type=template&id=17a57dac&scoped=true& ***!
               \****************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /*! exports provided: render, staticRenderFns */
             /***/
             (function(module, __webpack_exports__, __webpack_require__) {
 
                 "use strict";
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"Modal\",\n    _vm._g(\n      _vm._b(\n        {\n          attrs: { title: \"系统邮件发件人\", width: 450, \"footer-hide\": false },\n          on: { \"on-ok\": _vm.onOK },\n          model: {\n            value: _vm.showDialog,\n            callback: function ($$v) {\n              _vm.showDialog = $$v\n            },\n            expression: \"showDialog\",\n          },\n        },\n        \"Modal\",\n        _vm.$attrs,\n        false\n      ),\n      _vm.$listeners\n    ),\n    [\n      _c(\n        \"el-form\",\n        {\n          ref: \"form\",\n          attrs: {\n            size: \"mini\",\n            rules: _vm.rules,\n            \"label-width\": \"100px\",\n            model: _vm.formData,\n          },\n        },\n        [\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"发件人地址\", prop: \"mailAddr\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.mailAddr,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"mailAddr\", $$v)\n                  },\n                  expression: \"formData.mailAddr\",\n                },\n              }),\n            ],\n            1\n          ),\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"服务器地址\", prop: \"serverAddr\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.serverAddr,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"serverAddr\", $$v)\n                  },\n                  expression: \"formData.serverAddr\",\n                },\n              }),\n            ],\n            1\n          ),\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"服务器端口\", prop: \"mailPort\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.mailPort,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"mailPort\", $$v)\n                  },\n                  expression: \"formData.mailPort\",\n                },\n              }),\n            ],\n            1\n          ),\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"邮件授权码\", prop: \"authCode\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.authCode,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"authCode\", $$v)\n                  },\n                  expression: \"formData.authCode\",\n                },\n              }),\n            ],\n            1\n          ),\n        ],\n        1\n      ),\n      _c(\n        \"div\",\n        { attrs: { slot: \"footer\" }, slot: \"footer\" },\n        [\n          _c(\n            \"Button\",\n            {\n              attrs: { type: \"text\" },\n              on: {\n                click: function ($event) {\n                  _vm.showDialog = false\n                },\n              },\n            },\n            [_vm._v(\"取消\")]\n          ),\n          _c(\n            \"Button\",\n            { attrs: { type: \"primary\" }, on: { click: _vm.onOK } },\n            [_vm._v(\"确定\")]\n          ),\n        ],\n        1\n      ),\n    ],\n    1\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Settings/components/ModalMailSender.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"Modal\",\n    _vm._g(\n      _vm._b(\n        {\n          attrs: { title: \"系统邮件发件人\", width: 450, \"footer-hide\": false },\n          on: { \"on-ok\": _vm.onOK },\n          model: {\n            value: _vm.showDialog,\n            callback: function ($$v) {\n              _vm.showDialog = $$v\n            },\n            expression: \"showDialog\",\n          },\n        },\n        \"Modal\",\n        _vm.$attrs,\n        false\n      ),\n      _vm.$listeners\n    ),\n    [\n      _c(\n        \"el-form\",\n        {\n          ref: \"form\",\n          attrs: {\n            size: \"mini\",\n            rules: _vm.rules,\n            \"label-width\": \"100px\",\n            model: _vm.formData,\n          },\n        },\n        [\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"发件人地址\", prop: \"mailAddr\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.mailAddr,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"mailAddr\", $$v)\n                  },\n                  expression: \"formData.mailAddr\",\n                },\n              }),\n            ],\n            1\n          ),\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"服务器地址\", prop: \"serverAddr\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.serverAddr,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"serverAddr\", $$v)\n                  },\n                  expression: \"formData.serverAddr\",\n                },\n              }),\n            ],\n            1\n          ),\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"服务器端口\", prop: \"mailPort\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\" },\n                model: {\n                  value: _vm.formData.mailPort,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"mailPort\", $$v)\n                  },\n                  expression: \"formData.mailPort\",\n                },\n              }),\n            ],\n            1\n          ),\n          _c(\n            \"el-form-item\",\n            { attrs: { label: \"邮件授权码\", prop: \"authCode\" } },\n            [\n              _c(\"el-input\", {\n                attrs: { placeholder: \"\", type: \"password\" },\n                model: {\n                  value: _vm.formData.authCode,\n                  callback: function ($$v) {\n                    _vm.$set(_vm.formData, \"authCode\", $$v)\n                  },\n                  expression: \"formData.authCode\",\n                },\n              }),\n            ],\n            1\n          ),\n        ],\n        1\n      ),\n      _c(\n        \"div\",\n        { attrs: { slot: \"footer\" }, slot: \"footer\" },\n        [\n          _c(\n            \"Button\",\n            {\n              attrs: { type: \"text\" },\n              on: {\n                click: function ($event) {\n                  _vm.showDialog = false\n                },\n              },\n            },\n            [_vm._v(\"取消\")]\n          ),\n          _c(\n            \"Button\",\n            { attrs: { type: \"primary\" }, on: { click: _vm.onOK } },\n            [_vm._v(\"确定\")]\n          ),\n        ],\n        1\n      ),\n    ],\n    1\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Settings/components/ModalMailSender.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
 
                 /***/
             }),
 
         /***/
         "./node_modules/cache-loader/dist/cjs.js?{\"cacheDirectory\":\"node_modules/.cache/vue-loader\",\"cacheIdentifier\":\"023ef482-vue-loader-template\"}!./node_modules/vue-loader/lib/loaders/templateLoader.js?!./node_modules/cache-loader/dist/cjs.js?!./node_modules/vue-loader/lib/index.js?!./src/components/Settings/components/ModalMonitorRev.vue?vue&type=template&id=8b6a656e&scoped=true&":
             /*!****************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
               !*** ./node_modules/cache-loader/dist/cjs.js?{"cacheDirectory":"node_modules/.cache/vue-loader","cacheIdentifier":"023ef482-vue-loader-template"}!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options!./src/components/Settings/components/ModalMonitorRev.vue?vue&type=template&id=8b6a656e&scoped=true& ***!
               \****************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /*! exports provided: render, staticRenderFns */
             /***/
             (function(module, __webpack_exports__, __webpack_require__) {
 
                 "use strict";
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"Modal\",\n    _vm._g(\n      _vm._b(\n        {\n          attrs: { title: \"监控收件人\", width: 700, \"footer-hide\": true },\n          model: {\n            value: _vm.showDialog,\n            callback: function ($$v) {\n              _vm.showDialog = $$v\n            },\n            expression: \"showDialog\",\n          },\n        },\n        \"Modal\",\n        _vm.$attrs,\n        false\n      ),\n      _vm.$listeners\n    ),\n    [\n      _c(\n        \"div\",\n        { staticClass: \"alert-page\" },\n        [\n          _c(\n            \"el-form\",\n            { attrs: { inline: true, size: \"mini\" } },\n            [\n              _c(\n                \"el-form-item\",\n                { attrs: { label: \"\" } },\n                [\n                  _c(\n                    \"el-select\",\n                    {\n                      attrs: { placeholder: \"收件方式\" },\n                      model: {\n                        value: _vm.formData.method,\n                        callback: function ($$v) {\n                          _vm.$set(_vm.formData, \"method\", $$v)\n                        },\n                        expression: \"formData.method\",\n                      },\n                    },\n                    [\n                      _c(\"el-option\", {\n                        attrs: { value: \"钉钉\", label: \"钉钉\" },\n                      }),\n                      _c(\"el-option\", {\n                        attrs: { value: \"邮件\", label: \"邮件\" },\n                      }),\n                    ],\n                    1\n                  ),\n                ],\n                1\n              ),\n              _c(\n                \"el-form-item\",\n                { attrs: { label: \"\" } },\n                [\n                  _c(\"el-input\", {\n                    attrs: { placeholder: \"收件人名称\" },\n                    model: {\n                      value: _vm.formData.revName,\n                      callback: function ($$v) {\n                        _vm.$set(_vm.formData, \"revName\", $$v)\n                      },\n                      expression: \"formData.revName\",\n                    },\n                  }),\n                ],\n                1\n              ),\n              _c(\n                \"el-form-item\",\n                { attrs: { label: \"\" } },\n                [\n                  _c(\"el-input\", {\n                    attrs: { placeholder: \"收件人地址\" },\n                    model: {\n                      value: _vm.formData.revAddr,\n                      callback: function ($$v) {\n                        _vm.$set(_vm.formData, \"revAddr\", $$v)\n                      },\n                      expression: \"formData.revAddr\",\n                    },\n                  }),\n                ],\n                1\n              ),\n              _c(\n                \"el-button\",\n                {\n                  attrs: { type: \"primary\", size: \"mini\" },\n                  on: { click: _vm.apiAdd },\n                },\n                [_vm._v(\"新增\")]\n              ),\n            ],\n            1\n          ),\n          _c(\n            \"el-table\",\n            {\n              ref: \"table\",\n              staticStyle: { width: \"100%\", \"margin-top\": \"20px\" },\n              attrs: {\n                data: _vm.tableData,\n                height: \"300\",\n                stripe: \"\",\n                fit: \"\",\n                size: \"mini\",\n                \"row-class-name\": _vm.rowClassName,\n              },\n            },\n            [\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  prop: \"id\",\n                  width: \"70\",\n                  label: \"ID\",\n                },\n              }),\n              _c(\"el-table-column\", {\n                attrs: { align: \"center\", prop: \"method\", label: \"收件方式\" },\n              }),\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  prop: \"revName\",\n                  label: \"收件人名称\",\n                },\n              }),\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  prop: \"revAddr\",\n                  label: \"收件人地址\",\n                },\n              }),\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  label: \"操作\",\n                  \"show-overflow-tooltip\": \"\",\n                },\n                scopedSlots: _vm._u([\n                  {\n                    key: \"default\",\n                    fn: function (scope) {\n                      return [\n                        _c(\n                          \"el-button-group\",\n                          [\n                            _c(\"el-button\", {\n                              attrs: {\n                                size: \"mini\",\n                                type: \"danger\",\n                                icon: \"el-icon-delete\",\n                              },\n                              on: {\n                                click: function ($event) {\n                                  return _vm.apiDelete(scope.row.revAddr)\n                                },\n                              },\n                            }),\n                          ],\n                          1\n                        ),\n                      ]\n                    },\n                  },\n                ]),\n              }),\n            ],\n            1\n          ),\n        ],\n        1\n      ),\n    ]\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Settings/components/ModalMonitorRev.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"Modal\",\n    _vm._g(\n      _vm._b(\n        {\n          attrs: { title: \"监控收件人\", width: 700, \"footer-hide\": true },\n          model: {\n            value: _vm.showDialog,\n            callback: function ($$v) {\n              _vm.showDialog = $$v\n            },\n            expression: \"showDialog\",\n          },\n        },\n        \"Modal\",\n        _vm.$attrs,\n        false\n      ),\n      _vm.$listeners\n    ),\n    [\n      _c(\n        \"div\",\n        { staticClass: \"alert-page\" },\n        [\n          _c(\n            \"el-form\",\n            { attrs: { inline: true, size: \"mini\" } },\n            [\n              _c(\n                \"el-form-item\",\n                { attrs: { label: \"\" } },\n                [\n                  _c(\n                    \"el-select\",\n                    {\n                      attrs: { placeholder: \"收件方式\" },\n                      model: {\n                        value: _vm.formData.method,\n                        callback: function ($$v) {\n                          _vm.$set(_vm.formData, \"method\", $$v)\n                        },\n                        expression: \"formData.method\",\n                      },\n                    },\n                    [\n                      _c(\"el-option\", {\n                        attrs: { value: \"钉钉\", label: \"钉钉机器人\" },\n                      }),\n                      _c(\"el-option\", {\n                        attrs: { value: \"邮件\", label: \"邮件\" },\n                      }),\n                    ],\n                    1\n                  ),\n                ],\n                1\n              ),\n              _c(\n                \"el-form-item\",\n                { attrs: { label: \"\" } },\n                [\n                  _c(\"el-input\", {\n                    attrs: { placeholder: \"收件人名称\" },\n                    model: {\n                      value: _vm.formData.revName,\n                      callback: function ($$v) {\n                        _vm.$set(_vm.formData, \"revName\", $$v)\n                      },\n                      expression: \"formData.revName\",\n                    },\n                  }),\n                ],\n                1\n              ),\n              _c(\n                \"el-form-item\",\n                { attrs: { label: \"\" } },\n                [\n                  _c(\"el-input\", {\n                    attrs: { placeholder: \"收件人地址\" },\n                    model: {\n                      value: _vm.formData.revAddr,\n                      callback: function ($$v) {\n                        _vm.$set(_vm.formData, \"revAddr\", $$v)\n                      },\n                      expression: \"formData.revAddr\",\n                    },\n                  }),\n                ],\n                1\n              ),\n              _c(\n                \"el-button\",\n                {\n                  attrs: { type: \"primary\", size: \"mini\" },\n                  on: { click: _vm.apiAdd },\n                },\n                [_vm._v(\"新增\")]\n              ),\n            ],\n            1\n          ),\n          _c(\n            \"el-table\",\n            {\n              ref: \"table\",\n              staticStyle: { width: \"100%\", \"margin-top\": \"20px\" },\n              attrs: {\n                data: _vm.tableData,\n                height: \"300\",\n                stripe: \"\",\n                fit: \"\",\n                size: \"mini\",\n                \"row-class-name\": _vm.rowClassName,\n              },\n            },\n            [\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  prop: \"id\",\n                  width: \"70\",\n                  label: \"ID\",\n                },\n              }),\n              _c(\"el-table-column\", {\n                attrs: { align: \"center\", prop: \"method\", label: \"收件方式\" },\n              }),\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  prop: \"revName\",\n                  label: \"收件人名称\",\n                },\n              }),\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  prop: \"revAddr\",\n                  label: \"收件人地址\",\n                },\n              }),\n              _c(\"el-table-column\", {\n                attrs: {\n                  align: \"center\",\n                  label: \"操作\",\n                  \"show-overflow-tooltip\": \"\",\n                },\n                scopedSlots: _vm._u([\n                  {\n                    key: \"default\",\n                    fn: function (scope) {\n                      return [\n                        _c(\n                          \"el-button-group\",\n                          [\n                            _c(\"el-button\", {\n                              attrs: {\n                                size: \"mini\",\n                                type: \"danger\",\n                                icon: \"el-icon-delete\",\n                              },\n                              on: {\n                                click: function ($event) {\n                                  return _vm.apiDelete(scope.row.revAddr)\n                                },\n                              },\n                            }),\n                          ],\n                          1\n                        ),\n                      ]\n                    },\n                  },\n                ]),\n              }),\n            ],\n            1\n          ),\n        ],\n        1\n      ),\n    ]\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Settings/components/ModalMonitorRev.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
 
                 /***/
             }),
 
         /***/
         "./node_modules/cache-loader/dist/cjs.js?{\"cacheDirectory\":\"node_modules/.cache/vue-loader\",\"cacheIdentifier\":\"023ef482-vue-loader-template\"}!./node_modules/vue-loader/lib/loaders/templateLoader.js?!./node_modules/cache-loader/dist/cjs.js?!./node_modules/vue-loader/lib/index.js?!./src/components/Settings/components/ModalScrapydServer.vue?vue&type=template&id=370f88cf&scoped=true&":
             /*!*******************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
               !*** ./node_modules/cache-loader/dist/cjs.js?{"cacheDirectory":"node_modules/.cache/vue-loader","cacheIdentifier":"023ef482-vue-loader-template"}!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options!./src/components/Settings/components/ModalScrapydServer.vue?vue&type=template&id=370f88cf&scoped=true& ***!
               \*******************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /*! exports provided: render, staticRenderFns */
             /***/
             (function(module, __webpack_exports__, __webpack_require__) {
 
                 "use strict";
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"Modal\",\n    _vm._g(\n      _vm._b(\n        { attrs: { title: \"Scrapyd Server\", width: 600, \"footer-hide\": true } },\n        \"Modal\",\n        _vm.$attrs,\n        false\n      ),\n      _vm.$listeners\n    ),\n    [\n      _c(\n        \"div\",\n        { staticClass: \"alert-page\" },\n        [\n          _c(\n            \"el-row\",\n            [\n              _c(\n                \"el-form\",\n                {\n                  staticClass: \"demo-form-inline\",\n                  attrs: { inline: true, model: _vm.server, size: \"mini\" },\n                },\n                [\n                  _c(\n                    \"el-form-item\",\n                    { attrs: { label: \"\" } },\n                    [\n                      _c(\"el-input\", {\n                        attrs: { placeholder: \"服务器地址\" },\n                        model: {\n                          value: _vm.server.addr,\n                          callback: function ($$v) {\n                            _vm.$set(_vm.server, \"addr\", $$v)\n                          },\n                          expression: \"server.addr\",\n                        },\n                      }),\n                    ],\n                    1\n                  ),\n                  _c(\n                    \"el-form-item\",\n                    { attrs: { label: \"\" } },\n                    [\n                      _c(\"el-input\", {\n                        attrs: { placeholder: \"服务器名称\" },\n                        model: {\n                          value: _vm.server.alias,\n                          callback: function ($$v) {\n                            _vm.$set(_vm.server, \"alias\", $$v)\n                          },\n                          expression: \"server.alias\",\n                        },\n                      }),\n                    ],\n                    1\n                  ),\n                  _c(\n                    \"el-form-item\",\n                    [\n                      _c(\n                        \"el-button\",\n                        {\n                          attrs: { type: \"primary\" },\n                          on: {\n                            click: function ($event) {\n                              return _vm.apiAdd(\n                                _vm.server.addr,\n                                _vm.server.alias\n                              )\n                            },\n                          },\n                        },\n                        [_vm._v(\"新增\")]\n                      ),\n                    ],\n                    1\n                  ),\n                ],\n                1\n              ),\n            ],\n            1\n          ),\n          _c(\n            \"el-row\",\n            [\n              _c(\n                \"el-table\",\n                {\n                  staticStyle: { width: \"100%\" },\n                  attrs: {\n                    data: _vm.serverData,\n                    height: \"500\",\n                    stripe: \"\",\n                    fit: \"\",\n                    \"row-class-name\": _vm.rowClassName,\n                  },\n                },\n                [\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      prop: \"xh\",\n                      width: \"70\",\n                      label: \"ID\",\n                    },\n                  }),\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      prop: \"addr\",\n                      label: \"服务器地址\",\n                    },\n                  }),\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      prop: \"alias\",\n                      label: \"服务器名称\",\n                    },\n                  }),\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      label: \"操作\",\n                      \"show-overflow-tooltip\": \"\",\n                    },\n                    scopedSlots: _vm._u([\n                      {\n                        key: \"default\",\n                        fn: function (scope) {\n                          return [\n                            _c(\n                              \"el-button-group\",\n                              [\n                                _c(\"el-button\", {\n                                  attrs: {\n                                    size: \"mini\",\n                                    type: \"danger\",\n                                    icon: \"el-icon-delete\",\n                                    disabled: scope.row.isDefault === 1,\n                                  },\n                                  on: {\n                                    click: function ($event) {\n                                      return _vm.apiDelete(scope.row.addr)\n                                    },\n                                  },\n                                }),\n                                scope.row.isDefault\n                                  ? _c(\"el-button\", {\n                                      attrs: {\n                                        size: \"mini\",\n                                        type: \"primary\",\n                                        icon: \"el-icon-circle-check\",\n                                      },\n                                    })\n                                  : _c(\"el-button\", {\n                                      attrs: {\n                                        size: \"mini\",\n                                        type: \"info\",\n                                        plain: \"\",\n                                        icon: \"el-icon-circle-plus-outline\",\n                                      },\n                                      on: {\n                                        click: function ($event) {\n                                          return _vm.apiPut(scope.row.addr)\n                                        },\n                                      },\n                                    }),\n                              ],\n                              1\n                            ),\n                          ]\n                        },\n                      },\n                    ]),\n                  }),\n                ],\n                1\n              ),\n            ],\n            1\n          ),\n        ],\n        1\n      ),\n    ]\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Settings/components/ModalScrapydServer.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"Modal\",\n    _vm._g(\n      _vm._b(\n        { attrs: { title: \"Scrapyd Server\", width: 600, \"footer-hide\": true } },\n        \"Modal\",\n        _vm.$attrs,\n        false\n      ),\n      _vm.$listeners\n    ),\n    [\n      _c(\n        \"div\",\n        { staticClass: \"alert-page\" },\n        [\n          _c(\n            \"el-row\",\n            [\n              _c(\n                \"el-form\",\n                {\n                  staticClass: \"demo-form-inline\",\n                  attrs: { inline: true, model: _vm.server, size: \"mini\" },\n                },\n                [\n                  _c(\n                    \"el-form-item\",\n                    { attrs: { label: \"\" } },\n                    [\n                      _c(\"el-input\", {\n                        attrs: { placeholder: \"http://localhost:6800\" },\n                        model: {\n                          value: _vm.server.addr,\n                          callback: function ($$v) {\n                            _vm.$set(_vm.server, \"addr\", $$v)\n                          },\n                          expression: \"server.addr\",\n                        },\n                      }),\n                    ],\n                    1\n                  ),\n                  _c(\n                    \"el-form-item\",\n                    { attrs: { label: \"\" } },\n                    [\n                      _c(\"el-input\", {\n                        attrs: { placeholder: \"服务器名称\" },\n                        model: {\n                          value: _vm.server.alias,\n                          callback: function ($$v) {\n                            _vm.$set(_vm.server, \"alias\", $$v)\n                          },\n                          expression: \"server.alias\",\n                        },\n                      }),\n                    ],\n                    1\n                  ),\n                  _c(\n                    \"el-form-item\",\n                    [\n                      _c(\n                        \"el-button\",\n                        {\n                          attrs: { type: \"primary\" },\n                          on: {\n                            click: function ($event) {\n                              return _vm.apiAdd(\n                                _vm.server.addr,\n                                _vm.server.alias\n                              )\n                            },\n                          },\n                        },\n                        [_vm._v(\"新增\")]\n                      ),\n                    ],\n                    1\n                  ),\n                ],\n                1\n              ),\n            ],\n            1\n          ),\n          _c(\n            \"el-row\",\n            [\n              _c(\n                \"el-table\",\n                {\n                  staticStyle: { width: \"100%\" },\n                  attrs: {\n                    data: _vm.serverData,\n                    height: \"500\",\n                    stripe: \"\",\n                    fit: \"\",\n                    \"row-class-name\": _vm.rowClassName,\n                  },\n                },\n                [\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      prop: \"xh\",\n                      width: \"70\",\n                      label: \"ID\",\n                    },\n                  }),\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      prop: \"addr\",\n                      label: \"服务器地址\",\n                    },\n                  }),\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      prop: \"alias\",\n                      label: \"服务器名称\",\n                    },\n                  }),\n                  _c(\"el-table-column\", {\n                    attrs: {\n                      align: \"center\",\n                      label: \"操作\",\n                      \"show-overflow-tooltip\": \"\",\n                    },\n                    scopedSlots: _vm._u([\n                      {\n                        key: \"default\",\n                        fn: function (scope) {\n                          return [\n                            _c(\n                              \"el-button-group\",\n                              [\n                                _c(\"el-button\", {\n                                  attrs: {\n                                    size: \"mini\",\n                                    type: \"danger\",\n                                    icon: \"el-icon-delete\",\n                                    disabled: scope.row.isDefault === 1,\n                                  },\n                                  on: {\n                                    click: function ($event) {\n                                      return _vm.apiDelete(scope.row.addr)\n                                    },\n                                  },\n                                }),\n                                scope.row.isDefault\n                                  ? _c(\"el-button\", {\n                                      attrs: {\n                                        size: \"mini\",\n                                        type: \"primary\",\n                                        icon: \"el-icon-circle-check\",\n                                      },\n                                    })\n                                  : _c(\"el-button\", {\n                                      attrs: {\n                                        size: \"mini\",\n                                        type: \"info\",\n                                        plain: \"\",\n                                        icon: \"el-icon-circle-plus-outline\",\n                                      },\n                                      on: {\n                                        click: function ($event) {\n                                          return _vm.apiPut(scope.row.addr)\n                                        },\n                                      },\n                                    }),\n                              ],\n                              1\n                            ),\n                          ]\n                        },\n                      },\n                    ]),\n                  }),\n                ],\n                1\n              ),\n            ],\n            1\n          ),\n        ],\n        1\n      ),\n    ]\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Settings/components/ModalScrapydServer.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
 
                 /***/
             }),
 
         /***/
         "./node_modules/css-loader/dist/cjs.js?!./node_modules/vue-loader/lib/loaders/stylePostLoader.js!./node_modules/postcss-loader/src/index.js?!./node_modules/less-loader/dist/cjs.js?!./node_modules/cache-loader/dist/cjs.js?!./node_modules/vue-loader/lib/index.js?!./src/components/Settings/components/ModalMailSender.vue?vue&type=style&index=0&id=17a57dac&lang=less&scoped=true&":
             /*!***************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
```

### Comparing `crawler_studio-1.5.5/crawler_studio/static/js/2.js` & `crawler_studio-1.5.6/crawler_studio/static/js/2.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/js/3.js` & `crawler_studio-1.5.6/crawler_studio/static/js/3.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/js/4.js` & `crawler_studio-1.5.6/crawler_studio/static/js/4.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -7,30 +7,30 @@
               !*** ./node_modules/cache-loader/dist/cjs.js??ref--13-0!./node_modules/babel-loader/lib!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options!./src/components/Scrapyd/SpiderRunning.vue?vue&type=script&lang=js& ***!
               \******************************************************************************************************************************************************************************************************************************************************************/
             /*! exports provided: default */
             /***/
             (function(module, __webpack_exports__, __webpack_require__) {
 
                 "use strict";
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var core_js_modules_es_object_to_string_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! core-js/modules/es.object.to-string.js */ \"./node_modules/core-js/modules/es.object.to-string.js\");\n/* harmony import */ var core_js_modules_es_object_to_string_js__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_object_to_string_js__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var core_js_modules_es_regexp_to_string_js__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! core-js/modules/es.regexp.to-string.js */ \"./node_modules/core-js/modules/es.regexp.to-string.js\");\n/* harmony import */ var core_js_modules_es_regexp_to_string_js__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_regexp_to_string_js__WEBPACK_IMPORTED_MODULE_1__);\n/* harmony import */ var core_js_modules_es_array_concat_js__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! core-js/modules/es.array.concat.js */ \"./node_modules/core-js/modules/es.array.concat.js\");\n/* harmony import */ var core_js_modules_es_array_concat_js__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_array_concat_js__WEBPACK_IMPORTED_MODULE_2__);\n/* harmony import */ var _SpiderRunningHeader__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! ./SpiderRunningHeader */ \"./src/components/Scrapyd/SpiderRunningHeader.vue\");\n/* harmony import */ var _ModalMonitor__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! ./ModalMonitor */ \"./src/components/Scrapyd/ModalMonitor.vue\");\n/* harmony import */ var _utils_date__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/date */ \"./src/utils/date.js\");\n\n\n\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n\n\n\n\nfunction timer(span) {\n  return new Promise(function (r) {\n    setTimeout(function () {\n      r(undefined);\n    }, span);\n  });\n}\n\n/* harmony default export */ __webpack_exports__[\"default\"] = ({\n  name: \"spider_running\",\n  props: {\n    city: String\n  },\n  components: {\n    RunningHeader: _SpiderRunningHeader__WEBPACK_IMPORTED_MODULE_3__[\"default\"],\n    monitorModal: _ModalMonitor__WEBPACK_IMPORTED_MODULE_4__[\"default\"]\n  },\n  mounted: function mounted() {\n    if (this.currentServer) this.reloadPage();\n  },\n  data: function data() {\n    return {\n      showRecentLogsModal: false,\n      showMonitorModal: false,\n      tableData: [],\n      checkedData: [],\n      loading: true,\n      statsData: null,\n      spiderParams: {\n        project: '',\n        spider: '',\n        jobId: ''\n      },\n      timeoutID: 0\n    };\n  },\n  computed: {\n    currentServer: function currentServer() {\n      return this.$main.currentServer;\n    }\n  },\n  watch: {\n    currentServer: function currentServer(newVal, oldVal) {\n      this.reloadPage();\n    }\n  },\n  methods: {\n    cellStyle: function cellStyle(_ref) {\n      var row = _ref.row,\n          column = _ref.column,\n          rowIndex = _ref.rowIndex,\n          columnIndex = _ref.columnIndex;\n      var cellStyle;\n\n      if (row.last_run) {\n        var rowTime = new Date(row.last_run); // 开始时间\n\n        var curTime = new Date();\n        var days = Math.floor((curTime - rowTime) / 1000 / 60 / 60 / 24);\n\n        if (days === 0) {\n          cellStyle = 'background-color: #67C23A; color: white;';\n        } else if (days < 10) {\n          cellStyle = 'background-color: #fdf6ec; color: white;';\n        } else {\n          cellStyle = 'background: #F56C6C; color: white;';\n        }\n      }\n\n      if (column.label === '上次运行') return cellStyle;\n    },\n    formatStartRun: function formatStartRun(row, col) {\n      if (row.startTime) {\n        return Object(_utils_date__WEBPACK_IMPORTED_MODULE_5__[\"diffDate\"])(row.startTime);\n      } else {\n        return '';\n      }\n    },\n    formatLastRun: function formatLastRun(row, col) {\n      if (row.lastRun) {\n        return Object(_utils_date__WEBPACK_IMPORTED_MODULE_5__[\"diffDate\"])(row.lastRun);\n      } else {\n        return '';\n      }\n    },\n    openMonitorModal: function openMonitorModal(jobId) {\n      var _this = this;\n\n      this.$api.scrapyd.getSpiderStats({\n        jobId: jobId\n      }).then(function (response) {\n        _this.statsData = response.data.data;\n        _this.showMonitorModal = true;\n      });\n    },\n    rowClassName: function rowClassName(_ref2) {\n      var row = _ref2.row,\n          rowIndex = _ref2.rowIndex;\n      row.xh = rowIndex + 1;\n    },\n    reloadPage: function reloadPage() {\n      var _this2 = this;\n\n      this.tableData = [];\n      this.loading = true;\n      this.$api.scrapyd.getRunningSpider({\n        host: this.currentServer\n      }).then(function (response) {\n        _this2.tableData = response.data.data;\n        _this2.loading = false;\n      }).catch(function (error) {\n        return console.log(error);\n      });\n    },\n    closeSpider: function closeSpider(row) {\n      var _this3 = this;\n\n      var project = row.project;\n      var jobId = row.jobId;\n      var body = {\n        host: this.currentServer,\n        checkedData: [{\n          project: project,\n          jobId: jobId\n        }]\n      };\n      this.$api.scrapyd.delRunningSpider(body).then(function (response) {\n        _this3.$message.success(\"\\u5173\\u95ED\\u722C\\u866B\\u4EFB\\u52A1\\u6210\\u529F\");\n      }).catch(function (error) {\n        return _this3.$message.error(error.toString());\n      });\n    },\n    redirectLog: function redirectLog(project, spider, jobId) {\n      window.open(\"\".concat(this.currentServer, \"/logs/\").concat(project, \"/\").concat(spider, \"/\").concat(jobId, \".log\"));\n    } // handleSelectionChange(data) {\n    //   this.checkedData = data\n    // },\n\n  }\n});\n\n//# sourceURL=webpack:///./src/components/Scrapyd/SpiderRunning.vue?./node_modules/cache-loader/dist/cjs.js??ref--13-0!./node_modules/babel-loader/lib!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var core_js_modules_es_object_to_string_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! core-js/modules/es.object.to-string.js */ \"./node_modules/core-js/modules/es.object.to-string.js\");\n/* harmony import */ var core_js_modules_es_object_to_string_js__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_object_to_string_js__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var core_js_modules_es_regexp_to_string_js__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! core-js/modules/es.regexp.to-string.js */ \"./node_modules/core-js/modules/es.regexp.to-string.js\");\n/* harmony import */ var core_js_modules_es_regexp_to_string_js__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_regexp_to_string_js__WEBPACK_IMPORTED_MODULE_1__);\n/* harmony import */ var core_js_modules_es_array_concat_js__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! core-js/modules/es.array.concat.js */ \"./node_modules/core-js/modules/es.array.concat.js\");\n/* harmony import */ var core_js_modules_es_array_concat_js__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_array_concat_js__WEBPACK_IMPORTED_MODULE_2__);\n/* harmony import */ var _SpiderRunningHeader__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! ./SpiderRunningHeader */ \"./src/components/Scrapyd/SpiderRunningHeader.vue\");\n/* harmony import */ var _ModalMonitor__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! ./ModalMonitor */ \"./src/components/Scrapyd/ModalMonitor.vue\");\n/* harmony import */ var _utils_date__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/date */ \"./src/utils/date.js\");\n\n\n\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n//\n\n\n\n\nfunction timer(span) {\n  return new Promise(function (r) {\n    setTimeout(function () {\n      r(undefined);\n    }, span);\n  });\n}\n\n/* harmony default export */ __webpack_exports__[\"default\"] = ({\n  name: \"spider_running\",\n  props: {\n    city: String\n  },\n  components: {\n    RunningHeader: _SpiderRunningHeader__WEBPACK_IMPORTED_MODULE_3__[\"default\"],\n    monitorModal: _ModalMonitor__WEBPACK_IMPORTED_MODULE_4__[\"default\"]\n  },\n  mounted: function mounted() {\n    if (this.currentServer) this.reloadPage();\n  },\n  data: function data() {\n    return {\n      showRecentLogsModal: false,\n      showMonitorModal: false,\n      tableData: [],\n      checkedData: [],\n      loading: true,\n      statsData: null,\n      spiderParams: {\n        project: '',\n        spider: '',\n        jobId: ''\n      },\n      timeoutID: 0\n    };\n  },\n  computed: {\n    currentServer: function currentServer() {\n      return this.$main.currentServer;\n    }\n  },\n  watch: {\n    currentServer: function currentServer(newVal, oldVal) {\n      this.reloadPage();\n    }\n  },\n  methods: {\n    cellStyle: function cellStyle(_ref) {\n      var row = _ref.row,\n          column = _ref.column,\n          rowIndex = _ref.rowIndex,\n          columnIndex = _ref.columnIndex;\n      var cellStyle;\n\n      if (row.last_run) {\n        var rowTime = new Date(row.last_run); // 开始时间\n\n        var curTime = new Date();\n        var days = Math.floor((curTime - rowTime) / 1000 / 60 / 60 / 24);\n\n        if (days === 0) {\n          cellStyle = 'background-color: #67C23A; color: white;';\n        } else if (days < 10) {\n          cellStyle = 'background-color: #fdf6ec; color: white;';\n        } else {\n          cellStyle = 'background: #F56C6C; color: white;';\n        }\n      }\n\n      if (column.label === '上次运行') return cellStyle;\n    },\n    formatStartRun: function formatStartRun(row, col) {\n      if (row.startTime) {\n        return Object(_utils_date__WEBPACK_IMPORTED_MODULE_5__[\"diffDate\"])(row.startTime);\n      } else {\n        return '';\n      }\n    },\n    formatLastRun: function formatLastRun(row, col) {\n      if (row.lastRun) {\n        return Object(_utils_date__WEBPACK_IMPORTED_MODULE_5__[\"diffDate\"])(row.lastRun);\n      } else {\n        return '';\n      }\n    },\n    openMonitorModal: function openMonitorModal(jobId) {\n      var _this = this;\n\n      this.$api.scrapyd.getSpiderStats({\n        jobId: jobId\n      }).then(function (response) {\n        _this.statsData = response.data.data;\n        _this.showMonitorModal = true;\n      });\n    },\n    rowClassName: function rowClassName(_ref2) {\n      var row = _ref2.row,\n          rowIndex = _ref2.rowIndex;\n      row.xh = rowIndex + 1;\n    },\n    reloadPage: function reloadPage() {\n      var _this2 = this;\n\n      this.tableData = [];\n      this.loading = true;\n      this.$api.scrapyd.getRunningSpider({\n        host: this.currentServer\n      }).then(function (response) {\n        _this2.tableData = response.data.data;\n        _this2.loading = false;\n      }).catch(function (error) {\n        return console.log(error);\n      });\n    },\n    closeSpider: function closeSpider(row) {\n      var _this3 = this;\n\n      var project = row.project;\n      var jobId = row.jobId;\n      var body = {\n        host: this.currentServer,\n        checkedData: [{\n          project: project,\n          jobId: jobId\n        }]\n      };\n      this.$api.scrapyd.delRunningSpider(body).then(function (response) {\n        _this3.$message.success(\"\\u5173\\u95ED\\u722C\\u866B\\u4EFB\\u52A1\\u6210\\u529F\");\n      }).catch(function (error) {\n        return _this3.$message.error(error.toString());\n      });\n    },\n    redirectLog: function redirectLog(project, spider, jobId) {\n      window.open(\"\".concat(this.currentServer, \"/logs/\").concat(project, \"/\").concat(spider, \"/\").concat(jobId, \".log\"));\n    } // handleSelectionChange(data) {\n    //   this.checkedData = data\n    // },\n\n  }\n});\n\n//# sourceURL=webpack:///./src/components/Scrapyd/SpiderRunning.vue?./node_modules/cache-loader/dist/cjs.js??ref--13-0!./node_modules/babel-loader/lib!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
 
                 /***/
             }),
 
         /***/
         "./node_modules/cache-loader/dist/cjs.js?{\"cacheDirectory\":\"node_modules/.cache/vue-loader\",\"cacheIdentifier\":\"023ef482-vue-loader-template\"}!./node_modules/vue-loader/lib/loaders/templateLoader.js?!./node_modules/cache-loader/dist/cjs.js?!./node_modules/vue-loader/lib/index.js?!./src/components/Scrapyd/SpiderRunning.vue?vue&type=template&id=596c9572&scoped=true&":
             /*!**************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
               !*** ./node_modules/cache-loader/dist/cjs.js?{"cacheDirectory":"node_modules/.cache/vue-loader","cacheIdentifier":"023ef482-vue-loader-template"}!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options!./src/components/Scrapyd/SpiderRunning.vue?vue&type=template&id=596c9572&scoped=true& ***!
               \**************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /*! exports provided: render, staticRenderFns */
             /***/
             (function(module, __webpack_exports__, __webpack_require__) {
 
                 "use strict";
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"div\",\n    [\n      _c(\"running-header\", {\n        attrs: { title: \"运行中的爬虫\", \"checked-data\": _vm.checkedData },\n        on: { reload: _vm.reloadPage },\n      }),\n      _c(\n        \"el-table\",\n        {\n          directives: [\n            {\n              name: \"loading\",\n              rawName: \"v-loading\",\n              value: _vm.loading,\n              expression: \"loading\",\n            },\n          ],\n          staticStyle: { width: \"100%\" },\n          attrs: {\n            data: _vm.tableData,\n            height: \"75vh\",\n            stripe: \"\",\n            fit: \"\",\n            size: \"mini\",\n            \"row-class-name\": _vm.rowClassName,\n          },\n        },\n        [\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"xh\", width: \"70\", label: \"ID\" },\n          }),\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"project\", label: \"项目\" },\n          }),\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"spider\", label: \"爬虫\" },\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              \"show-overflow-tooltip\": \"\",\n              align: \"center\",\n              prop: \"jobId\",\n              label: \"Job ID\",\n            },\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              align: \"center\",\n              prop: \"startTime\",\n              formatter: _vm.formatStartRun,\n              label: \"开始时间\",\n            },\n          }),\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"memoryUse\", label: \"占用内存\" },\n            scopedSlots: _vm._u([\n              {\n                key: \"default\",\n                fn: function (scope) {\n                  return [\n                    _c(\n                      \"el-tooltip\",\n                      {\n                        staticClass: \"item\",\n                        attrs: {\n                          effect: \"dark\",\n                          content: \"Limit \" + scope.row.memoryUseLimit + \"MB\",\n                          placement: \"top\",\n                        },\n                      },\n                      [\n                        _c(\n                          \"span\",\n                          {\n                            class: {\n                              \"cell-error\":\n                                scope.row.memoryUse > scope.row.memoryUseLimit,\n                              \"cell-ok\":\n                                scope.row.memoryUse < scope.row.memoryUseLimit,\n                              \"cell-unset\":\n                                scope.row.memoryUseLimit === \"Unknown\",\n                            },\n                          },\n                          [\n                            _vm._v(\n                              \" \" + _vm._s(scope.row.memoryUse + \"MB\") + \" \"\n                            ),\n                          ]\n                        ),\n                      ]\n                    ),\n                  ]\n                },\n              },\n            ]),\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              align: \"center\",\n              prop: \"logHourlyErrorRate\",\n              label: \"日志错误率\",\n            },\n            scopedSlots: _vm._u([\n              {\n                key: \"default\",\n                fn: function (scope) {\n                  return [\n                    _c(\n                      \"el-tooltip\",\n                      {\n                        staticClass: \"item\",\n                        attrs: {\n                          effect: \"dark\",\n                          content:\n                            \"Limit \" +\n                            ((scope.row.logHourlyErrorLimit * 100).toFixed(2) +\n                              \"%\"),\n                          placement: \"top\",\n                        },\n                      },\n                      [\n                        _c(\n                          \"span\",\n                          {\n                            class: {\n                              \"cell-error\":\n                                scope.row.logHourlyErrorRate >\n                                scope.row.logHourlyErrorLimit,\n                              \"cell-ok\":\n                                scope.row.logHourlyErrorRate <\n                                scope.row.logHourlyErrorLimit,\n                              \"cell-unset\":\n                                scope.row.logHourlyErrorLimit === \"Unknown\",\n                            },\n                          },\n                          [\n                            _vm._v(\n                              \" \" +\n                                _vm._s(\n                                  (scope.row.logHourlyErrorRate * 100).toFixed(\n                                    2\n                                  ) + \"%\"\n                                ) +\n                                \" \"\n                            ),\n                          ]\n                        ),\n                      ]\n                    ),\n                  ]\n                },\n              },\n            ]),\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              width: \"300\",\n              align: \"center\",\n              fixed: \"right\",\n              label: \"操作\",\n            },\n            scopedSlots: _vm._u([\n              {\n                key: \"default\",\n                fn: function (scope) {\n                  return [\n                    _c(\n                      \"el-button-group\",\n                      [\n                        _c(\n                          \"el-button\",\n                          {\n                            attrs: { size: \"mini\", plain: \"\", type: \"success\" },\n                            on: {\n                              click: function ($event) {\n                                return _vm.redirectLog(\n                                  scope.row.project,\n                                  scope.row.spider,\n                                  scope.row.jobId\n                                )\n                              },\n                            },\n                          },\n                          [_vm._v(\"Log\")]\n                        ),\n                        _c(\n                          \"el-button\",\n                          {\n                            attrs: { size: \"mini\", plain: \"\", type: \"success\" },\n                            on: {\n                              click: function ($event) {\n                                return _vm.openMonitorModal(scope.row.jobId)\n                              },\n                            },\n                          },\n                          [_vm._v(\"Stats\")]\n                        ),\n                        _c(\n                          \"el-popconfirm\",\n                          {\n                            attrs: { title: \"确定关闭吗？\" },\n                            on: {\n                              confirm: function ($event) {\n                                return _vm.closeSpider(scope.row)\n                              },\n                            },\n                          },\n                          [\n                            _c(\n                              \"el-button\",\n                              {\n                                attrs: {\n                                  slot: \"reference\",\n                                  size: \"mini\",\n                                  plain: \"\",\n                                  type: \"danger\",\n                                },\n                                slot: \"reference\",\n                              },\n                              [_vm._v(\"Close\")]\n                            ),\n                          ],\n                          1\n                        ),\n                      ],\n                      1\n                    ),\n                  ]\n                },\n              },\n            ]),\n          }),\n        ],\n        1\n      ),\n      _c(\"monitor-modal\", {\n        attrs: { \"stats-data\": _vm.statsData, width: 500 },\n        model: {\n          value: _vm.showMonitorModal,\n          callback: function ($$v) {\n            _vm.showMonitorModal = $$v\n          },\n          expression: \"showMonitorModal\",\n        },\n      }),\n    ],\n    1\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Scrapyd/SpiderRunning.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"render\", function() { return render; });\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"staticRenderFns\", function() { return staticRenderFns; });\nvar render = function () {\n  var _vm = this\n  var _h = _vm.$createElement\n  var _c = _vm._self._c || _h\n  return _c(\n    \"div\",\n    [\n      _c(\"running-header\", {\n        attrs: { title: \"运行中的爬虫\", \"checked-data\": _vm.checkedData },\n        on: { reload: _vm.reloadPage },\n      }),\n      _c(\n        \"el-table\",\n        {\n          directives: [\n            {\n              name: \"loading\",\n              rawName: \"v-loading\",\n              value: _vm.loading,\n              expression: \"loading\",\n            },\n          ],\n          staticStyle: { width: \"100%\" },\n          attrs: {\n            data: _vm.tableData,\n            height: \"75vh\",\n            stripe: \"\",\n            fit: \"\",\n            size: \"mini\",\n            \"row-class-name\": _vm.rowClassName,\n          },\n        },\n        [\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"xh\", width: \"70\", label: \"ID\" },\n          }),\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"project\", label: \"项目\" },\n          }),\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"spider\", label: \"爬虫\" },\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              \"show-overflow-tooltip\": \"\",\n              align: \"center\",\n              prop: \"jobId\",\n              label: \"Job ID\",\n            },\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              \"show-overflow-tooltip\": \"\",\n              align: \"center\",\n              prop: \"startParams\",\n              label: \"启动参数\",\n            },\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              align: \"center\",\n              prop: \"startTime\",\n              formatter: _vm.formatStartRun,\n              label: \"开始时间\",\n            },\n          }),\n          _c(\"el-table-column\", {\n            attrs: { align: \"center\", prop: \"memoryUse\", label: \"占用内存\" },\n            scopedSlots: _vm._u([\n              {\n                key: \"default\",\n                fn: function (scope) {\n                  return [\n                    _c(\n                      \"el-tooltip\",\n                      {\n                        staticClass: \"item\",\n                        attrs: {\n                          effect: \"dark\",\n                          content: \"Limit \" + scope.row.memoryUseLimit + \"MB\",\n                          placement: \"top\",\n                        },\n                      },\n                      [\n                        _c(\n                          \"span\",\n                          {\n                            class: {\n                              \"cell-error\":\n                                scope.row.memoryUse > scope.row.memoryUseLimit,\n                              \"cell-ok\":\n                                scope.row.memoryUse < scope.row.memoryUseLimit,\n                              \"cell-unset\":\n                                scope.row.memoryUseLimit === \"Unknown\",\n                            },\n                          },\n                          [\n                            _vm._v(\n                              \" \" + _vm._s(scope.row.memoryUse + \"MB\") + \" \"\n                            ),\n                          ]\n                        ),\n                      ]\n                    ),\n                  ]\n                },\n              },\n            ]),\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              align: \"center\",\n              prop: \"logHourlyErrorRate\",\n              label: \"日志错误率\",\n            },\n            scopedSlots: _vm._u([\n              {\n                key: \"default\",\n                fn: function (scope) {\n                  return [\n                    _c(\n                      \"el-tooltip\",\n                      {\n                        staticClass: \"item\",\n                        attrs: {\n                          effect: \"dark\",\n                          content:\n                            \"Limit \" +\n                            ((scope.row.logHourlyErrorLimit * 100).toFixed(2) +\n                              \"%\"),\n                          placement: \"top\",\n                        },\n                      },\n                      [\n                        _c(\n                          \"span\",\n                          {\n                            class: {\n                              \"cell-error\":\n                                scope.row.logHourlyErrorRate >\n                                scope.row.logHourlyErrorLimit,\n                              \"cell-ok\":\n                                scope.row.logHourlyErrorRate <\n                                scope.row.logHourlyErrorLimit,\n                              \"cell-unset\":\n                                scope.row.logHourlyErrorLimit === \"Unknown\",\n                            },\n                          },\n                          [\n                            _vm._v(\n                              \" \" +\n                                _vm._s(\n                                  (scope.row.logHourlyErrorRate * 100).toFixed(\n                                    2\n                                  ) + \"%\"\n                                ) +\n                                \" \"\n                            ),\n                          ]\n                        ),\n                      ]\n                    ),\n                  ]\n                },\n              },\n            ]),\n          }),\n          _c(\"el-table-column\", {\n            attrs: {\n              width: \"300\",\n              align: \"center\",\n              fixed: \"right\",\n              label: \"操作\",\n            },\n            scopedSlots: _vm._u([\n              {\n                key: \"default\",\n                fn: function (scope) {\n                  return [\n                    _c(\n                      \"el-button-group\",\n                      [\n                        _c(\n                          \"el-button\",\n                          {\n                            attrs: { size: \"mini\", plain: \"\", type: \"success\" },\n                            on: {\n                              click: function ($event) {\n                                return _vm.redirectLog(\n                                  scope.row.project,\n                                  scope.row.spider,\n                                  scope.row.jobId\n                                )\n                              },\n                            },\n                          },\n                          [_vm._v(\"Log\")]\n                        ),\n                        _c(\n                          \"el-button\",\n                          {\n                            attrs: { size: \"mini\", plain: \"\", type: \"success\" },\n                            on: {\n                              click: function ($event) {\n                                return _vm.openMonitorModal(scope.row.jobId)\n                              },\n                            },\n                          },\n                          [_vm._v(\"Stats\")]\n                        ),\n                        _c(\n                          \"el-popconfirm\",\n                          {\n                            attrs: { title: \"确定关闭吗？\" },\n                            on: {\n                              confirm: function ($event) {\n                                return _vm.closeSpider(scope.row)\n                              },\n                            },\n                          },\n                          [\n                            _c(\n                              \"el-button\",\n                              {\n                                attrs: {\n                                  slot: \"reference\",\n                                  size: \"mini\",\n                                  plain: \"\",\n                                  type: \"danger\",\n                                },\n                                slot: \"reference\",\n                              },\n                              [_vm._v(\"Close\")]\n                            ),\n                          ],\n                          1\n                        ),\n                      ],\n                      1\n                    ),\n                  ]\n                },\n              },\n            ]),\n          }),\n        ],\n        1\n      ),\n      _c(\"monitor-modal\", {\n        attrs: { \"stats-data\": _vm.statsData, width: 500 },\n        model: {\n          value: _vm.showMonitorModal,\n          callback: function ($$v) {\n            _vm.showMonitorModal = $$v\n          },\n          expression: \"showMonitorModal\",\n        },\n      }),\n    ],\n    1\n  )\n}\nvar staticRenderFns = []\nrender._withStripped = true\n\n\n\n//# sourceURL=webpack:///./src/components/Scrapyd/SpiderRunning.vue?./node_modules/cache-loader/dist/cjs.js?%7B%22cacheDirectory%22:%22node_modules/.cache/vue-loader%22,%22cacheIdentifier%22:%22023ef482-vue-loader-template%22%7D!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options");
 
                 /***/
             }),
 
         /***/
         "./node_modules/core-js/internals/array-fill.js":
             /*!******************************************************!*\
```

### Comparing `crawler_studio-1.5.5/crawler_studio/static/js/5.js` & `crawler_studio-1.5.6/crawler_studio/static/js/5.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/js/6.js` & `crawler_studio-1.5.6/crawler_studio/static/js/6.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/js/app.js` & `crawler_studio-1.5.6/crawler_studio/static/js/app.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/js/chunk-vendors.js` & `crawler_studio-1.5.6/crawler_studio/static/js/chunk-vendors.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/bootstrap-theme.min.css` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/bootstrap-theme.min.css.map` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/bootstrap-tweaks.css` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/bootstrap-tweaks.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/bootstrap.min.css` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/bootstrap.min.css.map` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/default.css` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/default.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/font-awesome-4.0.3.css` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/font-awesome-4.0.3.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/css/prettify.css` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/css/prettify.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/css/base.css` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/css/base.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/css/highlight.css` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/css/highlight.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/css/jquery.json-view.min.css` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/css/jquery.json-view.min.css`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/img/favicon.ico` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/img/grid.png` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/img/grid.png`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/js/api.js` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/js/api.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/js/highlight.pack.js` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/docs/js/jquery.json-view.min.js` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/docs/js/jquery.json-view.min.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.eot` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.svg` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.ttf` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.woff` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.eot` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.svg` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.ttf` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.woff` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.woff2` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/img/glyphicons-halflings-white.png` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/img/glyphicons-halflings.png` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/img/grid.png` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/img/grid.png`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/ajax-form.js` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/ajax-form.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/bootstrap.min.js` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/coreapi-0.1.1.js` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/coreapi-0.1.1.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/csrf.js` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/csrf.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/default.js` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/default.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/jquery-3.5.1.min.js` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/jquery-3.5.1.min.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/static/rest_framework/js/prettify-min.js` & `crawler_studio-1.5.6/crawler_studio/static/rest_framework/js/prettify-min.js`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/utils/message_transmit.py` & `crawler_studio-1.5.6/crawler_studio/utils/message_transmit.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/utils/time.py` & `crawler_studio-1.5.6/crawler_studio/utils/time.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/utils/variable_rule_trans.py` & `crawler_studio-1.5.6/crawler_studio/utils/variable_rule_trans.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio/utils/verifycation.py` & `crawler_studio-1.5.6/crawler_studio/utils/verifycation.py`

 * *Files identical despite different names*

### Comparing `crawler_studio-1.5.5/crawler_studio.egg-info/PKG-INFO` & `crawler_studio-1.5.6/crawler_studio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: crawler-studio
-Version: 1.5.5
+Version: 1.5.6
 Summary: crawler_studio
 Home-page: UNKNOWN
 Author: liuxianglong
 Author-email: 862187570@qq.com
 Maintainer: liuxianglong
 Maintainer-email: 862187570@qq.com
 License: BSD License
```

### Comparing `crawler_studio-1.5.5/crawler_studio.egg-info/SOURCES.txt` & `crawler_studio-1.5.6/crawler_studio.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 crawler_studio/app_schedule/apps.py
 crawler_studio/app_schedule/models.py
 crawler_studio/app_schedule/ser.py
 crawler_studio/app_schedule/urls.py
 crawler_studio/app_schedule/views.py
 crawler_studio/app_schedule/worker.py
 crawler_studio/app_schedule/migrations/0001_initial.py
+crawler_studio/app_schedule/migrations/0002_monitorrules_start_params.py
 crawler_studio/app_schedule/migrations/__init__.py
 crawler_studio/app_scrapyd/__init__.py
 crawler_studio/app_scrapyd/admin.py
 crawler_studio/app_scrapyd/apps.py
 crawler_studio/app_scrapyd/models.py
 crawler_studio/app_scrapyd/ser.py
 crawler_studio/app_scrapyd/urls.py
```

### Comparing `crawler_studio-1.5.5/setup.py` & `crawler_studio-1.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             for filename in filenames:
                 paths.append(join('..', path, filename))
     return paths
 
 
 setup_args = {
     'name': 'crawler_studio',
-    'version': 'V1.5.5',
+    'version': 'V1.5.6',
     'description': 'crawler_studio',
     'author': 'liuxianglong',
     'author_email': '862187570@qq.com',
     'maintainer': 'liuxianglong',
     'maintainer_email': '862187570@qq.com',
     'license': 'BSD License',
     'packages': find_packages(),
```

