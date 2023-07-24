# Comparing `tmp/wagtailvideos-4.2.1.tar.gz` & `tmp/wagtailvideos-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailvideos-4.2.1.tar", last modified: Wed Jul 19 00:21:19 2023, max compression
+gzip compressed data, was "wagtailvideos-4.2.2.tar", last modified: Mon Jul 24 23:02:41 2023, max compression
```

## Comparing `wagtailvideos-4.2.1.tar` & `wagtailvideos-4.2.2.tar`

### file list

```diff
@@ -1,103 +1,108 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.592485 wagtailvideos-4.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1481 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5529 2023-07-19 00:21:19.592485 wagtailvideos-4.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4746 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-19 00:21:19.592485 wagtailvideos-4.2.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1285 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.579485 wagtailvideos-4.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.580485 wagtailvideos-4.2.1/tests/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.580485 wagtailvideos-4.2.1/tests/app/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    32030 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/migrations/0002_alter_testpage_video_streamfield.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2218 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/test_block.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     6455 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    24716 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/test_admin_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/test_custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1628 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/test_template_tag.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.583485 wagtailvideos-4.2.1/wagtailvideos/
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/edit_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     2106 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/ffmpeg.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     3206 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/jinja2tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.587485 wagtailvideos-4.2.1/wagtailvideos/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1966 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0002_auto_20160321_1610.py
--rw-rw-rw-   0 root         (0) root         (0)     1273 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0003_auto_20160705_1646.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0004_auto_20160706_1153.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0005_videotranscode_error_message.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0006_auto_20160707_1413.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0007_video_duration.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0008_auto_20160728_1523.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0009_videotranscode_quality.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0010_video_ordering.py
--rw-rw-rw-   0 root         (0) root         (0)    28229 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0011_video_tracks.py
--rw-rw-rw-   0 root         (0) root         (0)    26753 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0012_remove_unique_constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     3473 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0013_add_choose_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)    44986 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13468 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/models.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2642 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.575485 wagtailvideos-4.2.1/wagtailvideos/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.575485 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.587485 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/css/
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/css/edit-video.css
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/css/summary-override.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.588485 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/js/
--rw-rw-rw-   0 root         (0) root         (0)     5536 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/js/add-multiple.js
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/js/video-chooser-telepath.js
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/js/video-chooser.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.575485 wagtailvideos-4.2.1/wagtailvideos/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.576485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.588485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/chooser/
--rw-rw-rw-   0 root         (0) root         (0)      926 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/chooser/chooser.html
--rw-rw-rw-   0 root         (0) root         (0)     1988 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/chooser/results.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.588485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/homepage/
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.589485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/multiple/
--rw-rw-rw-   0 root         (0) root         (0)     4414 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/multiple/add.html
--rw-rw-rw-   0 root         (0) root         (0)     1042 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.576485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/permissions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.589485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/permissions/includes/
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/permissions/includes/video_permissions_formset.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.590485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/_file_field.html
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/_file_field_as_li.html
--rw-rw-rw-   0 root         (0) root         (0)     1222 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/add.html
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     6496 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/edit.html
--rw-rw-rw-   0 root         (0) root         (0)     1393 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/index.html
--rw-rw-rw-   0 root         (0) root         (0)     2019 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/results.html
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/usage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.590485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/widgets/
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/widgets/video_chooser.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.591485 wagtailvideos-4.2.1/wagtailvideos/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templatetags/wagtailvideos_tags.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.591485 wagtailvideos-4.2.1/wagtailvideos/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5285 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/views/chooser.py
--rw-rw-rw-   0 root         (0) root         (0)     4921 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/views/multiple.py
--rw-rw-rw-   0 root         (0) root         (0)     7923 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/views/videos.py
--rw-rw-rw-   0 root         (0) root         (0)     4347 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/wagtail_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2085 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.584485 wagtailvideos-4.2.1/wagtailvideos.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5529 2023-07-19 00:21:19.000000 wagtailvideos-4.2.1/wagtailvideos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3225 2023-07-19 00:21:19.000000 wagtailvideos-4.2.1/wagtailvideos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:19.000000 wagtailvideos-4.2.1/wagtailvideos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:19.000000 wagtailvideos-4.2.1/wagtailvideos.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-19 00:21:19.000000 wagtailvideos-4.2.1/wagtailvideos.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-19 00:21:19.000000 wagtailvideos-4.2.1/wagtailvideos.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.672375 wagtailvideos-4.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5529 2023-07-24 23:02:41.672375 wagtailvideos-4.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4746 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-24 23:02:41.673375 wagtailvideos-4.2.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1285 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.657375 wagtailvideos-4.2.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 23:02:33.000000 wagtailvideos-4.2.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.658375 wagtailvideos-4.2.2/tests/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 23:02:33.000000 wagtailvideos-4.2.2/tests/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.659376 wagtailvideos-4.2.2/tests/app/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    32030 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/tests/app/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/tests/app/migrations/0002_alter_testpage_video_streamfield.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 23:02:33.000000 wagtailvideos-4.2.2/tests/app/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/tests/app/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2218 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/tests/app/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/tests/app/test_block.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/tests/app/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     6455 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/tests/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    24716 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/tests/test_admin_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/tests/test_custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/tests/test_template_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.662375 wagtailvideos-4.2.2/wagtailvideos/
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/edit_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2106 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/ffmpeg.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3206 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/jinja2tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.653375 wagtailvideos-4.2.2/wagtailvideos/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.653375 wagtailvideos-4.2.2/wagtailvideos/locale/ru_RU/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.663375 wagtailvideos-4.2.2/wagtailvideos/locale/ru_RU/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9219 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13787 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.667375 wagtailvideos-4.2.2/wagtailvideos/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0002_auto_20160321_1610.py
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0003_auto_20160705_1646.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0004_auto_20160706_1153.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0005_videotranscode_error_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0006_auto_20160707_1413.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0007_video_duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0008_auto_20160728_1523.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0009_videotranscode_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0010_video_ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)    28229 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0011_video_tracks.py
+-rw-rw-rw-   0 root         (0) root         (0)    26753 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0012_remove_unique_constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0013_add_choose_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    44986 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 23:02:33.000000 wagtailvideos-4.2.2/wagtailvideos/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13468 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2642 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.653375 wagtailvideos-4.2.2/wagtailvideos/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.653375 wagtailvideos-4.2.2/wagtailvideos/static/wagtailvideos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.667375 wagtailvideos-4.2.2/wagtailvideos/static/wagtailvideos/css/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/static/wagtailvideos/css/edit-video.css
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/static/wagtailvideos/css/summary-override.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.668375 wagtailvideos-4.2.2/wagtailvideos/static/wagtailvideos/js/
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/static/wagtailvideos/js/add-multiple.js
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/static/wagtailvideos/js/video-chooser-telepath.js
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/static/wagtailvideos/js/video-chooser.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.654375 wagtailvideos-4.2.2/wagtailvideos/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.655376 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.668375 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/chooser/
+-rw-rw-rw-   0 root         (0) root         (0)      926 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/chooser/chooser.html
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/chooser/results.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.668375 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/homepage/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.669375 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/multiple/
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/multiple/add.html
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.654375 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/permissions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.669375 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/permissions/includes/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/permissions/includes/video_permissions_formset.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.670375 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/_file_field.html
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/_file_field_as_li.html
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/add.html
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     6496 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/edit.html
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/results.html
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/usage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.671375 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/widgets/video_chooser.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.671375 wagtailvideos-4.2.2/wagtailvideos/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 23:02:33.000000 wagtailvideos-4.2.2/wagtailvideos/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/templatetags/wagtailvideos_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.672375 wagtailvideos-4.2.2/wagtailvideos/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 23:02:33.000000 wagtailvideos-4.2.2/wagtailvideos/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/views/chooser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4921 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/views/multiple.py
+-rw-rw-rw-   0 root         (0) root         (0)     7923 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/views/videos.py
+-rw-rw-rw-   0 root         (0) root         (0)     4347 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/wagtail_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2023-07-24 23:02:32.000000 wagtailvideos-4.2.2/wagtailvideos/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 23:02:41.663375 wagtailvideos-4.2.2/wagtailvideos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5529 2023-07-24 23:02:41.000000 wagtailvideos-4.2.2/wagtailvideos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3323 2023-07-24 23:02:41.000000 wagtailvideos-4.2.2/wagtailvideos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 23:02:41.000000 wagtailvideos-4.2.2/wagtailvideos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 23:02:41.000000 wagtailvideos-4.2.2/wagtailvideos.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-24 23:02:41.000000 wagtailvideos-4.2.2/wagtailvideos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-24 23:02:41.000000 wagtailvideos-4.2.2/wagtailvideos.egg-info/top_level.txt
```

### Comparing `wagtailvideos-4.2.1/LICENSE` & `wagtailvideos-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/PKG-INFO` & `wagtailvideos-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailvideos
-Version: 4.2.1
+Version: 4.2.2
 Summary: A wagtail module for uploading and displaying videos in various codecs.
 Home-page: https://github.com/neon-jungle/wagtailvideos
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `wagtailvideos-4.2.1/README.rst` & `wagtailvideos-4.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/setup.py` & `wagtailvideos-4.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.rst", "r") as f:
     readme = f.read()
 
 from setuptools import find_packages, setup  # noqa: E4
 
 setup(
     name="wagtailvideos",
-    version="4.2.1",
+    version="4.2.2",
     description="A wagtail module for uploading and displaying videos in various codecs.",
     long_description=readme,
     author="Neon Jungle",
     author_email="developers@neonjungle.studio",
     url="https://github.com/neon-jungle/wagtailvideos",
     install_requires=[
         "wagtail>=4.2",
```

### Comparing `wagtailvideos-4.2.1/tests/app/migrations/0001_initial.py` & `wagtailvideos-4.2.2/tests/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/tests/app/models.py` & `wagtailvideos-4.2.2/tests/app/models.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/tests/app/settings.py` & `wagtailvideos-4.2.2/tests/app/settings.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/tests/app/test_block.py` & `wagtailvideos-4.2.2/tests/app/test_block.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/tests/app/urls.py` & `wagtailvideos-4.2.2/tests/app/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/tests/storage.py` & `wagtailvideos-4.2.2/tests/storage.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/tests/test_admin_views.py` & `wagtailvideos-4.2.2/tests/test_admin_views.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/tests/test_custom_model.py` & `wagtailvideos-4.2.2/tests/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/tests/test_template_tag.py` & `wagtailvideos-4.2.2/tests/test_template_tag.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/__init__.py` & `wagtailvideos-4.2.2/wagtailvideos/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/apps.py` & `wagtailvideos-4.2.2/wagtailvideos/apps.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/blocks.py` & `wagtailvideos-4.2.2/wagtailvideos/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/ffmpeg.py` & `wagtailvideos-4.2.2/wagtailvideos/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/fields.py` & `wagtailvideos-4.2.2/wagtailvideos/fields.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/forms.py` & `wagtailvideos-4.2.2/wagtailvideos/forms.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/jinja2tags.py` & `wagtailvideos-4.2.2/wagtailvideos/jinja2tags.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/migrations/0001_initial.py` & `wagtailvideos-4.2.2/wagtailvideos/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/migrations/0002_auto_20160321_1610.py` & `wagtailvideos-4.2.2/wagtailvideos/migrations/0002_auto_20160321_1610.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/migrations/0003_auto_20160705_1646.py` & `wagtailvideos-4.2.2/wagtailvideos/migrations/0003_auto_20160705_1646.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/migrations/0004_auto_20160706_1153.py` & `wagtailvideos-4.2.2/wagtailvideos/migrations/0004_auto_20160706_1153.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/migrations/0006_auto_20160707_1413.py` & `wagtailvideos-4.2.2/wagtailvideos/migrations/0006_auto_20160707_1413.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/migrations/0009_videotranscode_quality.py` & `wagtailvideos-4.2.2/wagtailvideos/migrations/0009_videotranscode_quality.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/migrations/0011_video_tracks.py` & `wagtailvideos-4.2.2/wagtailvideos/migrations/0011_video_tracks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/migrations/0012_remove_unique_constraint.py` & `wagtailvideos-4.2.2/wagtailvideos/migrations/0012_remove_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/migrations/0013_add_choose_permissions.py` & `wagtailvideos-4.2.2/wagtailvideos/migrations/0013_add_choose_permissions.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py` & `wagtailvideos-4.2.2/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/models.py` & `wagtailvideos-4.2.2/wagtailvideos/models.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/signals.py` & `wagtailvideos-4.2.2/wagtailvideos/signals.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/js/add-multiple.js` & `wagtailvideos-4.2.2/wagtailvideos/static/wagtailvideos/js/add-multiple.js`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/chooser/chooser.html` & `wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/chooser/chooser.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/chooser/results.html` & `wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/chooser/results.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/multiple/add.html` & `wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/multiple/add.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html` & `wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/add.html` & `wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/add.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html` & `wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/edit.html` & `wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/edit.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/index.html` & `wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/index.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/results.html` & `wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/results.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/usage.html` & `wagtailvideos-4.2.2/wagtailvideos/templates/wagtailvideos/videos/usage.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/templatetags/wagtailvideos_tags.py` & `wagtailvideos-4.2.2/wagtailvideos/templatetags/wagtailvideos_tags.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/urls.py` & `wagtailvideos-4.2.2/wagtailvideos/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/views/chooser.py` & `wagtailvideos-4.2.2/wagtailvideos/views/chooser.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/views/multiple.py` & `wagtailvideos-4.2.2/wagtailvideos/views/multiple.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/views/videos.py` & `wagtailvideos-4.2.2/wagtailvideos/views/videos.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/wagtail_hooks.py` & `wagtailvideos-4.2.2/wagtailvideos/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos/widgets.py` & `wagtailvideos-4.2.2/wagtailvideos/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.1/wagtailvideos.egg-info/PKG-INFO` & `wagtailvideos-4.2.2/wagtailvideos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailvideos
-Version: 4.2.1
+Version: 4.2.2
 Summary: A wagtail module for uploading and displaying videos in various codecs.
 Home-page: https://github.com/neon-jungle/wagtailvideos
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `wagtailvideos-4.2.1/wagtailvideos.egg-info/SOURCES.txt` & `wagtailvideos-4.2.2/wagtailvideos.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 wagtailvideos/widgets.py
 wagtailvideos.egg-info/PKG-INFO
 wagtailvideos.egg-info/SOURCES.txt
 wagtailvideos.egg-info/dependency_links.txt
 wagtailvideos.egg-info/not-zip-safe
 wagtailvideos.egg-info/requires.txt
 wagtailvideos.egg-info/top_level.txt
+wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo
+wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po
 wagtailvideos/migrations/0001_initial.py
 wagtailvideos/migrations/0002_auto_20160321_1610.py
 wagtailvideos/migrations/0003_auto_20160705_1646.py
 wagtailvideos/migrations/0004_auto_20160706_1153.py
 wagtailvideos/migrations/0005_videotranscode_error_message.py
 wagtailvideos/migrations/0006_auto_20160707_1413.py
 wagtailvideos/migrations/0007_video_duration.py
```

