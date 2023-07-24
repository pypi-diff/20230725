# Comparing `tmp/deriva-qt-1.6.1.tar.gz` & `tmp/deriva-qt-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deriva-qt-1.6.1.tar", last modified: Thu Dec  1 20:49:15 2022, max compression
+gzip compressed data, was "deriva-qt-1.6.3.tar", last modified: Mon Jul 24 22:37:14 2023, max compression
```

## Comparing `deriva-qt-1.6.1.tar` & `deriva-qt-1.6.3.tar`

### file list

```diff
@@ -1,83 +1,77 @@
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.521926 deriva-qt-1.6.1/
--rw-rw-rw-   0        0        0     1065 2018-10-02 02:51:38.000000 deriva-qt-1.6.1/.gitignore
--rw-rw-rw-   0        0        0    35141 2017-04-06 17:32:39.000000 deriva-qt-1.6.1/LICENSE
--rw-rw-rw-   0        0        0     1274 2022-12-01 20:49:15.521926 deriva-qt-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     1222 2021-03-04 20:45:13.000000 deriva-qt-1.6.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.066989 deriva-qt-1.6.1/deriva/
--rw-rw-rw-   0        0        0       65 2019-03-14 18:34:35.000000 deriva-qt-1.6.1/deriva/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.082610 deriva-qt-1.6.1/deriva/qt/
--rw-rw-rw-   0        0        0     1086 2022-12-01 20:37:39.000000 deriva-qt-1.6.1/deriva/qt/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.098282 deriva-qt-1.6.1/deriva/qt/auth_agent/
--rw-rw-rw-   0        0        0        0 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/__init__.py
--rw-rw-rw-   0        0        0     1645 2021-04-15 23:35:15.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/__main__.py
--rw-rw-rw-   0        0        0     1406 2017-12-09 01:11:32.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/deriva-auth-agent-mac.spec
--rw-rw-rw-   0        0        0      834 2019-01-18 19:36:03.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/deriva-auth-agent-win.spec
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.113908 deriva-qt-1.6.1/deriva/qt/auth_agent/resources/
--rw-rw-rw-   0        0        0        0 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.113908 deriva-qt-1.6.1/deriva/qt/auth_agent/resources/images/
--rw-rw-rw-   0        0        0    44796 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/resources/images/keys.icns
--rw-rw-rw-   0        0        0    99678 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/resources/images/keys.ico
--rw-rw-rw-   0        0        0    12455 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/resources/images/keys.png
--rw-rw-rw-   0        0        0    52818 2019-04-09 23:05:16.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/resources/resources.py
--rw-rw-rw-   0        0        0      139 2019-04-09 23:05:16.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/resources/resources.qrc
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.146859 deriva-qt-1.6.1/deriva/qt/auth_agent/ui/
--rw-rw-rw-   0        0        0        0 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/ui/__init__.py
--rw-rw-rw-   0        0        0    14682 2021-04-16 01:30:53.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/ui/auth_widget.py
--rw-rw-rw-   0        0        0    19548 2021-04-16 00:54:51.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/ui/auth_window.py
--rw-rw-rw-   0        0        0     4288 2021-06-22 20:00:26.000000 deriva-qt-1.6.1/deriva/qt/auth_agent/ui/embedded_auth_window.py
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.162506 deriva-qt-1.6.1/deriva/qt/common/
--rw-rw-rw-   0        0        0        0 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/common/__init__.py
--rw-rw-rw-   0        0        0     1957 2020-05-22 23:47:14.000000 deriva-qt-1.6.1/deriva/qt/common/async_task.py
--rw-rw-rw-   0        0        0     6916 2018-05-25 04:56:43.000000 deriva-qt-1.6.1/deriva/qt/common/json_editor.py
--rw-rw-rw-   0        0        0      667 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/common/log_widget.py
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.178135 deriva-qt-1.6.1/deriva/qt/common/resources/
--rw-rw-rw-   0        0        0        0 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/common/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.209380 deriva-qt-1.6.1/deriva/qt/common/resources/images/
--rw-rw-rw-   0        0        0    41280 2019-02-12 03:01:58.000000 deriva-qt-1.6.1/deriva/qt/common/resources/images/deriva-star.icns
--rw-rw-rw-   0        0        0    99678 2019-02-12 03:01:45.000000 deriva-qt-1.6.1/deriva/qt/common/resources/images/deriva-star.ico
--rw-rw-rw-   0        0        0     3515 2019-02-12 03:00:59.000000 deriva-qt-1.6.1/deriva/qt/common/resources/images/deriva-star.png
--rw-rw-rw-   0        0        0     1064 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/common/table_widget.py
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.240631 deriva-qt-1.6.1/deriva/qt/upload_gui/
--rw-rw-rw-   0        0        0        0 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/__init__.py
--rw-rw-rw-   0        0        0      335 2021-03-04 02:19:05.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/__main__.py
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.256300 deriva-qt-1.6.1/deriva/qt/upload_gui/conf/
--rw-rw-rw-   0        0        0      404 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/conf/config.json
--rw-rw-rw-   0        0        0     1478 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/deriva-upload-mac.spec
--rw-rw-rw-   0        0        0      889 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/deriva-upload-win.spec
--rw-rw-rw-   0        0        0     2996 2021-03-04 02:34:57.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/deriva_upload_gui.py
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.256300 deriva-qt-1.6.1/deriva/qt/upload_gui/impl/
--rw-rw-rw-   0        0        0        0 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/impl/__init__.py
--rw-rw-rw-   0        0        0     3335 2020-05-27 02:08:34.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/impl/upload_tasks.py
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.287520 deriva-qt-1.6.1/deriva/qt/upload_gui/resources/
--rw-rw-rw-   0        0        0        0 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.318799 deriva-qt-1.6.1/deriva/qt/upload_gui/resources/images/
--rw-rw-rw-   0        0        0    67702 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/resources/images/upload.icns
--rw-rw-rw-   0        0        0   370070 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/resources/images/upload.ico
--rw-rw-rw-   0        0        0     8655 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/resources/images/upload.png
--rw-rw-rw-   0        0        0    36618 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/resources/resources.py
--rw-rw-rw-   0        0        0      143 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/resources/resources.qrc
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.350035 deriva-qt-1.6.1/deriva/qt/upload_gui/ui/
--rw-rw-rw-   0        0        0        0 2017-10-19 23:08:23.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/ui/__init__.py
--rw-rw-rw-   0        0        0    18923 2021-03-24 03:15:33.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/ui/options_window.py
--rw-rw-rw-   0        0        0    28822 2021-06-22 20:01:01.000000 deriva-qt-1.6.1/deriva/qt/upload_gui/ui/upload_window.py
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.381255 deriva-qt-1.6.1/deriva_qt.egg-info/
--rw-rw-rw-   0        0        0     1274 2022-12-01 20:49:14.000000 deriva-qt-1.6.1/deriva_qt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2216 2022-12-01 20:49:14.000000 deriva-qt-1.6.1/deriva_qt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-01 20:49:14.000000 deriva-qt-1.6.1/deriva_qt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2022-12-01 20:49:14.000000 deriva-qt-1.6.1/deriva_qt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2022-12-01 20:49:14.000000 deriva-qt-1.6.1/deriva_qt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-12-01 20:49:14.000000 deriva-qt-1.6.1/deriva_qt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.381255 deriva-qt-1.6.1/docs/
--rw-rw-rw-   0        0        0       63 2019-05-28 22:50:32.000000 deriva-qt-1.6.1/docs/auth.md
-drwxrwxrwx   0        0        0        0 2022-12-01 20:49:15.490627 deriva-qt-1.6.1/docs/images/
--rw-rw-rw-   0        0        0    19303 2018-10-02 02:51:38.000000 deriva-qt-1.6.1/docs/images/deriva-auth-empty.png
--rw-rw-rw-   0        0        0    77958 2018-10-02 02:51:38.000000 deriva-qt-1.6.1/docs/images/deriva-auth-globus.png
--rw-rw-rw-   0        0        0   158546 2018-10-02 02:51:38.000000 deriva-qt-1.6.1/docs/images/pending.png
--rw-rw-rw-   0        0        0    52848 2018-10-02 02:51:38.000000 deriva-qt-1.6.1/docs/images/server-config.blank.png
--rw-rw-rw-   0        0        0    21025 2018-10-02 02:51:38.000000 deriva-qt-1.6.1/docs/images/server-config.gudmap.png
--rw-rw-rw-   0        0        0    20171 2018-10-02 02:51:38.000000 deriva-qt-1.6.1/docs/images/show-details.png
--rw-rw-rw-   0        0        0    33347 2018-10-02 02:51:38.000000 deriva-qt-1.6.1/docs/images/update-config.png
--rw-rw-rw-   0        0        0      164 2019-05-28 22:55:13.000000 deriva-qt-1.6.1/docs/index.rst
--rw-rw-rw-   0        0        0     5313 2018-10-02 02:51:38.000000 deriva-qt-1.6.1/docs/uploading.md
--rw-rw-rw-   0        0        0      110 2022-12-01 20:49:15.521926 deriva-qt-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     2179 2021-12-03 00:35:54.000000 deriva-qt-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:14.128697 deriva-qt-1.6.3/
+-rw-rw-rw-   0        0        0     1157 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/.gitignore
+-rw-rw-rw-   0        0        0    35815 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0     1267 2023-07-24 22:37:14.129697 deriva-qt-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1254 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:13.774847 deriva-qt-1.6.3/deriva/
+-rw-rw-rw-   0        0        0       66 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:13.776849 deriva-qt-1.6.3/deriva/qt/
+-rw-rw-rw-   0        0        0     1086 2023-05-03 03:42:36.000000 deriva-qt-1.6.3/deriva/qt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:13.806849 deriva-qt-1.6.3/deriva/qt/auth_agent/
+-rw-rw-rw-   0        0        0        0 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/__init__.py
+-rw-rw-rw-   0        0        0     1688 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/__main__.py
+-rw-rw-rw-   0        0        0     1454 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/deriva-auth-agent-mac.spec
+-rw-rw-rw-   0        0        0      866 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/deriva-auth-agent-win.spec
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:13.825847 deriva-qt-1.6.3/deriva/qt/auth_agent/resources/
+-rw-rw-rw-   0        0        0        0 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:13.841848 deriva-qt-1.6.3/deriva/qt/auth_agent/resources/images/
+-rw-rw-rw-   0        0        0    44796 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/resources/images/keys.icns
+-rw-rw-rw-   0        0        0    99678 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/resources/images/keys.ico
+-rw-rw-rw-   0        0        0    12455 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/resources/images/keys.png
+-rw-rw-rw-   0        0        0    53653 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/resources/resources.py
+-rw-rw-rw-   0        0        0      144 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/resources/resources.qrc
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:13.922891 deriva-qt-1.6.3/deriva/qt/auth_agent/ui/
+-rw-rw-rw-   0        0        0        0 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/ui/__init__.py
+-rw-rw-rw-   0        0        0    16468 2023-07-21 02:49:19.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/ui/auth_widget.py
+-rw-rw-rw-   0        0        0    20012 2023-07-19 19:29:43.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/ui/auth_window.py
+-rw-rw-rw-   0        0        0     4431 2023-07-20 22:24:02.000000 deriva-qt-1.6.3/deriva/qt/auth_agent/ui/embedded_auth_window.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:13.958599 deriva-qt-1.6.3/deriva/qt/common/
+-rw-rw-rw-   0        0        0        0 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/common/__init__.py
+-rw-rw-rw-   0        0        0     2034 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/common/async_task.py
+-rw-rw-rw-   0        0        0     7123 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/common/json_editor.py
+-rw-rw-rw-   0        0        0      692 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/common/log_widget.py
+-rw-rw-rw-   0        0        0     1099 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/common/table_widget.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:13.996592 deriva-qt-1.6.3/deriva/qt/upload_gui/
+-rw-rw-rw-   0        0        0        0 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/__init__.py
+-rw-rw-rw-   0        0        0      350 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:14.003592 deriva-qt-1.6.3/deriva/qt/upload_gui/conf/
+-rw-rw-rw-   0        0        0      415 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/conf/config.json
+-rw-rw-rw-   0        0        0     1527 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/deriva-upload-mac.spec
+-rw-rw-rw-   0        0        0      922 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/deriva-upload-win.spec
+-rw-rw-rw-   0        0        0     3073 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/deriva_upload_gui.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:14.014592 deriva-qt-1.6.3/deriva/qt/upload_gui/impl/
+-rw-rw-rw-   0        0        0        0 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/impl/__init__.py
+-rw-rw-rw-   0        0        0     3429 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/impl/upload_tasks.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:14.031592 deriva-qt-1.6.3/deriva/qt/upload_gui/resources/
+-rw-rw-rw-   0        0        0        0 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:14.048592 deriva-qt-1.6.3/deriva/qt/upload_gui/resources/images/
+-rw-rw-rw-   0        0        0    67702 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/resources/images/upload.icns
+-rw-rw-rw-   0        0        0   370070 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/resources/images/upload.ico
+-rw-rw-rw-   0        0        0     8655 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/resources/images/upload.png
+-rw-rw-rw-   0        0        0    37198 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/resources/resources.py
+-rw-rw-rw-   0        0        0      148 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/resources/resources.qrc
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:14.071592 deriva-qt-1.6.3/deriva/qt/upload_gui/ui/
+-rw-rw-rw-   0        0        0        0 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/ui/__init__.py
+-rw-rw-rw-   0        0        0    19334 2023-03-04 00:59:39.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/ui/options_window.py
+-rw-rw-rw-   0        0        0    29650 2023-07-21 02:57:39.000000 deriva-qt-1.6.3/deriva/qt/upload_gui/ui/upload_window.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:14.094696 deriva-qt-1.6.3/deriva_qt.egg-info/
+-rw-rw-rw-   0        0        0     1267 2023-07-24 22:37:13.000000 deriva-qt-1.6.3/deriva_qt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2026 2023-07-24 22:37:13.000000 deriva-qt-1.6.3/deriva_qt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 22:37:13.000000 deriva-qt-1.6.3/deriva_qt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-07-24 22:37:13.000000 deriva-qt-1.6.3/deriva_qt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-07-24 22:37:13.000000 deriva-qt-1.6.3/deriva_qt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-24 22:37:13.000000 deriva-qt-1.6.3/deriva_qt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:14.115697 deriva-qt-1.6.3/docs/
+-rw-rw-rw-   0        0        0       65 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/docs/auth.md
+drwxrwxrwx   0        0        0        0 2023-07-24 22:37:14.127697 deriva-qt-1.6.3/docs/images/
+-rw-rw-rw-   0        0        0    19303 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/docs/images/deriva-auth-empty.png
+-rw-rw-rw-   0        0        0    77958 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/docs/images/deriva-auth-globus.png
+-rw-rw-rw-   0        0        0   158546 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/docs/images/pending.png
+-rw-rw-rw-   0        0        0    52848 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/docs/images/server-config.blank.png
+-rw-rw-rw-   0        0        0    21025 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/docs/images/server-config.gudmap.png
+-rw-rw-rw-   0        0        0    20171 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/docs/images/show-details.png
+-rw-rw-rw-   0        0        0    33347 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/docs/images/update-config.png
+-rw-rw-rw-   0        0        0      172 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/docs/index.rst
+-rw-rw-rw-   0        0        0     5091 2023-02-03 01:11:51.000000 deriva-qt-1.6.3/docs/uploading.md
+-rw-rw-rw-   0        0        0      110 2023-07-24 22:37:14.131697 deriva-qt-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     2250 2022-01-18 19:12:41.000000 deriva-qt-1.6.3/setup.py
```

### Comparing `deriva-qt-1.6.1/LICENSE` & `deriva-qt-1.6.3/LICENSE`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    {one line to give the program's name and a brief idea of what it does.}
-    Copyright (C) {year}  {name of author}
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    {project}  Copyright (C) {year}  {fullname}
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    {one line to give the program's name and a brief idea of what it does.}
+    Copyright (C) {year}  {name of author}
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    {project}  Copyright (C) {year}  {fullname}
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

### Comparing `deriva-qt-1.6.1/PKG-INFO` & `deriva-qt-1.6.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: deriva-qt
-Version: 1.6.1
+Version: 1.6.3
 Summary: Graphical User Interface tools for DERIVA built on PyQt5
 Home-page: https://github.com/informatics-isi-edu/deriva-qt
 Author: USC Information Sciences Institute, Informatics Systems Research Division
 Author-email: isrd-support@isi.edu
 Maintainer: USC Information Sciences Institute, Informatics Systems Research Division
 Maintainer-email: isrd-support@isi.edu
 License: GNU GPL 3.0
-Description: For further information, visit the project [homepage](https://github.com/informatics-isi-edu/deriva-qt).
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
@@ -21,7 +19,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: PyQt5
 Provides-Extra: PyQtWebEngine
+License-File: LICENSE
+
+For further information, visit the project [homepage](https://github.com/informatics-isi-edu/deriva-qt).
```

### Comparing `deriva-qt-1.6.1/README.md` & `deriva-qt-1.6.3/README.md`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# deriva-qt
-[![PyPi Version](https://img.shields.io/pypi/v/deriva-qt.svg)](https://pypi.python.org/pypi/deriva-qt)
-[![PyPi Downloads](https://img.shields.io/pypi/dm/deriva-qt.svg)](https://pypistats.org/packages/deriva-qt)
-[![PyPi Wheel](https://img.shields.io/pypi/wheel/deriva-qt.svg)](https://pypi.python.org/pypi/deriva-qt)
-[![Python Versions](https://img.shields.io/pypi/pyversions/deriva-qt.svg)](https://pypi.python.org/pypi/deriva-qt)
-[![License](https://img.shields.io/pypi/l/deriva-qt.svg)](https://www.gnu.org/licenses/gpl-3.0)
-
-Graphical User Interface tools for DERIVA using PyQt5
-
-* Authentication Agent
-* File Uploader
-
-## Installation
-### Windows / MacOS
-Windows and MacOS users can download prebuilt bundles which include all
-dependencies [here](https://github.com/informatics-isi-edu/deriva-client-bundle/releases).
-Download the appropriate file for your OS.
-
-## Install from source
-
-See the source installation instructions [here](https://github.com/informatics-isi-edu/deriva-client-bundle/blob/master/README.md).
-
-
-## User Instructions 
-
-TBD
-
-
-## Additional information
-Links:
-* [Build status](http://buildbot.isrd.isi.edu/)
-* [Downloads](http://buildbot.isrd.isi.edu/~buildbot/deriva-client-bundle/)
+# deriva-qt
+[![PyPi Version](https://img.shields.io/pypi/v/deriva-qt.svg)](https://pypi.python.org/pypi/deriva-qt)
+[![PyPi Downloads](https://img.shields.io/pypi/dm/deriva-qt.svg)](https://pypistats.org/packages/deriva-qt)
+[![PyPi Wheel](https://img.shields.io/pypi/wheel/deriva-qt.svg)](https://pypi.python.org/pypi/deriva-qt)
+[![Python Versions](https://img.shields.io/pypi/pyversions/deriva-qt.svg)](https://pypi.python.org/pypi/deriva-qt)
+[![License](https://img.shields.io/pypi/l/deriva-qt.svg)](https://www.gnu.org/licenses/gpl-3.0)
+
+Graphical User Interface tools for DERIVA using PyQt5
+
+* Authentication Agent
+* File Uploader
+
+## Installation
+### Windows / MacOS
+Windows and MacOS users can download prebuilt bundles which include all
+dependencies [here](https://github.com/informatics-isi-edu/deriva-client-bundle/releases).
+Download the appropriate file for your OS.
+
+## Install from source
+
+See the source installation instructions [here](https://github.com/informatics-isi-edu/deriva-client-bundle/blob/master/README.md).
+
+
+## User Instructions 
+
+TBD
+
+
+## Additional information
+Links:
+* [Build status](http://buildbot.isrd.isi.edu/)
+* [Downloads](http://buildbot.isrd.isi.edu/~buildbot/deriva-client-bundle/)
```

### Comparing `deriva-qt-1.6.1/deriva/qt/__init__.py` & `deriva-qt-1.6.3/deriva/qt/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.6.1"
+__version__ = "1.6.3"
 
 from deriva.qt.common.async_task import async_execute, Task
 from deriva.qt.common.log_widget import QPlainTextEditLogger
 from deriva.qt.common.table_widget import TableWidget
 from deriva.qt.common.json_editor import JSONEditor
 
 from deriva.qt.auth_agent.ui.auth_window import AuthWindow
```

### Comparing `deriva-qt-1.6.1/deriva/qt/auth_agent/__main__.py` & `deriva-qt-1.6.3/deriva/qt/auth_agent/__main__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import sys
-import logging
-import traceback
-from PyQt5 import QtCore
-from PyQt5.QtWidgets import QApplication, QStyleFactory, QMessageBox
-from deriva.core import read_config, format_exception, BaseCLI
-from deriva.qt import AuthWindow, __version__ as VERSION
-
-
-def excepthook(etype, value, tb):
-    traceback.print_tb(tb)
-    print(format_exception(value), file=sys.stderr)
-    msg = QMessageBox()
-    msg.setText(str(value))
-    msg.setStandardButtons(QMessageBox.Close)
-    msg.setWindowTitle("Unhandled Exception: %s" % etype.__name__)
-    msg.setIcon(QMessageBox.Critical)
-    msg.setDetailedText('\n'.join(traceback.format_exception(etype, value, tb)))
-    msg.exec_()
-
-
-def main():
-    sys.excepthook = excepthook
-    cli = BaseCLI("DERIVA Authentication Agent",
-                  "For more information see: https://github.com/informatics-isi-edu/deriva-qt", VERSION)
-    cli.parser.add_argument(
-        "--cookie-persistence", action="store_true",
-        help="Enable cookie and local storage persistence for QtWebEngine.")
-    args = cli.parse_cli()
-    QApplication.setDesktopSettingsAware(False)
-    QApplication.setStyle(QStyleFactory.create("Fusion"))
-    app = QApplication(sys.argv)
-    app.setAttribute(QtCore.Qt.AA_UseHighDpiPixmaps)
-    config = read_config(args.config_file, create_default=False) if args.config_file else None
-    log_level = logging.DEBUG if args.debug else logging.INFO
-    auth_window = AuthWindow(config, args.credential_file,
-                             cookie_persistence=args.cookie_persistence, log_level=log_level)
-    auth_window.show()
-    return app.exec()
-
-
-if __name__ == '__main__':
-    main()
+import sys
+import logging
+import traceback
+from PyQt5 import QtCore
+from PyQt5.QtWidgets import QApplication, QStyleFactory, QMessageBox
+from deriva.core import read_config, format_exception, BaseCLI
+from deriva.qt import AuthWindow, __version__ as VERSION
+
+
+def excepthook(etype, value, tb):
+    traceback.print_tb(tb)
+    print(format_exception(value), file=sys.stderr)
+    msg = QMessageBox()
+    msg.setText(str(value))
+    msg.setStandardButtons(QMessageBox.Close)
+    msg.setWindowTitle("Unhandled Exception: %s" % etype.__name__)
+    msg.setIcon(QMessageBox.Critical)
+    msg.setDetailedText('\n'.join(traceback.format_exception(etype, value, tb)))
+    msg.exec_()
+
+
+def main():
+    sys.excepthook = excepthook
+    cli = BaseCLI("DERIVA Authentication Agent",
+                  "For more information see: https://github.com/informatics-isi-edu/deriva-qt", VERSION)
+    cli.parser.add_argument(
+        "--cookie-persistence", action="store_true",
+        help="Enable cookie and local storage persistence for QtWebEngine.")
+    args = cli.parse_cli()
+    QApplication.setDesktopSettingsAware(False)
+    QApplication.setStyle(QStyleFactory.create("Fusion"))
+    app = QApplication(sys.argv)
+    app.setAttribute(QtCore.Qt.AA_UseHighDpiPixmaps)
+    config = read_config(args.config_file, create_default=False) if args.config_file else None
+    log_level = logging.DEBUG if args.debug else logging.INFO
+    auth_window = AuthWindow(config, args.credential_file,
+                             cookie_persistence=args.cookie_persistence, log_level=log_level)
+    auth_window.show()
+    return app.exec()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `deriva-qt-1.6.1/deriva/qt/auth_agent/deriva-auth-agent-win.spec` & `deriva-qt-1.6.3/deriva/qt/auth_agent/deriva-auth-agent-win.spec`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# -*- mode: python -*-
-
-block_cipher = None
-
-from os import environ as env
-from deriva.qt import __version__
-
-a = Analysis(['./__main__.py'],
-             pathex=[],
-             binaries=[],
-             datas=[],
-             hiddenimports=[],
-             hookspath=[],
-             runtime_hooks=[],
-             excludes=['numpy','scipy','pandas'],
-             win_no_prefer_redirects=False,
-             win_private_assemblies=False,
-             cipher=block_cipher)
-
-pyz = PYZ(a.pure, a.zipped_data, cipher=block_cipher)
-
-exe = EXE(pyz,
-          a.scripts,
-          a.binaries,
-          a.zipfiles,
-          a.datas,
-          name='DERIVA-Auth',
-          strip=False,
-          upx=False,
-          debug=env.get("DEBUG", False),
-          console=env.get("DEBUG", False),
-          icon='./resources/images/keys.ico')
+# -*- mode: python -*-
+
+block_cipher = None
+
+from os import environ as env
+from deriva.qt import __version__
+
+a = Analysis(['./__main__.py'],
+             pathex=[],
+             binaries=[],
+             datas=[],
+             hiddenimports=[],
+             hookspath=[],
+             runtime_hooks=[],
+             excludes=['numpy','scipy','pandas'],
+             win_no_prefer_redirects=False,
+             win_private_assemblies=False,
+             cipher=block_cipher)
+
+pyz = PYZ(a.pure, a.zipped_data, cipher=block_cipher)
+
+exe = EXE(pyz,
+          a.scripts,
+          a.binaries,
+          a.zipfiles,
+          a.datas,
+          name='DERIVA-Auth',
+          strip=False,
+          upx=False,
+          debug=env.get("DEBUG", False),
+          console=env.get("DEBUG", False),
+          icon='./resources/images/keys.ico')
```

### Comparing `deriva-qt-1.6.1/deriva/qt/auth_agent/resources/images/keys.icns` & `deriva-qt-1.6.3/deriva/qt/auth_agent/resources/images/keys.icns`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/deriva/qt/auth_agent/resources/images/keys.ico` & `deriva-qt-1.6.3/deriva/qt/auth_agent/resources/images/keys.ico`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/deriva/qt/auth_agent/resources/images/keys.png` & `deriva-qt-1.6.3/deriva/qt/auth_agent/resources/images/keys.png`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/deriva/qt/auth_agent/resources/resources.py` & `deriva-qt-1.6.3/deriva/qt/auth_agent/resources/resources.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,835 +1,835 @@
-# -*- coding: utf-8 -*-
-
-# Resource object code
-#
-# Created by: The Resource Compiler for PyQt5 (Qt v5.9.1)
-#
-# WARNING! All changes made in this file will be lost!
-
-from PyQt5 import QtCore
-
-qt_resource_data = b"\
-\x00\x00\x30\xa7\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x80\x00\x00\x00\x80\x08\x06\x00\x00\x00\xc3\x3e\x61\xcb\
-\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\x00\x48\x00\x00\x00\x48\
-\x00\x46\xc9\x6b\x3e\x00\x00\x00\x09\x76\x70\x41\x67\x00\x00\x00\
-\x80\x00\x00\x00\x80\x00\x30\xe1\x31\x9a\x00\x00\x00\x06\x62\x4b\
-\x47\x44\x00\xff\x00\xff\x00\xff\xa0\xbd\xa7\x93\x00\x00\x2f\xd0\
-\x49\x44\x41\x54\x78\xda\xed\x9d\x07\x78\x14\x55\xf7\xc6\x43\x97\
-\xa2\x02\x36\xc4\xde\xb1\xa0\x9f\x80\x8a\xa2\xc2\xa7\x62\xfd\x2c\
-\x90\xd0\x9b\x88\x58\x10\xe9\x2d\xf4\xd0\xab\xd4\x14\x12\x5a\xe8\
-\x1d\x02\xa4\xf7\xde\x7b\xef\xbd\xf7\x6c\x49\x76\x93\xec\xfb\x3f\
-\x77\x66\x77\x76\xb6\x04\x1b\x68\xf8\xb3\xf3\x3c\xef\x83\x84\x98\
-\xdd\xcc\xef\x3d\xe7\x9e\x73\xef\x9d\xbb\x66\x66\xa6\xeb\x96\x5d\
-\xa1\x56\x77\x3f\x12\xb6\xe1\xde\x91\xe1\x1b\xfb\xcc\x0d\x58\x62\
-\xb6\x9f\x74\x82\x74\x8d\xe4\x49\xba\x4c\x72\x0c\x5a\xd1\x75\x6d\
-\xc8\x9a\x1e\xe6\xc1\x2b\xbb\x3d\x6e\xba\x63\xb7\xf9\x15\xb9\xbd\
-\x5f\x5f\x82\x3d\x89\xc0\x1e\x22\xe5\x90\xf0\x27\xa4\x22\x45\x06\
-\x2d\xef\xbc\x30\xd4\xaa\xd7\xdd\xa6\xbb\x79\xbb\x40\xdf\xd1\xaf\
-\x7b\xf8\xa6\xbe\xe3\x08\x9e\x13\x49\xf1\x27\xa1\xb7\xa5\xca\xa0\
-\xe5\x5d\x16\x84\x59\xdd\xdd\xd1\x74\x87\xdb\xe9\x15\xfd\xdb\x23\
-\xfd\x29\x75\x6f\x24\x58\x55\xc6\x20\x52\x14\x23\xe9\xe0\xcb\xc8\
-\xba\x3c\x02\xc5\xfe\x16\x28\x8f\x9c\x86\xaa\x84\x1f\x50\x9d\xf8\
-\x13\xf7\xdf\xc5\x81\x63\x91\x75\x69\x38\xe2\xad\x9f\x06\x0d\x03\
-\x6d\x19\xc1\x2b\x62\x43\xef\x7e\xa6\xbb\xdd\x8e\x2e\x8a\xf6\xa7\
-\x08\xcc\x51\xfd\x68\xa7\xd4\x4d\xc0\x5f\x42\x49\xd0\x38\xc8\x4b\
-\x57\x03\x8a\x7d\x80\x72\xbf\xae\xd8\xd7\x98\x9a\xf6\x02\x8d\x7b\
-\x00\xd9\x2e\x40\xb2\x13\xad\x55\x9b\x50\x11\x32\x09\xc9\x0e\x2f\
-\x21\x60\x69\x07\x7d\x13\x64\x44\x6e\xec\x6b\x32\xc1\xbf\x1e\xf1\
-\xbb\x1e\x7d\x90\x22\x7e\xaf\x3e\xf8\xd8\x7d\x4f\xa2\x34\x78\x02\
-\x9a\x1b\xb6\x1b\x02\x17\x83\x17\x41\x57\x11\x74\x34\xec\x00\xea\
-\xb6\x01\x35\x5b\x00\x32\x00\x2a\x36\x00\x65\xeb\x20\x4d\x9c\x85\
-\x24\xbb\x17\xf4\x4d\x90\x10\xb5\xb1\x6f\x4f\x13\x85\x7f\xe1\x8a\
-\xda\xd9\xbf\x53\xc8\xea\x1e\xf3\x09\x42\x83\x00\x84\xa2\x34\xf5\
-\xc4\x60\x34\xe4\x2c\xba\x21\x74\x96\x09\x58\xba\xcf\xba\xcc\x52\
-\xfd\x33\x08\xdf\xd8\x9b\xcb\x14\x9a\x8c\x11\xb6\xfe\x1e\xc4\xef\
-\x7d\x02\xb9\x17\x87\x43\x92\xf0\x33\x50\xb2\x16\x28\xa2\xec\x51\
-\xb0\x12\x95\xde\xa3\x11\xb2\xb2\x9b\x60\x02\xfa\xef\xdd\x26\x1a\
-\xff\x74\xba\xdf\x7c\xdf\xeb\x74\xf3\xa3\x74\xc0\x1f\x1f\x04\x79\
-\xf1\x2a\xa3\xd0\x5b\x1b\x77\xa3\x26\x69\x16\x32\xce\xbe\xcd\xd5\
-\x00\x7a\x51\x2c\x25\x45\x90\xae\x93\xae\x92\x42\x75\x4c\x45\x4a\
-\xb4\x7e\x16\x4d\x89\xbf\x00\x59\x4b\x81\xcc\xc5\x90\x86\x4e\x45\
-\xe8\xea\xee\x9a\x7f\x6f\x89\xb0\xba\x7b\x88\x89\xca\x3f\x13\xf5\
-\x9d\x29\xea\x37\xd0\x4d\x6f\x16\xa7\xfa\x86\x9c\xc5\x46\xc1\x2b\
-\xaa\x36\x22\xcf\xf5\x33\x2e\xa2\xf5\xa0\xa7\x84\x6d\xe8\xbd\x3c\
-\x66\xcf\xe3\x83\x93\x8f\xbc\x6a\x50\xd1\x27\x1e\x78\xa1\x6b\xf4\
-\xf6\x7e\x9f\xd3\xf7\x85\x09\xc5\x23\x01\x97\x06\x4f\x06\x52\xe6\
-\x01\x89\x73\x50\xef\x6d\x8e\xc0\x65\x1d\x35\x3f\xef\x8c\x89\xce\
-\x2d\xaf\xee\x1f\x7d\x82\x6e\x74\xb0\x06\x48\xf0\xaa\xbb\xb8\x31\
-\x5e\xa5\x5f\xd4\xd1\xdf\x9b\xaa\x36\x20\xf3\xc2\xbb\x08\xb4\xec\
-\x24\x86\xde\xca\x26\x79\xa2\x76\xf4\x1b\xf6\x47\x5f\x33\x6e\xf7\
-\xe3\x1d\x82\x57\x76\x5b\xaf\x9e\x0b\x40\xb8\xd5\xdd\x68\x8e\x9c\
-\x09\xc4\xce\x02\xa2\x7f\x42\xce\xe1\xd7\x34\x3f\x5b\x19\xb1\xb6\
-\xd7\x23\x26\x4a\xb7\xe8\x0a\x5e\xdd\xfd\x6b\xba\xc9\x35\x1a\x98\
-\x09\x76\xcf\xa3\xa9\x62\x9d\x01\xf8\x16\x2a\xe0\x72\xae\x7e\x28\
-\x8c\xe7\x9a\x14\x4d\x3a\x48\x5d\xc2\xf3\x7f\xf9\xf5\x97\x77\xd9\
-\xab\xf9\x79\x79\x47\x07\x01\x11\x64\x82\xb0\x19\x68\x0e\x98\x84\
-\x60\x4b\xfe\xb5\x42\x56\x74\x9b\x6b\x22\x75\x6b\xe0\xcf\x52\x43\
-\xe4\xc6\x7a\x96\xd2\x55\xac\x72\xd7\x6b\xdf\x2a\xa3\xa7\x23\x7c\
-\x43\x6f\xfd\x54\xef\x47\xa9\xfe\xb5\xbf\x5d\x73\xac\xed\xd5\x8d\
-\x7e\x56\x11\x37\x14\x50\xe6\x41\xc8\xb7\x40\x30\x29\x68\x2a\xd2\
-\xf7\x3e\xad\x79\x2d\x0f\x13\xad\x9b\x7c\x85\xac\xee\x2e\xa4\x5f\
-\x36\x29\x53\x9d\xf0\xa3\x6e\xfb\x46\x6a\xae\xde\x84\x54\xc7\xd7\
-\xf5\xc1\x97\x53\xea\x1e\x77\x53\xdf\xcb\x8a\xae\xcb\x35\x3f\x5f\
-\xea\xfc\x25\xe0\x3f\x09\xf0\x9d\x80\xf2\xe3\x43\x35\xaf\xd9\x10\
-\xb3\xbe\x8f\x69\x86\xf0\x26\xc2\xdf\x29\x9e\xbd\x6b\xc8\x5e\xa4\
-\x05\x2f\xdf\x0d\x48\x7f\x43\x7d\xea\xaf\xc6\xa2\xde\x37\x62\xf3\
-\x7d\xfd\x6f\x7a\xe7\xb1\xba\xe7\xeb\x9a\xd7\xa8\x3a\xfd\x1e\xe0\
-\x35\x16\xf0\xb0\x80\xf4\xc2\x47\xc2\x6b\x47\xac\xe9\xf9\xbc\x89\
-\xdc\xcd\x81\x6f\x29\xdc\xd4\x2d\xf7\xf3\xed\x9d\x68\x86\x0e\xf5\
-\xdb\x51\x16\x30\x56\xbf\xc8\x6b\xf1\x5f\xde\xdd\x2a\x60\xed\x03\
-\x9d\x6e\xc5\x7b\x8a\x59\xdf\xbb\xb3\xba\x90\x44\xd9\xd1\x21\x80\
-\xeb\x68\xc0\xf9\x1b\x28\x2e\x7d\x22\xbc\x87\xc8\x35\xbd\x3e\x35\
-\xd1\xfb\xfb\xf0\xbf\xd7\xa4\xfd\xe8\x9d\xfd\xa1\xa8\x5c\xcf\x45\
-\xbb\x78\x86\x2e\xf7\xf2\x7f\xf5\xa3\xbe\xc1\x73\xc9\x3d\x9f\xdc\
-\xea\xf7\xa6\x29\x44\x2b\x8f\xbc\x01\x5c\xa5\x61\xe0\xca\x17\x50\
-\x9e\xfb\x50\x6b\x80\xd5\x3d\xa7\x98\x08\xfe\x9d\x82\x6f\x55\xf7\
-\x4f\x35\x3d\x7e\xd4\xb6\x07\xa1\x28\xb3\xe2\xa2\x1d\xb5\x5b\x81\
-\xea\xcd\x40\xe5\x46\xe4\x9c\x1b\x66\x30\xde\x5f\x5c\xf8\xec\x3f\
-\x32\x11\x43\xaf\x55\xcf\x5e\xb3\xce\x71\x28\x70\xf1\x53\xe0\xfc\
-\xc7\x68\x3c\x36\x4c\x64\x80\x1e\x33\x4d\x14\xff\xe2\xe5\xb7\xee\
-\xb1\x67\x35\x11\x16\xb9\xf9\x3e\x28\x8a\x56\xea\xcd\xc7\xaf\xe7\
-\xa6\x66\xf5\xe0\xe7\x1c\x9e\x3f\xe2\xb9\x7f\xe2\xfd\xc5\xaf\xef\
-\xdb\x53\x93\x99\x9a\x4f\xff\x17\x38\xf3\x21\x70\xfa\x03\xd4\x39\
-\x68\x0b\xd0\x88\x55\xdd\xc7\x9b\x48\xfe\x85\xcb\x69\xe9\x33\xbd\
-\xe8\x06\x26\x71\x93\x2d\xeb\xef\x45\x53\xee\x52\x2e\xda\x19\x74\
-\x94\x52\xbf\x5f\x6a\x85\x72\x5f\x73\x1d\xf8\x17\xe7\xf6\x57\x4d\
-\x1f\xbb\x3a\x64\xd4\xa8\xfd\x67\xa7\x8e\xdf\xb6\xed\xa7\x29\xeb\
-\x7f\xfa\x7e\xd2\xe6\x21\x3f\x7e\xbb\xbd\xcb\x2d\x99\x88\x5a\xd3\
-\xeb\x4d\x2e\x33\xad\xee\xc1\x81\xc7\xa9\xff\x72\x2a\xde\xfb\x9c\
-\xf0\x9e\xc2\x57\x74\xfb\xc4\x44\xf3\x4f\x5e\xfb\x67\x7d\xd0\x81\
-\x6e\xde\x45\xcd\xec\x9e\x34\xe5\x57\x6e\xf5\x8d\x41\x97\xa7\xcd\
-\x43\x9a\xcb\x74\x5c\xd9\x3d\x1d\x9b\x67\x5a\x60\xe9\x94\xef\x30\
-\x6b\xc2\x02\x4c\x19\xb3\x1e\xa3\x47\xed\x05\xc1\x37\x26\x19\xc9\
-\x69\xda\xd4\x03\xd3\x66\x4e\xb7\xb9\x69\x3b\x78\xc2\x96\x77\x5d\
-\xcc\xde\x63\xce\x8e\xc7\x04\xf8\x38\x39\x02\xa9\x9b\x1e\xd4\xee\
-\x35\x58\xde\xd5\xd4\x05\xfc\xd9\xeb\xda\xfc\xfb\x57\xb2\x9b\x17\
-\xb8\xac\x13\xca\x7c\xcc\x91\xea\xf6\x33\x4e\xee\x5e\x8c\x15\xb3\
-\x96\x60\xac\xf9\x8e\xb6\x20\xff\x51\xd5\x4f\x1c\xb3\x63\xef\x8c\
-\xf1\x6b\x9f\xbc\x09\xe3\x3f\x5b\x24\x42\x83\xc3\x60\x0e\x3c\x93\
-\xea\xf8\x70\x82\xde\x45\x63\x80\x5a\xca\x12\x1d\x4c\x44\xff\xc4\
-\x75\x79\x5e\xbf\xff\xf9\x2f\xee\xd0\xe4\xf8\xcb\xcb\x8a\x15\xdf\
-\x4e\x55\x4d\x34\xdf\x72\x43\xa0\x93\x27\xdb\x63\xc9\xe2\x73\xb0\
-\x5a\x7b\x05\xdb\xb6\x3a\x73\x5a\x67\xe5\x84\x05\xf3\x4f\x63\xe2\
-\x44\xfb\x1b\xfd\xbf\x4d\x53\x2d\xac\x76\xae\x9a\x32\xba\xf7\x5f\
-\x4a\xff\xab\x7b\xbe\xc4\xc6\xff\xe8\xd5\xbd\x80\x13\x04\xff\xc4\
-\x70\x80\xe0\xd7\xd8\x0e\x14\x0f\x4b\x6e\x26\xa2\x7f\xe2\xb2\xfa\
-\x6e\x42\xe7\x2d\x33\xbe\x38\x3d\xd1\x62\x4b\x5d\x5b\xe0\xbe\xfb\
-\xee\x30\x6c\xac\xbd\x11\x12\x94\x8e\x9a\xaa\x3a\xa0\x45\xd9\xa6\
-\x54\xcd\x4a\x94\x14\x55\xc2\xd7\x3b\x19\x3b\x77\xb8\x92\x21\x0e\
-\x18\xfb\x99\x45\x33\xc6\x5a\x7e\xfa\x17\xa2\xff\x28\xd7\xff\xef\
-\x7d\x81\xc0\xbf\xcf\xeb\xd8\x7b\x48\xdb\xf4\x80\x60\x00\x1a\x22\
-\x4c\x1d\xc0\x1f\xbd\xa6\x8e\xdb\xda\x87\x60\x9c\x6f\x0b\xfc\xfa\
-\x75\x4e\x88\x08\xcd\x84\xb2\x51\x01\xb9\xb4\x19\xf5\x75\x2d\x64\
-\x80\x56\x54\x93\xaa\x2a\x5b\x51\x53\xdd\x8a\xba\xda\x56\x48\x1b\
-\x5a\xa0\x90\x37\x73\xf0\x35\x46\x90\x57\x66\xa3\x34\xe6\x1c\x92\
-\x2e\x2f\x87\xe3\xa2\x0f\x60\x37\xf3\x45\x1c\xfc\xe1\x59\x4e\x36\
-\xdf\xbf\x82\x3d\xdf\xbd\xa1\x3a\x38\xeb\x3f\x47\xaf\x2e\xec\x37\
-\xf6\xfa\x82\x3e\x4f\xff\xde\x7b\x8d\x58\xd9\x7d\x20\x6b\x4d\x23\
-\x56\xde\x05\xd5\xb1\x77\x39\xf0\x70\x7c\x0f\x8a\x43\x6f\x22\x50\
-\xbb\x4d\x4c\x41\x05\xe0\x7d\x26\xb2\x7f\xe0\x9a\x38\x6e\xf7\x73\
-\x04\x39\xcd\x18\xf8\x95\x2b\x2e\x22\x39\xb1\x88\x00\xb7\xa0\xb0\
-\x50\x85\x9c\x1c\x70\xca\xcd\x05\xf2\xf2\x80\xfc\x7c\xa0\xa0\x80\
-\x57\x61\x21\x50\x54\x04\x14\x17\xab\x90\x1d\x1d\x8e\xb8\xd3\xf3\
-\xe0\xb7\xee\x39\x38\xff\x6a\xf6\x67\x95\x4d\xb2\x76\x5f\x7c\xcf\
-\xdb\xfa\xef\x35\x72\x65\xcf\x8e\x04\xd7\x9f\x9b\xfc\xd9\x37\x80\
-\xc0\xbf\x2b\x28\x7b\x6b\x7f\x71\xfa\x77\x34\x91\xfd\x03\xd7\xe8\
-\xd1\xfb\xdf\x20\xd0\xd5\xfa\xe0\x59\xba\xbe\x7e\x2d\x01\x25\xc5\
-\xad\x48\x4f\x07\x32\x32\x80\xcc\x4c\x20\x2b\x0b\xc8\xce\x36\x6e\
-\x82\xdc\x8c\x1a\xc4\x5e\xda\x01\xcf\x55\xcf\xfc\x15\xe8\x6d\x29\
-\xcd\x6d\x41\xb7\x9f\x02\x57\xdc\xd7\x8d\x9b\x98\x5a\xd6\x65\x21\
-\xb7\x23\x68\x5d\x6f\x1e\xfc\xd1\x61\x9c\x9a\x1c\x86\x20\x48\x1b\
-\xfd\xad\xa1\x96\x5d\x5e\x34\xd1\xfd\x5d\xf8\xd6\x83\x08\x76\x8d\
-\x3e\xfc\xb9\x73\x4e\x21\x21\xbe\x16\xa9\xa9\xe0\x94\x96\x86\x1b\
-\x9a\x20\x2b\xb5\x12\xe1\xc7\x16\xc3\x75\x41\x4f\x03\x80\x2e\x73\
-\x3b\x23\x70\xf3\xab\x88\x3f\x3e\x0d\x59\x1e\x1b\x91\x1f\x68\x83\
-\x92\xa8\x53\x28\x8d\x3d\x8f\xa2\xb0\xa3\xc8\xf6\xdc\x82\xa4\xb3\
-\xb3\x10\xb2\x6b\x18\xdc\x16\x74\xbf\x91\x11\x0a\x3c\xe7\x9b\x6d\
-\x62\xa9\x3d\x98\xba\x93\x46\x56\xf9\xab\xe1\x33\x25\xaf\xeb\x2b\
-\x8e\xfe\x13\x26\xba\xbf\x73\x8d\x1b\x77\xe0\x09\x82\x5d\xa1\x0f\
-\x7f\xf5\xaa\x6b\x48\x4e\x56\x22\x29\x09\xf4\x27\x90\x92\xd2\xb6\
-\x09\xb2\x32\x95\x88\x3c\xb7\x15\xae\x0b\xef\xd6\x81\xe5\xb6\xb0\
-\x07\x01\x9f\x8a\xf2\xf8\xcb\x68\x69\xac\xbf\x61\xa1\x28\x56\x6b\
-\x93\x04\x95\xc9\xce\x48\x3c\xf5\x3d\x28\xfd\xeb\xfc\x4c\xd7\x39\
-\x66\xf0\x5f\xcc\x03\x2e\xdf\xf3\x1c\x0f\xfe\xc8\x3b\x9c\x2a\xf7\
-\x3c\x2f\x86\x5f\x17\xb1\xe2\xae\x87\x4d\x84\x6f\x0c\xbf\x07\xc1\
-\x8e\xd1\x87\xbf\x71\x93\x17\x81\x57\x21\x31\x11\x9c\x6e\x64\x82\
-\xa4\xe0\x28\x78\xae\x7d\x45\x07\x92\xa7\xe5\x03\x5c\x44\x2b\x25\
-\x15\x7f\x18\x7a\x5b\x6a\x91\xd7\x21\xcf\x6f\x37\x7c\x56\x3f\xc6\
-\xc1\xf7\x53\xc3\xcf\xda\xdc\x8f\x07\x7f\x98\xe9\x6d\x28\x1d\xde\
-\x00\xa5\x7b\xed\x33\x07\x4b\x3b\xce\x36\x11\xfe\x9d\xcb\xc2\xc2\
-\xc6\x5a\x0c\x9e\x86\x02\x58\xdb\x84\x23\x3e\x5e\x85\xb8\x38\x20\
-\x21\x81\x97\x71\x13\xa8\x10\x7e\x6e\x37\xa5\xf6\xae\x3a\x69\x3e\
-\xed\xca\x22\x34\xcb\x6a\x8c\x03\x6d\x2e\x07\x94\xf4\x83\x15\x6e\
-\x40\xd3\x31\xd2\x01\xd2\x1e\xa0\x71\x07\xbf\xa4\xdc\xe8\x40\x7f\
-\x3f\x47\xff\xee\x47\xdf\x47\xee\x6a\x69\x14\xfe\xdf\xba\x2c\x1f\
-\x04\x5a\xf2\x5b\xbe\x13\xd7\xde\x0b\x15\x41\x67\xe0\x71\xe8\x6d\
-\xa8\x0e\x0d\xa5\xd4\xdf\x47\x1c\xfd\x2e\x11\x2b\xba\x9b\x26\x7e\
-\x6e\x18\xfd\xe3\x0f\xbc\x4f\xd0\x5b\x35\xf0\xc7\x8c\xb5\xc5\x11\
-\xc7\x38\xc4\xc4\xa8\x48\x40\x6c\x2c\x38\x13\xc4\xc7\x1b\x9a\x20\
-\x39\x49\x89\x00\x9b\x19\x3a\x51\xef\xb7\xfe\x79\xd4\xe7\x47\x1a\
-\x81\x5e\x45\x40\x7d\x08\xac\x35\x01\xb6\xe2\x25\x5f\x6b\x44\x6b\
-\x78\xc9\x34\x5a\x4d\xda\xc0\x19\xa2\x3c\x72\x17\x82\x56\xf4\xe0\
-\xe0\xc6\xad\xb9\x1b\x2d\x07\xdf\xe4\xc0\x83\xc0\xe3\xe0\x5b\xc8\
-\xdb\xfa\x88\x18\x7e\x49\xc8\xb2\xae\x0f\x98\x08\xdf\xa8\xdd\x9b\
-\xe4\xd0\x89\xa0\x27\x6b\xe0\x8f\x1d\x6b\x87\x83\x8e\xb1\x08\x8f\
-\x50\x22\x2a\x0a\x88\x8e\x46\x9b\x26\x48\x8c\x57\xc0\x67\xc7\x97\
-\x3a\xf0\xa3\xec\xbf\x32\x8c\xfa\xe6\x32\x02\x7f\x89\x80\xaf\xfb\
-\x83\xd0\x57\x1b\xa8\xb9\x66\x29\x32\xce\x68\x57\xf4\xe2\xd6\xf4\
-\x42\x33\xa5\x7a\x1c\xe4\xc1\xc3\xe1\x2d\x54\xee\x7a\x56\xf8\x77\
-\xaa\x0d\x5a\x03\x96\x76\x1e\x66\x22\xfc\x3b\xd7\x98\x31\xb6\x93\
-\x35\xf0\xcd\xcd\x6d\x60\xeb\x10\x01\xbf\xc0\x3a\x44\x52\x00\x33\
-\xb5\x69\x82\xf8\x16\xf8\xec\x1c\xa5\x03\x3f\xe1\xd4\x0c\xa8\x94\
-\x8d\x22\xf8\x72\x02\xef\x41\xd0\xd7\x1b\x00\x57\x11\xe8\xa6\xd2\
-\xf9\xa8\x4f\x9f\x01\x59\xfe\x2c\xa8\xa4\xab\x0c\xc1\xb3\xaf\x91\
-\xaa\x62\xc6\x21\x7c\x83\xf6\x99\x01\x96\xe2\x5b\x38\xf8\x0c\xfc\
-\x9b\x9c\x6a\xf7\xbc\x20\x6e\xf9\xe0\x3e\x97\x34\xbf\x8b\xbd\x89\
-\xf0\x0d\xae\xe9\xdf\x1d\xed\x40\xe0\x33\x34\x06\xd8\xbc\xdd\x17\
-\xd7\xdc\x0a\x10\x1e\x4e\x63\x7a\x38\x10\x11\xd1\xb6\x09\xfc\xed\
-\x17\xe8\xc0\x67\x15\xbe\xaa\xb9\x49\x14\xf5\x25\x04\xde\xda\x20\
-\xca\x5b\x25\x2b\x51\xe8\x39\x12\xe1\x1b\x75\x1f\x02\x09\x59\xd3\
-\x1d\x39\x97\xa9\x80\xab\x5c\x24\x80\x97\x64\x7e\x8f\x04\xdb\x27\
-\x75\xbe\x2f\x77\xf3\xc3\x50\xa9\xa1\x73\xb2\x7f\x03\x75\x7b\x06\
-\xb0\x42\x4f\xf8\x1e\x6a\x0d\xb5\x9d\xc2\xbc\xce\xb3\x4c\xa4\xdb\
-\x4e\xff\x1f\x69\xe0\xcf\x9e\x73\x16\x97\xae\x65\xc3\x2f\x40\x82\
-\xb0\x30\x70\x06\x68\xcb\x04\x21\x97\xce\xe8\xc0\x0f\xdb\x33\x1c\
-\x2a\x85\x5c\x0b\x5f\x49\xad\x81\x7c\x93\xc1\x58\xde\x5c\xb5\x04\
-\x71\xfb\x1e\xbb\xe1\xb3\xfd\x61\xeb\x7b\xa1\x34\xe0\x0b\x24\xd9\
-\x3f\xa3\xfb\x75\xaa\xea\x6b\x76\x3f\xaf\x03\x9e\x89\x45\x7e\xb0\
-\x08\x7e\xd8\x96\x01\xfa\x73\x05\x4d\x6e\x0b\xee\x1a\x6c\xa2\x6d\
-\xe4\x22\xf0\xa7\x34\xa9\xdf\xf1\x64\x22\x9c\x5c\xf2\x10\x12\xa2\
-\x42\x68\x28\x38\x69\x8c\x20\x36\x41\x44\x60\x21\x5c\x16\xf6\x11\
-\x6e\xb0\xd7\x8a\x7e\x50\xd4\x95\x88\xe0\x53\x71\x20\x5f\x67\x30\
-\x96\xb3\x14\x9f\x60\xf7\x94\x00\x2a\x66\xc7\x83\x28\x72\xfe\x18\
-\xd5\x61\x3f\xa1\x3a\x6a\x1d\x32\x2f\xcc\xa0\xca\xde\xf8\x73\xfe\
-\x19\x1b\x1e\x40\xb3\xdd\x20\x01\xba\x46\x65\x3b\x9e\x44\xe0\x12\
-\x6d\xda\xcf\xbe\x32\x91\x9a\x85\x06\x04\x6c\x7e\x55\xdf\x04\x09\
-\xae\x0b\xba\x77\x36\x11\x17\x2f\xf4\x4c\x3b\xdc\x95\xe0\x4b\x99\
-\x01\x16\x2e\xbe\x8c\x8b\xd7\xb2\xe0\xe1\x5d\x8d\xe0\x60\x8a\xf0\
-\x10\xb4\x69\x02\xef\x9d\xe3\x74\x6e\x6e\x45\xe2\x55\x11\x7c\x6a\
-\xd7\x64\x56\x46\xc7\xf2\xf2\xd0\xaf\x05\x50\x39\xe7\xdf\x82\x22\
-\x6b\x16\x14\x99\x3f\xa2\xf0\xea\x7b\x88\xdd\xf9\x90\xb1\xe7\xfa\
-\x91\x44\x2d\x9e\x64\xff\xcb\xba\xe0\x0f\x0c\x81\x8a\xc4\x86\x02\
-\xf1\xf7\xe6\x5d\x7d\x07\xa8\x5b\x4a\x9d\x42\x3c\x24\x45\x71\x70\
-\x99\xd7\x45\x7f\xf6\x71\x91\x89\xba\xe8\x9a\x34\xc9\x61\x84\x26\
-\xfd\xdb\x1d\x8c\xe2\x0c\xe0\xe7\xdf\x84\xa0\x20\x70\x26\x10\x1b\
-\x41\x63\x82\x60\xe7\x60\x9d\x9b\x1a\xed\x30\x4a\x34\xe6\x57\x10\
-\xec\x4d\x06\x05\x1c\xaf\x95\x88\xd9\xc5\x03\x4b\x3d\x38\x00\x8a\
-\x9c\x5f\xd1\x94\xf1\x13\xd2\x0e\x0d\x30\x80\xce\xd2\x39\x8b\x78\
-\xc9\xbe\x97\x0c\xc0\x33\x29\xac\x5f\x45\xe2\x1a\xdd\xfa\xa1\xd0\
-\xed\x7d\xa0\x66\x01\x50\x3d\x9f\xb4\x8c\x8c\x58\x86\xb4\x2b\x4b\
-\xf4\xb3\x40\xbd\xeb\xfc\xbb\xfa\x98\xc8\xab\xaf\xb1\xe3\xec\xd6\
-\x33\xf8\x13\x26\xda\xe3\xc2\xd5\x4c\x5c\xbe\x9e\x8b\x80\x00\x20\
-\x30\x10\x6d\x9a\xc0\x73\xf3\xe7\x3a\x13\x3d\xb2\xf2\x34\xb5\x01\
-\xa8\xf8\x93\x1f\x30\x80\xae\x91\xb2\x62\x81\x00\x4b\x92\x30\x1d\
-\x8a\xec\xd9\x48\x3d\x34\x40\x78\x72\x38\x62\x79\x57\xa4\x6f\xb8\
-\x1f\x95\xbf\x3d\x8b\x16\x71\xaa\x57\x43\x87\x1d\xd3\x60\x54\xff\
-\xf6\x0c\x42\x97\x69\x9f\x27\x64\xcf\x1b\x94\xfb\x7f\x0c\x54\xcd\
-\x05\x2a\x66\x93\x66\x01\x65\x3f\x93\x09\x76\xa1\x59\x5a\x05\x8f\
-\xa5\x7d\xf4\xb2\x40\x27\x2b\x13\x79\xed\xf8\x7f\x95\x19\xe0\xd7\
-\xb9\xe7\xc8\x00\x59\x70\x76\x2f\x85\x9f\x1f\x04\x13\x88\x8d\xc0\
-\x4c\x10\xe4\x9e\xa2\x73\x33\xe3\x1c\x27\x69\xa3\x5f\x11\xa4\x03\
-\x5c\x90\x84\x57\x7d\xea\x34\x7e\x3b\xf6\xe6\xbe\x2c\xfa\x15\x85\
-\xd7\x47\x5c\x88\x5c\x71\x17\xea\xf6\xbe\x88\x96\x03\x83\x0d\xc6\
-\x76\x2d\xf8\xc1\x9c\x14\xfb\x07\x22\x4d\x77\x61\x07\xa1\x6b\xbb\
-\xa3\x3e\xce\x1c\x28\x27\xe0\x65\x3f\x01\x25\x3f\x90\x66\x02\xc5\
-\x33\x80\xa2\xef\xe8\xf5\xa3\x90\xe9\xb2\x46\x3f\x0b\xd4\xb8\xcc\
-\xeb\xdc\xdd\x44\x9f\x37\x00\xd7\xfe\xad\x58\xed\xcc\x19\xc0\xcd\
-\xb3\x0a\xbe\xbe\x68\xd3\x04\xde\xb6\x4b\x75\x6e\x66\x5d\x4e\x88\
-\x3a\xf5\x37\xd0\xcd\xde\x60\x00\x1d\x92\x15\x82\x6a\x13\x26\xf2\
-\x93\x37\xbb\x1f\x81\x24\x76\xda\xcf\xc1\xcb\x3a\xf9\x34\xd9\xbc\
-\xd6\x06\x74\x35\x78\xdb\xc1\x68\xb5\x79\x1d\x85\x9b\x1f\xd1\xa9\
-\xf2\xf9\x9f\xf3\x10\x0d\x21\x93\xd4\xc0\xbf\xe7\xa1\x17\x4e\x27\
-\x4d\x03\xf2\xa7\x00\x79\xf4\x6f\xc5\x96\x68\xaa\x2d\x30\xa8\x05\
-\xa8\x2d\x9c\x68\x1a\xff\x27\x1f\x64\xb3\x7f\xcd\xcc\x00\xeb\x36\
-\x7a\xe0\x22\x19\xc0\xd5\xbd\x16\x3e\x3e\x10\x4c\xe0\xef\x0f\x9d\
-\x21\xc1\x75\xd9\x53\xc2\x4d\x0c\xd8\xf4\xb2\x36\xfa\x9b\xbc\x0c\
-\x80\xf3\x5a\x0e\x34\xf0\x92\x66\xcf\xe4\xb7\x63\xaf\xbf\xa7\x31\
-\xdd\x7e\x40\xa7\x9c\x4d\xfd\x94\x3a\xe0\x45\xd0\x99\x5a\xac\xff\
-\x83\xa2\x2d\x8f\x22\x5c\xaf\x2b\x08\x5c\xd6\x01\xf9\x97\x07\x43\
-\xc5\x22\x9c\xa9\xf0\x5b\xa0\x60\x2a\x41\x9f\x0c\xe4\x4e\x04\x72\
-\xc6\x03\xd9\xe3\x48\x63\x80\x2c\x0b\x32\x64\x12\xe2\x8f\x7c\xa3\
-\x9f\x05\xdc\x4d\xe3\xff\x58\xbb\x3e\x9a\x02\x70\xc3\x66\x2f\xae\
-\x00\x74\xf3\xa8\x87\xb7\x37\x8c\x9a\xc0\xdf\x25\x4d\xe7\x26\xa6\
-\x5f\xb5\xd4\x8e\xfd\xd2\x2d\x5a\xe0\x22\xe8\xbc\x2c\x39\xa9\xa8\
-\x3a\x0f\x5e\xc5\x60\x76\x80\x97\xdd\xfc\xdf\x2a\x69\x2c\x37\x04\
-\x3f\x08\xf2\xbd\x2f\x23\x6f\x63\x3f\x1a\xe7\x3b\x19\x14\x87\x2c\
-\xea\x25\x31\x5f\x69\xa3\x3c\x9f\xa2\x3c\x77\x02\x41\x67\xc0\xc7\
-\xf2\xc0\x33\x69\x48\xc8\x18\x0d\xa4\x7f\x03\xa4\x7d\x09\x94\x5a\
-\xa3\x3e\xe5\x84\xe1\xbc\xc0\xbc\x8e\x77\xf6\x81\x51\x63\xc6\xda\
-\x3e\xae\x31\xc0\xaa\xb5\xae\x9c\x01\x3c\xbd\x25\xf0\xa2\x60\x36\
-\x66\x02\x6f\xc7\x83\x3a\x37\xb1\x26\xc3\x57\x3d\xf6\xa7\xb4\x09\
-\x9d\x53\xfd\x32\x41\xe9\x27\xf8\x9d\xb9\x67\x96\xbe\x81\x92\xed\
-\xcf\xea\x40\x67\xd1\x1e\xbb\xb2\x87\xd1\x39\x80\x88\x8d\x77\xa3\
-\x22\xe4\x17\x02\x3e\x4d\x2f\xca\x35\xd0\x09\x78\x06\x75\x23\x69\
-\x64\x8e\xb4\xff\x01\x29\x5f\x00\xc9\x9f\x01\x49\x9f\xd0\xdf\x27\
-\x41\x25\xcd\x47\xf8\x86\x5e\x7a\xc3\x40\x87\x3b\xfb\xe1\x50\x8b\
-\x31\xb6\x03\x34\x06\x58\xb2\xcc\x49\x6d\x80\x06\x78\x7a\xc2\xa8\
-\x09\xdc\x77\xcf\xd2\xa9\xfe\x85\x0d\x1d\xf2\x4b\x6d\x43\x67\x3d\
-\x79\xdd\x12\xa0\x76\x31\x69\x11\xe4\x59\xd3\xb9\x14\xce\x2d\xe1\
-\x5a\xf5\x41\x32\xf5\xf8\xe2\x8a\xde\x98\x8a\x9c\x06\x41\x95\xff\
-\x23\xbd\x56\x39\x19\xe0\x27\xdd\x28\xcf\x50\x47\x79\x2a\x01\x4f\
-\xf9\x9c\x80\x7f\xca\x43\x4f\x1c\x09\x24\x7c\x04\xc4\xfd\x17\x88\
-\x1d\x4e\x43\x54\x39\x4a\xce\x0d\xd4\xeb\x06\x3a\xac\xbf\xb3\x0d\
-\x60\x61\xf3\xa4\xc6\x00\xb3\x7e\x39\xcd\x4d\x01\xbb\x7b\xd6\xc2\
-\xc3\x03\x46\x4d\xe0\xb6\xe1\x63\xe1\xe6\xf9\x6f\x78\x51\x3b\xfe\
-\x4b\x77\x19\x42\x57\x03\x47\xcd\x42\xbe\x2f\xaf\x9a\x47\x9a\xc3\
-\xb5\x69\x85\xd7\x86\xb6\x09\x3b\x68\xb9\x6e\xda\x4f\xdc\xfb\x10\
-\x45\x39\x45\xbb\x3c\x06\x40\x23\x15\x76\x54\xed\xa7\x7f\x6d\x18\
-\xe5\x89\x1f\xf3\xd0\xe3\x3f\x20\xe8\x23\x80\x98\xf7\x49\xef\x91\
-\xde\x05\xa2\x87\xd1\xfb\x08\x84\x2c\x6c\x2a\x7c\x2d\x75\x8a\xc1\
-\x0b\x77\xb4\x01\xcc\xcd\xad\xef\x17\x96\x7f\xc7\xd9\x71\x45\xa0\
-\xaf\x7f\x35\xdc\xdd\x61\xd4\x04\x2e\xcb\x5f\x12\x6e\x5e\x84\xed\
-\x67\xea\xea\x5f\x4e\xc0\xf5\xa1\xb3\xc9\x98\x79\x7c\x5f\x5e\xf9\
-\x2b\x41\xff\x85\xef\xcb\x4b\x7f\xe4\xdb\x34\xaa\xd8\x73\xce\x0e\
-\xfc\xdd\xb3\x7e\xa3\xb7\xdc\x03\x65\x22\x45\x77\x83\x27\x0f\x1f\
-\xf4\x5a\x69\xa3\xda\x8e\x72\x31\x70\xa6\xa8\x77\x80\xc8\xa1\x40\
-\xc4\x5b\xf4\xfa\xe7\xd0\x18\xbf\x1c\xc9\x7b\x74\xe6\x04\x92\xee\
-\xf4\x0c\xd0\x85\xe0\xb7\x68\x4c\x70\xf8\x78\x3c\x02\x82\xcb\xe1\
-\xe6\x06\xa3\x26\x70\x59\xfc\xa8\x68\xd5\x6f\x9a\x7a\xda\xb7\x88\
-\x8f\x72\x06\x5d\x14\xe5\x42\x5f\x5e\xaa\xd7\x97\xb3\x36\xad\x88\
-\xfe\xad\xf6\x28\xaa\xfc\x46\x20\x72\xd3\xdd\x06\xe0\xd9\x71\x6e\
-\x59\x47\x9e\x44\x4b\x32\xa5\x78\x49\x80\x1a\x3e\x49\x16\x77\xe3\
-\x28\x67\x8a\x7c\x5b\x0d\xfd\x4d\x20\x9c\xba\x8b\xd0\x41\x40\xc8\
-\x7f\xa8\x4b\xb0\x47\x53\xf2\x16\x94\x9c\xec\x2f\x36\x40\xb9\x69\
-\x1e\x60\xd4\xfe\x7c\x61\x19\x78\x9b\x0f\xbc\x03\x0a\x09\xb6\xca\
-\xa8\x09\x9c\x17\xde\x2f\xdc\xbc\xa4\xb3\x3f\xab\xdb\xbf\xf4\x36\
-\xa3\x9c\x87\x3e\x5d\xaf\x62\x9f\xc8\x57\xec\xf2\x68\x32\x4f\x1e\
-\x54\x15\x76\x68\x08\xfb\x1a\x25\x4e\xaf\xa1\xe8\xe2\xcb\xa8\x72\
-\x1b\x8c\xe6\x78\x4a\xef\x25\x3b\x79\x73\x69\xe0\x33\xe5\x6f\xb8\
-\x71\x94\x33\xe8\x61\x54\x54\x86\xbe\x0e\x04\xbf\x46\x1a\x48\xbd\
-\xeb\x2b\xd4\xc3\xbe\x44\xaf\xbb\x07\x8a\x0c\x1b\xd4\x3b\x3d\x01\
-\xb7\x79\x1d\x34\xbf\x47\xa3\xc9\x00\xa3\xf6\xfb\x6a\x0c\xf0\xd3\
-\xcf\x27\xe1\xe4\x92\x83\xa8\xa8\x16\xb8\xba\xc2\xc0\x04\x2e\x8b\
-\x1f\x11\x0c\xc0\x76\xe7\xf2\x05\x60\x82\xf1\x28\xd7\xf4\xe5\x79\
-\x6d\x54\xec\x05\x94\x35\x54\x12\x6d\x6a\x57\xe4\x50\x84\xd3\x38\
-\xdf\x98\x22\xfa\xba\x48\x92\x30\x2d\xf8\xb6\xa2\x3c\xf8\x55\x35\
-\xf0\x97\xa9\x6f\x25\xe8\x01\x03\xa8\x7d\x79\x81\x0a\x98\xe7\xc8\
-\x00\x36\x50\xa4\x5b\xa3\xc1\xe9\x71\x04\xae\x14\xf6\x2c\xaa\x02\
-\x56\x74\xed\x70\xa7\x1b\x40\x67\x13\xe8\xc9\xf3\x29\x88\x8d\x93\
-\xc0\xc5\x05\x06\x26\x70\x59\xf6\x82\x60\x80\x98\x43\x16\xbc\x01\
-\x1a\xd3\xd4\x51\xfe\xad\x61\x94\x73\xc0\xc7\xe8\x55\xec\x5f\x69\
-\x2b\xf6\xe2\x6d\x04\x5b\x6a\x08\xdb\x00\x7e\x14\xc1\xff\xa8\x8d\
-\x28\x7f\x55\x1b\xe5\x01\x2f\xf2\xc0\xfd\x9e\x27\xe8\xd4\x62\xfa\
-\x3c\x4d\x63\xd7\x93\x94\xbe\x9e\xa0\xf7\x78\x16\x4d\x29\xdb\x39\
-\x03\x84\xaf\x17\x9e\x31\x90\xde\xf1\x19\x60\xf4\x68\xeb\xa9\x62\
-\x03\x6c\xda\xea\x8d\xd8\xf8\x72\x4a\xf9\x2a\xc1\x04\x4c\xcc\x04\
-\x2e\x56\x1f\x08\x06\x08\xdf\xff\xa1\x7a\x08\xc8\xe7\xa3\x9c\x4d\
-\xc6\x18\xeb\xcb\xb9\x8a\xfd\x4b\x51\xc5\xfe\xa9\xa8\x62\xa7\x9f\
-\x91\x49\xf5\x82\x2c\xd1\x38\x78\x65\x09\x65\x0a\xea\x30\x22\x86\
-\xde\x20\xca\x5f\xd4\x46\xb9\xcf\x33\x04\xfc\x29\x1e\xb8\xa0\xc7\
-\x29\x7d\x3d\x46\x45\x69\x18\x1a\x63\x17\xa3\xe1\xca\x63\x88\xda\
-\xdc\x43\xf3\x7b\x94\x9a\x86\x80\x51\xfb\x9f\x17\x1b\x60\xda\xb7\
-\x47\xe0\xec\x99\x87\xd4\x94\x66\x38\x3b\x83\x33\x81\xc6\x08\x2e\
-\xdb\xbe\x13\x0c\xc0\xf6\xe4\xf3\x5d\x80\x8c\x6f\xd3\x18\x74\x63\
-\x51\x9e\xac\x57\xb1\xb3\x02\xce\x58\xc5\x9e\xcc\xe6\xee\x37\x52\
-\x26\xd9\x47\x7f\x6e\xa6\xbf\xd3\x70\x12\xf6\xe6\x9f\x8b\x72\x01\
-\xb8\x1a\x3a\x93\xc7\xa3\xf4\x27\x7d\x5d\xd1\x00\x59\xf0\x38\x32\
-\xc0\xa3\xe2\x0c\x10\x6d\x32\xc0\xa8\xfd\x6c\x3f\x60\x91\xd8\x04\
-\x36\xf6\xe1\xc8\xc9\xad\x83\x87\xbb\x8a\x33\x81\x60\x04\xbb\xbd\
-\x3a\x13\x29\xc2\x0e\xa0\xbc\x39\x37\x8e\x72\xd6\xa6\x19\xab\xd8\
-\xa3\xf4\xc6\x72\x96\xda\x85\x28\x1f\xf8\xe7\xa3\x5c\x03\xdc\xe3\
-\x11\x52\x7f\x4a\x5b\x4c\x0f\xd3\xcf\x26\x43\xb6\x28\x20\x71\x19\
-\xc8\x19\x20\x68\x95\x50\x03\x9c\x34\x2d\x07\xf2\x26\xb0\x15\x1b\
-\x80\xed\x0b\xf4\x09\x2c\x44\x4e\x56\x0b\xae\x5f\x07\x27\xce\x04\
-\xa7\x42\x74\x77\x01\x25\x5d\xe7\x0d\x50\xbc\xe7\x8f\x45\x39\x57\
-\xb1\xbf\x2d\x1a\xcb\x87\xdc\x60\x2c\x1f\xf0\xe7\xa2\x5c\x80\xfe\
-\xb0\x5a\xfd\xa8\x80\x61\x62\x13\x49\xfb\xd1\x5a\x97\xca\xa5\xff\
-\xfa\xcb\x8f\xc0\x7d\x3e\xdf\x05\xb8\x2f\xe8\xb8\xd2\x44\x9f\x37\
-\xc0\xe7\xfa\x8f\x82\x5d\xba\x9e\x89\xfc\x82\x3a\x04\x07\xa9\x70\
-\xed\x9a\xda\x04\xd7\x95\x70\x9e\xdf\x5b\x30\x40\xca\x85\x39\xbc\
-\x01\xea\x42\xff\xfd\x28\x67\xc0\xdd\xd5\xc0\x99\x5c\x1f\xe4\xe5\
-\x46\xdf\x27\x2f\x81\x22\xd3\x8e\x33\x40\xe9\xf1\x07\x85\xf7\xef\
-\xbd\xa4\xd3\xfb\x26\xfa\xbc\x01\xfa\x8b\xe1\x8f\x19\x63\x8b\x6b\
-\xee\xb9\xf0\xf0\x2b\x40\x4d\x55\x13\x75\x02\x22\x13\x6c\x1c\xa3\
-\xad\x03\xd6\x3c\xc1\x6f\x01\x6f\xa6\x82\x2d\x71\xd4\x0d\xa2\x7c\
-\xd0\xad\x8f\x72\x0d\x70\x97\x07\xd4\xba\x9f\xde\x2c\x29\x8e\x9f\
-\xaf\x90\x05\x7c\xc3\xa5\xff\xf8\xed\xc2\x82\x90\xd4\xcf\xb2\x4b\
-\x57\x13\x7d\x23\x85\xe0\x77\x33\x1c\x71\xdd\x23\x8f\x2b\x06\xa3\
-\xa9\x23\xa8\x2c\x6f\xe6\xe0\x73\x26\x38\x7c\x59\x67\x18\xa8\x4c\
-\x76\x51\x0f\x03\x47\xfe\xbd\x28\xd7\x00\xe7\xa0\xdf\xa7\x56\x5f\
-\xfa\x3b\xfd\x5b\x43\xba\x90\xfe\xeb\x2e\xf6\x87\xc7\xc2\x8e\x9a\
-\xf7\x7e\xd9\x44\x5e\x6b\x80\x21\x62\x03\x2c\x58\x78\x91\x37\x80\
-\x57\x1e\x5c\xbd\xf3\xa9\x20\xac\x45\x51\x01\x5f\x0f\x5c\xbb\xaa\
-\x80\xf3\x42\x6d\x1a\x8d\xb4\xfd\x5c\xbd\x24\x5c\x4f\x91\xff\xc1\
-\x1f\x88\xf2\xa7\x6e\x7e\x94\x6b\x80\x33\x5d\xef\x43\xea\x4d\x6f\
-\xf4\x5e\x2a\x48\x57\x72\xef\xad\x31\x76\x09\x67\x80\x94\x3d\xda\
-\xc7\xca\xbd\x16\x77\x1e\x65\x22\xaf\x99\x0b\x30\xb7\xfe\x40\x6c\
-\x80\xcd\xdb\xbc\x75\x0c\xe0\xe6\x5b\x80\xf2\x72\x29\x4a\x8b\xf9\
-\x4c\x70\x7d\xb7\x95\xee\xb6\xb0\x5c\xf5\xb6\xb0\xb2\x2b\x6d\x44\
-\xf9\x93\xb7\x2e\xca\xaf\xab\xa1\x5f\x53\x43\xbf\x76\x0f\x70\x95\
-\xe4\x43\x59\x48\x51\x87\x56\x49\x1e\x1a\xae\x3d\x8b\xea\x73\xfd\
-\x85\xe2\x8f\x54\xe1\xb3\xb4\x73\x17\x13\x79\xcd\xa2\xd0\x18\xdb\
-\x6f\xc4\x06\x38\xe8\x18\xa3\x63\x00\x9f\xa0\x2a\x84\xc7\xb4\xa2\
-\xa2\xa2\x09\x35\x95\xcd\xf0\x70\xae\x82\xf3\x3c\xed\xc1\x0f\xa1\
-\xbb\xa9\xf0\x6b\x56\xf0\x26\x48\xfc\xf9\x9f\x8d\x72\x01\xfa\xdd\
-\x6a\xf5\xa2\xef\xa1\x9f\x53\x1b\xcb\x1f\x42\x15\x39\x0b\x0d\x4e\
-\x8f\x21\xcc\xea\x2e\xed\x21\x15\xf3\x3a\xae\x31\x51\x17\x5d\xe3\
-\xc6\xd9\x7d\xaf\x3d\xff\xc7\x01\x57\xdd\x72\x70\x9d\xc6\x7f\x17\
-\x32\x80\x57\x40\x39\x22\xe3\x54\x24\x1a\xe2\x63\x55\x28\x29\x69\
-\x42\x93\x4c\x89\xb0\x93\xeb\x75\xb2\x40\x51\xd8\x41\xf5\xcc\x60\
-\x0d\x8d\xff\x1f\xfe\x33\x51\x2e\x86\xee\xd4\x53\x2d\xfa\x7a\xb1\
-\x13\xf7\x5e\x9a\x4b\x3d\xd1\x70\xf5\x09\xa4\xed\xef\x2d\x7e\xaf\
-\x75\xde\x4b\x3a\xf7\x36\x51\x17\x5d\x54\xf5\x6f\xd4\x18\x80\xed\
-\x0e\xd6\x14\x80\x1e\x7e\x25\x04\xbe\x15\x51\xf1\x10\xc4\xcc\x90\
-\x9e\xd5\x00\xa5\xac\x9e\xba\x80\x27\x85\x1b\xeb\xb1\xe4\x1e\x28\
-\xeb\x72\x78\x13\xc8\xf2\x69\x28\x78\xeb\xd6\x46\xb9\x93\x1a\xfa\
-\x15\x8d\x7a\xf0\xf0\x0b\xce\xf0\xe7\x10\xca\x4a\x20\x71\x7f\x13\
-\xf9\x87\x1f\x80\xcb\x1c\xf1\x36\xb0\x8e\x6b\x4d\xc4\x45\xd7\xb7\
-\xd3\x8f\x76\x26\xf0\x09\x9a\xf6\xef\xf4\x85\x14\xce\x00\xae\x3e\
-\x85\x04\xbb\x19\xd1\x09\xe0\x15\xcf\x2b\x34\x4a\x06\x9f\xe0\x62\
-\x84\x46\x97\x21\x2b\xd2\x85\x6e\x6a\x07\xed\x99\x00\x36\xef\x40\
-\xa5\x54\x6f\x13\x93\x15\x50\x41\x38\xfc\xd6\x44\xb9\x06\x38\xd3\
-\x65\xa6\xee\xf4\xfd\xf4\xb3\x4b\xf8\x8e\x44\xa5\x94\x42\x16\x64\
-\xc1\xad\xfd\x8b\x96\x7e\xb9\x23\xe6\x3c\x17\x75\xba\xf3\x9e\x07\
-\x30\x37\xb7\x1e\x60\x61\x61\x33\x7c\xcc\x58\xdb\xf7\xc6\x8d\x3b\
-\x30\x6c\xc2\x44\xfb\xf7\x27\x4d\x3e\x38\x72\xea\xd4\xc3\x33\x09\
-\xbc\xbf\x76\x67\xb0\x27\xa5\xff\x5c\x8a\xfe\x7c\x44\xc4\x28\x10\
-\x9b\x08\xc4\x68\x44\x26\x08\x8f\x69\x82\x77\x50\x11\x67\x00\xdf\
-\x90\x62\xf8\x85\x95\xc0\xdb\xee\x67\x9d\xa1\x20\xcf\xe3\x07\xaa\
-\x07\xa4\xea\xe1\xa0\x96\xfe\xc7\x19\x37\x37\xca\xaf\xa8\x81\x73\
-\xba\x0b\xb8\x44\xf2\x19\x0a\xd4\xa5\xa8\xd7\x26\x1a\xb9\x71\xbf\
-\xe4\xe4\x23\x6c\xa6\x4f\x7f\x0f\xe0\x67\x77\x22\x7c\x76\xf0\x83\
-\xe2\xf7\x0e\x6a\x5e\x6a\xe9\x04\x27\xd7\x1c\x5c\x73\xcf\x43\x78\
-\x74\x23\xe2\x92\xc0\x89\x99\x80\x29\x2a\x4e\x49\xf0\x8b\x79\x03\
-\x10\x7c\x9f\xe0\x12\x5c\x77\x2d\x83\x9b\x67\x31\x5c\xd7\xbd\x23\
-\xba\xc9\x1d\x51\x1e\xb6\x50\x9b\x09\x98\x8a\xce\x51\x31\x38\xe0\
-\xef\x47\x39\x03\xce\x41\xef\xc6\xcb\x89\x7e\x5e\xda\x36\xd0\x78\
-\x24\x44\x7e\x63\xf4\x6c\x14\x9f\x60\xd3\xbd\x1d\xf5\xb7\x81\x1f\
-\xbd\x13\xe1\xaf\x20\xb8\xaa\x1b\x81\x9f\x34\xe9\x20\xb6\xef\x0a\
-\xc0\x15\xe7\x1c\xce\x00\x21\x91\x12\xc4\x27\x13\x7c\x8d\x92\xd8\
-\x10\xd0\x42\xe0\x4b\xe0\x15\x58\x24\x64\x00\x17\x8f\x72\x5c\x77\
-\xa9\xc0\x35\x17\xfa\xd3\x29\x15\xce\x96\xda\x53\x3f\xdd\xe6\x77\
-\x46\x69\xe0\xf7\x50\x35\x16\x8b\x1e\x1c\xa1\xe2\x30\x6d\x13\xd5\
-\x02\x4f\xff\xb5\x28\x67\xc0\x2f\x76\xe5\xe5\x44\x59\x24\x7e\x31\
-\x0d\x33\xda\x9f\xaf\x92\x97\x41\x1e\x3a\x09\x79\x47\x1e\x66\xdb\
-\xbd\xf5\xe1\x27\xbb\xcd\xbf\xc3\x9e\x01\x30\x37\xb7\x59\xa7\x0f\
-\x9b\x9d\xfb\x43\x63\x3e\x66\xfd\x72\x06\xcb\x57\x39\xc3\xc6\x3e\
-\x02\x17\x9c\xd8\x03\xa1\xd9\xb8\xe2\x92\x83\xc0\xb0\x5a\x24\x50\
-\x26\x65\x62\x26\x60\x8a\x4d\x6c\xa5\x36\xb0\x0c\x9e\x01\x85\x82\
-\x01\xdc\xbd\xcb\xe0\xec\x56\xc1\xe9\xba\x6b\x05\x5c\x3d\xcb\xe1\
-\xe9\x11\x0e\xa7\x05\x0f\xeb\x64\x82\xec\xcb\x23\xd1\x5a\x17\xa0\
-\x7b\x4e\x90\xa2\x81\x0a\xb5\xd3\x40\x98\x05\x65\x80\x07\x7e\x3f\
-\xca\x39\xe8\x5d\xe8\x6b\x64\x94\xa0\xff\x01\x39\x07\xf9\xa1\x45\
-\x7c\x6c\x5c\xb9\x3f\xa4\x3e\xef\x23\xcd\xe6\x41\x63\x87\x48\x4a\
-\x5d\xe7\x76\x78\xf9\xce\x82\x6f\x61\xf3\xbd\x7e\xe4\xcf\x5f\x78\
-\x09\x27\xcf\xa5\xe2\xec\xa5\x0c\x9c\xbb\x9c\x89\xf3\x04\x9e\x3d\
-\x07\x70\x89\xe0\x5f\x76\xce\x86\x6f\x60\x15\x12\x53\x21\x88\x37\
-\x82\x0a\xbe\xc1\x15\xf0\xf0\x2f\xe4\x0d\x40\xf0\x3d\x7d\xcb\xe0\
-\xea\x5e\x09\x17\xf7\x0a\x41\xfe\x61\xa5\x98\x3b\xff\x2c\x26\x59\
-\x6c\xc0\x89\x9f\xfa\xe9\x00\x88\xdc\xf3\x14\x64\xe9\xeb\xa9\x2a\
-\xcf\x35\x3c\x2d\x4c\x29\x01\x2a\x83\x80\x2c\x6b\x3e\xa2\x23\xa6\
-\x50\x0b\x69\x4e\x95\xe6\x58\x1a\x73\x66\xd2\xd7\x16\x01\xd9\xf6\
-\x40\x55\x04\x7d\xaf\xd4\xf0\xf0\x48\x69\x01\x1a\xe3\x97\x40\xe2\
-\xf6\x32\xaa\x2e\x3f\x6b\x0c\x7e\x33\xe9\x8b\x3b\x6b\x52\xc7\xc2\
-\xe6\x13\x02\xae\x14\x9f\xf3\x67\xb5\xc1\x13\xa7\xcf\xa7\xe3\xcc\
-\xc5\x0c\xa3\x06\xf0\xf4\x2b\x43\x52\xaa\x0a\x49\x69\xa0\x3f\x79\
-\x31\x13\x04\x84\x56\x73\xb3\x80\x1a\x03\x78\xfa\x97\xc0\xcd\xa3\
-\x52\x47\xbe\xc1\x65\xd8\xb4\xcd\x53\x30\xda\x78\xf3\xad\xb0\x9f\
-\xa9\x7b\x3c\x8b\xc7\xe2\x6e\xc8\xbd\xfc\x1e\x94\x05\x7b\xd1\x2a\
-\x49\xfb\xdb\x07\x45\xb6\x36\x64\xa0\x29\x75\x23\xa4\x5e\x43\xa8\
-\xd5\x7b\x85\x0c\xf0\x12\x32\x0e\xf4\xd3\x87\xaf\x22\x4d\xbf\xa3\
-\xe0\xd3\x78\xce\x56\xf5\x2a\x35\x30\x2c\xa8\xad\xdb\xb1\x2b\x88\
-\x22\x3f\xad\x4d\x03\xb8\x7a\x15\x11\xf8\x56\x24\xa7\x83\x57\x1a\
-\xaf\xe0\x88\x3a\x6a\x05\xf3\xb5\x06\xf0\x2f\x86\x87\x77\x25\xdc\
-\x3d\x79\xb9\x91\xbc\x03\xca\x71\xf8\x44\x94\x7e\x5d\x91\x33\x6f\
-\xda\x22\x8b\x53\xb3\x1f\xb3\x26\x00\x2d\x62\x28\x01\xeb\xee\x43\
-\xa9\xe7\x48\x28\x32\x16\xa3\xb9\xe4\x0c\x99\x21\x95\x5f\x49\xfc\
-\x3d\xe8\xf4\x3d\xaa\xba\x18\xa8\x8a\xf6\xa1\x35\xe9\x33\x28\x83\
-\x5f\x82\xd4\xf3\x3f\x90\x78\x0c\xe4\xa2\x5f\xe2\xfa\x22\x77\xa6\
-\x90\x9e\x01\x76\xdc\x89\x8b\x3a\xce\x1a\x10\xe3\xc6\x1f\xc0\x5e\
-\xeb\x70\x9c\x38\x9b\x86\x53\xcc\x00\x17\x44\x06\xb8\x92\xc9\x1d\
-\x06\x71\xcd\xbd\x80\x22\xbd\x05\x29\x19\xd0\x2a\x9d\xb5\x7b\x12\
-\xb8\x78\xe7\x73\x06\x70\xf7\x2b\x20\xf8\x64\x00\x9f\x4a\x78\x7a\
-\x57\x91\x09\x78\x79\xf9\x56\xe0\x8a\x6b\x06\xc6\x8d\xb3\xd3\xf9\
-\xa4\x8f\x1f\x26\xae\x15\x3e\x12\xee\xe2\xbc\x7e\x43\x09\x44\x8a\
-\x7e\x6a\x0e\xdd\xda\x0f\x65\x9e\x1f\xa2\x31\xce\x82\x34\x0e\x8a\
-\xb4\x45\x50\x64\x6d\x85\x32\xcf\x8e\xb2\xc4\x11\x28\xf3\x0f\x41\
-\x91\xbd\x1b\x4d\x34\x74\x34\xc6\xfd\x04\x65\xe4\x3b\x34\x1c\x0c\
-\xe0\x15\xf7\x02\x5a\xa3\x07\xe8\x18\xa0\xde\x79\x80\x7e\xe1\xa7\
-\x24\xdd\x59\x9f\x0e\x3e\x66\x8c\xad\xb9\xf8\x29\x9f\x7d\xb6\x91\
-\x38\x7e\x3a\x95\x37\x00\x45\xbf\xc6\x00\x5c\xf4\x93\x01\xae\xb8\
-\xe4\x22\x21\x59\x89\xd4\x4c\x20\x35\x43\xab\xe8\x78\x39\x5c\xbc\
-\xf2\xf9\x45\x20\x9f\x02\xce\x00\xde\x7e\x15\xf0\xf2\xa9\xd2\xca\
-\xb7\x92\x1b\x12\x66\xcc\x74\xd4\x2d\x32\x2d\xf6\xfe\xaa\xff\xbe\
-\x9c\x16\x3e\xd8\xd5\x65\x5e\x97\xb9\x04\xa4\xca\xc0\x08\x5b\x1e\
-\x44\x99\xdb\xfb\x90\x47\x7d\x45\xbd\xfb\xff\x20\x0d\x79\x1f\xd2\
-\xa0\x61\x90\x04\xbe\x0d\x69\xe0\x30\xc8\x82\x46\x40\x16\xf8\x3e\
-\x9a\x42\xde\xa2\x82\xe4\x65\x5e\xf1\x2f\x71\x92\x7a\xbf\x2a\xa4\
-\xff\xa2\x93\x8f\xeb\x47\xff\xc5\x3b\x0a\xfe\xe4\x29\x87\x3a\x6b\
-\x0e\x7a\x60\x63\xfe\xce\xdd\xc1\x38\x76\x2a\xb5\x4d\x03\xb0\x47\
-\xc0\x62\x13\x1b\x91\x96\x05\x5e\x99\xbc\xe2\x93\x15\x1c\x7c\x61\
-\x15\x90\x0c\xe0\xe5\x57\x0e\x1f\xbf\x6a\x41\xde\xbe\xd5\x34\xee\
-\x97\x62\x89\xe5\x15\xfd\xd4\x7f\xc3\xe7\xec\x3c\x96\xf4\xb8\xd7\
-\x75\x7e\xe7\x25\x04\xa7\x48\xdf\x08\x21\x9b\xee\x47\xb5\xf7\x08\
-\x02\xff\x26\x1a\xfc\x07\x91\x5e\x27\x0d\x51\x1b\xe0\x3d\xc8\x02\
-\xde\x81\x2a\xe1\x35\x2a\x4c\x48\x09\xaf\x92\x06\xa2\x29\x68\x20\
-\x6f\x00\xd7\x97\x90\x6e\xfb\x90\xfe\x84\xcf\xc8\x3b\x2d\xfa\x85\
-\xad\xdd\xcb\x96\x3b\xc3\xf1\x64\xca\x0d\x0d\x10\x15\x2b\x45\x46\
-\x36\x90\x9e\xa5\x55\x52\x6a\x33\x41\x2f\xd0\x59\x05\xf4\xf4\x2b\
-\x85\x5f\x40\x35\x27\xf6\xcc\x20\x93\x4f\x60\x19\x7e\xdb\xeb\xaf\
-\x0f\x3f\x6b\xfc\x84\x03\xf7\xfe\x91\xf7\x4a\x05\x61\x57\xf7\x85\
-\x5d\x46\xb1\x28\x55\xa7\x6a\x0e\x5a\xb2\xc3\xb3\x90\x06\xbf\x0b\
-\x49\xc0\x60\x41\xb2\xa0\xf7\x09\xfe\xbb\x90\xf9\xbf\x83\x96\x98\
-\x21\xf4\x26\x07\x93\x09\x06\x91\x5e\x47\x73\xe4\x6b\xc2\xf8\x1f\
-\xff\x5b\x5f\xb1\x01\x32\x3d\x16\x75\xea\x70\xa7\x8d\xfd\x91\xdc\
-\xa7\x74\x4d\x39\x84\xc3\xc7\x92\x78\x03\x30\xf8\x67\xd2\x0c\x0a\
-\xc0\xd0\xc8\x3a\x64\xe6\x80\x13\x33\x01\x53\x6a\x46\x2b\x45\x7b\
-\x91\xb0\x08\xc4\xb2\x80\x87\x6f\x11\xfc\x03\xab\x49\x35\x9c\xfc\
-\x02\x6a\xe0\x1b\x54\x89\x13\xe7\xe2\x61\x6e\x6e\x2d\x86\xdf\x38\
-\x76\xac\xdd\xa0\xbf\xf2\xbe\x09\xd6\x75\x61\x38\xd8\x74\x1f\x64\
-\x21\x2c\x0b\xbc\xa1\xd6\x10\x7e\x18\x08\x18\x06\xa9\xdf\xdb\x50\
-\x84\xd3\x30\x90\x4c\x4a\x7a\x93\xf4\x06\x65\x84\xc1\x5c\xfa\x97\
-\xb8\x0c\x40\xcc\xb6\x7b\x45\x93\x50\x77\xd8\x46\xcf\x09\x13\x1d\
-\x84\xed\x5c\xeb\x36\x78\xe3\xe8\x89\x94\x36\x0d\xe0\x1f\x5c\x85\
-\x2c\x35\x7c\xad\x09\x54\x14\xe9\x25\xdc\x1a\x80\xc6\x00\x6e\x94\
-\x09\x02\x82\x6a\x10\x18\x5c\xcb\xfd\xc9\xe4\x1f\x58\x45\x45\x63\
-\x36\x26\x4d\x76\xd0\x89\x7e\x73\x73\x9b\xbf\x7c\x04\xab\xf3\x9c\
-\x0e\x6b\x05\x70\x0b\x3a\x43\x16\xfa\x11\x24\x41\x43\xd5\x7a\x8b\
-\x0c\xf0\xb6\x60\x00\x59\x00\x81\x4f\xa1\x62\x30\xe5\x6d\xd2\x50\
-\xce\x0c\x72\xbf\x81\x9c\x01\xe2\x76\x6a\x97\x7b\xbd\x96\x74\x7e\
-\xf5\xce\x6a\xfd\x26\x1f\xe2\xd6\xf2\xa9\xff\xc7\x21\xc7\xc4\x36\
-\x0d\xe0\xe9\x5b\x8a\xec\x5c\x70\xca\xd2\x88\x0c\xe0\x1b\x58\xce\
-\x3d\x0f\x28\x18\x80\xd2\x7f\x20\x19\x25\x28\xa4\x96\x17\x99\x20\
-\x30\xb8\x86\xeb\x04\x66\xcd\x3e\xa5\x9f\xfa\xcf\xfc\x9d\xf7\x4e\
-\x06\xf8\x42\x67\x9b\xb9\x2b\x81\x0f\xa1\x22\x30\xf8\x1d\xb5\xde\
-\xe6\xd2\xbf\xd4\x6f\x28\xa4\x3e\x6f\xa0\x35\xf1\x5d\x4a\x57\xef\
-\x91\xe8\xcf\x94\x61\x50\x86\x0d\x22\x03\x3c\x4f\x35\xc0\x03\xda\
-\x9d\xbe\x4b\xbb\xf4\xbe\xd3\xd2\xbf\x03\x83\xf1\xc3\x8f\xa7\x70\
-\xe4\x78\xb2\xd1\xf1\xdf\xd9\xa3\x90\x80\xab\x90\x93\x07\x4e\xd9\
-\x6a\x05\x85\x57\x73\x53\xc0\xfc\x22\x10\x6f\x00\x7f\x4a\xf3\x21\
-\x61\x75\x08\x09\xad\xe5\x14\x4c\xf2\x09\x2a\xc5\x9a\x75\x2e\xfa\
-\xf0\xd3\xa9\xd5\xfc\x5b\x1f\xf5\x4a\xc0\x1e\x12\x1b\x20\xf3\x18\
-\xb5\x77\xa1\xc3\xc9\x04\xef\x91\xde\xe5\x24\x65\x06\xf0\x25\x03\
-\x78\x0f\x81\x92\xed\x38\x4e\xfb\x2f\x69\x04\x99\x60\x38\x5a\x13\
-\xde\x41\x83\xf3\xf3\xa8\x38\xaf\xed\x02\x3c\x16\x74\x5c\x72\xa7\
-\x19\x20\x94\x01\x59\xbe\xd2\xd5\xa8\x01\x9c\x9c\xf3\x28\xd2\x5b\
-\x91\x9b\x4f\xf0\x35\x22\xf8\x11\x31\xf5\xc2\x1a\x80\xc6\x00\x3e\
-\x01\x65\x08\x0b\xaf\xe3\x14\x1a\xc6\xcb\x2f\xb8\x1c\x36\xf6\xa1\
-\xfa\xf0\xe5\x63\xc6\xda\xbe\x76\x33\xde\x3f\x41\xcb\x17\x4e\x1c\
-\xfd\xad\x1f\x19\xe0\xbf\x90\x86\x8d\xe0\x8c\xc0\x29\x80\x19\xe0\
-\x4d\x32\xc0\x60\x34\xd2\xb0\x80\xf4\x8f\x78\xa5\x7d\x48\xfa\x00\
-\x52\x8f\x17\xd1\x70\xfd\x19\x44\x6c\xec\x29\x9e\x01\x3c\xea\xb1\
-\xb0\xe3\xd3\x77\x8a\x01\xb8\x0f\x77\xfa\x6d\x4f\xa8\x81\x01\xce\
-\x5f\xc9\xa2\x31\xbe\x19\x79\x05\xe0\x94\xab\x56\x5c\xa2\x94\x5f\
-\x03\x10\x19\xc0\xd3\xb7\x18\x11\x91\xf5\x08\x8f\xa8\xe3\x14\x46\
-\x0a\x0a\xad\xc2\x99\x4b\xc9\xdc\x46\x11\xdd\x71\xdf\xfa\x87\x9b\
-\xf5\xfe\xd9\x31\x2d\xc2\x73\x06\xcb\xbb\x53\x21\x48\x06\x08\xff\
-\x40\x2d\xfa\xef\xa0\x77\xb9\xf4\x2f\xf5\x1a\x44\x7a\x1d\xaa\xb4\
-\x8f\xa9\x70\xf9\x84\x4c\x40\x7f\xa6\x8f\xa4\x76\x90\x5a\xc6\x6b\
-\x4f\xa3\xea\xfc\x63\xf0\x5a\xd4\x49\x7f\x32\xe8\xa8\xfb\x82\x0e\
-\xff\x7f\x3f\x20\x7a\xfa\x77\x8e\x3d\xd9\xa2\x0f\x03\x74\xc8\x31\
-\x89\xc6\x7f\xad\x01\x4e\x9f\xcf\x40\x6a\x7a\x13\xf2\x0b\x21\x28\
-\xaf\x90\x4d\xf3\x36\x71\xe0\xd9\x79\x40\x6c\x11\x88\x19\xc0\xc5\
-\xb3\x80\xe0\xd7\x21\x32\xaa\x1e\x11\x6a\x85\x46\xd4\x52\x41\x98\
-\x8b\x6f\xa7\x1f\xd1\x8f\xfe\x9b\xfa\x3c\x1d\x41\x5a\xaa\xb3\xc3\
-\xd8\x87\x8a\xbe\x88\x8f\xb4\x62\x19\xc1\x67\x08\x6f\x00\xcf\xff\
-\xa0\x99\x7b\xa2\xf8\x0b\x32\xc1\xe7\xa4\xcf\xd0\x1c\xfb\x1e\x67\
-\x00\xb6\xf7\xaf\xec\x64\x3f\x78\xea\x9a\x00\xea\xe9\xe8\xd3\x64\
-\x84\x67\xff\xdf\x19\x60\xea\xb4\x23\xaf\xf3\x07\x3b\x9c\xe6\xa2\
-\x5f\x53\x00\xb2\xe2\x2f\x31\x45\x86\x82\x22\xe8\x28\x23\x4b\xc9\
-\x01\x17\xaf\x02\x5e\xa3\xe2\x2f\x22\xaa\x16\x51\xd1\x0d\x6a\xd5\
-\x73\x46\xf0\xf4\x2f\xc2\xfc\x85\x17\xf4\xe1\xa7\x8e\x1d\x67\xd7\
-\xeb\x26\x1b\xe0\x43\x31\xb0\xfc\x73\xaf\x50\xe4\x8f\x84\x34\xf2\
-\x13\x5e\x11\x23\xd5\x06\x78\x1d\x12\x8f\x57\xd1\x14\x36\x8c\xaa\
-\xd7\xaf\x49\x5f\x91\xbe\x84\x2a\xe3\x0b\x1a\x02\x9e\xe6\x9e\xfb\
-\x67\x4f\xfe\x54\x9e\x7e\x08\x41\xab\xbb\x1a\x5b\x19\xf4\xbb\x7d\
-\x97\x77\xcd\x6d\x96\x51\x95\xbf\x99\x8a\xae\x6f\xc7\x4f\xb0\x7f\
-\x7f\xe2\xc4\x83\x03\x08\xfe\x00\x6a\x01\xcf\xf3\x1b\x39\xdd\x04\
-\x03\x1c\x3b\x95\x82\xe8\xb8\x7a\x14\x15\x03\x85\x22\xe5\xe4\xb7\
-\xe0\x9a\x6b\x9e\xce\x2a\x20\x33\x43\x28\x15\x82\x31\xb1\x0d\x82\
-\xa2\x63\x1a\xa8\xdf\x67\x2b\x7c\x5e\xfa\xf0\x65\x94\x69\x06\xde\
-\xec\xdf\x8d\xc0\xdc\x4b\x6a\x15\x4e\x1e\xb1\x79\x0c\xb2\xb0\x8f\
-\x20\x8b\xfa\x8c\x57\xe4\xa7\x54\x08\xbe\x4d\xd1\xcf\x1b\x40\xea\
-\xf3\x3a\x55\xb0\xa3\x49\xa3\x78\x65\x7d\x03\xb9\xcf\x40\xde\x00\
-\x97\x1f\x45\xfd\xa5\x87\x51\x77\xe1\x41\x64\xee\xef\x45\x05\xa1\
-\xce\xfa\x80\xca\x6d\x9e\xd9\xa0\xdb\x0e\x3e\x81\x9f\x73\xa3\x1d\
-\x3d\xec\x43\x1e\xac\xed\xa2\x05\x03\x84\x84\x55\xa1\xb8\x04\x9c\
-\x8a\xd4\x2a\x28\x6c\x85\xab\x67\xa1\xc1\x32\x70\x60\x48\x05\x62\
-\xe3\x1a\x38\x69\x0c\x10\x14\x5a\x09\x87\xa3\x51\x18\x3d\x5a\xff\
-\x75\xac\x67\xdc\xaa\xdf\x91\x7d\x04\xac\x06\x54\xf0\xba\x7b\xa9\
-\x0e\xf8\x00\xb2\xe8\xff\xa9\xf5\x05\xa4\xc1\xc3\x75\x16\x7f\x5a\
-\xd3\x28\x03\xe4\x8c\x21\x59\x90\x09\xcc\xa1\x88\x7c\x97\x7b\xf2\
-\xa7\xe1\xf2\x23\x64\x80\x7e\xa8\x27\x03\xd4\x9f\xbf\x1f\x79\x76\
-\x3d\x6f\xef\x6d\x61\x04\xff\x73\xcd\x59\xbe\xc6\x64\x61\x61\x0b\
-\xab\xf5\xde\x38\x7c\x2c\x99\x33\x80\x8f\x7f\x29\x8a\x4b\xa1\xa3\
-\xa2\x12\x15\xbc\xfc\x4a\x84\x45\x20\x76\x20\x34\x1b\xff\x7d\xfc\
-\x4b\x10\x9f\x20\x41\x5c\xbc\x56\x6c\x28\x38\xef\x94\x86\x09\x13\
-\xec\xf5\x5f\xeb\xd8\xad\xfc\x3d\x09\xcc\x09\xd1\xb6\x6d\x8a\xf8\
-\x61\x90\xc5\x7c\x4d\xfa\x8a\xf4\x25\x64\x11\x9f\x10\xfc\xd7\x84\
-\xc5\x1f\x65\xf4\x47\xfc\x89\x24\xb9\xe3\xb9\xa3\x68\x98\x21\x58\
-\xfa\xaf\xbf\xd4\x1f\xf5\x17\x1f\x22\x03\x3c\x80\xfa\x73\xf7\xa1\
-\xee\xcc\xbd\xf0\xb7\xd4\xd9\x1b\x58\xe7\x3e\xdf\xec\xf6\x78\x20\
-\x74\xfc\x78\xfb\x57\xe8\xc6\xd7\x6b\x20\x7c\x3b\xdd\x11\x9b\xb6\
-\x06\x62\xfd\x26\x3f\x58\x6d\xf0\xc1\xe6\x6d\x81\xb0\x73\x88\xc3\
-\xa1\xa3\x49\x9c\x01\x5c\xdc\x0b\x50\x52\xa6\x22\x41\x2b\x32\x00\
-\x8b\x72\xf1\x2a\x20\x77\x22\xb8\x57\x21\x12\x12\x25\x24\x29\x67\
-\x02\xa6\x18\x1a\x36\xd8\x2c\xe0\x0f\x3f\x1e\xd7\x87\x9f\x4c\x2d\
-\xdf\x2d\xdd\x4f\xe7\x3c\xc7\x6c\xae\x38\x52\xcb\xae\xbc\xca\xc3\
-\x8f\x1b\x05\x59\xec\x37\xa4\xaf\x21\x61\x19\x40\xbd\xf8\x23\xf7\
-\x7f\x93\x2a\xda\xc9\xbc\x72\xf9\x33\x89\xa4\xae\xcf\x71\xe9\x9f\
-\x33\xc0\x79\x66\x80\xbe\x9c\x01\xb2\xf7\xdf\xa5\x93\x05\xdc\xe7\
-\x99\xb5\xff\xe3\x61\x27\x4e\x3a\xf8\x10\xdd\xf8\x5c\x0d\x84\x19\
-\x33\x4e\x60\xaf\x75\x34\x6c\xed\xe3\x61\x77\x30\x01\xf6\x87\x12\
-\x61\x7f\x38\x11\x0e\x47\x12\x39\x03\x5c\xbe\x9a\x43\x29\xbf\x15\
-\x65\xe5\x40\xa9\x48\x91\xd1\x35\x06\xcb\xc0\x57\x5d\x73\x09\x7c\
-\x03\x12\x93\xa4\x82\x98\x19\xbc\xfc\x8b\xb1\x6c\xc5\x55\x7d\xf8\
-\x52\xca\x42\xb7\x7c\x3f\x1d\x81\x79\x47\xe7\x10\xea\x43\x4f\xd1\
-\xd8\xff\x39\xe4\xf1\x16\x90\xc7\x99\x93\x46\x53\x56\x18\x2a\x2c\
-\xfe\x48\x5c\x07\x40\x95\x3b\x85\x3f\x37\x38\x7f\x2a\x19\x61\x0a\
-\x9a\x82\x87\xea\xa4\xff\xfa\xb3\xbd\xc9\x00\xf7\xa0\xf6\x54\x2f\
-\x78\x2f\xd2\xa9\x05\x6c\xda\x7b\xe4\xdf\xa5\x99\xdc\x61\x9a\xf9\
-\xc3\x29\xec\xb3\x89\x81\xcd\x01\x82\xef\x90\x80\x03\xcc\x00\x0c\
-\x3e\xe9\x20\xc1\x3f\x7b\x21\x93\x0a\xbe\x16\x94\x57\x80\x13\x33\
-\x01\x53\x42\xb2\x44\x77\x13\x08\x19\x80\xa5\xfe\xd8\xf8\x7a\x24\
-\x53\x87\x90\x9c\x22\xe5\x94\x94\x2c\x45\x40\x48\x39\x7e\xdb\x1b\
-\x60\x30\xc4\x8c\x1e\x6d\xfd\xed\x3f\xf1\x3b\x13\x94\xee\xea\xfd\
-\x7b\xfc\x3e\xc2\x6d\xf7\x43\x16\x3a\x12\xf2\x84\xb1\x64\x82\x31\
-\x9c\x64\xa1\x1f\x08\x06\x60\xb3\x7f\xcd\x49\xdf\x50\x71\x33\x83\
-\xf4\x1d\x69\x3a\xfd\xfd\x2b\x8a\x7e\xad\x01\xea\x98\x01\x4e\xdf\
-\x83\xba\x53\x3d\x91\xbc\xa3\xb3\xd8\x00\x51\xed\x77\xcc\x1f\x63\
-\xdb\x41\xf3\x09\x5e\x4c\x3f\xcf\x3a\x8b\x7d\xd6\xb1\x54\xe4\xc5\
-\x19\x35\xc0\xf1\xd3\x69\xc8\x2b\x50\xa0\xa2\x12\x82\x98\x09\xd2\
-\x33\xe5\x04\x3f\x43\x67\x15\x90\x45\x7f\x44\x74\x35\x52\xd3\x64\
-\x48\x4d\x95\x21\x45\xad\x88\xa8\x1a\x2a\x1e\xe3\xb9\xb5\x04\x3d\
-\x03\x1c\xfe\x27\x7f\x77\x02\x13\x27\x2c\xe8\x2c\xed\x0a\x69\xe0\
-\x7b\x90\x27\x4e\x20\x8d\xe7\x24\x8b\xfe\x5a\x58\xfd\x6b\x70\x7e\
-\x0e\x8d\xa1\xc3\xa9\xbd\xf9\x91\xf4\x03\x69\x26\x54\xf9\xdf\x51\
-\x1d\xf0\x88\x7a\xfc\xe7\xd3\x7f\xdd\xe9\xbb\xc9\x00\x3d\x50\x75\
-\xb4\x9b\xf8\xf1\xb0\x26\xaf\x45\x66\xed\xf3\xc9\x60\x8a\xb8\x77\
-\xc5\x9b\x39\xf7\x5a\xc7\x60\xbf\x4d\x9c\x51\x03\xb0\x71\x3f\x2b\
-\x5b\x8e\xca\x2a\xe8\x28\x2f\x5f\x81\xb3\x17\x33\x0d\x96\x81\x03\
-\x29\xca\xd3\xd3\xe5\x48\x4b\x97\x71\x62\x46\x88\x4f\xac\xc7\xc5\
-\xab\x19\x98\x32\xf5\x90\x3e\xfc\x44\x8b\x31\x36\x3d\xfe\x61\x03\
-\x38\xe8\x1c\x45\xef\xf2\x1f\x02\x3f\x11\xf2\xa4\x49\xa4\x89\x9c\
-\x19\xb8\x1a\xc0\xe5\x05\xea\xfb\x9f\x85\xd4\xe3\x65\xfe\xc8\xd9\
-\xa2\x9f\x78\x91\x19\x64\xde\xaf\xa9\xd3\x7f\x1f\x2e\xfd\xd7\x51\
-\xfa\xaf\x3b\xd9\x1d\x75\x27\xba\x21\x68\x79\x07\xd1\x7a\x81\xd9\
-\xc0\xf6\x69\x00\x73\xeb\x51\xc2\x9e\xbe\x71\x07\xb8\xe8\xdf\x6f\
-\xcb\x1b\x80\x1b\xff\x99\x01\x0e\x25\x70\x63\x7f\x52\x4a\x03\xaa\
-\xaa\xa1\x55\x15\x6b\xfd\x9a\x71\xf1\x4a\xb6\xc1\x3e\x40\x36\xcd\
-\x9b\x41\x59\x81\x53\x86\x1c\xe9\xa4\xd4\x54\x29\x5c\x3c\xf3\x31\
-\xfb\xd7\xb3\xfa\xf0\x25\x94\x0d\x5e\xfc\xa7\x7f\x77\x02\xf3\xa3\
-\xd8\x00\xb9\xc7\x9f\x86\x3c\x76\x34\x1a\x93\xa7\x70\x92\x93\xd8\
-\xaa\x20\x4b\xff\x6c\xee\x9f\xcd\xfe\xb5\x66\x53\x0d\x50\xf4\x0b\
-\x69\x16\x27\x45\xcc\x27\x06\xe9\x9f\x33\xc0\xf1\x6e\x48\xde\xa6\
-\xed\x06\xbc\x16\x9a\xb5\xcf\x1d\x43\xe6\x16\x36\x3f\x68\x40\x4c\
-\x9e\x72\x98\xc6\x7e\x3d\x03\xa8\x0b\xc0\xe8\xd8\x1a\x54\xd7\x40\
-\x47\xe5\x15\xad\x70\x72\xce\x35\xd8\x05\xc4\x26\x7f\x32\x09\x7c\
-\x56\x56\x23\x32\x99\xe8\xbf\x99\x7c\x02\x4a\xb0\x66\x9d\x9b\xb1\
-\x71\x7f\xf2\xbf\xf1\xbb\x13\x98\x41\x3a\x1f\x41\xbb\xfb\x41\x6a\
-\xff\x3e\x47\x63\xca\xb7\xa4\x69\x9c\x64\x61\x1f\x73\xe9\x9f\x33\
-\xc0\xd5\xa7\xa0\x88\xfd\x1f\xb9\x7e\x2e\x69\x0e\xe9\x57\xb4\xe6\
-\xce\x30\x48\xff\x75\x27\xee\x22\x03\x74\x45\xa1\xad\x76\x8a\xd8\
-\x7b\x91\xd9\x98\x76\x3a\xe3\x67\xbd\x41\x7b\x6e\xef\x59\xa3\x06\
-\x08\x0c\x2e\x43\x6d\x2d\x50\xa3\x11\x33\x40\xb5\x0a\x6e\x9e\x05\
-\x06\xcb\xc0\x17\x9d\xb2\x28\xdd\x4b\x91\x9d\xd3\x88\xec\x6c\x5e\
-\x59\xa4\xd0\x88\x4a\xec\xb3\x0d\x33\x36\xb7\xe0\xf0\x6f\xfd\xee\
-\x04\xa6\x0b\x3b\xbc\x59\x03\x29\x70\x75\x4f\xc8\x82\x86\xa3\x31\
-\xf5\x3b\x41\xf2\xb8\xb1\x5c\xfa\xe7\xe7\xfe\x9f\x84\xcc\xf7\x0d\
-\x6a\x77\x16\x52\xbf\xbb\x80\x34\x9f\x93\xc4\xf9\x69\xad\x01\x4e\
-\x6a\x0d\x50\x79\x58\x5b\x08\x7a\x2f\x36\x9b\xd9\x5e\x57\xf6\x84\
-\x83\x9b\x17\x2f\xb9\x6e\x60\x00\x36\xfe\x5f\xbc\x9c\x8d\x2b\xd7\
-\x72\x70\x9d\x22\x9b\x41\xf7\xa6\xf4\xee\xec\x96\x6f\xb0\x0c\x7c\
-\x86\x8a\xc0\xc4\xe4\x7a\xe4\xe6\x36\x71\xca\xc9\x6d\x44\x0e\x19\
-\x21\x81\xc6\xfd\x63\xa7\x13\xf5\xb7\x73\x33\xc5\x53\xea\xff\x57\
-\x1f\x9d\x26\x38\x61\xa2\x8d\x9d\x68\xf0\x1c\x84\xc6\xf4\x99\xbc\
-\xd2\xbe\x27\xcd\x40\x03\xab\x01\xd4\x8b\x3f\xcc\x04\xaa\x12\x32\
-\x40\xd9\x12\x32\xc2\x62\x4e\x4d\x21\xc3\x0d\xc6\xff\xba\xe3\x5d\
-\x50\xeb\xa8\x35\x80\xcf\x62\xb3\xef\xdb\x1d\xfc\x09\x13\xec\xd9\
-\x47\xb8\xca\x85\x73\x7a\xb6\x06\xb5\x59\x00\x6a\x5a\x40\xb6\x02\
-\x28\x5e\x04\x12\xef\x02\x8a\x8a\xa9\x46\x7e\x7e\x13\xf2\xf2\xb4\
-\xca\xc8\x94\xe1\xf2\xb5\x2c\xee\x14\x30\x3d\xf8\x0d\x63\xc6\xd8\
-\xfe\xeb\xcb\xa6\x04\x67\x9f\x78\x18\x28\x3e\xf3\x0c\x8d\xff\x53\
-\xd1\x94\xf1\x23\x99\x80\xe9\x07\x48\x7d\xdf\xe2\xd2\xbf\x66\xf1\
-\xa7\x39\x75\x0a\x8d\x7f\x96\x64\x82\x65\x9c\x9a\xd3\xa7\xaa\xd3\
-\x7f\x4f\x21\xfa\x79\x03\x74\x12\x1b\x60\x42\xbb\x33\x00\x45\xa4\
-\x50\x00\x4e\x9e\x7c\x98\x2f\x00\xff\xa2\x01\x02\x82\x4a\x51\x40\
-\xed\xa1\x46\xf9\xd4\x19\x30\x03\xb8\x7b\x17\x62\xc1\xa2\x4b\xfa\
-\xf0\x55\x34\xee\x8f\x6f\x0f\xf7\x80\xe0\x4c\x15\x1b\x20\xd5\xb6\
-\x1f\xe4\x31\xa3\xd1\x94\x39\x8b\x4c\xc0\xf4\x33\x64\xe1\x9f\x71\
-\x91\xaf\x59\xfc\x69\x0c\xfd\x90\xfa\xdf\x55\x64\x82\x95\x9c\x54\
-\x65\x96\x54\x08\xde\xa7\x93\xfe\xeb\x8e\x75\x46\xc9\x01\x1d\x03\
-\xbc\xd6\x1e\xd3\xbf\xb3\x36\xfd\x3b\xff\x69\x03\xb0\x55\x40\x36\
-\xee\xbb\x7b\x15\xa2\xb0\xb0\x89\xa4\xd0\x51\x40\x48\x19\x77\x12\
-\xb8\x91\xa2\xcf\xb6\xbd\xdc\x03\x82\xf3\xa2\xd8\x00\xe1\x1b\xef\
-\x81\x2c\x64\x24\x9a\xb2\x7e\x25\xcd\x26\x23\xcc\x46\x63\xd2\x14\
-\x3e\xfd\xab\x17\x7f\x24\xd4\x15\xa0\xd2\x8a\x4c\xb0\x56\xad\x35\
-\xd4\x0e\x0e\xd2\x49\xff\xcc\x00\x99\xbb\x84\x2e\x40\x12\x68\x69\
-\xd6\xa9\x9d\xf5\xff\xfb\x9f\xd3\x7c\x74\x0b\xdb\xda\x7d\x90\x2a\
-\xfd\x93\xa7\xd3\x70\x9e\xfa\xf9\xab\xd7\x72\xe1\xe6\x51\x00\x1f\
-\xbf\x62\x04\x51\x01\x18\x4e\x05\x5c\x4c\x6c\x35\x12\x93\xea\xa8\
-\xc0\x6b\xa0\xc2\x4e\x46\x11\xde\x88\xe2\x62\x05\x49\x29\xa8\xa8\
-\x48\x21\x28\x36\xbe\x06\x36\x0e\x91\xfa\xdb\xb9\x99\x62\xe8\x6b\
-\x77\xb5\x23\x03\x74\x24\x35\x68\x0c\xe0\xb9\xa8\x33\xb7\x1b\xa8\
-\x29\x7b\xae\x5a\x73\x38\x33\x70\x85\xa0\xfa\xdc\x5f\x36\xfb\xd7\
-\xca\x3e\x7c\xa2\x72\x03\x69\x3d\x27\x45\xfc\x18\xa1\xfd\xd3\x18\
-\x20\x6e\xa3\x30\x0f\xe0\xd9\x1e\xa3\x5f\x98\xfd\x5b\xbe\xc2\x19\
-\xa5\xa5\x4a\x54\x56\xb4\x70\xaa\xa8\x68\xe6\x55\xde\x8c\x72\x8d\
-\xca\x9a\x51\xa6\x11\x7d\x6f\xa9\x46\x25\x4a\x94\x68\xa4\x36\x42\
-\x46\xa6\x94\x86\x85\x64\x4c\x98\xe8\xa0\x0f\xbf\x9e\x8a\xbe\x76\
-\xb7\x4b\x86\x00\xf9\xea\x9c\x44\x7a\xe9\x39\x0e\xba\x22\x67\x01\
-\x69\x3e\x27\xb6\x49\x54\xbc\xfa\xa7\x88\x1b\x43\xad\xd0\x66\xa0\
-\x8a\x69\x13\x54\xc5\x96\x6a\x03\x74\x15\x0c\x10\xb4\x5c\x98\x04\
-\x9a\xdb\xde\xe0\x3f\x4a\x6a\xd5\x9e\xd3\x6b\x47\x51\x9f\x8d\xaa\
-\xaa\x16\x54\x55\xf2\xaa\xac\x6c\xf9\x4b\x86\x28\x2c\x68\xa2\xa2\
-\x2f\x1b\xdf\xcf\x3c\x6e\x64\xdc\xdf\xdf\x2e\x7b\x61\x82\xb4\x5d\
-\x6c\x80\xec\x83\xfd\x29\xed\x4f\x85\x22\x77\x91\x5a\x0b\x21\x8f\
-\xf8\x52\xbd\xf6\xff\x30\x37\xf7\x2f\xf3\x1e\x42\xfd\xf0\x76\xb5\
-\xb6\x91\x19\xb6\x42\x72\xed\x29\x01\x3e\x2b\x00\xdd\xe6\xf1\x9b\
-\x42\x7c\x97\x98\x3d\xd9\x1e\x33\x80\xa7\x18\xd0\xac\x5f\xce\x23\
-\x31\xb1\x96\xfa\xfb\x16\x54\x57\xf1\xfa\xa3\x86\x60\x43\x41\x66\
-\x26\x5b\xe1\xab\x85\x8b\x87\xd1\x99\x3e\x36\xee\xb7\xdb\x47\xa7\
-\x09\xd2\x58\xb1\x01\x62\x77\xf4\x86\x3c\xf2\x4b\x28\xf2\x96\x92\
-\x96\x70\x6a\x4a\x9d\x29\xa4\x7f\x6e\xf1\x87\xb2\x80\xaa\x6a\x2b\
-\x50\xfb\x1b\xaf\x9a\x9d\x68\x0c\xfb\x54\x30\x80\xa8\x00\x8c\x68\
-\xaf\x13\x40\xec\x23\x5c\xab\xc5\x90\x56\xaf\x71\xa7\x28\x56\xa0\
-\xa6\xa6\x15\x35\xd5\x4c\x2d\x82\x21\xca\xe8\xeb\x59\xd9\x6c\x2d\
-\xbf\x06\x21\x61\xe5\xf0\xf2\x2d\xc2\x55\x97\x5c\x61\x0d\x80\x15\
-\x83\xfb\x6c\xc3\x31\xe3\xfb\x63\xc6\x26\x7b\x3c\x46\x9b\x5b\x77\
-\x6a\xc7\x06\x78\x4a\x6c\x00\xff\x15\xdd\xb8\x0d\x22\x8a\xfc\x65\
-\x22\x2d\xe5\x3a\x01\xed\xe6\x8f\xbe\x68\xa6\x2e\x01\x75\x7b\x49\
-\x7b\xc8\x04\xbb\xd1\x92\x3b\x5f\x30\x40\xf6\x1e\xa1\x00\xdc\xdb\
-\x6e\x57\x02\x29\x2a\x87\xb3\xe7\xec\xc4\xb0\xb6\x6c\xf1\x40\x74\
-\x4c\x25\x82\xa9\x82\x77\xf7\x2c\xc0\xc5\x2b\x59\x38\x76\x32\x55\
-\xe8\x00\x0e\x1c\x8a\xc3\xee\x7d\x61\xd8\xb4\xc5\x0f\x6b\xac\x3c\
-\x60\xb9\xe2\x3a\x66\xcf\x39\xc7\x1d\xfc\xd4\xc6\x2e\xa2\x6c\x73\
-\x73\x9b\xbe\x66\xed\xfc\x22\x50\x95\xc2\x84\xd0\x1c\x33\xd4\x5d\
-\x7f\x1e\x8a\x02\x4b\xd2\x72\xb5\x2c\x21\xf1\x79\x53\xb4\xf6\xdf\
-\x07\xf2\x90\x8f\x81\x7a\x1b\x92\x35\x99\x60\x3f\x99\x60\x0f\xea\
-\xd9\x8c\xa0\x6e\x07\x10\x1f\xb2\xd2\xec\xd1\x76\xfb\x8b\x9b\xf3\
-\x87\x36\xd7\xea\xef\xf9\xfb\x75\xce\x45\xac\x5a\xe3\x81\x45\x4b\
-\xae\xd2\xf0\x70\x96\xdb\x1d\xc4\x0e\x7c\xfa\xbd\xa3\xdf\xf4\x54\
-\xfd\x4f\x6c\xee\xb8\x49\x06\x70\x15\x67\x81\x82\x63\xfd\xd1\x94\
-\x31\x1b\xca\xc2\x55\xa4\x95\x9c\xe4\x51\xdf\xe8\x6c\xfe\x68\x70\
-\x7a\x02\x68\xb0\x27\x1d\x20\x13\xd8\x91\x6c\x21\xf3\x19\xca\x19\
-\xa0\xd4\x5e\x67\xab\xb8\x94\xe4\xe8\xb9\xc0\xec\x63\xef\xf6\xb8\
-\x2c\x3c\x69\x92\xfd\x13\x04\x2b\xe0\x4f\xc2\xfd\x3d\xb1\x87\x47\
-\x86\x9a\xdd\x26\x17\x01\x5a\x27\x36\x40\xd2\xde\xbe\x68\x8c\x1b\
-\x0f\x65\xd1\x1a\x41\x4d\x19\xbf\xe8\xec\xfd\x63\xb3\x7f\x2d\xa5\
-\x1b\x01\xc9\x41\x32\x81\x03\x27\x65\xca\x4c\xce\x00\x4c\xa9\xdb\
-\x3b\xea\x1c\x19\xab\xd9\x23\x48\x3a\x45\x66\xe8\xd8\xce\xa6\x85\
-\x0f\x74\xa2\x68\x9d\x47\xd0\x4a\xff\x26\x78\x76\x40\xe4\x49\xd2\
-\xe3\x66\xb7\xd1\x45\x50\xbe\xd4\x39\x49\xc4\xaa\x07\x64\xc1\x1f\
-\x42\x59\xb2\x8e\x57\xb1\x15\x69\x2d\xdf\x0a\x8a\x56\xff\x9a\xe2\
-\xa7\x00\xd2\xa3\xa4\x23\xa4\xc3\x50\x55\xef\x11\xea\x00\x4d\x31\
-\x18\xbe\xda\xcc\xc0\x08\x1e\xf3\xcd\xde\x68\x97\x37\x82\x2d\xce\
-\x50\xbb\x36\x97\x00\x5e\x24\x9d\x55\xc3\x74\x24\x1d\x22\x1d\x20\
-\xd9\x90\xf6\x91\x76\x91\xb6\x92\xac\x48\x4b\x48\xd3\x48\x23\x48\
-\xb7\xe5\xe1\x88\x04\xe5\x61\x9d\x8d\x9c\x0b\x3a\x42\xe2\xf6\x0a\
-\x94\x14\xe1\xca\xd2\x0d\x64\x02\xa6\xf5\x90\xfa\xbc\x25\xec\xfd\
-\x63\x8b\x3f\x52\xcf\x41\x80\xec\x04\xe9\x38\xe9\x18\x99\xc0\x11\
-\x12\xe7\x17\x04\x03\xf0\xea\x84\x8a\x43\x1d\x85\x79\x01\xee\xd1\
-\xf4\xb9\x66\x96\x66\xa6\xab\xdd\x99\xa0\x50\x67\xa7\xf0\xa9\x87\
-\xb9\x1a\xa0\xb9\x6c\x33\xaf\xd2\x4d\x68\x8c\xb6\x10\xad\xfd\xf7\
-\xe4\x4c\xa0\x6a\xa0\x0c\x20\x3f\x4d\x3a\x45\x26\x38\x89\xa6\xe8\
-\x71\x3a\xf0\x35\xca\xd9\xab\xb3\x51\xd4\xcb\x74\xc7\xdb\x9f\x01\
-\x2e\xe9\x3c\x3a\x6e\xdb\x97\xfa\xff\x1f\xd1\x5c\xbe\x8d\xb4\x95\
-\xb4\x05\x8a\xec\x05\x06\x9b\x3f\x94\x39\xcb\x80\xc6\x73\xa4\xb3\
-\x64\x82\x33\x68\x29\xd9\x62\xd4\x00\xb5\x8e\x1d\x41\x63\xbf\xf0\
-\x21\xd2\x3e\x8b\xcd\xba\x9b\xee\x7a\xfb\x32\xc0\x72\xb1\x01\xa2\
-\x37\xf7\x84\x3c\xe2\x6b\x34\x57\xec\x50\x6b\x3b\x67\x86\xfa\x0b\
-\x0f\xe9\xac\xfd\xcb\x43\x3e\x07\x9a\x2e\x91\x2e\x92\x09\x2e\x90\
-\xce\x53\x9d\x70\xbf\x81\x01\x98\xe2\x37\x69\xb3\x00\x99\x61\xa4\
-\xe9\xae\xb7\x2f\x03\x8c\x14\x1b\xc0\x77\x69\x67\x48\xbd\xdf\x40\
-\x73\xd5\x2e\x34\x57\xfe\x46\xda\xc9\x49\xe2\xfd\xa6\xce\xde\xbf\
-\x86\x8b\xfd\x01\xc5\x55\x92\x13\x99\xe0\x0a\xe9\x32\xe4\x81\x23\
-\x0d\xe0\xd7\x39\x76\x42\x99\x7d\x47\xd1\xc7\xc8\x98\x6d\x31\xdd\
-\xf5\xf6\x65\x80\x3e\xe2\x87\x46\x99\xaa\xcf\x3f\xc2\xc1\x6f\xa9\
-\xda\x43\xda\xcd\xa9\x31\x66\x9c\xce\xde\x3f\x56\xf5\x4b\xdd\x07\
-\x43\x99\xbb\x86\x37\x82\xf2\x1a\x94\xd9\x96\x46\x0d\xc0\x14\x68\
-\x79\x1b\x3c\x2f\x70\x07\x9b\x20\x41\x67\xa7\xb0\x7d\x1f\x28\x72\
-\x97\xa1\xa5\x7a\x3f\x69\x1f\x27\x65\xde\x72\x83\xb5\x7f\x8d\x1a\
-\x2e\x3d\x8a\xa6\xa4\x1f\xd1\x5a\x77\x54\xbd\x31\x44\xd7\x00\xd5\
-\x47\x3a\x6a\x16\x89\x98\x5a\xa9\x3d\xbc\xcf\x74\xd7\xdb\x97\x01\
-\xac\x75\x16\x86\xb6\xf5\x40\x23\xf5\xfa\x2d\xb5\x36\x68\xa9\xb1\
-\x56\x6b\x3f\x14\x99\xf3\xd0\x70\xf5\x69\x03\x03\x08\xd2\xd4\x08\
-\x7a\x06\xc8\xf8\x4d\xa7\x13\x68\x21\x03\x3c\x66\xba\xeb\xed\xcb\
-\x00\xe3\xc5\x06\xf0\x5e\xd2\x09\xb2\x80\x11\x68\xa9\x3b\x40\xb2\
-\xe3\x55\x6b\xcb\x8b\xcc\xd0\x98\x30\x15\xf5\x67\xfb\x1a\x31\x81\
-\xf1\xf4\x1f\xb6\x5a\x67\x42\xc8\xc9\x74\xc7\xdb\x9f\x01\xfa\xab\
-\x0f\x7d\x12\x0d\x03\xbd\xa9\xff\x1f\x4b\xd0\xed\xd0\x5a\xef\x40\
-\x26\xb0\x57\x1b\x82\x37\x45\x33\xd5\x07\xf2\xb0\x2f\xf9\x3d\x81\
-\x37\x30\x40\xed\x51\x9d\xf4\xcf\x9e\x1a\xfe\xc6\x74\xc7\xdb\xa7\
-\x09\x62\xc5\x06\xf0\x5c\xd4\x11\x15\xc7\xee\x41\x83\xf3\x00\x28\
-\x8b\xac\xc8\x04\x07\x45\x72\x10\x4c\xd1\x5c\xb6\x15\x32\xdf\x77\
-\x09\x78\x97\xdf\xed\x00\xd8\x81\x52\x9e\x0b\xcd\xee\x36\xdd\xed\
-\xf6\x69\x80\x45\xfa\xe7\xfd\x78\x2d\xea\x80\x22\x87\x1e\xdc\x04\
-\x90\x3c\x72\x34\x5a\x18\xf8\x86\xc3\xa4\x43\xbc\x44\xa6\x50\xe6\
-\xaf\x82\xc4\xe5\x45\x83\xf4\x9f\xb3\x47\x67\xfc\x0f\x33\xdd\xe9\
-\xf6\x6b\x80\xbb\xf5\xa7\x85\x35\xfb\x04\xe2\xb7\x74\x46\xb5\x63\
-\x37\xee\x39\x01\x65\xd1\x3a\xb4\x4a\x8e\xaa\x75\x84\x17\x67\x0a\
-\xde\x18\x8a\xf4\xd9\xd4\x15\x3c\x2c\x18\x40\xaf\x00\x3c\x6a\xba\
-\xd3\xed\xdb\x04\x6f\x91\x6a\x8d\x9c\xfc\x05\x4a\xdd\xc8\xde\xdb\
-\x89\x9f\x05\x8c\x18\x85\x16\x06\x5c\xea\xc8\x4b\xe2\xa8\x63\x8a\
-\x16\xca\x08\x8d\xb1\x93\x50\x7f\xea\x1e\xa4\xed\xe8\x20\x9a\x04\
-\xea\xb0\xda\x74\x97\xdb\xbf\x09\x06\xb0\xc9\x1a\x63\x26\xe0\x9e\
-\x21\x58\xd3\x01\x95\x87\x3a\xa1\xc1\xe9\x29\x34\x17\x6f\x40\xab\
-\xec\x04\xe9\x38\x19\x81\xe9\x98\x8e\x29\x58\xc7\x50\x70\xe9\x6d\
-\xf1\xf1\xb2\xf3\x4c\x77\xf8\xf6\x30\x41\x27\xd2\x6c\x52\xb9\x31\
-\x13\x78\xcc\x37\x43\xd6\xae\x8e\xdc\xa4\x4f\x23\xd5\x06\x0c\xbc\
-\x4a\x7e\x92\x13\x6f\x88\x13\xdc\x70\x20\x8b\xb0\x40\xc4\xfa\x6e\
-\xe2\xe5\xe6\x1f\x4d\x77\xf7\xf6\x32\x42\x4f\xf5\x62\x51\xb5\x31\
-\x23\x84\xae\xea\x80\x8a\x83\x2c\x1b\x3c\x89\xe6\x92\xcd\x50\x35\
-\x9e\x21\x13\x9c\x82\x22\xed\x57\x14\x1c\x7a\x00\xbe\x8b\x75\xbf\
-\xdf\x6d\x7e\x27\x53\x06\xb8\x8d\x0b\x44\x4b\xf1\x26\x52\x51\x5f\
-\x8f\x84\xcd\x1d\x90\xba\xb3\x33\xb2\x9d\xbe\x40\xa2\xdd\xf3\x06\
-\xe0\x45\x06\x58\x6e\xba\x9b\xb7\xf1\x45\x1d\x41\x2f\x17\xfe\xcc\
-\xe1\xf2\xb6\x6a\x84\x36\xa4\x74\x99\xdb\x61\x33\x19\xc0\xb4\x17\
-\xe0\xff\xc3\xe5\x36\xd7\xac\x27\x99\x81\xcd\x1b\x94\xfd\x0e\xf8\
-\x2a\x97\xb9\x1d\x77\xba\xce\xfd\x7f\x78\x80\xb4\xe9\x32\x33\x73\
-\x9d\x6b\xd6\x83\x8c\xb0\x80\x40\xbb\xb3\x87\x41\x49\xe7\x49\x07\
-\x5c\xe7\x76\x9c\x4f\xe0\xdf\x72\x9d\xd7\xe9\xa6\x9f\x16\xfa\x7f\
-\xc1\xff\x93\x2f\x0d\xe2\xa8\xdc\x00\x00\x00\x25\x74\x45\x58\x74\
-\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x31\x30\
-\x2d\x30\x32\x2d\x31\x31\x54\x31\x35\x3a\x33\x30\x3a\x33\x30\x2d\
-\x30\x36\x3a\x30\x30\x43\x7c\x8c\xaa\x00\x00\x00\x25\x74\x45\x58\
-\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\x30\
-\x38\x2d\x31\x32\x2d\x31\x34\x54\x31\x30\x3a\x30\x32\x3a\x35\x30\
-\x2d\x30\x36\x3a\x30\x30\x49\x78\x12\x3a\x00\x00\x00\x00\x49\x45\
-\x4e\x44\xae\x42\x60\x82\
-"
-
-qt_resource_name = b"\
-\x00\x06\
-\x07\x03\x7d\xc3\
-\x00\x69\
-\x00\x6d\x00\x61\x00\x67\x00\x65\x00\x73\
-\x00\x08\
-\x0d\x06\x59\x67\
-\x00\x6b\
-\x00\x65\x00\x79\x00\x73\x00\x2e\x00\x70\x00\x6e\x00\x67\
-"
-
-qt_resource_struct_v1 = b"\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
-\x00\x00\x00\x12\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-"
-
-qt_resource_struct_v2 = b"\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
-\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
-\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x12\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x5e\xba\xa8\xab\x48\
-"
-
-qt_version = QtCore.qVersion().split('.')
-if qt_version < ['5', '8', '0']:
-    rcc_version = 1
-    qt_resource_struct = qt_resource_struct_v1
-else:
-    rcc_version = 2
-    qt_resource_struct = qt_resource_struct_v2
-
-def qInitResources():
-    QtCore.qRegisterResourceData(rcc_version, qt_resource_struct, qt_resource_name, qt_resource_data)
-
-def qCleanupResources():
-    QtCore.qUnregisterResourceData(rcc_version, qt_resource_struct, qt_resource_name, qt_resource_data)
-
-qInitResources()
+# -*- coding: utf-8 -*-
+
+# Resource object code
+#
+# Created by: The Resource Compiler for PyQt5 (Qt v5.9.1)
+#
+# WARNING! All changes made in this file will be lost!
+
+from PyQt5 import QtCore
+
+qt_resource_data = b"\
+\x00\x00\x30\xa7\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x80\x00\x00\x00\x80\x08\x06\x00\x00\x00\xc3\x3e\x61\xcb\
+\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\x00\x48\x00\x00\x00\x48\
+\x00\x46\xc9\x6b\x3e\x00\x00\x00\x09\x76\x70\x41\x67\x00\x00\x00\
+\x80\x00\x00\x00\x80\x00\x30\xe1\x31\x9a\x00\x00\x00\x06\x62\x4b\
+\x47\x44\x00\xff\x00\xff\x00\xff\xa0\xbd\xa7\x93\x00\x00\x2f\xd0\
+\x49\x44\x41\x54\x78\xda\xed\x9d\x07\x78\x14\x55\xf7\xc6\x43\x97\
+\xa2\x02\x36\xc4\xde\xb1\xa0\x9f\x80\x8a\xa2\xc2\xa7\x62\xfd\x2c\
+\x90\xd0\x9b\x88\x58\x10\xe9\x2d\xf4\xd0\xab\xd4\x14\x12\x5a\xe8\
+\x1d\x02\xa4\xf7\xde\x7b\xef\xbd\xf7\x6c\x49\x76\x93\xec\xfb\x3f\
+\x77\x66\x77\x76\xb6\x04\x1b\x68\xf8\xb3\xf3\x3c\xef\x83\x84\x98\
+\xdd\xcc\xef\x3d\xe7\x9e\x73\xef\x9d\xbb\x66\x66\xa6\xeb\x96\x5d\
+\xa1\x56\x77\x3f\x12\xb6\xe1\xde\x91\xe1\x1b\xfb\xcc\x0d\x58\x62\
+\xb6\x9f\x74\x82\x74\x8d\xe4\x49\xba\x4c\x72\x0c\x5a\xd1\x75\x6d\
+\xc8\x9a\x1e\xe6\xc1\x2b\xbb\x3d\x6e\xba\x63\xb7\xf9\x15\xb9\xbd\
+\x5f\x5f\x82\x3d\x89\xc0\x1e\x22\xe5\x90\xf0\x27\xa4\x22\x45\x06\
+\x2d\xef\xbc\x30\xd4\xaa\xd7\xdd\xa6\xbb\x79\xbb\x40\xdf\xd1\xaf\
+\x7b\xf8\xa6\xbe\xe3\x08\x9e\x13\x49\xf1\x27\xa1\xb7\xa5\xca\xa0\
+\xe5\x5d\x16\x84\x59\xdd\xdd\xd1\x74\x87\xdb\xe9\x15\xfd\xdb\x23\
+\xfd\x29\x75\x6f\x24\x58\x55\xc6\x20\x52\x14\x23\xe9\xe0\xcb\xc8\
+\xba\x3c\x02\xc5\xfe\x16\x28\x8f\x9c\x86\xaa\x84\x1f\x50\x9d\xf8\
+\x13\xf7\xdf\xc5\x81\x63\x91\x75\x69\x38\xe2\xad\x9f\x06\x0d\x03\
+\x6d\x19\xc1\x2b\x62\x43\xef\x7e\xa6\xbb\xdd\x8e\x2e\x8a\xf6\xa7\
+\x08\xcc\x51\xfd\x68\xa7\xd4\x4d\xc0\x5f\x42\x49\xd0\x38\xc8\x4b\
+\x57\x03\x8a\x7d\x80\x72\xbf\xae\xd8\xd7\x98\x9a\xf6\x02\x8d\x7b\
+\x00\xd9\x2e\x40\xb2\x13\xad\x55\x9b\x50\x11\x32\x09\xc9\x0e\x2f\
+\x21\x60\x69\x07\x7d\x13\x64\x44\x6e\xec\x6b\x32\xc1\xbf\x1e\xf1\
+\xbb\x1e\x7d\x90\x22\x7e\xaf\x3e\xf8\xd8\x7d\x4f\xa2\x34\x78\x02\
+\x9a\x1b\xb6\x1b\x02\x17\x83\x17\x41\x57\x11\x74\x34\xec\x00\xea\
+\xb6\x01\x35\x5b\x00\x32\x00\x2a\x36\x00\x65\xeb\x20\x4d\x9c\x85\
+\x24\xbb\x17\xf4\x4d\x90\x10\xb5\xb1\x6f\x4f\x13\x85\x7f\xe1\x8a\
+\xda\xd9\xbf\x53\xc8\xea\x1e\xf3\x09\x42\x83\x00\x84\xa2\x34\xf5\
+\xc4\x60\x34\xe4\x2c\xba\x21\x74\x96\x09\x58\xba\xcf\xba\xcc\x52\
+\xfd\x33\x08\xdf\xd8\x9b\xcb\x14\x9a\x8c\x11\xb6\xfe\x1e\xc4\xef\
+\x7d\x02\xb9\x17\x87\x43\x92\xf0\x33\x50\xb2\x16\x28\xa2\xec\x51\
+\xb0\x12\x95\xde\xa3\x11\xb2\xb2\x9b\x60\x02\xfa\xef\xdd\x26\x1a\
+\xff\x74\xba\xdf\x7c\xdf\xeb\x74\xf3\xa3\x74\xc0\x1f\x1f\x04\x79\
+\xf1\x2a\xa3\xd0\x5b\x1b\x77\xa3\x26\x69\x16\x32\xce\xbe\xcd\xd5\
+\x00\x7a\x51\x2c\x25\x45\x90\xae\x93\xae\x92\x42\x75\x4c\x45\x4a\
+\xb4\x7e\x16\x4d\x89\xbf\x00\x59\x4b\x81\xcc\xc5\x90\x86\x4e\x45\
+\xe8\xea\xee\x9a\x7f\x6f\x89\xb0\xba\x7b\x88\x89\xca\x3f\x13\xf5\
+\x9d\x29\xea\x37\xd0\x4d\x6f\x16\xa7\xfa\x86\x9c\xc5\x46\xc1\x2b\
+\xaa\x36\x22\xcf\xf5\x33\x2e\xa2\xf5\xa0\xa7\x84\x6d\xe8\xbd\x3c\
+\x66\xcf\xe3\x83\x93\x8f\xbc\x6a\x50\xd1\x27\x1e\x78\xa1\x6b\xf4\
+\xf6\x7e\x9f\xd3\xf7\x85\x09\xc5\x23\x01\x97\x06\x4f\x06\x52\xe6\
+\x01\x89\x73\x50\xef\x6d\x8e\xc0\x65\x1d\x35\x3f\xef\x8c\x89\xce\
+\x2d\xaf\xee\x1f\x7d\x82\x6e\x74\xb0\x06\x48\xf0\xaa\xbb\xb8\x31\
+\x5e\xa5\x5f\xd4\xd1\xdf\x9b\xaa\x36\x20\xf3\xc2\xbb\x08\xb4\xec\
+\x24\x86\xde\xca\x26\x79\xa2\x76\xf4\x1b\xf6\x47\x5f\x33\x6e\xf7\
+\xe3\x1d\x82\x57\x76\x5b\xaf\x9e\x0b\x40\xb8\xd5\xdd\x68\x8e\x9c\
+\x09\xc4\xce\x02\xa2\x7f\x42\xce\xe1\xd7\x34\x3f\x5b\x19\xb1\xb6\
+\xd7\x23\x26\x4a\xb7\xe8\x0a\x5e\xdd\xfd\x6b\xba\xc9\x35\x1a\x98\
+\x09\x76\xcf\xa3\xa9\x62\x9d\x01\xf8\x16\x2a\xe0\x72\xae\x7e\x28\
+\x8c\xe7\x9a\x14\x4d\x3a\x48\x5d\xc2\xf3\x7f\xf9\xf5\x97\x77\xd9\
+\xab\xf9\x79\x79\x47\x07\x01\x11\x64\x82\xb0\x19\x68\x0e\x98\x84\
+\x60\x4b\xfe\xb5\x42\x56\x74\x9b\x6b\x22\x75\x6b\xe0\xcf\x52\x43\
+\xe4\xc6\x7a\x96\xd2\x55\xac\x72\xd7\x6b\xdf\x2a\xa3\xa7\x23\x7c\
+\x43\x6f\xfd\x54\xef\x47\xa9\xfe\xb5\xbf\x5d\x73\xac\xed\xd5\x8d\
+\x7e\x56\x11\x37\x14\x50\xe6\x41\xc8\xb7\x40\x30\x29\x68\x2a\xd2\
+\xf7\x3e\xad\x79\x2d\x0f\x13\xad\x9b\x7c\x85\xac\xee\x2e\xa4\x5f\
+\x36\x29\x53\x9d\xf0\xa3\x6e\xfb\x46\x6a\xae\xde\x84\x54\xc7\xd7\
+\xf5\xc1\x97\x53\xea\x1e\x77\x53\xdf\xcb\x8a\xae\xcb\x35\x3f\x5f\
+\xea\xfc\x25\xe0\x3f\x09\xf0\x9d\x80\xf2\xe3\x43\x35\xaf\xd9\x10\
+\xb3\xbe\x8f\x69\x86\xf0\x26\xc2\xdf\x29\x9e\xbd\x6b\xc8\x5e\xa4\
+\x05\x2f\xdf\x0d\x48\x7f\x43\x7d\xea\xaf\xc6\xa2\xde\x37\x62\xf3\
+\x7d\xfd\x6f\x7a\xe7\xb1\xba\xe7\xeb\x9a\xd7\xa8\x3a\xfd\x1e\xe0\
+\x35\x16\xf0\xb0\x80\xf4\xc2\x47\xc2\x6b\x47\xac\xe9\xf9\xbc\x89\
+\xdc\xcd\x81\x6f\x29\xdc\xd4\x2d\xf7\xf3\xed\x9d\x68\x86\x0e\xf5\
+\xdb\x51\x16\x30\x56\xbf\xc8\x6b\xf1\x5f\xde\xdd\x2a\x60\xed\x03\
+\x9d\x6e\xc5\x7b\x8a\x59\xdf\xbb\xb3\xba\x90\x44\xd9\xd1\x21\x80\
+\xeb\x68\xc0\xf9\x1b\x28\x2e\x7d\x22\xbc\x87\xc8\x35\xbd\x3e\x35\
+\xd1\xfb\xfb\xf0\xbf\xd7\xa4\xfd\xe8\x9d\xfd\xa1\xa8\x5c\xcf\x45\
+\xbb\x78\x86\x2e\xf7\xf2\x7f\xf5\xa3\xbe\xc1\x73\xc9\x3d\x9f\xdc\
+\xea\xf7\xa6\x29\x44\x2b\x8f\xbc\x01\x5c\xa5\x61\xe0\xca\x17\x50\
+\x9e\xfb\x50\x6b\x80\xd5\x3d\xa7\x98\x08\xfe\x9d\x82\x6f\x55\xf7\
+\x4f\x35\x3d\x7e\xd4\xb6\x07\xa1\x28\xb3\xe2\xa2\x1d\xb5\x5b\x81\
+\xea\xcd\x40\xe5\x46\xe4\x9c\x1b\x66\x30\xde\x5f\x5c\xf8\xec\x3f\
+\x32\x11\x43\xaf\x55\xcf\x5e\xb3\xce\x71\x28\x70\xf1\x53\xe0\xfc\
+\xc7\x68\x3c\x36\x4c\x64\x80\x1e\x33\x4d\x14\xff\xe2\xe5\xb7\xee\
+\xb1\x67\x35\x11\x16\xb9\xf9\x3e\x28\x8a\x56\xea\xcd\xc7\xaf\xe7\
+\xa6\x66\xf5\xe0\xe7\x1c\x9e\x3f\xe2\xb9\x7f\xe2\xfd\xc5\xaf\xef\
+\xdb\x53\x93\x99\x9a\x4f\xff\x17\x38\xf3\x21\x70\xfa\x03\xd4\x39\
+\x68\x0b\xd0\x88\x55\xdd\xc7\x9b\x48\xfe\x85\xcb\x69\xe9\x33\xbd\
+\xe8\x06\x26\x71\x93\x2d\xeb\xef\x45\x53\xee\x52\x2e\xda\x19\x74\
+\x94\x52\xbf\x5f\x6a\x85\x72\x5f\x73\x1d\xf8\x17\xe7\xf6\x57\x4d\
+\x1f\xbb\x3a\x64\xd4\xa8\xfd\x67\xa7\x8e\xdf\xb6\xed\xa7\x29\xeb\
+\x7f\xfa\x7e\xd2\xe6\x21\x3f\x7e\xbb\xbd\xcb\x2d\x99\x88\x5a\xd3\
+\xeb\x4d\x2e\x33\xad\xee\xc1\x81\xc7\xa9\xff\x72\x2a\xde\xfb\x9c\
+\xf0\x9e\xc2\x57\x74\xfb\xc4\x44\xf3\x4f\x5e\xfb\x67\x7d\xd0\x81\
+\x6e\xde\x45\xcd\xec\x9e\x34\xe5\x57\x6e\xf5\x8d\x41\x97\xa7\xcd\
+\x43\x9a\xcb\x74\x5c\xd9\x3d\x1d\x9b\x67\x5a\x60\xe9\x94\xef\x30\
+\x6b\xc2\x02\x4c\x19\xb3\x1e\xa3\x47\xed\x05\xc1\x37\x26\x19\xc9\
+\x69\xda\xd4\x03\xd3\x66\x4e\xb7\xb9\x69\x3b\x78\xc2\x96\x77\x5d\
+\xcc\xde\x63\xce\x8e\xc7\x04\xf8\x38\x39\x02\xa9\x9b\x1e\xd4\xee\
+\x35\x58\xde\xd5\xd4\x05\xfc\xd9\xeb\xda\xfc\xfb\x57\xb2\x9b\x17\
+\xb8\xac\x13\xca\x7c\xcc\x91\xea\xf6\x33\x4e\xee\x5e\x8c\x15\xb3\
+\x96\x60\xac\xf9\x8e\xb6\x20\xff\x51\xd5\x4f\x1c\xb3\x63\xef\x8c\
+\xf1\x6b\x9f\xbc\x09\xe3\x3f\x5b\x24\x42\x83\xc3\x60\x0e\x3c\x93\
+\xea\xf8\x70\x82\xde\x45\x63\x80\x5a\xca\x12\x1d\x4c\x44\xff\xc4\
+\x75\x79\x5e\xbf\xff\xf9\x2f\xee\xd0\xe4\xf8\xcb\xcb\x8a\x15\xdf\
+\x4e\x55\x4d\x34\xdf\x72\x43\xa0\x93\x27\xdb\x63\xc9\xe2\x73\xb0\
+\x5a\x7b\x05\xdb\xb6\x3a\x73\x5a\x67\xe5\x84\x05\xf3\x4f\x63\xe2\
+\x44\xfb\x1b\xfd\xbf\x4d\x53\x2d\xac\x76\xae\x9a\x32\xba\xf7\x5f\
+\x4a\xff\xab\x7b\xbe\xc4\xc6\xff\xe8\xd5\xbd\x80\x13\x04\xff\xc4\
+\x70\x80\xe0\xd7\xd8\x0e\x14\x0f\x4b\x6e\x26\xa2\x7f\xe2\xb2\xfa\
+\x6e\x42\xe7\x2d\x33\xbe\x38\x3d\xd1\x62\x4b\x5d\x5b\xe0\xbe\xfb\
+\xee\x30\x6c\xac\xbd\x11\x12\x94\x8e\x9a\xaa\x3a\xa0\x45\xd9\xa6\
+\x54\xcd\x4a\x94\x14\x55\xc2\xd7\x3b\x19\x3b\x77\xb8\x92\x21\x0e\
+\x18\xfb\x99\x45\x33\xc6\x5a\x7e\xfa\x17\xa2\xff\x28\xd7\xff\xef\
+\x7d\x81\xc0\xbf\xcf\xeb\xd8\x7b\x48\xdb\xf4\x80\x60\x00\x1a\x22\
+\x4c\x1d\xc0\x1f\xbd\xa6\x8e\xdb\xda\x87\x60\x9c\x6f\x0b\xfc\xfa\
+\x75\x4e\x88\x08\xcd\x84\xb2\x51\x01\xb9\xb4\x19\xf5\x75\x2d\x64\
+\x80\x56\x54\x93\xaa\x2a\x5b\x51\x53\xdd\x8a\xba\xda\x56\x48\x1b\
+\x5a\xa0\x90\x37\x73\xf0\x35\x46\x90\x57\x66\xa3\x34\xe6\x1c\x92\
+\x2e\x2f\x87\xe3\xa2\x0f\x60\x37\xf3\x45\x1c\xfc\xe1\x59\x4e\x36\
+\xdf\xbf\x82\x3d\xdf\xbd\xa1\x3a\x38\xeb\x3f\x47\xaf\x2e\xec\x37\
+\xf6\xfa\x82\x3e\x4f\xff\xde\x7b\x8d\x58\xd9\x7d\x20\x6b\x4d\x23\
+\x56\xde\x05\xd5\xb1\x77\x39\xf0\x70\x7c\x0f\x8a\x43\x6f\x22\x50\
+\xbb\x4d\x4c\x41\x05\xe0\x7d\x26\xb2\x7f\xe0\x9a\x38\x6e\xf7\x73\
+\x04\x39\xcd\x18\xf8\x95\x2b\x2e\x22\x39\xb1\x88\x00\xb7\xa0\xb0\
+\x50\x85\x9c\x1c\x70\xca\xcd\x05\xf2\xf2\x80\xfc\x7c\xa0\xa0\x80\
+\x57\x61\x21\x50\x54\x04\x14\x17\xab\x90\x1d\x1d\x8e\xb8\xd3\xf3\
+\xe0\xb7\xee\x39\x38\xff\x6a\xf6\x67\x95\x4d\xb2\x76\x5f\x7c\xcf\
+\xdb\xfa\xef\x35\x72\x65\xcf\x8e\x04\xd7\x9f\x9b\xfc\xd9\x37\x80\
+\xc0\xbf\x2b\x28\x7b\x6b\x7f\x71\xfa\x77\x34\x91\xfd\x03\xd7\xe8\
+\xd1\xfb\xdf\x20\xd0\xd5\xfa\xe0\x59\xba\xbe\x7e\x2d\x01\x25\xc5\
+\xad\x48\x4f\x07\x32\x32\x80\xcc\x4c\x20\x2b\x0b\xc8\xce\x36\x6e\
+\x82\xdc\x8c\x1a\xc4\x5e\xda\x01\xcf\x55\xcf\xfc\x15\xe8\x6d\x29\
+\xcd\x6d\x41\xb7\x9f\x02\x57\xdc\xd7\x8d\x9b\x98\x5a\xd6\x65\x21\
+\xb7\x23\x68\x5d\x6f\x1e\xfc\xd1\x61\x9c\x9a\x1c\x86\x20\x48\x1b\
+\xfd\xad\xa1\x96\x5d\x5e\x34\xd1\xfd\x5d\xf8\xd6\x83\x08\x76\x8d\
+\x3e\xfc\xb9\x73\x4e\x21\x21\xbe\x16\xa9\xa9\xe0\x94\x96\x86\x1b\
+\x9a\x20\x2b\xb5\x12\xe1\xc7\x16\xc3\x75\x41\x4f\x03\x80\x2e\x73\
+\x3b\x23\x70\xf3\xab\x88\x3f\x3e\x0d\x59\x1e\x1b\x91\x1f\x68\x83\
+\x92\xa8\x53\x28\x8d\x3d\x8f\xa2\xb0\xa3\xc8\xf6\xdc\x82\xa4\xb3\
+\xb3\x10\xb2\x6b\x18\xdc\x16\x74\xbf\x91\x11\x0a\x3c\xe7\x9b\x6d\
+\x62\xa9\x3d\x98\xba\x93\x46\x56\xf9\xab\xe1\x33\x25\xaf\xeb\x2b\
+\x8e\xfe\x13\x26\xba\xbf\x73\x8d\x1b\x77\xe0\x09\x82\x5d\xa1\x0f\
+\x7f\xf5\xaa\x6b\x48\x4e\x56\x22\x29\x09\xf4\x27\x90\x92\xd2\xb6\
+\x09\xb2\x32\x95\x88\x3c\xb7\x15\xae\x0b\xef\xd6\x81\xe5\xb6\xb0\
+\x07\x01\x9f\x8a\xf2\xf8\xcb\x68\x69\xac\xbf\x61\xa1\x28\x56\x6b\
+\x93\x04\x95\xc9\xce\x48\x3c\xf5\x3d\x28\xfd\xeb\xfc\x4c\xd7\x39\
+\x66\xf0\x5f\xcc\x03\x2e\xdf\xf3\x1c\x0f\xfe\xc8\x3b\x9c\x2a\xf7\
+\x3c\x2f\x86\x5f\x17\xb1\xe2\xae\x87\x4d\x84\x6f\x0c\xbf\x07\xc1\
+\x8e\xd1\x87\xbf\x71\x93\x17\x81\x57\x21\x31\x11\x9c\x6e\x64\x82\
+\xa4\xe0\x28\x78\xae\x7d\x45\x07\x92\xa7\xe5\x03\x5c\x44\x2b\x25\
+\x15\x7f\x18\x7a\x5b\x6a\x91\xd7\x21\xcf\x6f\x37\x7c\x56\x3f\xc6\
+\xc1\xf7\x53\xc3\xcf\xda\xdc\x8f\x07\x7f\x98\xe9\x6d\x28\x1d\xde\
+\x00\xa5\x7b\xed\x33\x07\x4b\x3b\xce\x36\x11\xfe\x9d\xcb\xc2\xc2\
+\xc6\x5a\x0c\x9e\x86\x02\x58\xdb\x84\x23\x3e\x5e\x85\xb8\x38\x20\
+\x21\x81\x97\x71\x13\xa8\x10\x7e\x6e\x37\xa5\xf6\xae\x3a\x69\x3e\
+\xed\xca\x22\x34\xcb\x6a\x8c\x03\x6d\x2e\x07\x94\xf4\x83\x15\x6e\
+\x40\xd3\x31\xd2\x01\xd2\x1e\xa0\x71\x07\xbf\xa4\xdc\xe8\x40\x7f\
+\x3f\x47\xff\xee\x47\xdf\x47\xee\x6a\x69\x14\xfe\xdf\xba\x2c\x1f\
+\x04\x5a\xf2\x5b\xbe\x13\xd7\xde\x0b\x15\x41\x67\xe0\x71\xe8\x6d\
+\xa8\x0e\x0d\xa5\xd4\xdf\x47\x1c\xfd\x2e\x11\x2b\xba\x9b\x26\x7e\
+\x6e\x18\xfd\xe3\x0f\xbc\x4f\xd0\x5b\x35\xf0\xc7\x8c\xb5\xc5\x11\
+\xc7\x38\xc4\xc4\xa8\x48\x40\x6c\x2c\x38\x13\xc4\xc7\x1b\x9a\x20\
+\x39\x49\x89\x00\x9b\x19\x3a\x51\xef\xb7\xfe\x79\xd4\xe7\x47\x1a\
+\x81\x5e\x45\x40\x7d\x08\xac\x35\x01\xb6\xe2\x25\x5f\x6b\x44\x6b\
+\x78\xc9\x34\x5a\x4d\xda\xc0\x19\xa2\x3c\x72\x17\x82\x56\xf4\xe0\
+\xe0\xc6\xad\xb9\x1b\x2d\x07\xdf\xe4\xc0\x83\xc0\xe3\xe0\x5b\xc8\
+\xdb\xfa\x88\x18\x7e\x49\xc8\xb2\xae\x0f\x98\x08\xdf\xa8\xdd\x9b\
+\xe4\xd0\x89\xa0\x27\x6b\xe0\x8f\x1d\x6b\x87\x83\x8e\xb1\x08\x8f\
+\x50\x22\x2a\x0a\x88\x8e\x46\x9b\x26\x48\x8c\x57\xc0\x67\xc7\x97\
+\x3a\xf0\xa3\xec\xbf\x32\x8c\xfa\xe6\x32\x02\x7f\x89\x80\xaf\xfb\
+\x83\xd0\x57\x1b\xa8\xb9\x66\x29\x32\xce\x68\x57\xf4\xe2\xd6\xf4\
+\x42\x33\xa5\x7a\x1c\xe4\xc1\xc3\xe1\x2d\x54\xee\x7a\x56\xf8\x77\
+\xaa\x0d\x5a\x03\x96\x76\x1e\x66\x22\xfc\x3b\xd7\x98\x31\xb6\x93\
+\x35\xf0\xcd\xcd\x6d\x60\xeb\x10\x01\xbf\xc0\x3a\x44\x52\x00\x33\
+\xb5\x69\x82\xf8\x16\xf8\xec\x1c\xa5\x03\x3f\xe1\xd4\x0c\xa8\x94\
+\x8d\x22\xf8\x72\x02\xef\x41\xd0\xd7\x1b\x00\x57\x11\xe8\xa6\xd2\
+\xf9\xa8\x4f\x9f\x01\x59\xfe\x2c\xa8\xa4\xab\x0c\xc1\xb3\xaf\x91\
+\xaa\x62\xc6\x21\x7c\x83\xf6\x99\x01\x96\xe2\x5b\x38\xf8\x0c\xfc\
+\x9b\x9c\x6a\xf7\xbc\x20\x6e\xf9\xe0\x3e\x97\x34\xbf\x8b\xbd\x89\
+\xf0\x0d\xae\xe9\xdf\x1d\xed\x40\xe0\x33\x34\x06\xd8\xbc\xdd\x17\
+\xd7\xdc\x0a\x10\x1e\x4e\x63\x7a\x38\x10\x11\xd1\xb6\x09\xfc\xed\
+\x17\xe8\xc0\x67\x15\xbe\xaa\xb9\x49\x14\xf5\x25\x04\xde\xda\x20\
+\xca\x5b\x25\x2b\x51\xe8\x39\x12\xe1\x1b\x75\x1f\x02\x09\x59\xd3\
+\x1d\x39\x97\xa9\x80\xab\x5c\x24\x80\x97\x64\x7e\x8f\x04\xdb\x27\
+\x75\xbe\x2f\x77\xf3\xc3\x50\xa9\xa1\x73\xb2\x7f\x03\x75\x7b\x06\
+\xb0\x42\x4f\xf8\x1e\x6a\x0d\xb5\x9d\xc2\xbc\xce\xb3\x4c\xa4\xdb\
+\x4e\xff\x1f\x69\xe0\xcf\x9e\x73\x16\x97\xae\x65\xc3\x2f\x40\x82\
+\xb0\x30\x70\x06\x68\xcb\x04\x21\x97\xce\xe8\xc0\x0f\xdb\x33\x1c\
+\x2a\x85\x5c\x0b\x5f\x49\xad\x81\x7c\x93\xc1\x58\xde\x5c\xb5\x04\
+\x71\xfb\x1e\xbb\xe1\xb3\xfd\x61\xeb\x7b\xa1\x34\xe0\x0b\x24\xd9\
+\x3f\xa3\xfb\x75\xaa\xea\x6b\x76\x3f\xaf\x03\x9e\x89\x45\x7e\xb0\
+\x08\x7e\xd8\x96\x01\xfa\x73\x05\x4d\x6e\x0b\xee\x1a\x6c\xa2\x6d\
+\xe4\x22\xf0\xa7\x34\xa9\xdf\xf1\x64\x22\x9c\x5c\xf2\x10\x12\xa2\
+\x42\x68\x28\x38\x69\x8c\x20\x36\x41\x44\x60\x21\x5c\x16\xf6\x11\
+\x6e\xb0\xd7\x8a\x7e\x50\xd4\x95\x88\xe0\x53\x71\x20\x5f\x67\x30\
+\x96\xb3\x14\x9f\x60\xf7\x94\x00\x2a\x66\xc7\x83\x28\x72\xfe\x18\
+\xd5\x61\x3f\xa1\x3a\x6a\x1d\x32\x2f\xcc\xa0\xca\xde\xf8\x73\xfe\
+\x19\x1b\x1e\x40\xb3\xdd\x20\x01\xba\x46\x65\x3b\x9e\x44\xe0\x12\
+\x6d\xda\xcf\xbe\x32\x91\x9a\x85\x06\x04\x6c\x7e\x55\xdf\x04\x09\
+\xae\x0b\xba\x77\x36\x11\x17\x2f\xf4\x4c\x3b\xdc\x95\xe0\x4b\x99\
+\x01\x16\x2e\xbe\x8c\x8b\xd7\xb2\xe0\xe1\x5d\x8d\xe0\x60\x8a\xf0\
+\x10\xb4\x69\x02\xef\x9d\xe3\x74\x6e\x6e\x45\xe2\x55\x11\x7c\x6a\
+\xd7\x64\x56\x46\xc7\xf2\xf2\xd0\xaf\x05\x50\x39\xe7\xdf\x82\x22\
+\x6b\x16\x14\x99\x3f\xa2\xf0\xea\x7b\x88\xdd\xf9\x90\xb1\xe7\xfa\
+\x91\x44\x2d\x9e\x64\xff\xcb\xba\xe0\x0f\x0c\x81\x8a\xc4\x86\x02\
+\xf1\xf7\xe6\x5d\x7d\x07\xa8\x5b\x4a\x9d\x42\x3c\x24\x45\x71\x70\
+\x99\xd7\x45\x7f\xf6\x71\x91\x89\xba\xe8\x9a\x34\xc9\x61\x84\x26\
+\xfd\xdb\x1d\x8c\xe2\x0c\xe0\xe7\xdf\x84\xa0\x20\x70\x26\x10\x1b\
+\x41\x63\x82\x60\xe7\x60\x9d\x9b\x1a\xed\x30\x4a\x34\xe6\x57\x10\
+\xec\x4d\x06\x05\x1c\xaf\x95\x88\xd9\xc5\x03\x4b\x3d\x38\x00\x8a\
+\x9c\x5f\xd1\x94\xf1\x13\xd2\x0e\x0d\x30\x80\xce\xd2\x39\x8b\x78\
+\xc9\xbe\x97\x0c\xc0\x33\x29\xac\x5f\x45\xe2\x1a\xdd\xfa\xa1\xd0\
+\xed\x7d\xa0\x66\x01\x50\x3d\x9f\xb4\x8c\x8c\x58\x86\xb4\x2b\x4b\
+\xf4\xb3\x40\xbd\xeb\xfc\xbb\xfa\x98\xc8\xab\xaf\xb1\xe3\xec\xd6\
+\x33\xf8\x13\x26\xda\xe3\xc2\xd5\x4c\x5c\xbe\x9e\x8b\x80\x00\x20\
+\x30\x10\x6d\x9a\xc0\x73\xf3\xe7\x3a\x13\x3d\xb2\xf2\x34\xb5\x01\
+\xa8\xf8\x93\x1f\x30\x80\xae\x91\xb2\x62\x81\x00\x4b\x92\x30\x1d\
+\x8a\xec\xd9\x48\x3d\x34\x40\x78\x72\x38\x62\x79\x57\xa4\x6f\xb8\
+\x1f\x95\xbf\x3d\x8b\x16\x71\xaa\x57\x43\x87\x1d\xd3\x60\x54\xff\
+\xf6\x0c\x42\x97\x69\x9f\x27\x64\xcf\x1b\x94\xfb\x7f\x0c\x54\xcd\
+\x05\x2a\x66\x93\x66\x01\x65\x3f\x93\x09\x76\xa1\x59\x5a\x05\x8f\
+\xa5\x7d\xf4\xb2\x40\x27\x2b\x13\x79\xed\xf8\x7f\x95\x19\xe0\xd7\
+\xb9\xe7\xc8\x00\x59\x70\x76\x2f\x85\x9f\x1f\x04\x13\x88\x8d\xc0\
+\x4c\x10\xe4\x9e\xa2\x73\x33\xe3\x1c\x27\x69\xa3\x5f\x11\xa4\x03\
+\x5c\x90\x84\x57\x7d\xea\x34\x7e\x3b\xf6\xe6\xbe\x2c\xfa\x15\x85\
+\xd7\x47\x5c\x88\x5c\x71\x17\xea\xf6\xbe\x88\x96\x03\x83\x0d\xc6\
+\x76\x2d\xf8\xc1\x9c\x14\xfb\x07\x22\x4d\x77\x61\x07\xa1\x6b\xbb\
+\xa3\x3e\xce\x1c\x28\x27\xe0\x65\x3f\x01\x25\x3f\x90\x66\x02\xc5\
+\x33\x80\xa2\xef\xe8\xf5\xa3\x90\xe9\xb2\x46\x3f\x0b\xd4\xb8\xcc\
+\xeb\xdc\xdd\x44\x9f\x37\x00\xd7\xfe\xad\x58\xed\xcc\x19\xc0\xcd\
+\xb3\x0a\xbe\xbe\x68\xd3\x04\xde\xb6\x4b\x75\x6e\x66\x5d\x4e\x88\
+\x3a\xf5\x37\xd0\xcd\xde\x60\x00\x1d\x92\x15\x82\x6a\x13\x26\xf2\
+\x93\x37\xbb\x1f\x81\x24\x76\xda\xcf\xc1\xcb\x3a\xf9\x34\xd9\xbc\
+\xd6\x06\x74\x35\x78\xdb\xc1\x68\xb5\x79\x1d\x85\x9b\x1f\xd1\xa9\
+\xf2\xf9\x9f\xf3\x10\x0d\x21\x93\xd4\xc0\xbf\xe7\xa1\x17\x4e\x27\
+\x4d\x03\xf2\xa7\x00\x79\xf4\x6f\xc5\x96\x68\xaa\x2d\x30\xa8\x05\
+\xa8\x2d\x9c\x68\x1a\xff\x27\x1f\x64\xb3\x7f\xcd\xcc\x00\xeb\x36\
+\x7a\xe0\x22\x19\xc0\xd5\xbd\x16\x3e\x3e\x10\x4c\xe0\xef\x0f\x9d\
+\x21\xc1\x75\xd9\x53\xc2\x4d\x0c\xd8\xf4\xb2\x36\xfa\x9b\xbc\x0c\
+\x80\xf3\x5a\x0e\x34\xf0\x92\x66\xcf\xe4\xb7\x63\xaf\xbf\xa7\x31\
+\xdd\x7e\x40\xa7\x9c\x4d\xfd\x94\x3a\xe0\x45\xd0\x99\x5a\xac\xff\
+\x83\xa2\x2d\x8f\x22\x5c\xaf\x2b\x08\x5c\xd6\x01\xf9\x97\x07\x43\
+\xc5\x22\x9c\xa9\xf0\x5b\xa0\x60\x2a\x41\x9f\x0c\xe4\x4e\x04\x72\
+\xc6\x03\xd9\xe3\x48\x63\x80\x2c\x0b\x32\x64\x12\xe2\x8f\x7c\xa3\
+\x9f\x05\xdc\x4d\xe3\xff\x58\xbb\x3e\x9a\x02\x70\xc3\x66\x2f\xae\
+\x00\x74\xf3\xa8\x87\xb7\x37\x8c\x9a\xc0\xdf\x25\x4d\xe7\x26\xa6\
+\x5f\xb5\xd4\x8e\xfd\xd2\x2d\x5a\xe0\x22\xe8\xbc\x2c\x39\xa9\xa8\
+\x3a\x0f\x5e\xc5\x60\x76\x80\x97\xdd\xfc\xdf\x2a\x69\x2c\x37\x04\
+\x3f\x08\xf2\xbd\x2f\x23\x6f\x63\x3f\x1a\xe7\x3b\x19\x14\x87\x2c\
+\xea\x25\x31\x5f\x69\xa3\x3c\x9f\xa2\x3c\x77\x02\x41\x67\xc0\xc7\
+\xf2\xc0\x33\x69\x48\xc8\x18\x0d\xa4\x7f\x03\xa4\x7d\x09\x94\x5a\
+\xa3\x3e\xe5\x84\xe1\xbc\xc0\xbc\x8e\x77\xf6\x81\x51\x63\xc6\xda\
+\x3e\xae\x31\xc0\xaa\xb5\xae\x9c\x01\x3c\xbd\x25\xf0\xa2\x60\x36\
+\x66\x02\x6f\xc7\x83\x3a\x37\xb1\x26\xc3\x57\x3d\xf6\xa7\xb4\x09\
+\x9d\x53\xfd\x32\x41\xe9\x27\xf8\x9d\xb9\x67\x96\xbe\x81\x92\xed\
+\xcf\xea\x40\x67\xd1\x1e\xbb\xb2\x87\xd1\x39\x80\x88\x8d\x77\xa3\
+\x22\xe4\x17\x02\x3e\x4d\x2f\xca\x35\xd0\x09\x78\x06\x75\x23\x69\
+\x64\x8e\xb4\xff\x01\x29\x5f\x00\xc9\x9f\x01\x49\x9f\xd0\xdf\x27\
+\x41\x25\xcd\x47\xf8\x86\x5e\x7a\xc3\x40\x87\x3b\xfb\xe1\x50\x8b\
+\x31\xb6\x03\x34\x06\x58\xb2\xcc\x49\x6d\x80\x06\x78\x7a\xc2\xa8\
+\x09\xdc\x77\xcf\xd2\xa9\xfe\x85\x0d\x1d\xf2\x4b\x6d\x43\x67\x3d\
+\x79\xdd\x12\xa0\x76\x31\x69\x11\xe4\x59\xd3\xb9\x14\xce\x2d\xe1\
+\x5a\xf5\x41\x32\xf5\xf8\xe2\x8a\xde\x98\x8a\x9c\x06\x41\x95\xff\
+\x23\xbd\x56\x39\x19\xe0\x27\xdd\x28\xcf\x50\x47\x79\x2a\x01\x4f\
+\xf9\x9c\x80\x7f\xca\x43\x4f\x1c\x09\x24\x7c\x04\xc4\xfd\x17\x88\
+\x1d\x4e\x43\x54\x39\x4a\xce\x0d\xd4\xeb\x06\x3a\xac\xbf\xb3\x0d\
+\x60\x61\xf3\xa4\xc6\x00\xb3\x7e\x39\xcd\x4d\x01\xbb\x7b\xd6\xc2\
+\xc3\x03\x46\x4d\xe0\xb6\xe1\x63\xe1\xe6\xf9\x6f\x78\x51\x3b\xfe\
+\x4b\x77\x19\x42\x57\x03\x47\xcd\x42\xbe\x2f\xaf\x9a\x47\x9a\xc3\
+\xb5\x69\x85\xd7\x86\xb6\x09\x3b\x68\xb9\x6e\xda\x4f\xdc\xfb\x10\
+\x45\x39\x45\xbb\x3c\x06\x40\x23\x15\x76\x54\xed\xa7\x7f\x6d\x18\
+\xe5\x89\x1f\xf3\xd0\xe3\x3f\x20\xe8\x23\x80\x98\xf7\x49\xef\x91\
+\xde\x05\xa2\x87\xd1\xfb\x08\x84\x2c\x6c\x2a\x7c\x2d\x75\x8a\xc1\
+\x0b\x77\xb4\x01\xcc\xcd\xad\xef\x17\x96\x7f\xc7\xd9\x71\x45\xa0\
+\xaf\x7f\x35\xdc\xdd\x61\xd4\x04\x2e\xcb\x5f\x12\x6e\x5e\x84\xed\
+\x67\xea\xea\x5f\x4e\xc0\xf5\xa1\xb3\xc9\x98\x79\x7c\x5f\x5e\xf9\
+\x2b\x41\xff\x85\xef\xcb\x4b\x7f\xe4\xdb\x34\xaa\xd8\x73\xce\x0e\
+\xfc\xdd\xb3\x7e\xa3\xb7\xdc\x03\x65\x22\x45\x77\x83\x27\x0f\x1f\
+\xf4\x5a\x69\xa3\xda\x8e\x72\x31\x70\xa6\xa8\x77\x80\xc8\xa1\x40\
+\xc4\x5b\xf4\xfa\xe7\xd0\x18\xbf\x1c\xc9\x7b\x74\xe6\x04\x92\xee\
+\xf4\x0c\xd0\x85\xe0\xb7\x68\x4c\x70\xf8\x78\x3c\x02\x82\xcb\xe1\
+\xe6\x06\xa3\x26\x70\x59\xfc\xa8\x68\xd5\x6f\x9a\x7a\xda\xb7\x88\
+\x8f\x72\x06\x5d\x14\xe5\x42\x5f\x5e\xaa\xd7\x97\xb3\x36\xad\x88\
+\xfe\xad\xf6\x28\xaa\xfc\x46\x20\x72\xd3\xdd\x06\xe0\xd9\x71\x6e\
+\x59\x47\x9e\x44\x4b\x32\xa5\x78\x49\x80\x1a\x3e\x49\x16\x77\xe3\
+\x28\x67\x8a\x7c\x5b\x0d\xfd\x4d\x20\x9c\xba\x8b\xd0\x41\x40\xc8\
+\x7f\xa8\x4b\xb0\x47\x53\xf2\x16\x94\x9c\xec\x2f\x36\x40\xb9\x69\
+\x1e\x60\xd4\xfe\x7c\x61\x19\x78\x9b\x0f\xbc\x03\x0a\x09\xb6\xca\
+\xa8\x09\x9c\x17\xde\x2f\xdc\xbc\xa4\xb3\x3f\xab\xdb\xbf\xf4\x36\
+\xa3\x9c\x87\x3e\x5d\xaf\x62\x9f\xc8\x57\xec\xf2\x68\x32\x4f\x1e\
+\x54\x15\x76\x68\x08\xfb\x1a\x25\x4e\xaf\xa1\xe8\xe2\xcb\xa8\x72\
+\x1b\x8c\xe6\x78\x4a\xef\x25\x3b\x79\x73\x69\xe0\x33\xe5\x6f\xb8\
+\x71\x94\x33\xe8\x61\x54\x54\x86\xbe\x0e\x04\xbf\x46\x1a\x48\xbd\
+\xeb\x2b\xd4\xc3\xbe\x44\xaf\xbb\x07\x8a\x0c\x1b\xd4\x3b\x3d\x01\
+\xb7\x79\x1d\x34\xbf\x47\xa3\xc9\x00\xa3\xf6\xfb\x6a\x0c\xf0\xd3\
+\xcf\x27\xe1\xe4\x92\x83\xa8\xa8\x16\xb8\xba\xc2\xc0\x04\x2e\x8b\
+\x1f\x11\x0c\xc0\x76\xe7\xf2\x05\x60\x82\xf1\x28\xd7\xf4\xe5\x79\
+\x6d\x54\xec\x05\x94\x35\x54\x12\x6d\x6a\x57\xe4\x50\x84\xd3\x38\
+\xdf\x98\x22\xfa\xba\x48\x92\x30\x2d\xf8\xb6\xa2\x3c\xf8\x55\x35\
+\xf0\x97\xa9\x6f\x25\xe8\x01\x03\xa8\x7d\x79\x81\x0a\x98\xe7\xc8\
+\x00\x36\x50\xa4\x5b\xa3\xc1\xe9\x71\x04\xae\x14\xf6\x2c\xaa\x02\
+\x56\x74\xed\x70\xa7\x1b\x40\x67\x13\xe8\xc9\xf3\x29\x88\x8d\x93\
+\xc0\xc5\x05\x06\x26\x70\x59\xf6\x82\x60\x80\x98\x43\x16\xbc\x01\
+\x1a\xd3\xd4\x51\xfe\xad\x61\x94\x73\xc0\xc7\xe8\x55\xec\x5f\x69\
+\x2b\xf6\xe2\x6d\x04\x5b\x6a\x08\xdb\x00\x7e\x14\xc1\xff\xa8\x8d\
+\x28\x7f\x55\x1b\xe5\x01\x2f\xf2\xc0\xfd\x9e\x27\xe8\xd4\x62\xfa\
+\x3c\x4d\x63\xd7\x93\x94\xbe\x9e\xa0\xf7\x78\x16\x4d\x29\xdb\x39\
+\x03\x84\xaf\x17\x9e\x31\x90\xde\xf1\x19\x60\xf4\x68\xeb\xa9\x62\
+\x03\x6c\xda\xea\x8d\xd8\xf8\x72\x4a\xf9\x2a\xc1\x04\x4c\xcc\x04\
+\x2e\x56\x1f\x08\x06\x08\xdf\xff\xa1\x7a\x08\xc8\xe7\xa3\x9c\x4d\
+\xc6\x18\xeb\xcb\xb9\x8a\xfd\x4b\x51\xc5\xfe\xa9\xa8\x62\xa7\x9f\
+\x91\x49\xf5\x82\x2c\xd1\x38\x78\x65\x09\x65\x0a\xea\x30\x22\x86\
+\xde\x20\xca\x5f\xd4\x46\xb9\xcf\x33\x04\xfc\x29\x1e\xb8\xa0\xc7\
+\x29\x7d\x3d\x46\x45\x69\x18\x1a\x63\x17\xa3\xe1\xca\x63\x88\xda\
+\xdc\x43\xf3\x7b\x94\x9a\x86\x80\x51\xfb\x9f\x17\x1b\x60\xda\xb7\
+\x47\xe0\xec\x99\x87\xd4\x94\x66\x38\x3b\x83\x33\x81\xc6\x08\x2e\
+\xdb\xbe\x13\x0c\xc0\xf6\xe4\xf3\x5d\x80\x8c\x6f\xd3\x18\x74\x63\
+\x51\x9e\xac\x57\xb1\xb3\x02\xce\x58\xc5\x9e\xcc\xe6\xee\x37\x52\
+\x26\xd9\x47\x7f\x6e\xa6\xbf\xd3\x70\x12\xf6\xe6\x9f\x8b\x72\x01\
+\xb8\x1a\x3a\x93\xc7\xa3\xf4\x27\x7d\x5d\xd1\x00\x59\xf0\x38\x32\
+\xc0\xa3\xe2\x0c\x10\x6d\x32\xc0\xa8\xfd\x6c\x3f\x60\x91\xd8\x04\
+\x36\xf6\xe1\xc8\xc9\xad\x83\x87\xbb\x8a\x33\x81\x60\x04\xbb\xbd\
+\x3a\x13\x29\xc2\x0e\xa0\xbc\x39\x37\x8e\x72\xd6\xa6\x19\xab\xd8\
+\xa3\xf4\xc6\x72\x96\xda\x85\x28\x1f\xf8\xe7\xa3\x5c\x03\xdc\xe3\
+\x11\x52\x7f\x4a\x5b\x4c\x0f\xd3\xcf\x26\x43\xb6\x28\x20\x71\x19\
+\xc8\x19\x20\x68\x95\x50\x03\x9c\x34\x2d\x07\xf2\x26\xb0\x15\x1b\
+\x80\xed\x0b\xf4\x09\x2c\x44\x4e\x56\x0b\xae\x5f\x07\x27\xce\x04\
+\xa7\x42\x74\x77\x01\x25\x5d\xe7\x0d\x50\xbc\xe7\x8f\x45\x39\x57\
+\xb1\xbf\x2d\x1a\xcb\x87\xdc\x60\x2c\x1f\xf0\xe7\xa2\x5c\x80\xfe\
+\xb0\x5a\xfd\xa8\x80\x61\x62\x13\x49\xfb\xd1\x5a\x97\xca\xa5\xff\
+\xfa\xcb\x8f\xc0\x7d\x3e\xdf\x05\xb8\x2f\xe8\xb8\xd2\x44\x9f\x37\
+\xc0\xe7\xfa\x8f\x82\x5d\xba\x9e\x89\xfc\x82\x3a\x04\x07\xa9\x70\
+\xed\x9a\xda\x04\xd7\x95\x70\x9e\xdf\x5b\x30\x40\xca\x85\x39\xbc\
+\x01\xea\x42\xff\xfd\x28\x67\xc0\xdd\xd5\xc0\x99\x5c\x1f\xe4\xe5\
+\x46\xdf\x27\x2f\x81\x22\xd3\x8e\x33\x40\xe9\xf1\x07\x85\xf7\xef\
+\xbd\xa4\xd3\xfb\x26\xfa\xbc\x01\xfa\x8b\xe1\x8f\x19\x63\x8b\x6b\
+\xee\xb9\xf0\xf0\x2b\x40\x4d\x55\x13\x75\x02\x22\x13\x6c\x1c\xa3\
+\xad\x03\xd6\x3c\xc1\x6f\x01\x6f\xa6\x82\x2d\x71\xd4\x0d\xa2\x7c\
+\xd0\xad\x8f\x72\x0d\x70\x97\x07\xd4\xba\x9f\xde\x2c\x29\x8e\x9f\
+\xaf\x90\x05\x7c\xc3\xa5\xff\xf8\xed\xc2\x82\x90\xd4\xcf\xb2\x4b\
+\x57\x13\x7d\x23\x85\xe0\x77\x33\x1c\x71\xdd\x23\x8f\x2b\x06\xa3\
+\xa9\x23\xa8\x2c\x6f\xe6\xe0\x73\x26\x38\x7c\x59\x67\x18\xa8\x4c\
+\x76\x51\x0f\x03\x47\xfe\xbd\x28\xd7\x00\xe7\xa0\xdf\xa7\x56\x5f\
+\xfa\x3b\xfd\x5b\x43\xba\x90\xfe\xeb\x2e\xf6\x87\xc7\xc2\x8e\x9a\
+\xf7\x7e\xd9\x44\x5e\x6b\x80\x21\x62\x03\x2c\x58\x78\x91\x37\x80\
+\x57\x1e\x5c\xbd\xf3\xa9\x20\xac\x45\x51\x01\x5f\x0f\x5c\xbb\xaa\
+\x80\xf3\x42\x6d\x1a\x8d\xb4\xfd\x5c\xbd\x24\x5c\x4f\x91\xff\xc1\
+\x1f\x88\xf2\xa7\x6e\x7e\x94\x6b\x80\x33\x5d\xef\x43\xea\x4d\x6f\
+\xf4\x5e\x2a\x48\x57\x72\xef\xad\x31\x76\x09\x67\x80\x94\x3d\xda\
+\xc7\xca\xbd\x16\x77\x1e\x65\x22\xaf\x99\x0b\x30\xb7\xfe\x40\x6c\
+\x80\xcd\xdb\xbc\x75\x0c\xe0\xe6\x5b\x80\xf2\x72\x29\x4a\x8b\xf9\
+\x4c\x70\x7d\xb7\x95\xee\xb6\xb0\x5c\xf5\xb6\xb0\xb2\x2b\x6d\x44\
+\xf9\x93\xb7\x2e\xca\xaf\xab\xa1\x5f\x53\x43\xbf\x76\x0f\x70\x95\
+\xe4\x43\x59\x48\x51\x87\x56\x49\x1e\x1a\xae\x3d\x8b\xea\x73\xfd\
+\x85\xe2\x8f\x54\xe1\xb3\xb4\x73\x17\x13\x79\xcd\xa2\xd0\x18\xdb\
+\x6f\xc4\x06\x38\xe8\x18\xa3\x63\x00\x9f\xa0\x2a\x84\xc7\xb4\xa2\
+\xa2\xa2\x09\x35\x95\xcd\xf0\x70\xae\x82\xf3\x3c\xed\xc1\x0f\xa1\
+\xbb\xa9\xf0\x6b\x56\xf0\x26\x48\xfc\xf9\x9f\x8d\x72\x01\xfa\xdd\
+\x6a\xf5\xa2\xef\xa1\x9f\x53\x1b\xcb\x1f\x42\x15\x39\x0b\x0d\x4e\
+\x8f\x21\xcc\xea\x2e\xed\x21\x15\xf3\x3a\xae\x31\x51\x17\x5d\xe3\
+\xc6\xd9\x7d\xaf\x3d\xff\xc7\x01\x57\xdd\x72\x70\x9d\xc6\x7f\x17\
+\x32\x80\x57\x40\x39\x22\xe3\x54\x24\x1a\xe2\x63\x55\x28\x29\x69\
+\x42\x93\x4c\x89\xb0\x93\xeb\x75\xb2\x40\x51\xd8\x41\xf5\xcc\x60\
+\x0d\x8d\xff\x1f\xfe\x33\x51\x2e\x86\xee\xd4\x53\x2d\xfa\x7a\xb1\
+\x13\xf7\x5e\x9a\x4b\x3d\xd1\x70\xf5\x09\xa4\xed\xef\x2d\x7e\xaf\
+\x75\xde\x4b\x3a\xf7\x36\x51\x17\x5d\x54\xf5\x6f\xd4\x18\x80\xed\
+\x0e\xd6\x14\x80\x1e\x7e\x25\x04\xbe\x15\x51\xf1\x10\xc4\xcc\x90\
+\x9e\xd5\x00\xa5\xac\x9e\xba\x80\x27\x85\x1b\xeb\xb1\xe4\x1e\x28\
+\xeb\x72\x78\x13\xc8\xf2\x69\x28\x78\xeb\xd6\x46\xb9\x93\x1a\xfa\
+\x15\x8d\x7a\xf0\xf0\x0b\xce\xf0\xe7\x10\xca\x4a\x20\x71\x7f\x13\
+\xf9\x87\x1f\x80\xcb\x1c\xf1\x36\xb0\x8e\x6b\x4d\xc4\x45\xd7\xb7\
+\xd3\x8f\x76\x26\xf0\x09\x9a\xf6\xef\xf4\x85\x14\xce\x00\xae\x3e\
+\x85\x04\xbb\x19\xd1\x09\xe0\x15\xcf\x2b\x34\x4a\x06\x9f\xe0\x62\
+\x84\x46\x97\x21\x2b\xd2\x85\x6e\x6a\x07\xed\x99\x00\x36\xef\x40\
+\xa5\x54\x6f\x13\x93\x15\x50\x41\x38\xfc\xd6\x44\xb9\x06\x38\xd3\
+\x65\xa6\xee\xf4\xfd\xf4\xb3\x4b\xf8\x8e\x44\xa5\x94\x42\x16\x64\
+\xc1\xad\xfd\x8b\x96\x7e\xb9\x23\xe6\x3c\x17\x75\xba\xf3\x9e\x07\
+\x30\x37\xb7\x1e\x60\x61\x61\x33\x7c\xcc\x58\xdb\xf7\xc6\x8d\x3b\
+\x30\x6c\xc2\x44\xfb\xf7\x27\x4d\x3e\x38\x72\xea\xd4\xc3\x33\x09\
+\xbc\xbf\x76\x67\xb0\x27\xa5\xff\x5c\x8a\xfe\x7c\x44\xc4\x28\x10\
+\x9b\x08\xc4\x68\x44\x26\x08\x8f\x69\x82\x77\x50\x11\x67\x00\xdf\
+\x90\x62\xf8\x85\x95\xc0\xdb\xee\x67\x9d\xa1\x20\xcf\xe3\x07\xaa\
+\x07\xa4\xea\xe1\xa0\x96\xfe\xc7\x19\x37\x37\xca\xaf\xa8\x81\x73\
+\xba\x0b\xb8\x44\xf2\x19\x0a\xd4\xa5\xa8\xd7\x26\x1a\xb9\x71\xbf\
+\xe4\xe4\x23\x6c\xa6\x4f\x7f\x0f\xe0\x67\x77\x22\x7c\x76\xf0\x83\
+\xe2\xf7\x0e\x6a\x5e\x6a\xe9\x04\x27\xd7\x1c\x5c\x73\xcf\x43\x78\
+\x74\x23\xe2\x92\xc0\x89\x99\x80\x29\x2a\x4e\x49\xf0\x8b\x79\x03\
+\x10\x7c\x9f\xe0\x12\x5c\x77\x2d\x83\x9b\x67\x31\x5c\xd7\xbd\x23\
+\xba\xc9\x1d\x51\x1e\xb6\x50\x9b\x09\x98\x8a\xce\x51\x31\x38\xe0\
+\xef\x47\x39\x03\xce\x41\xef\xc6\xcb\x89\x7e\x5e\xda\x36\xd0\x78\
+\x24\x44\x7e\x63\xf4\x6c\x14\x9f\x60\xd3\xbd\x1d\xf5\xb7\x81\x1f\
+\xbd\x13\xe1\xaf\x20\xb8\xaa\x1b\x81\x9f\x34\xe9\x20\xb6\xef\x0a\
+\xc0\x15\xe7\x1c\xce\x00\x21\x91\x12\xc4\x27\x13\x7c\x8d\x92\xd8\
+\x10\xd0\x42\xe0\x4b\xe0\x15\x58\x24\x64\x00\x17\x8f\x72\x5c\x77\
+\xa9\xc0\x35\x17\xfa\xd3\x29\x15\xce\x96\xda\x53\x3f\xdd\xe6\x77\
+\x46\x69\xe0\xf7\x50\x35\x16\x8b\x1e\x1c\xa1\xe2\x30\x6d\x13\xd5\
+\x02\x4f\xff\xb5\x28\x67\xc0\x2f\x76\xe5\xe5\x44\x59\x24\x7e\x31\
+\x0d\x33\xda\x9f\xaf\x92\x97\x41\x1e\x3a\x09\x79\x47\x1e\x66\xdb\
+\xbd\xf5\xe1\x27\xbb\xcd\xbf\xc3\x9e\x01\x30\x37\xb7\x59\xa7\x0f\
+\x9b\x9d\xfb\x43\x63\x3e\x66\xfd\x72\x06\xcb\x57\x39\xc3\xc6\x3e\
+\x02\x17\x9c\xd8\x03\xa1\xd9\xb8\xe2\x92\x83\xc0\xb0\x5a\x24\x50\
+\x26\x65\x62\x26\x60\x8a\x4d\x6c\xa5\x36\xb0\x0c\x9e\x01\x85\x82\
+\x01\xdc\xbd\xcb\xe0\xec\x56\xc1\xe9\xba\x6b\x05\x5c\x3d\xcb\xe1\
+\xe9\x11\x0e\xa7\x05\x0f\xeb\x64\x82\xec\xcb\x23\xd1\x5a\x17\xa0\
+\x7b\x4e\x90\xa2\x81\x0a\xb5\xd3\x40\x98\x05\x65\x80\x07\x7e\x3f\
+\xca\x39\xe8\x5d\xe8\x6b\x64\x94\xa0\xff\x01\x39\x07\xf9\xa1\x45\
+\x7c\x6c\x5c\xb9\x3f\xa4\x3e\xef\x23\xcd\xe6\x41\x63\x87\x48\x4a\
+\x5d\xe7\x76\x78\xf9\xce\x82\x6f\x61\xf3\xbd\x7e\xe4\xcf\x5f\x78\
+\x09\x27\xcf\xa5\xe2\xec\xa5\x0c\x9c\xbb\x9c\x89\xf3\x04\x9e\x3d\
+\x07\x70\x89\xe0\x5f\x76\xce\x86\x6f\x60\x15\x12\x53\x21\x88\x37\
+\x82\x0a\xbe\xc1\x15\xf0\xf0\x2f\xe4\x0d\x40\xf0\x3d\x7d\xcb\xe0\
+\xea\x5e\x09\x17\xf7\x0a\x41\xfe\x61\xa5\x98\x3b\xff\x2c\x26\x59\
+\x6c\xc0\x89\x9f\xfa\xe9\x00\x88\xdc\xf3\x14\x64\xe9\xeb\xa9\x2a\
+\xcf\x35\x3c\x2d\x4c\x29\x01\x2a\x83\x80\x2c\x6b\x3e\xa2\x23\xa6\
+\x50\x0b\x69\x4e\x95\xe6\x58\x1a\x73\x66\xd2\xd7\x16\x01\xd9\xf6\
+\x40\x55\x04\x7d\xaf\xd4\xf0\xf0\x48\x69\x01\x1a\xe3\x97\x40\xe2\
+\xf6\x32\xaa\x2e\x3f\x6b\x0c\x7e\x33\xe9\x8b\x3b\x6b\x52\xc7\xc2\
+\xe6\x13\x02\xae\x14\x9f\xf3\x67\xb5\xc1\x13\xa7\xcf\xa7\xe3\xcc\
+\xc5\x0c\xa3\x06\xf0\xf4\x2b\x43\x52\xaa\x0a\x49\x69\xa0\x3f\x79\
+\x31\x13\x04\x84\x56\x73\xb3\x80\x1a\x03\x78\xfa\x97\xc0\xcd\xa3\
+\x52\x47\xbe\xc1\x65\xd8\xb4\xcd\x53\x30\xda\x78\xf3\xad\xb0\x9f\
+\xa9\x7b\x3c\x8b\xc7\xe2\x6e\xc8\xbd\xfc\x1e\x94\x05\x7b\xd1\x2a\
+\x49\xfb\xdb\x07\x45\xb6\x36\x64\xa0\x29\x75\x23\xa4\x5e\x43\xa8\
+\xd5\x7b\x85\x0c\xf0\x12\x32\x0e\xf4\xd3\x87\xaf\x22\x4d\xbf\xa3\
+\xe0\xd3\x78\xce\x56\xf5\x2a\x35\x30\x2c\xa8\xad\xdb\xb1\x2b\x88\
+\x22\x3f\xad\x4d\x03\xb8\x7a\x15\x11\xf8\x56\x24\xa7\x83\x57\x1a\
+\xaf\xe0\x88\x3a\x6a\x05\xf3\xb5\x06\xf0\x2f\x86\x87\x77\x25\xdc\
+\x3d\x79\xb9\x91\xbc\x03\xca\x71\xf8\x44\x94\x7e\x5d\x91\x33\x6f\
+\xda\x22\x8b\x53\xb3\x1f\xb3\x26\x00\x2d\x62\x28\x01\xeb\xee\x43\
+\xa9\xe7\x48\x28\x32\x16\xa3\xb9\xe4\x0c\x99\x21\x95\x5f\x49\xfc\
+\x3d\xe8\xf4\x3d\xaa\xba\x18\xa8\x8a\xf6\xa1\x35\xe9\x33\x28\x83\
+\x5f\x82\xd4\xf3\x3f\x90\x78\x0c\xe4\xa2\x5f\xe2\xfa\x22\x77\xa6\
+\x90\x9e\x01\x76\xdc\x89\x8b\x3a\xce\x1a\x10\xe3\xc6\x1f\xc0\x5e\
+\xeb\x70\x9c\x38\x9b\x86\x53\xcc\x00\x17\x44\x06\xb8\x92\xc9\x1d\
+\x06\x71\xcd\xbd\x80\x22\xbd\x05\x29\x19\xd0\x2a\x9d\xb5\x7b\x12\
+\xb8\x78\xe7\x73\x06\x70\xf7\x2b\x20\xf8\x64\x00\x9f\x4a\x78\x7a\
+\x57\x91\x09\x78\x79\xf9\x56\xe0\x8a\x6b\x06\xc6\x8d\xb3\xd3\xf9\
+\xa4\x8f\x1f\x26\xae\x15\x3e\x12\xee\xe2\xbc\x7e\x43\x09\x44\x8a\
+\x7e\x6a\x0e\xdd\xda\x0f\x65\x9e\x1f\xa2\x31\xce\x82\x34\x0e\x8a\
+\xb4\x45\x50\x64\x6d\x85\x32\xcf\x8e\xb2\xc4\x11\x28\xf3\x0f\x41\
+\x91\xbd\x1b\x4d\x34\x74\x34\xc6\xfd\x04\x65\xe4\x3b\x34\x1c\x0c\
+\xe0\x15\xf7\x02\x5a\xa3\x07\xe8\x18\xa0\xde\x79\x80\x7e\xe1\xa7\
+\x24\xdd\x59\x9f\x0e\x3e\x66\x8c\xad\xb9\xf8\x29\x9f\x7d\xb6\x91\
+\x38\x7e\x3a\x95\x37\x00\x45\xbf\xc6\x00\x5c\xf4\x93\x01\xae\xb8\
+\xe4\x22\x21\x59\x89\xd4\x4c\x20\x35\x43\xab\xe8\x78\x39\x5c\xbc\
+\xf2\xf9\x45\x20\x9f\x02\xce\x00\xde\x7e\x15\xf0\xf2\xa9\xd2\xca\
+\xb7\x92\x1b\x12\x66\xcc\x74\xd4\x2d\x32\x2d\xf6\xfe\xaa\xff\xbe\
+\x9c\x16\x3e\xd8\xd5\x65\x5e\x97\xb9\x04\xa4\xca\xc0\x08\x5b\x1e\
+\x44\x99\xdb\xfb\x90\x47\x7d\x45\xbd\xfb\xff\x20\x0d\x79\x1f\xd2\
+\xa0\x61\x90\x04\xbe\x0d\x69\xe0\x30\xc8\x82\x46\x40\x16\xf8\x3e\
+\x9a\x42\xde\xa2\x82\xe4\x65\x5e\xf1\x2f\x71\x92\x7a\xbf\x2a\xa4\
+\xff\xa2\x93\x8f\xeb\x47\xff\xc5\x3b\x0a\xfe\xe4\x29\x87\x3a\x6b\
+\x0e\x7a\x60\x63\xfe\xce\xdd\xc1\x38\x76\x2a\xb5\x4d\x03\xb0\x47\
+\xc0\x62\x13\x1b\x91\x96\x05\x5e\x99\xbc\xe2\x93\x15\x1c\x7c\x61\
+\x15\x90\x0c\xe0\xe5\x57\x0e\x1f\xbf\x6a\x41\xde\xbe\xd5\x34\xee\
+\x97\x62\x89\xe5\x15\xfd\xd4\x7f\xc3\xe7\xec\x3c\x96\xf4\xb8\xd7\
+\x75\x7e\xe7\x25\x04\xa7\x48\xdf\x08\x21\x9b\xee\x47\xb5\xf7\x08\
+\x02\xff\x26\x1a\xfc\x07\x91\x5e\x27\x0d\x51\x1b\xe0\x3d\xc8\x02\
+\xde\x81\x2a\xe1\x35\x2a\x4c\x48\x09\xaf\x92\x06\xa2\x29\x68\x20\
+\x6f\x00\xd7\x97\x90\x6e\xfb\x90\xfe\x84\xcf\xc8\x3b\x2d\xfa\x85\
+\xad\xdd\xcb\x96\x3b\xc3\xf1\x64\xca\x0d\x0d\x10\x15\x2b\x45\x46\
+\x36\x90\x9e\xa5\x55\x52\x6a\x33\x41\x2f\xd0\x59\x05\xf4\xf4\x2b\
+\x85\x5f\x40\x35\x27\xf6\xcc\x20\x93\x4f\x60\x19\x7e\xdb\xeb\xaf\
+\x0f\x3f\x6b\xfc\x84\x03\xf7\xfe\x91\xf7\x4a\x05\x61\x57\xf7\x85\
+\x5d\x46\xb1\x28\x55\xa7\x6a\x0e\x5a\xb2\xc3\xb3\x90\x06\xbf\x0b\
+\x49\xc0\x60\x41\xb2\xa0\xf7\x09\xfe\xbb\x90\xf9\xbf\x83\x96\x98\
+\x21\xf4\x26\x07\x93\x09\x06\x91\x5e\x47\x73\xe4\x6b\xc2\xf8\x1f\
+\xff\x5b\x5f\xb1\x01\x32\x3d\x16\x75\xea\x70\xa7\x8d\xfd\x91\xdc\
+\xa7\x74\x4d\x39\x84\xc3\xc7\x92\x78\x03\x30\xf8\x67\xd2\x0c\x0a\
+\xc0\xd0\xc8\x3a\x64\xe6\x80\x13\x33\x01\x53\x6a\x46\x2b\x45\x7b\
+\x91\xb0\x08\xc4\xb2\x80\x87\x6f\x11\xfc\x03\xab\x49\x35\x9c\xfc\
+\x02\x6a\xe0\x1b\x54\x89\x13\xe7\xe2\x61\x6e\x6e\x2d\x86\xdf\x38\
+\x76\xac\xdd\xa0\xbf\xf2\xbe\x09\xd6\x75\x61\x38\xd8\x74\x1f\x64\
+\x21\x2c\x0b\xbc\xa1\xd6\x10\x7e\x18\x08\x18\x06\xa9\xdf\xdb\x50\
+\x84\xd3\x30\x90\x4c\x4a\x7a\x93\xf4\x06\x65\x84\xc1\x5c\xfa\x97\
+\xb8\x0c\x40\xcc\xb6\x7b\x45\x93\x50\x77\xd8\x46\xcf\x09\x13\x1d\
+\x84\xed\x5c\xeb\x36\x78\xe3\xe8\x89\x94\x36\x0d\xe0\x1f\x5c\x85\
+\x2c\x35\x7c\xad\x09\x54\x14\xe9\x25\xdc\x1a\x80\xc6\x00\x6e\x94\
+\x09\x02\x82\x6a\x10\x18\x5c\xcb\xfd\xc9\xe4\x1f\x58\x45\x45\x63\
+\x36\x26\x4d\x76\xd0\x89\x7e\x73\x73\x9b\xbf\x7c\x04\xab\xf3\x9c\
+\x0e\x6b\x05\x70\x0b\x3a\x43\x16\xfa\x11\x24\x41\x43\xd5\x7a\x8b\
+\x0c\xf0\xb6\x60\x00\x59\x00\x81\x4f\xa1\x62\x30\xe5\x6d\xd2\x50\
+\xce\x0c\x72\xbf\x81\x9c\x01\xe2\x76\x6a\x97\x7b\xbd\x96\x74\x7e\
+\xf5\xce\x6a\xfd\x26\x1f\xe2\xd6\xf2\xa9\xff\xc7\x21\xc7\xc4\x36\
+\x0d\xe0\xe9\x5b\x8a\xec\x5c\x70\xca\xd2\x88\x0c\xe0\x1b\x58\xce\
+\x3d\x0f\x28\x18\x80\xd2\x7f\x20\x19\x25\x28\xa4\x96\x17\x99\x20\
+\x30\xb8\x86\xeb\x04\x66\xcd\x3e\xa5\x9f\xfa\xcf\xfc\x9d\xf7\x4e\
+\x06\xf8\x42\x67\x9b\xb9\x2b\x81\x0f\xa1\x22\x30\xf8\x1d\xb5\xde\
+\xe6\xd2\xbf\xd4\x6f\x28\xa4\x3e\x6f\xa0\x35\xf1\x5d\x4a\x57\xef\
+\x91\xe8\xcf\x94\x61\x50\x86\x0d\x22\x03\x3c\x4f\x35\xc0\x03\xda\
+\x9d\xbe\x4b\xbb\xf4\xbe\xd3\xd2\xbf\x03\x83\xf1\xc3\x8f\xa7\x70\
+\xe4\x78\xb2\xd1\xf1\xdf\xd9\xa3\x90\x80\xab\x90\x93\x07\x4e\xd9\
+\x6a\x05\x85\x57\x73\x53\xc0\xfc\x22\x10\x6f\x00\x7f\x4a\xf3\x21\
+\x61\x75\x08\x09\xad\xe5\x14\x4c\xf2\x09\x2a\xc5\x9a\x75\x2e\xfa\
+\xf0\xd3\xa9\xd5\xfc\x5b\x1f\xf5\x4a\xc0\x1e\x12\x1b\x20\xf3\x18\
+\xb5\x77\xa1\xc3\xc9\x04\xef\x91\xde\xe5\x24\x65\x06\xf0\x25\x03\
+\x78\x0f\x81\x92\xed\x38\x4e\xfb\x2f\x69\x04\x99\x60\x38\x5a\x13\
+\xde\x41\x83\xf3\xf3\xa8\x38\xaf\xed\x02\x3c\x16\x74\x5c\x72\xa7\
+\x19\x20\x94\x01\x59\xbe\xd2\xd5\xa8\x01\x9c\x9c\xf3\x28\xd2\x5b\
+\x91\x9b\x4f\xf0\x35\x22\xf8\x11\x31\xf5\xc2\x1a\x80\xc6\x00\x3e\
+\x01\x65\x08\x0b\xaf\xe3\x14\x1a\xc6\xcb\x2f\xb8\x1c\x36\xf6\xa1\
+\xfa\xf0\xe5\x63\xc6\xda\xbe\x76\x33\xde\x3f\x41\xcb\x17\x4e\x1c\
+\xfd\xad\x1f\x19\xe0\xbf\x90\x86\x8d\xe0\x8c\xc0\x29\x80\x19\xe0\
+\x4d\x32\xc0\x60\x34\xd2\xb0\x80\xf4\x8f\x78\xa5\x7d\x48\xfa\x00\
+\x52\x8f\x17\xd1\x70\xfd\x19\x44\x6c\xec\x29\x9e\x01\x3c\xea\xb1\
+\xb0\xe3\xd3\x77\x8a\x01\xb8\x0f\x77\xfa\x6d\x4f\xa8\x81\x01\xce\
+\x5f\xc9\xa2\x31\xbe\x19\x79\x05\xe0\x94\xab\x56\x5c\xa2\x94\x5f\
+\x03\x10\x19\xc0\xd3\xb7\x18\x11\x91\xf5\x08\x8f\xa8\xe3\x14\x46\
+\x0a\x0a\xad\xc2\x99\x4b\xc9\xdc\x46\x11\xdd\x71\xdf\xfa\x87\x9b\
+\xf5\xfe\xd9\x31\x2d\xc2\x73\x06\xcb\xbb\x53\x21\x48\x06\x08\xff\
+\x40\x2d\xfa\xef\xa0\x77\xb9\xf4\x2f\xf5\x1a\x44\x7a\x1d\xaa\xb4\
+\x8f\xa9\x70\xf9\x84\x4c\x40\x7f\xa6\x8f\xa4\x76\x90\x5a\xc6\x6b\
+\x4f\xa3\xea\xfc\x63\xf0\x5a\xd4\x49\x7f\x32\xe8\xa8\xfb\x82\x0e\
+\xff\x7f\x3f\x20\x7a\xfa\x77\x8e\x3d\xd9\xa2\x0f\x03\x74\xc8\x31\
+\x89\xc6\x7f\xad\x01\x4e\x9f\xcf\x40\x6a\x7a\x13\xf2\x0b\x21\x28\
+\xaf\x90\x4d\xf3\x36\x71\xe0\xd9\x79\x40\x6c\x11\x88\x19\xc0\xc5\
+\xb3\x80\xe0\xd7\x21\x32\xaa\x1e\x11\x6a\x85\x46\xd4\x52\x41\x98\
+\x8b\x6f\xa7\x1f\xd1\x8f\xfe\x9b\xfa\x3c\x1d\x41\x5a\xaa\xb3\xc3\
+\xd8\x87\x8a\xbe\x88\x8f\xb4\x62\x19\xc1\x67\x08\x6f\x00\xcf\xff\
+\xa0\x99\x7b\xa2\xf8\x0b\x32\xc1\xe7\xa4\xcf\xd0\x1c\xfb\x1e\x67\
+\x00\xb6\xf7\xaf\xec\x64\x3f\x78\xea\x9a\x00\xea\xe9\xe8\xd3\x64\
+\x84\x67\xff\xdf\x19\x60\xea\xb4\x23\xaf\xf3\x07\x3b\x9c\xe6\xa2\
+\x5f\x53\x00\xb2\xe2\x2f\x31\x45\x86\x82\x22\xe8\x28\x23\x4b\xc9\
+\x01\x17\xaf\x02\x5e\xa3\xe2\x2f\x22\xaa\x16\x51\xd1\x0d\x6a\xd5\
+\x73\x46\xf0\xf4\x2f\xc2\xfc\x85\x17\xf4\xe1\xa7\x8e\x1d\x67\xd7\
+\xeb\x26\x1b\xe0\x43\x31\xb0\xfc\x73\xaf\x50\xe4\x8f\x84\x34\xf2\
+\x13\x5e\x11\x23\xd5\x06\x78\x1d\x12\x8f\x57\xd1\x14\x36\x8c\xaa\
+\xd7\xaf\x49\x5f\x91\xbe\x84\x2a\xe3\x0b\x1a\x02\x9e\xe6\x9e\xfb\
+\x67\x4f\xfe\x54\x9e\x7e\x08\x41\xab\xbb\x1a\x5b\x19\xf4\xbb\x7d\
+\x97\x77\xcd\x6d\x96\x51\x95\xbf\x99\x8a\xae\x6f\xc7\x4f\xb0\x7f\
+\x7f\xe2\xc4\x83\x03\x08\xfe\x00\x6a\x01\xcf\xf3\x1b\x39\xdd\x04\
+\x03\x1c\x3b\x95\x82\xe8\xb8\x7a\x14\x15\x03\x85\x22\xe5\xe4\xb7\
+\xe0\x9a\x6b\x9e\xce\x2a\x20\x33\x43\x28\x15\x82\x31\xb1\x0d\x82\
+\xa2\x63\x1a\xa8\xdf\x67\x2b\x7c\x5e\xfa\xf0\x65\x94\x69\x06\xde\
+\xec\xdf\x8d\xc0\xdc\x4b\x6a\x15\x4e\x1e\xb1\x79\x0c\xb2\xb0\x8f\
+\x20\x8b\xfa\x8c\x57\xe4\xa7\x54\x08\xbe\x4d\xd1\xcf\x1b\x40\xea\
+\xf3\x3a\x55\xb0\xa3\x49\xa3\x78\x65\x7d\x03\xb9\xcf\x40\xde\x00\
+\x97\x1f\x45\xfd\xa5\x87\x51\x77\xe1\x41\x64\xee\xef\x45\x05\xa1\
+\xce\xfa\x80\xca\x6d\x9e\xd9\xa0\xdb\x0e\x3e\x81\x9f\x73\xa3\x1d\
+\x3d\xec\x43\x1e\xac\xed\xa2\x05\x03\x84\x84\x55\xa1\xb8\x04\x9c\
+\x8a\xd4\x2a\x28\x6c\x85\xab\x67\xa1\xc1\x32\x70\x60\x48\x05\x62\
+\xe3\x1a\x38\x69\x0c\x10\x14\x5a\x09\x87\xa3\x51\x18\x3d\x5a\xff\
+\x75\xac\x67\xdc\xaa\xdf\x91\x7d\x04\xac\x06\x54\xf0\xba\x7b\xa9\
+\x0e\xf8\x00\xb2\xe8\xff\xa9\xf5\x05\xa4\xc1\xc3\x75\x16\x7f\x5a\
+\xd3\x28\x03\xe4\x8c\x21\x59\x90\x09\xcc\xa1\x88\x7c\x97\x7b\xf2\
+\xa7\xe1\xf2\x23\x64\x80\x7e\xa8\x27\x03\xd4\x9f\xbf\x1f\x79\x76\
+\x3d\x6f\xef\x6d\x61\x04\xff\x73\xcd\x59\xbe\xc6\x64\x61\x61\x0b\
+\xab\xf5\xde\x38\x7c\x2c\x99\x33\x80\x8f\x7f\x29\x8a\x4b\xa1\xa3\
+\xa2\x12\x15\xbc\xfc\x4a\x84\x45\x20\x76\x20\x34\x1b\xff\x7d\xfc\
+\x4b\x10\x9f\x20\x41\x5c\xbc\x56\x6c\x28\x38\xef\x94\x86\x09\x13\
+\xec\xf5\x5f\xeb\xd8\xad\xfc\x3d\x09\xcc\x09\xd1\xb6\x6d\x8a\xf8\
+\x61\x90\xc5\x7c\x4d\xfa\x8a\xf4\x25\x64\x11\x9f\x10\xfc\xd7\x84\
+\xc5\x1f\x65\xf4\x47\xfc\x89\x24\xb9\xe3\xb9\xa3\x68\x98\x21\x58\
+\xfa\xaf\xbf\xd4\x1f\xf5\x17\x1f\x22\x03\x3c\x80\xfa\x73\xf7\xa1\
+\xee\xcc\xbd\xf0\xb7\xd4\xd9\x1b\x58\xe7\x3e\xdf\xec\xf6\x78\x20\
+\x74\xfc\x78\xfb\x57\xe8\xc6\xd7\x6b\x20\x7c\x3b\xdd\x11\x9b\xb6\
+\x06\x62\xfd\x26\x3f\x58\x6d\xf0\xc1\xe6\x6d\x81\xb0\x73\x88\xc3\
+\xa1\xa3\x49\x9c\x01\x5c\xdc\x0b\x50\x52\xa6\x22\x41\x2b\x32\x00\
+\x8b\x72\xf1\x2a\x20\x77\x22\xb8\x57\x21\x12\x12\x25\x24\x29\x67\
+\x02\xa6\x18\x1a\x36\xd8\x2c\xe0\x0f\x3f\x1e\xd7\x87\x9f\x4c\x2d\
+\xdf\x2d\xdd\x4f\xe7\x3c\xc7\x6c\xae\x38\x52\xcb\xae\xbc\xca\xc3\
+\x8f\x1b\x05\x59\xec\x37\xa4\xaf\x21\x61\x19\x40\xbd\xf8\x23\xf7\
+\x7f\x93\x2a\xda\xc9\xbc\x72\xf9\x33\x89\xa4\xae\xcf\x71\xe9\x9f\
+\x33\xc0\x79\x66\x80\xbe\x9c\x01\xb2\xf7\xdf\xa5\x93\x05\xdc\xe7\
+\x99\xb5\xff\xe3\x61\x27\x4e\x3a\xf8\x10\xdd\xf8\x5c\x0d\x84\x19\
+\x33\x4e\x60\xaf\x75\x34\x6c\xed\xe3\x61\x77\x30\x01\xf6\x87\x12\
+\x61\x7f\x38\x11\x0e\x47\x12\x39\x03\x5c\xbe\x9a\x43\x29\xbf\x15\
+\x65\xe5\x40\xa9\x48\x91\xd1\x35\x06\xcb\xc0\x57\x5d\x73\x09\x7c\
+\x03\x12\x93\xa4\x82\x98\x19\xbc\xfc\x8b\xb1\x6c\xc5\x55\x7d\xf8\
+\x52\xca\x42\xb7\x7c\x3f\x1d\x81\x79\x47\xe7\x10\xea\x43\x4f\xd1\
+\xd8\xff\x39\xe4\xf1\x16\x90\xc7\x99\x93\x46\x53\x56\x18\x2a\x2c\
+\xfe\x48\x5c\x07\x40\x95\x3b\x85\x3f\x37\x38\x7f\x2a\x19\x61\x0a\
+\x9a\x82\x87\xea\xa4\xff\xfa\xb3\xbd\xc9\x00\xf7\xa0\xf6\x54\x2f\
+\x78\x2f\xd2\xa9\x05\x6c\xda\x7b\xe4\xdf\xa5\x99\xdc\x61\x9a\xf9\
+\xc3\x29\xec\xb3\x89\x81\xcd\x01\x82\xef\x90\x80\x03\xcc\x00\x0c\
+\x3e\xe9\x20\xc1\x3f\x7b\x21\x93\x0a\xbe\x16\x94\x57\x80\x13\x33\
+\x01\x53\x42\xb2\x44\x77\x13\x08\x19\x80\xa5\xfe\xd8\xf8\x7a\x24\
+\x53\x87\x90\x9c\x22\xe5\x94\x94\x2c\x45\x40\x48\x39\x7e\xdb\x1b\
+\x60\x30\xc4\x8c\x1e\x6d\xfd\xed\x3f\xf1\x3b\x13\x94\xee\xea\xfd\
+\x7b\xfc\x3e\xc2\x6d\xf7\x43\x16\x3a\x12\xf2\x84\xb1\x64\x82\x31\
+\x9c\x64\xa1\x1f\x08\x06\x60\xb3\x7f\xcd\x49\xdf\x50\x71\x33\x83\
+\xf4\x1d\x69\x3a\xfd\xfd\x2b\x8a\x7e\xad\x01\xea\x98\x01\x4e\xdf\
+\x83\xba\x53\x3d\x91\xbc\xa3\xb3\xd8\x00\x51\xed\x77\xcc\x1f\x63\
+\xdb\x41\xf3\x09\x5e\x4c\x3f\xcf\x3a\x8b\x7d\xd6\xb1\x54\xe4\xc5\
+\x19\x35\xc0\xf1\xd3\x69\xc8\x2b\x50\xa0\xa2\x12\x82\x98\x09\xd2\
+\x33\xe5\x04\x3f\x43\x67\x15\x90\x45\x7f\x44\x74\x35\x52\xd3\x64\
+\x48\x4d\x95\x21\x45\xad\x88\xa8\x1a\x2a\x1e\xe3\xb9\xb5\x04\x3d\
+\x03\x1c\xfe\x27\x7f\x77\x02\x13\x27\x2c\xe8\x2c\xed\x0a\x69\xe0\
+\x7b\x90\x27\x4e\x20\x8d\xe7\x24\x8b\xfe\x5a\x58\xfd\x6b\x70\x7e\
+\x0e\x8d\xa1\xc3\xa9\xbd\xf9\x91\xf4\x03\x69\x26\x54\xf9\xdf\x51\
+\x1d\xf0\x88\x7a\xfc\xe7\xd3\x7f\xdd\xe9\xbb\xc9\x00\x3d\x50\x75\
+\xb4\x9b\xf8\xf1\xb0\x26\xaf\x45\x66\xed\xf3\xc9\x60\x8a\xb8\x77\
+\xc5\x9b\x39\xf7\x5a\xc7\x60\xbf\x4d\x9c\x51\x03\xb0\x71\x3f\x2b\
+\x5b\x8e\xca\x2a\xe8\x28\x2f\x5f\x81\xb3\x17\x33\x0d\x96\x81\x03\
+\x29\xca\xd3\xd3\xe5\x48\x4b\x97\x71\x62\x46\x88\x4f\xac\xc7\xc5\
+\xab\x19\x98\x32\xf5\x90\x3e\xfc\x44\x8b\x31\x36\x3d\xfe\x61\x03\
+\x38\xe8\x1c\x45\xef\xf2\x1f\x02\x3f\x11\xf2\xa4\x49\xa4\x89\x9c\
+\x19\xb8\x1a\xc0\xe5\x05\xea\xfb\x9f\x85\xd4\xe3\x65\xfe\xc8\xd9\
+\xa2\x9f\x78\x91\x19\x64\xde\xaf\xa9\xd3\x7f\x1f\x2e\xfd\xd7\x51\
+\xfa\xaf\x3b\xd9\x1d\x75\x27\xba\x21\x68\x79\x07\xd1\x7a\x81\xd9\
+\xc0\xf6\x69\x00\x73\xeb\x51\xc2\x9e\xbe\x71\x07\xb8\xe8\xdf\x6f\
+\xcb\x1b\x80\x1b\xff\x99\x01\x0e\x25\x70\x63\x7f\x52\x4a\x03\xaa\
+\xaa\xa1\x55\x15\x6b\xfd\x9a\x71\xf1\x4a\xb6\xc1\x3e\x40\x36\xcd\
+\x9b\x41\x59\x81\x53\x86\x1c\xe9\xa4\xd4\x54\x29\x5c\x3c\xf3\x31\
+\xfb\xd7\xb3\xfa\xf0\x25\x94\x0d\x5e\xfc\xa7\x7f\x77\x02\xf3\xa3\
+\xd8\x00\xb9\xc7\x9f\x86\x3c\x76\x34\x1a\x93\xa7\x70\x92\x93\xd8\
+\xaa\x20\x4b\xff\x6c\xee\x9f\xcd\xfe\xb5\x66\x53\x0d\x50\xf4\x0b\
+\x69\x16\x27\x45\xcc\x27\x06\xe9\x9f\x33\xc0\xf1\x6e\x48\xde\xa6\
+\xed\x06\xbc\x16\x9a\xb5\xcf\x1d\x43\xe6\x16\x36\x3f\x68\x40\x4c\
+\x9e\x72\x98\xc6\x7e\x3d\x03\xa8\x0b\xc0\xe8\xd8\x1a\x54\xd7\x40\
+\x47\xe5\x15\xad\x70\x72\xce\x35\xd8\x05\xc4\x26\x7f\x32\x09\x7c\
+\x56\x56\x23\x32\x99\xe8\xbf\x99\x7c\x02\x4a\xb0\x66\x9d\x9b\xb1\
+\x71\x7f\xf2\xbf\xf1\xbb\x13\x98\x41\x3a\x1f\x41\xbb\xfb\x41\x6a\
+\xff\x3e\x47\x63\xca\xb7\xa4\x69\x9c\x64\x61\x1f\x73\xe9\x9f\x33\
+\xc0\xd5\xa7\xa0\x88\xfd\x1f\xb9\x7e\x2e\x69\x0e\xe9\x57\xb4\xe6\
+\xce\x30\x48\xff\x75\x27\xee\x22\x03\x74\x45\xa1\xad\x76\x8a\xd8\
+\x7b\x91\xd9\x98\x76\x3a\xe3\x67\xbd\x41\x7b\x6e\xef\x59\xa3\x06\
+\x08\x0c\x2e\x43\x6d\x2d\x50\xa3\x11\x33\x40\xb5\x0a\x6e\x9e\x05\
+\x06\xcb\xc0\x17\x9d\xb2\x28\xdd\x4b\x91\x9d\xd3\x88\xec\x6c\x5e\
+\x59\xa4\xd0\x88\x4a\xec\xb3\x0d\x33\x36\xb7\xe0\xf0\x6f\xfd\xee\
+\x04\xa6\x0b\x3b\xbc\x59\x03\x29\x70\x75\x4f\xc8\x82\x86\xa3\x31\
+\xf5\x3b\x41\xf2\xb8\xb1\x5c\xfa\xe7\xe7\xfe\x9f\x84\xcc\xf7\x0d\
+\x6a\x77\x16\x52\xbf\xbb\x80\x34\x9f\x93\xc4\xf9\x69\xad\x01\x4e\
+\x6a\x0d\x50\x79\x58\x5b\x08\x7a\x2f\x36\x9b\xd9\x5e\x57\xf6\x84\
+\x83\x9b\x17\x2f\xb9\x6e\x60\x00\x36\xfe\x5f\xbc\x9c\x8d\x2b\xd7\
+\x72\x70\x9d\x22\x9b\x41\xf7\xa6\xf4\xee\xec\x96\x6f\xb0\x0c\x7c\
+\x86\x8a\xc0\xc4\xe4\x7a\xe4\xe6\x36\x71\xca\xc9\x6d\x44\x0e\x19\
+\x21\x81\xc6\xfd\x63\xa7\x13\xf5\xb7\x73\x33\xc5\x53\xea\xff\x57\
+\x1f\x9d\x26\x38\x61\xa2\x8d\x9d\x68\xf0\x1c\x84\xc6\xf4\x99\xbc\
+\xd2\xbe\x27\xcd\x40\x03\xab\x01\xd4\x8b\x3f\xcc\x04\xaa\x12\x32\
+\x40\xd9\x12\x32\xc2\x62\x4e\x4d\x21\xc3\x0d\xc6\xff\xba\xe3\x5d\
+\x50\xeb\xa8\x35\x80\xcf\x62\xb3\xef\xdb\x1d\xfc\x09\x13\xec\xd9\
+\x47\xb8\xca\x85\x73\x7a\xb6\x06\xb5\x59\x00\x6a\x5a\x40\xb6\x02\
+\x28\x5e\x04\x12\xef\x02\x8a\x8a\xa9\x46\x7e\x7e\x13\xf2\xf2\xb4\
+\xca\xc8\x94\xe1\xf2\xb5\x2c\xee\x14\x30\x3d\xf8\x0d\x63\xc6\xd8\
+\xfe\xeb\xcb\xa6\x04\x67\x9f\x78\x18\x28\x3e\xf3\x0c\x8d\xff\x53\
+\xd1\x94\xf1\x23\x99\x80\xe9\x07\x48\x7d\xdf\xe2\xd2\xbf\x66\xf1\
+\xa7\x39\x75\x0a\x8d\x7f\x96\x64\x82\x65\x9c\x9a\xd3\xa7\xaa\xd3\
+\x7f\x4f\x21\xfa\x79\x03\x74\x12\x1b\x60\x42\xbb\x33\x00\x45\xa4\
+\x50\x00\x4e\x9e\x7c\x98\x2f\x00\xff\xa2\x01\x02\x82\x4a\x51\x40\
+\xed\xa1\x46\xf9\xd4\x19\x30\x03\xb8\x7b\x17\x62\xc1\xa2\x4b\xfa\
+\xf0\x55\x34\xee\x8f\x6f\x0f\xf7\x80\xe0\x4c\x15\x1b\x20\xd5\xb6\
+\x1f\xe4\x31\xa3\xd1\x94\x39\x8b\x4c\xc0\xf4\x33\x64\xe1\x9f\x71\
+\x91\xaf\x59\xfc\x69\x0c\xfd\x90\xfa\xdf\x55\x64\x82\x95\x9c\x54\
+\x65\x96\x54\x08\xde\xa7\x93\xfe\xeb\x8e\x75\x46\xc9\x01\x1d\x03\
+\xbc\xd6\x1e\xd3\xbf\xb3\x36\xfd\x3b\xff\x69\x03\xb0\x55\x40\x36\
+\xee\xbb\x7b\x15\xa2\xb0\xb0\x89\xa4\xd0\x51\x40\x48\x19\x77\x12\
+\xb8\x91\xa2\xcf\xb6\xbd\xdc\x03\x82\xf3\xa2\xd8\x00\xe1\x1b\xef\
+\x81\x2c\x64\x24\x9a\xb2\x7e\x25\xcd\x26\x23\xcc\x46\x63\xd2\x14\
+\x3e\xfd\xab\x17\x7f\x24\xd4\x15\xa0\xd2\x8a\x4c\xb0\x56\xad\x35\
+\xd4\x0e\x0e\xd2\x49\xff\xcc\x00\x99\xbb\x84\x2e\x40\x12\x68\x69\
+\xd6\xa9\x9d\xf5\xff\xfb\x9f\xd3\x7c\x74\x0b\xdb\xda\x7d\x90\x2a\
+\xfd\x93\xa7\xd3\x70\x9e\xfa\xf9\xab\xd7\x72\xe1\xe6\x51\x00\x1f\
+\xbf\x62\x04\x51\x01\x18\x4e\x05\x5c\x4c\x6c\x35\x12\x93\xea\xa8\
+\xc0\x6b\xa0\xc2\x4e\x46\x11\xde\x88\xe2\x62\x05\x49\x29\xa8\xa8\
+\x48\x21\x28\x36\xbe\x06\x36\x0e\x91\xfa\xdb\xb9\x99\x62\xe8\x6b\
+\x77\xb5\x23\x03\x74\x24\x35\x68\x0c\xe0\xb9\xa8\x33\xb7\x1b\xa8\
+\x29\x7b\xae\x5a\x73\x38\x33\x70\x85\xa0\xfa\xdc\x5f\x36\xfb\xd7\
+\xca\x3e\x7c\xa2\x72\x03\x69\x3d\x27\x45\xfc\x18\xa1\xfd\xd3\x18\
+\x20\x6e\xa3\x30\x0f\xe0\xd9\x1e\xa3\x5f\x98\xfd\x5b\xbe\xc2\x19\
+\xa5\xa5\x4a\x54\x56\xb4\x70\xaa\xa8\x68\xe6\x55\xde\x8c\x72\x8d\
+\xca\x9a\x51\xa6\x11\x7d\x6f\xa9\x46\x25\x4a\x94\x68\xa4\x36\x42\
+\x46\xa6\x94\x86\x85\x64\x4c\x98\xe8\xa0\x0f\xbf\x9e\x8a\xbe\x76\
+\xb7\x4b\x86\x00\xf9\xea\x9c\x44\x7a\xe9\x39\x0e\xba\x22\x67\x01\
+\x69\x3e\x27\xb6\x49\x54\xbc\xfa\xa7\x88\x1b\x43\xad\xd0\x66\xa0\
+\x8a\x69\x13\x54\xc5\x96\x6a\x03\x74\x15\x0c\x10\xb4\x5c\x98\x04\
+\x9a\xdb\xde\xe0\x3f\x4a\x6a\xd5\x9e\xd3\x6b\x47\x51\x9f\x8d\xaa\
+\xaa\x16\x54\x55\xf2\xaa\xac\x6c\xf9\x4b\x86\x28\x2c\x68\xa2\xa2\
+\x2f\x1b\xdf\xcf\x3c\x6e\x64\xdc\xdf\xdf\x2e\x7b\x61\x82\xb4\x5d\
+\x6c\x80\xec\x83\xfd\x29\xed\x4f\x85\x22\x77\x91\x5a\x0b\x21\x8f\
+\xf8\x52\xbd\xf6\xff\x30\x37\xf7\x2f\xf3\x1e\x42\xfd\xf0\x76\xb5\
+\xb6\x91\x19\xb6\x42\x72\xed\x29\x01\x3e\x2b\x00\xdd\xe6\xf1\x9b\
+\x42\x7c\x97\x98\x3d\xd9\x1e\x33\x80\xa7\x18\xd0\xac\x5f\xce\x23\
+\x31\xb1\x96\xfa\xfb\x16\x54\x57\xf1\xfa\xa3\x86\x60\x43\x41\x66\
+\x26\x5b\xe1\xab\x85\x8b\x87\xd1\x99\x3e\x36\xee\xb7\xdb\x47\xa7\
+\x09\xd2\x58\xb1\x01\x62\x77\xf4\x86\x3c\xf2\x4b\x28\xf2\x96\x92\
+\x96\x70\x6a\x4a\x9d\x29\xa4\x7f\x6e\xf1\x87\xb2\x80\xaa\x6a\x2b\
+\x50\xfb\x1b\xaf\x9a\x9d\x68\x0c\xfb\x54\x30\x80\xa8\x00\x8c\x68\
+\xaf\x13\x40\xec\x23\x5c\xab\xc5\x90\x56\xaf\x71\xa7\x28\x56\xa0\
+\xa6\xa6\x15\x35\xd5\x4c\x2d\x82\x21\xca\xe8\xeb\x59\xd9\x6c\x2d\
+\xbf\x06\x21\x61\xe5\xf0\xf2\x2d\xc2\x55\x97\x5c\x61\x0d\x80\x15\
+\x83\xfb\x6c\xc3\x31\xe3\xfb\x63\xc6\x26\x7b\x3c\x46\x9b\x5b\x77\
+\x6a\xc7\x06\x78\x4a\x6c\x00\xff\x15\xdd\xb8\x0d\x22\x8a\xfc\x65\
+\x22\x2d\xe5\x3a\x01\xed\xe6\x8f\xbe\x68\xa6\x2e\x01\x75\x7b\x49\
+\x7b\xc8\x04\xbb\xd1\x92\x3b\x5f\x30\x40\xf6\x1e\xa1\x00\xdc\xdb\
+\x6e\x57\x02\x29\x2a\x87\xb3\xe7\xec\xc4\xb0\xb6\x6c\xf1\x40\x74\
+\x4c\x25\x82\xa9\x82\x77\xf7\x2c\xc0\xc5\x2b\x59\x38\x76\x32\x55\
+\xe8\x00\x0e\x1c\x8a\xc3\xee\x7d\x61\xd8\xb4\xc5\x0f\x6b\xac\x3c\
+\x60\xb9\xe2\x3a\x66\xcf\x39\xc7\x1d\xfc\xd4\xc6\x2e\xa2\x6c\x73\
+\x73\x9b\xbe\x66\xed\xfc\x22\x50\x95\xc2\x84\xd0\x1c\x33\xd4\x5d\
+\x7f\x1e\x8a\x02\x4b\xd2\x72\xb5\x2c\x21\xf1\x79\x53\xb4\xf6\xdf\
+\x07\xf2\x90\x8f\x81\x7a\x1b\x92\x35\x99\x60\x3f\x99\x60\x0f\xea\
+\xd9\x8c\xa0\x6e\x07\x10\x1f\xb2\xd2\xec\xd1\x76\xfb\x8b\x9b\xf3\
+\x87\x36\xd7\xea\xef\xf9\xfb\x75\xce\x45\xac\x5a\xe3\x81\x45\x4b\
+\xae\xd2\xf0\x70\x96\xdb\x1d\xc4\x0e\x7c\xfa\xbd\xa3\xdf\xf4\x54\
+\xfd\x4f\x6c\xee\xb8\x49\x06\x70\x15\x67\x81\x82\x63\xfd\xd1\x94\
+\x31\x1b\xca\xc2\x55\xa4\x95\x9c\xe4\x51\xdf\xe8\x6c\xfe\x68\x70\
+\x7a\x02\x68\xb0\x27\x1d\x20\x13\xd8\x91\x6c\x21\xf3\x19\xca\x19\
+\xa0\xd4\x5e\x67\xab\xb8\x94\xe4\xe8\xb9\xc0\xec\x63\xef\xf6\xb8\
+\x2c\x3c\x69\x92\xfd\x13\x04\x2b\xe0\x4f\xc2\xfd\x3d\xb1\x87\x47\
+\x86\x9a\xdd\x26\x17\x01\x5a\x27\x36\x40\xd2\xde\xbe\x68\x8c\x1b\
+\x0f\x65\xd1\x1a\x41\x4d\x19\xbf\xe8\xec\xfd\x63\xb3\x7f\x2d\xa5\
+\x1b\x01\xc9\x41\x32\x81\x03\x27\x65\xca\x4c\xce\x00\x4c\xa9\xdb\
+\x3b\xea\x1c\x19\xab\xd9\x23\x48\x3a\x45\x66\xe8\xd8\xce\xa6\x85\
+\x0f\x74\xa2\x68\x9d\x47\xd0\x4a\xff\x26\x78\x76\x40\xe4\x49\xd2\
+\xe3\x66\xb7\xd1\x45\x50\xbe\xd4\x39\x49\xc4\xaa\x07\x64\xc1\x1f\
+\x42\x59\xb2\x8e\x57\xb1\x15\x69\x2d\xdf\x0a\x8a\x56\xff\x9a\xe2\
+\xa7\x00\xd2\xa3\xa4\x23\xa4\xc3\x50\x55\xef\x11\xea\x00\x4d\x31\
+\x18\xbe\xda\xcc\xc0\x08\x1e\xf3\xcd\xde\x68\x97\x37\x82\x2d\xce\
+\x50\xbb\x36\x97\x00\x5e\x24\x9d\x55\xc3\x74\x24\x1d\x22\x1d\x20\
+\xd9\x90\xf6\x91\x76\x91\xb6\x92\xac\x48\x4b\x48\xd3\x48\x23\x48\
+\xb7\xe5\xe1\x88\x04\xe5\x61\x9d\x8d\x9c\x0b\x3a\x42\xe2\xf6\x0a\
+\x94\x14\xe1\xca\xd2\x0d\x64\x02\xa6\xf5\x90\xfa\xbc\x25\xec\xfd\
+\x63\x8b\x3f\x52\xcf\x41\x80\xec\x04\xe9\x38\xe9\x18\x99\xc0\x11\
+\x12\xe7\x17\x04\x03\xf0\xea\x84\x8a\x43\x1d\x85\x79\x01\xee\xd1\
+\xf4\xb9\x66\x96\x66\xa6\xab\xdd\x99\xa0\x50\x67\xa7\xf0\xa9\x87\
+\xb9\x1a\xa0\xb9\x6c\x33\xaf\xd2\x4d\x68\x8c\xb6\x10\xad\xfd\xf7\
+\xe4\x4c\xa0\x6a\xa0\x0c\x20\x3f\x4d\x3a\x45\x26\x38\x89\xa6\xe8\
+\x71\x3a\xf0\x35\xca\xd9\xab\xb3\x51\xd4\xcb\x74\xc7\xdb\x9f\x01\
+\x2e\xe9\x3c\x3a\x6e\xdb\x97\xfa\xff\x1f\xd1\x5c\xbe\x8d\xb4\x95\
+\xb4\x05\x8a\xec\x05\x06\x9b\x3f\x94\x39\xcb\x80\xc6\x73\xa4\xb3\
+\x64\x82\x33\x68\x29\xd9\x62\xd4\x00\xb5\x8e\x1d\x41\x63\xbf\xf0\
+\x21\xd2\x3e\x8b\xcd\xba\x9b\xee\x7a\xfb\x32\xc0\x72\xb1\x01\xa2\
+\x37\xf7\x84\x3c\xe2\x6b\x34\x57\xec\x50\x6b\x3b\x67\x86\xfa\x0b\
+\x0f\xe9\xac\xfd\xcb\x43\x3e\x07\x9a\x2e\x91\x2e\x92\x09\x2e\x90\
+\xce\x53\x9d\x70\xbf\x81\x01\x98\xe2\x37\x69\xb3\x00\x99\x61\xa4\
+\xe9\xae\xb7\x2f\x03\x8c\x14\x1b\xc0\x77\x69\x67\x48\xbd\xdf\x40\
+\x73\xd5\x2e\x34\x57\xfe\x46\xda\xc9\x49\xe2\xfd\xa6\xce\xde\xbf\
+\x86\x8b\xfd\x01\xc5\x55\x92\x13\x99\xe0\x0a\xe9\x32\xe4\x81\x23\
+\x0d\xe0\xd7\x39\x76\x42\x99\x7d\x47\xd1\xc7\xc8\x98\x6d\x31\xdd\
+\xf5\xf6\x65\x80\x3e\xe2\x87\x46\x99\xaa\xcf\x3f\xc2\xc1\x6f\xa9\
+\xda\x43\xda\xcd\xa9\x31\x66\x9c\xce\xde\x3f\x56\xf5\x4b\xdd\x07\
+\x43\x99\xbb\x86\x37\x82\xf2\x1a\x94\xd9\x96\x46\x0d\xc0\x14\x68\
+\x79\x1b\x3c\x2f\x70\x07\x9b\x20\x41\x67\xa7\xb0\x7d\x1f\x28\x72\
+\x97\xa1\xa5\x7a\x3f\x69\x1f\x27\x65\xde\x72\x83\xb5\x7f\x8d\x1a\
+\x2e\x3d\x8a\xa6\xa4\x1f\xd1\x5a\x77\x54\xbd\x31\x44\xd7\x00\xd5\
+\x47\x3a\x6a\x16\x89\x98\x5a\xa9\x3d\xbc\xcf\x74\xd7\xdb\x97\x01\
+\xac\x75\x16\x86\xb6\xf5\x40\x23\xf5\xfa\x2d\xb5\x36\x68\xa9\xb1\
+\x56\x6b\x3f\x14\x99\xf3\xd0\x70\xf5\x69\x03\x03\x08\xd2\xd4\x08\
+\x7a\x06\xc8\xf8\x4d\xa7\x13\x68\x21\x03\x3c\x66\xba\xeb\xed\xcb\
+\x00\xe3\xc5\x06\xf0\x5e\xd2\x09\xb2\x80\x11\x68\xa9\x3b\x40\xb2\
+\xe3\x55\x6b\xcb\x8b\xcc\xd0\x98\x30\x15\xf5\x67\xfb\x1a\x31\x81\
+\xf1\xf4\x1f\xb6\x5a\x67\x42\xc8\xc9\x74\xc7\xdb\x9f\x01\xfa\xab\
+\x0f\x7d\x12\x0d\x03\xbd\xa9\xff\x1f\x4b\xd0\xed\xd0\x5a\xef\x40\
+\x26\xb0\x57\x1b\x82\x37\x45\x33\xd5\x07\xf2\xb0\x2f\xf9\x3d\x81\
+\x37\x30\x40\xed\x51\x9d\xf4\xcf\x9e\x1a\xfe\xc6\x74\xc7\xdb\xa7\
+\x09\x62\xc5\x06\xf0\x5c\xd4\x11\x15\xc7\xee\x41\x83\xf3\x00\x28\
+\x8b\xac\xc8\x04\x07\x45\x72\x10\x4c\xd1\x5c\xb6\x15\x32\xdf\x77\
+\x09\x78\x97\xdf\xed\x00\xd8\x81\x52\x9e\x0b\xcd\xee\x36\xdd\xed\
+\xf6\x69\x80\x45\xfa\xe7\xfd\x78\x2d\xea\x80\x22\x87\x1e\xdc\x04\
+\x90\x3c\x72\x34\x5a\x18\xf8\x86\xc3\xa4\x43\xbc\x44\xa6\x50\xe6\
+\xaf\x82\xc4\xe5\x45\x83\xf4\x9f\xb3\x47\x67\xfc\x0f\x33\xdd\xe9\
+\xf6\x6b\x80\xbb\xf5\xa7\x85\x35\xfb\x04\xe2\xb7\x74\x46\xb5\x63\
+\x37\xee\x39\x01\x65\xd1\x3a\xb4\x4a\x8e\xaa\x75\x84\x17\x67\x0a\
+\xde\x18\x8a\xf4\xd9\xd4\x15\x3c\x2c\x18\x40\xaf\x00\x3c\x6a\xba\
+\xd3\xed\xdb\x04\x6f\x91\x6a\x8d\x9c\xfc\x05\x4a\xdd\xc8\xde\xdb\
+\x89\x9f\x05\x8c\x18\x85\x16\x06\x5c\xea\xc8\x4b\xe2\xa8\x63\x8a\
+\x16\xca\x08\x8d\xb1\x93\x50\x7f\xea\x1e\xa4\xed\xe8\x20\x9a\x04\
+\xea\xb0\xda\x74\x97\xdb\xbf\x09\x06\xb0\xc9\x1a\x63\x26\xe0\x9e\
+\x21\x58\xd3\x01\x95\x87\x3a\xa1\xc1\xe9\x29\x34\x17\x6f\x40\xab\
+\xec\x04\xe9\x38\x19\x81\xe9\x98\x8e\x29\x58\xc7\x50\x70\xe9\x6d\
+\xf1\xf1\xb2\xf3\x4c\x77\xf8\xf6\x30\x41\x27\xd2\x6c\x52\xb9\x31\
+\x13\x78\xcc\x37\x43\xd6\xae\x8e\xdc\xa4\x4f\x23\xd5\x06\x0c\xbc\
+\x4a\x7e\x92\x13\x6f\x88\x13\xdc\x70\x20\x8b\xb0\x40\xc4\xfa\x6e\
+\xe2\xe5\xe6\x1f\x4d\x77\xf7\xf6\x32\x42\x4f\xf5\x62\x51\xb5\x31\
+\x23\x84\xae\xea\x80\x8a\x83\x2c\x1b\x3c\x89\xe6\x92\xcd\x50\x35\
+\x9e\x21\x13\x9c\x82\x22\xed\x57\x14\x1c\x7a\x00\xbe\x8b\x75\xbf\
+\xdf\x6d\x7e\x27\x53\x06\xb8\x8d\x0b\x44\x4b\xf1\x26\x52\x51\x5f\
+\x8f\x84\xcd\x1d\x90\xba\xb3\x33\xb2\x9d\xbe\x40\xa2\xdd\xf3\x06\
+\xe0\x45\x06\x58\x6e\xba\x9b\xb7\xf1\x45\x1d\x41\x2f\x17\xfe\xcc\
+\xe1\xf2\xb6\x6a\x84\x36\xa4\x74\x99\xdb\x61\x33\x19\xc0\xb4\x17\
+\xe0\xff\xc3\xe5\x36\xd7\xac\x27\x99\x81\xcd\x1b\x94\xfd\x0e\xf8\
+\x2a\x97\xb9\x1d\x77\xba\xce\xfd\x7f\x78\x80\xb4\xe9\x32\x33\x73\
+\x9d\x6b\xd6\x83\x8c\xb0\x80\x40\xbb\xb3\x87\x41\x49\xe7\x49\x07\
+\x5c\xe7\x76\x9c\x4f\xe0\xdf\x72\x9d\xd7\xe9\xa6\x9f\x16\xfa\x7f\
+\xc1\xff\x93\x2f\x0d\xe2\xa8\xdc\x00\x00\x00\x25\x74\x45\x58\x74\
+\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x31\x30\
+\x2d\x30\x32\x2d\x31\x31\x54\x31\x35\x3a\x33\x30\x3a\x33\x30\x2d\
+\x30\x36\x3a\x30\x30\x43\x7c\x8c\xaa\x00\x00\x00\x25\x74\x45\x58\
+\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\x30\
+\x38\x2d\x31\x32\x2d\x31\x34\x54\x31\x30\x3a\x30\x32\x3a\x35\x30\
+\x2d\x30\x36\x3a\x30\x30\x49\x78\x12\x3a\x00\x00\x00\x00\x49\x45\
+\x4e\x44\xae\x42\x60\x82\
+"
+
+qt_resource_name = b"\
+\x00\x06\
+\x07\x03\x7d\xc3\
+\x00\x69\
+\x00\x6d\x00\x61\x00\x67\x00\x65\x00\x73\
+\x00\x08\
+\x0d\x06\x59\x67\
+\x00\x6b\
+\x00\x65\x00\x79\x00\x73\x00\x2e\x00\x70\x00\x6e\x00\x67\
+"
+
+qt_resource_struct_v1 = b"\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
+\x00\x00\x00\x12\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+"
+
+qt_resource_struct_v2 = b"\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x12\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x01\x5e\xba\xa8\xab\x48\
+"
+
+qt_version = QtCore.qVersion().split('.')
+if qt_version < ['5', '8', '0']:
+    rcc_version = 1
+    qt_resource_struct = qt_resource_struct_v1
+else:
+    rcc_version = 2
+    qt_resource_struct = qt_resource_struct_v2
+
+def qInitResources():
+    QtCore.qRegisterResourceData(rcc_version, qt_resource_struct, qt_resource_name, qt_resource_data)
+
+def qCleanupResources():
+    QtCore.qUnregisterResourceData(rcc_version, qt_resource_struct, qt_resource_name, qt_resource_data)
+
+qInitResources()
```

### Comparing `deriva-qt-1.6.1/deriva/qt/auth_agent/ui/auth_widget.py` & `deriva-qt-1.6.3/deriva/qt/auth_agent/ui/auth_widget.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,307 +1,327 @@
-import os
-import json
-import logging
-import requests
-import time
-import platform
-from requests.adapters import HTTPAdapter
-from requests.cookies import create_cookie
-from requests.packages.urllib3.util.retry import Retry
-from PyQt5.Qt import PYQT_VERSION_STR
-from PyQt5.QtCore import Qt, QTimer, QUrl
-from PyQt5.QtWidgets import qApp
-from PyQt5.QtNetwork import QNetworkCookie
-from PyQt5.QtWebEngineWidgets import QWebEngineView, QWebEnginePage, QWebEngineProfile
-from deriva.core import read_config, read_credential, write_credential, load_cookies_from_file, \
-    format_exception, DEFAULT_SESSION_CONFIG, DEFAULT_CREDENTIAL, DEFAULT_COOKIE_JAR_FILE
-from deriva.core.utils.version_utils import get_installed_version
-from deriva.qt import __version__ as VERSION
-
-DEFAULT_CONFIG = {
-    "servers": [],
-    "cookie_jars": [
-        DEFAULT_COOKIE_JAR_FILE,
-        os.path.join(os.path.expanduser(os.path.normpath("~/.bdbag")), "deriva-cookies.txt")
-    ]
-}
-
-DEFAULT_CONFIG_FILE = os.path.join(os.path.expanduser(os.path.normpath("~/.deriva")), "auth-agent-config.json")
-
-DEFAULT_HTML = '<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8"><title>DERIVA Auth Agent</title></head>' \
-               '<body style="text-align: center; vertical-align: middle;">' \
-               '<div style = "margin-top: 50px;"><font size="+2">' \
-               'Authenticating to:<br/><br/><b>%s</b><br/><br/>Please wait...</font></div>' \
-               '</body></html>'
-
-ERROR_HTML = '<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8"><title>Error</title></head>' \
-             '<body style="text-align: center; vertical-align: middle;">%s</body></html>'
-
-SUCCESS_HTML = '<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8">' \
-               '<title>Authentication Success</title></head>' \
-               '<body style="text-align: center; vertical-align: middle;">' \
-               '<div style = "margin-top: 50px;"><font size="+2"><b>Authentication Successful.</b></font></div>' \
-               '</body></html>'
-
-
-class AuthWidget(QWebEngineView):
-
-    def __init__(self, parent, config=None, credential_file=None, cookie_persistence=False, log_level=logging.INFO):
-        super(AuthWidget, self).__init__(parent)
-
-        self.parent = parent
-        self.config = None
-        self.config_file = DEFAULT_CONFIG_FILE
-        self.credential = DEFAULT_CREDENTIAL
-        self.credential_file = None
-        self.cookie_file = None
-        self.cookie_jar = None
-        self.auth_url = None
-        self.authn_session = None
-        self.authn_session_page = None
-        self.authn_cookie_name = None
-        self.authn_expires = time.time()
-        self._success_callback = None
-        self._failure_callback = None
-        self._session = requests.session()
-        self.token = None
-        self.default_profile = QWebEngineProfile("deriva-auth", self)
-        self.private_profile = QWebEngineProfile(self)
-
-        logging.getLogger().setLevel(log_level)
-        info = "%s v%s [Python: %s (PyQt: %s), %s]" % (
-            self.__class__.__name__, get_installed_version(VERSION),
-            platform.python_version(), PYQT_VERSION_STR, platform.platform(aliased=True))
-        logging.info("Initializing authorization provider: %s" % info)
-        self.cookie_persistence = cookie_persistence
-        self._timer = QTimer(self)
-        self._timer.timeout.connect(self._onTimerFired)
-        self.configure(config, credential_file)
-
-    def configure(self, config, credential_file):
-        self.config = config if config else read_config(self.config_file, create_default=True, default=DEFAULT_CONFIG)
-        self.credential_file = credential_file
-        host = self.config.get("host")
-        if not host:
-            self.set_current_html(ERROR_HTML % "Could not locate hostname parameter in configuration.")
-            return
-        self.auth_url = QUrl()
-        self.auth_url.setScheme(config.get("protocol", "https"))
-        self.auth_url.setHost(host)
-        if config.get("port") is not None:
-            self.auth_url.setPort(config["port"])
-        self.authn_cookie_name = self.config.get("cookie_name", "webauthn")
-
-        self.cookie_file = DEFAULT_SESSION_CONFIG.get("cookie_jar")
-        self.cookie_jar = load_cookies_from_file(self.cookie_file)
-
-        retries = Retry(connect=DEFAULT_SESSION_CONFIG['retry_connect'],
-                        read=DEFAULT_SESSION_CONFIG['retry_read'],
-                        backoff_factor=DEFAULT_SESSION_CONFIG['retry_backoff_factor'],
-                        status_forcelist=DEFAULT_SESSION_CONFIG['retry_status_forcelist'])
-
-        self._session.mount(self.auth_url.toString() + '/',
-                            HTTPAdapter(max_retries=retries))
-
-    def set_current_html(self, html):
-        page = QWebEnginePage(self.parent)
-        page.setHtml(html)
-        self.setPage(page)
-        self.update()
-        qApp.processEvents()
-
-    def authenticated(self):
-        if self.authn_session is None:
-            return False
-
-        now = time.time()
-        if now >= self.authn_expires:
-            return False
-
-        return True
-
-    def login(self):
-        if not (self.auth_url and (self.auth_url.host() and self.auth_url.scheme())):
-            logging.error("Missing or invalid hostname parameter in configuration.")
-            return
-        logging.info("Authenticating with host: %s" % self.auth_url.toString())
-        qApp.setOverrideCursor(Qt.WaitCursor)
-        self._cleanup()
-        self.authn_session_page = QWebEnginePage(self.private_profile, self.parent) \
-            if not self.cookie_persistence else QWebEnginePage(self.default_profile, self.parent)
-        self.authn_session_page.profile().setPersistentCookiesPolicy(
-            QWebEngineProfile.ForcePersistentCookies if self.cookie_persistence else
-            QWebEngineProfile.NoPersistentCookies)
-        if self.cookie_persistence:
-            logging.debug("QTWebEngine persistent storage located at: %s" %
-                          self.authn_session_page.profile().persistentStoragePath())
-        self.authn_session_page.profile().cookieStore().cookieAdded.connect(self._onCookieAdded)
-        self.authn_session_page.profile().cookieStore().cookieRemoved.connect(self._onCookieRemoved)
-        self.authn_session_page.loadProgress.connect(self._onLoadProgress)
-        self.authn_session_page.loadFinished.connect(self._onLoadFinished)
-
-        self.authn_session_page.setUrl(QUrl(self.auth_url.toString() + "/authn/preauth"))
-        self.setPage(self.authn_session_page)
-
-    def logout(self, delete_cookies=False):
-        if not (self.auth_url and (self.auth_url.host() and self.auth_url.scheme())):
-            return
-        if self.authenticated():
-            try:
-                logging.info("Logging out of host: %s" % self.auth_url.toString())
-                if delete_cookies and self.cookie_persistence:
-                    self.authn_session_page.profile().cookieStore().deleteAllCookies()
-                self._session.delete(self.auth_url.toString() + "/authn/session")
-                if self.credential_file:
-                    creds = read_credential(self.credential_file, create_default=True)
-                    host = self.auth_url.host()
-                    if creds.get(host):
-                        del creds[host]
-                    write_credential(self.credential_file, creds)
-            except Exception as e:
-                logging.warning("Logout error: %s" % format_exception(e))
-        self._cleanup()
-
-    def setSuccessCallback(self, callback=None):
-        self._success_callback = callback
-
-    def setFailureCallback(self, callback=None):
-        self._failure_callback = callback
-
-    def setStatus(self, message):
-        if self.window().statusBar is not None:
-            self.window().statusBar().showMessage(message)
-
-    def _execSuccessCallback(self):
-        if self._success_callback:
-            self._success_callback(host=self.auth_url.host(), credential=self.credential)
-
-    def _execFailureCallback(self, message):
-        if self._failure_callback:
-            self._failure_callback(host=self.auth_url.host(), message=message)
-
-    def _onTimerFired(self):
-        if not self.authenticated():
-            self.authn_session = None
-            return
-        resp = self._session.put(self.auth_url.toString() + "/authn/session")
-        seconds_remaining = self.authn_session['seconds_remaining']
-        self.authn_expires = time.time() + seconds_remaining + 1
-        if resp.ok:
-            logging.trace("webauthn session:\n%s\n", resp.json())
-            logging.info("Session refreshed for: %s" % self.auth_url.host())
-        else:
-            logging.warning(
-                "Unable to refresh session for: %s. Server responded: %s" %
-                (self.auth_url.host(),
-                 str.format("%s %s: %s" % (resp.status_code, resp.reason, resp.content.decode()))))
-
-    def _onSessionContent(self, content):
-        try:
-            qApp.restoreOverrideCursor()
-            self.set_current_html(SUCCESS_HTML)
-            try:
-                self.authn_session = json.loads(content)
-            except json.JSONDecodeError:
-                raise RuntimeError("Unable to parse response from server: %s" % content)
-            seconds_remaining = self.authn_session['seconds_remaining']
-            if not self._timer.isActive():
-                interval = seconds_remaining // 2
-                logging.info("Authentication successful for [%s]: credential refresh in %d seconds." %
-                             (self.auth_url.toString(), interval))
-                self._timer.start(interval * 1000)
-            self.authn_expires = time.time() + seconds_remaining + 1
-            logging.trace("webauthn session:\n%s\n", json.dumps(self.authn_session, indent=2))
-            QTimer.singleShot(100, self._execSuccessCallback)
-        except (ValueError, Exception) as e:
-            error = format_exception(e)
-            logging.error(error)
-            self.set_current_html(ERROR_HTML % content)
-            self._execFailureCallback(error)
-
-    def _onPreAuthContent(self, content):
-        try:
-            if not content:
-                logging.debug("no preauth content")
-                return
-            preauth = json.loads(content)
-            logging.trace("webauthn preauth:\n%s\n", json.dumps(preauth, indent=2))
-            qApp.setOverrideCursor(Qt.WaitCursor)
-            self.authn_session_page.setUrl(QUrl(preauth["redirect_url"]))
-        except (ValueError, Exception) as e:
-            logging.error(format_exception(e))
-            self.set_current_html(ERROR_HTML % content)
-
-    def _onLoadFinished(self, result):
-        qApp.restoreOverrideCursor()
-        qApp.processEvents()
-        if not result:
-            self.setPage(self.authn_session_page)
-            logging.debug("Page load error: %s" % self.authn_session_page.url().toDisplayString())
-            return
-        self.set_current_html(DEFAULT_HTML % self.auth_url.host())
-        path = self.authn_session_page.url().path()
-        if path == "/authn/preauth":
-            self.authn_session_page.toPlainText(self._onPreAuthContent)
-        elif path == "/authn/session":
-            self.authn_session_page.toPlainText(self._onSessionContent)
-        else:
-            if self.page() != self.authn_session_page:
-                self.page().deleteLater()
-                self.setPage(self.authn_session_page)
-
-    def _onLoadProgress(self, progress):
-        self.setStatus("Loading page: %s [%d%%]" % (self.page().url().host(), progress))
-
-    def _onCookieAdded(self, cookie):
-        cookie_str = str(cookie.toRawForm(QNetworkCookie.NameAndValueOnly), encoding='utf-8')
-        cookie_name = str(cookie.name(), encoding='utf-8')
-        cookie_val = str(cookie.value(), encoding='utf-8')
-        if (cookie_name == self.authn_cookie_name) and (cookie.domain() == self.config.get("host")):
-            logging.trace("%s cookie added:\n\n%s\n\n" % (self.authn_cookie_name, cookie_str))
-            self.credential["cookie"] = "%s=%s" % (self.authn_cookie_name, cookie_val)
-            host = self.auth_url.host()
-            cred_entry = dict()
-            cred_entry[host] = self.credential
-            if self.credential_file:
-                creds = read_credential(self.credential_file, create_default=True)
-                creds.update(cred_entry)
-                write_credential(self.credential_file, creds)
-            self.token = cookie_val
-            self._session.cookies.set(self.authn_cookie_name, cookie_val, domain=host, path='/')
-            if self.cookie_jar is not None:
-                self.cookie_jar.set_cookie(
-                    create_cookie(self.authn_cookie_name,
-                                  cookie_val,
-                                  domain=host,
-                                  path='/',
-                                  expires=0,
-                                  discard=False,
-                                  secure=True))
-                for path in self.config.get("cookie_jars", DEFAULT_CONFIG["cookie_jars"]):
-                    path_dir = os.path.dirname(path)
-                    if os.path.isdir(path_dir):
-                        logging.debug("Saving cookie jar to: %s" % path)
-                        self.cookie_jar.save(path, ignore_discard=True, ignore_expires=True)
-                    else:
-                        logging.debug("Cookie jar save path [%s] does not exist." % path_dir)
-
-    def _onCookieRemoved(self, cookie):
-        cookie_str = str(cookie.toRawForm(QNetworkCookie.NameAndValueOnly), encoding='utf-8')
-        cookie_name = str(cookie.name(), encoding='utf-8')
-        if cookie_name == self.authn_cookie_name and cookie.domain() == self.url().host():
-            logging.trace("%s cookie removed:\n\n%s\n\n" % (self.authn_cookie_name, cookie_str))
-            if self.cookie_jar:
-                self.cookie_jar.clear(cookie_name, path=cookie.path(), domain=cookie.domain())
-
-    def _cleanup(self):
-        self._timer.stop()
-        self.token = None
-        self.authn_session = None
-        self.authn_expires = time.time()
-        if self.authn_session_page:
-            self.authn_session_page.loadProgress.disconnect(self._onLoadProgress)
-            self.authn_session_page.loadFinished.disconnect(self._onLoadFinished)
-            self.authn_session_page.profile().cookieStore().cookieAdded.disconnect(self._onCookieAdded)
-            self.authn_session_page.profile().cookieStore().cookieRemoved.disconnect(self._onCookieRemoved)
-            self.authn_session_page.deleteLater()
-            self.authn_session_page = None
+import os
+import json
+import logging
+import requests
+import time
+import platform
+from requests.adapters import HTTPAdapter
+from requests.cookies import create_cookie
+from requests.packages.urllib3.util.retry import Retry
+from PyQt5.Qt import PYQT_VERSION_STR
+from PyQt5.QtCore import Qt, QTimer, QUrl
+from PyQt5.QtWidgets import qApp
+from PyQt5.QtNetwork import QNetworkCookie
+from PyQt5.QtWebEngineWidgets import QWebEngineView, QWebEnginePage, QWebEngineProfile
+from deriva.core import read_config, read_credential, write_credential, get_credential, load_cookies_from_file, \
+    format_exception, DEFAULT_SESSION_CONFIG, DEFAULT_CREDENTIAL, DEFAULT_COOKIE_JAR_FILE
+from deriva.core.utils.version_utils import get_installed_version
+from deriva.qt import __version__ as VERSION
+
+DEFAULT_CONFIG = {
+    "servers": [],
+    "cookie_jars": [
+        DEFAULT_COOKIE_JAR_FILE,
+        os.path.join(os.path.expanduser(os.path.normpath("~/.bdbag")), "deriva-cookies.txt")
+    ]
+}
+
+DEFAULT_CONFIG_FILE = os.path.join(os.path.expanduser(os.path.normpath("~/.deriva")), "auth-agent-config.json")
+
+DEFAULT_HTML = '<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8"><title>DERIVA Auth Agent</title></head>' \
+               '<body style="text-align: center; vertical-align: middle;">' \
+               '<div style = "margin-top: 50px;"><font size="+2">' \
+               'Authenticating to:<br/><br/><b>%s</b><br/><br/>Please wait...</font></div>' \
+               '</body></html>'
+
+ERROR_HTML = '<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8"><title>Error</title></head>' \
+             '<body style="text-align: center; vertical-align: middle;">%s</body></html>'
+
+SUCCESS_HTML = '<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8">' \
+               '<title>Authentication Success</title></head>' \
+               '<body style="text-align: center; vertical-align: middle;">' \
+               '<div style = "margin-top: 50px;"><font size="+2"><b>Authentication Successful.</b></font></div>' \
+               '</body></html>'
+
+
+class AuthWidget(QWebEngineView):
+
+    def __init__(self, parent, config=None, credential_file=None, cookie_persistence=False, log_level=logging.INFO):
+        super(AuthWidget, self).__init__(parent)
+
+        self.parent = parent
+        self.config = None
+        self.config_file = DEFAULT_CONFIG_FILE
+        self.credential = DEFAULT_CREDENTIAL
+        self.credential_file = None
+        self.cookie_file = None
+        self.cookie_jar = None
+        self.auth_url = None
+        self.authn_session = None
+        self.authn_session_page = None
+        self.authn_cookie_name = None
+        self.authn_expires = time.time()
+        self._success_callback = None
+        self._failure_callback = None
+        self._session = requests.session()
+        self.token = None
+        self.default_profile = QWebEngineProfile("deriva-auth", self)
+        self.private_profile = QWebEngineProfile(self)
+
+        logging.getLogger().setLevel(log_level)
+        info = "%s v%s [Python: %s (PyQt: %s), %s]" % (
+            self.__class__.__name__, get_installed_version(VERSION),
+            platform.python_version(), PYQT_VERSION_STR, platform.platform(aliased=True))
+        logging.info("Initializing authorization provider: %s" % info)
+        self.cookie_persistence = cookie_persistence
+        self._timer = QTimer(self)
+        self._timer.timeout.connect(self._onTimerFired)
+        self.configure(config, credential_file)
+
+    def configure(self, config, credential_file):
+        self.config = config if config else read_config(self.config_file, create_default=True, default=DEFAULT_CONFIG)
+        self.credential_file = credential_file
+        host = self.config.get("host")
+        if not host:
+            self.set_current_html(ERROR_HTML % "Could not locate hostname parameter in configuration.")
+            return
+        self.auth_url = QUrl()
+        self.auth_url.setScheme(config.get("protocol", "https"))
+        self.auth_url.setHost(host)
+        if config.get("port") is not None:
+            self.auth_url.setPort(config["port"])
+        self.authn_cookie_name = self.config.get("cookie_name", "webauthn")
+
+        self.cookie_file = DEFAULT_SESSION_CONFIG.get("cookie_jar")
+        self.cookie_jar = load_cookies_from_file(self.cookie_file)
+
+        retries = Retry(connect=DEFAULT_SESSION_CONFIG['retry_connect'],
+                        read=DEFAULT_SESSION_CONFIG['retry_read'],
+                        backoff_factor=DEFAULT_SESSION_CONFIG['retry_backoff_factor'],
+                        status_forcelist=DEFAULT_SESSION_CONFIG['retry_status_forcelist'])
+
+        self._session.mount(self.auth_url.toString() + '/',
+                            HTTPAdapter(max_retries=retries))
+
+    def set_current_html(self, html):
+        page = QWebEnginePage(self.parent)
+        page.setHtml(html)
+        self.setPage(page)
+        self.update()
+        qApp.processEvents()
+
+    def authenticated(self, get_session=True):
+        if self.authn_session is None and get_session:
+            credentials = get_credential(self.config["host"])
+            if credentials and 'bearer-token' in credentials:
+                if not self.token:
+                    logging.info("Authenticating to [%s] using externally issued bearer token." %
+                                 self.auth_url.toString())
+                    self._session.headers.update(
+                        {'Authorization': 'Bearer {token}'.format(token=credentials['bearer-token'])})
+                    r = self._session.get(self.auth_url.toString() + "/authn/session")
+                    if r.status_code == 200:
+                        self._onSessionContent(r.json())
+                        self.token = self._session.headers["Authorization"]
+                        return True
+            return False
+
+        now = time.time()
+        if now >= self.authn_expires:
+            return False
+
+        return True
+
+    def login(self):
+        if self.authenticated():
+            return
+        if not (self.auth_url and (self.auth_url.host() and self.auth_url.scheme())):
+            logging.error("Missing or invalid hostname parameter in configuration.")
+            return
+        logging.info("Authenticating to host: %s" % self.auth_url.toString())
+        qApp.setOverrideCursor(Qt.WaitCursor)
+        self._cleanup()
+        self.authn_session_page = QWebEnginePage(self.private_profile, self.parent) \
+            if not self.cookie_persistence else QWebEnginePage(self.default_profile, self.parent)
+        self.authn_session_page.profile().setPersistentCookiesPolicy(
+            QWebEngineProfile.ForcePersistentCookies if self.cookie_persistence else
+            QWebEngineProfile.NoPersistentCookies)
+        if self.cookie_persistence:
+            logging.debug("QTWebEngine persistent storage located at: %s" %
+                          self.authn_session_page.profile().persistentStoragePath())
+        self.authn_session_page.profile().cookieStore().cookieAdded.connect(self._onCookieAdded)
+        self.authn_session_page.profile().cookieStore().cookieRemoved.connect(self._onCookieRemoved)
+        self.authn_session_page.loadProgress.connect(self._onLoadProgress)
+        self.authn_session_page.loadFinished.connect(self._onLoadFinished)
+
+        self.authn_session_page.setUrl(QUrl(self.auth_url.toString() + "/authn/preauth"))
+        self.setPage(self.authn_session_page)
+
+    def logout(self, delete_cookies=False):
+        if not (self.auth_url and (self.auth_url.host() and self.auth_url.scheme())):
+            return
+        if self.authenticated(False):
+            try:
+                logging.info("Logging out of host: %s" % self.auth_url.toString())
+                auth_header = self._session.headers.get("Authorization")
+                if auth_header and (auth_header.startswith("Bearer ") or auth_header.startswith("bearer ")):
+                    logging.info("An externally created bearer token was used to login to: %s. The logout process will "
+                                 "invalidate your current session but will not automatically revoke this token." %
+                                 self.auth_url.toString())
+                if delete_cookies and self.cookie_persistence:
+                    if self.authn_session_page:
+                        self.authn_session_page.profile().cookieStore().deleteAllCookies()
+                self._session.delete(self.auth_url.toString() + "/authn/session")
+                if self.credential_file:
+                    creds = read_credential(self.credential_file, create_default=True)
+                    host = self.auth_url.host()
+                    if creds.get(host):
+                        del creds[host]
+                    write_credential(self.credential_file, creds)
+            except Exception as e:
+                logging.warning("Logout error: %s" % format_exception(e))
+        self._cleanup()
+
+    def setSuccessCallback(self, callback=None):
+        self._success_callback = callback
+
+    def setFailureCallback(self, callback=None):
+        self._failure_callback = callback
+
+    def setStatus(self, message):
+        if self.window().statusBar is not None:
+            self.window().statusBar().showMessage(message)
+
+    def _execSuccessCallback(self):
+        if self._success_callback:
+            self._success_callback(host=self.auth_url.host(), credential=self.credential)
+
+    def _execFailureCallback(self, message):
+        if self._failure_callback:
+            self._failure_callback(host=self.auth_url.host(), message=message)
+
+    def _onTimerFired(self):
+        if not self.authenticated():
+            self.authn_session = None
+            return
+        resp = self._session.put(self.auth_url.toString() + "/authn/session")
+        seconds_remaining = self.authn_session['seconds_remaining']
+        self.authn_expires = time.time() + seconds_remaining + 1
+        if resp.ok:
+            logging.trace("webauthn session:\n%s\n", resp.json())
+            logging.info("Session refreshed for: %s" % self.auth_url.host())
+        else:
+            logging.warning(
+                "Unable to refresh session for: %s. Server responded: %s" %
+                (self.auth_url.host(),
+                 str.format("%s %s: %s" % (resp.status_code, resp.reason, resp.content.decode()))))
+
+    def _onSessionContent(self, content):
+        try:
+            qApp.restoreOverrideCursor()
+            self.set_current_html(SUCCESS_HTML)
+            try:
+                self.authn_session = json.loads(content) if isinstance(content, str) else content
+            except json.JSONDecodeError:
+                raise RuntimeError("Unable to parse response from server: %s" % content)
+            seconds_remaining = self.authn_session['seconds_remaining']
+            if not self._timer.isActive():
+                interval = seconds_remaining // 2
+                logging.info("Authentication successful for [%s]: credential refresh in %d seconds." %
+                             (self.auth_url.toString(), interval))
+                self._timer.start(interval * 1000)
+            self.authn_expires = time.time() + seconds_remaining + 1
+            logging.trace("webauthn session:\n%s\n", json.dumps(self.authn_session, indent=2))
+            QTimer.singleShot(100, self._execSuccessCallback)
+        except (ValueError, Exception) as e:
+            error = format_exception(e)
+            logging.error(error)
+            self.set_current_html(ERROR_HTML % content)
+            self._execFailureCallback(error)
+
+    def _onPreAuthContent(self, content):
+        try:
+            if not content:
+                logging.debug("no preauth content")
+                return
+            preauth = json.loads(content)
+            logging.trace("webauthn preauth:\n%s\n", json.dumps(preauth, indent=2))
+            qApp.setOverrideCursor(Qt.WaitCursor)
+            self.authn_session_page.setUrl(QUrl(preauth["redirect_url"]))
+        except (ValueError, Exception) as e:
+            logging.error(format_exception(e))
+            self.set_current_html(ERROR_HTML % content)
+
+    def _onLoadFinished(self, result):
+        qApp.restoreOverrideCursor()
+        qApp.processEvents()
+        if not result:
+            self.setPage(self.authn_session_page)
+            logging.debug("Page load error: %s" % self.authn_session_page.url().toDisplayString())
+            return
+        self.set_current_html(DEFAULT_HTML % self.auth_url.host())
+        path = self.authn_session_page.url().path()
+        if path == "/authn/preauth":
+            self.authn_session_page.toPlainText(self._onPreAuthContent)
+        elif path == "/authn/session":
+            self.authn_session_page.toPlainText(self._onSessionContent)
+        else:
+            if self.page() != self.authn_session_page:
+                self.page().deleteLater()
+                self.setPage(self.authn_session_page)
+
+    def _onLoadProgress(self, progress):
+        self.setStatus("Loading page: %s [%d%%]" % (self.page().url().host(), progress))
+
+    def _onCookieAdded(self, cookie):
+        cookie_str = str(cookie.toRawForm(QNetworkCookie.NameAndValueOnly), encoding='utf-8')
+        cookie_name = str(cookie.name(), encoding='utf-8')
+        cookie_val = str(cookie.value(), encoding='utf-8')
+        if (cookie_name == self.authn_cookie_name) and (cookie.domain() == self.config.get("host")):
+            logging.trace("%s cookie added:\n\n%s\n\n" % (self.authn_cookie_name, cookie_str))
+            self.credential["cookie"] = "%s=%s" % (self.authn_cookie_name, cookie_val)
+            host = self.auth_url.host()
+            cred_entry = dict()
+            cred_entry[host] = self.credential
+            if self.credential_file:
+                creds = read_credential(self.credential_file, create_default=True)
+                creds.update(cred_entry)
+                write_credential(self.credential_file, creds)
+            self.token = "Cookie %s" % cookie_val
+            self._session.cookies.set(self.authn_cookie_name, cookie_val, domain=host, path='/')
+            if self.cookie_jar is not None:
+                self.cookie_jar.set_cookie(
+                    create_cookie(self.authn_cookie_name,
+                                  cookie_val,
+                                  domain=host,
+                                  path='/',
+                                  expires=0,
+                                  discard=False,
+                                  secure=True))
+                for path in self.config.get("cookie_jars", DEFAULT_CONFIG["cookie_jars"]):
+                    path_dir = os.path.dirname(path)
+                    if os.path.isdir(path_dir):
+                        logging.debug("Saving cookie jar to: %s" % path)
+                        self.cookie_jar.save(path, ignore_discard=True, ignore_expires=True)
+                    else:
+                        logging.debug("Cookie jar save path [%s] does not exist." % path_dir)
+
+    def _onCookieRemoved(self, cookie):
+        cookie_str = str(cookie.toRawForm(QNetworkCookie.NameAndValueOnly), encoding='utf-8')
+        cookie_name = str(cookie.name(), encoding='utf-8')
+        if cookie_name == self.authn_cookie_name and cookie.domain() == self.url().host():
+            logging.trace("%s cookie removed:\n\n%s\n\n" % (self.authn_cookie_name, cookie_str))
+            if self.cookie_jar:
+                self.cookie_jar.clear(cookie_name, path=cookie.path(), domain=cookie.domain())
+
+    def _cleanup(self):
+        self._timer.stop()
+        self.token = None
+        self.authn_session = None
+        self.authn_expires = time.time()
+        if self.authn_session_page:
+            self.authn_session_page.loadProgress.disconnect(self._onLoadProgress)
+            self.authn_session_page.loadFinished.disconnect(self._onLoadFinished)
+            self.authn_session_page.profile().cookieStore().cookieAdded.disconnect(self._onCookieAdded)
+            self.authn_session_page.profile().cookieStore().cookieRemoved.disconnect(self._onCookieRemoved)
+            self.authn_session_page.deleteLater()
+            self.authn_session_page = None
```

### Comparing `deriva-qt-1.6.1/deriva/qt/auth_agent/ui/embedded_auth_window.py` & `deriva-qt-1.6.3/deriva/qt/auth_agent/ui/embedded_auth_window.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-import logging
-from PyQt5.QtCore import Qt, QEvent, QMetaObject
-from PyQt5.QtGui import QIcon
-from PyQt5.QtWidgets import QWidget, QMainWindow, QStatusBar, QVBoxLayout, QMessageBox
-from deriva.qt import __version__ as VERSION
-from deriva.qt.auth_agent.ui.auth_widget import AuthWidget
-from deriva.qt.auth_agent.resources import resources
-
-
-class EmbeddedAuthWindow(QMainWindow):
-
-    def __init__(self,
-                 parent,
-                 config,
-                 credential_file=None,
-                 cookie_persistence=False,
-                 authentication_success_callback=None,
-                 authentication_failure_callback=None,
-                 log_level=logging.INFO):
-        super(EmbeddedAuthWindow, self).__init__(parent)
-        success_callback = \
-            self.successCallback if not authentication_success_callback else authentication_success_callback
-        failure_callback = \
-            self.failureCallback if not authentication_failure_callback else authentication_failure_callback
-        self.ui = EmbeddedAuthWindowUI(self,
-                                       config,
-                                       credential_file,
-                                       cookie_persistence,
-                                       success_callback,
-                                       failure_callback,
-                                       log_level)
-        self.cookie_persistence = cookie_persistence
-        self.log_level = log_level
-
-    def authenticated(self):
-        return self.ui.authWidget.authenticated()
-
-    def login(self):
-        self.ui.authWidget.login()
-
-    def logout(self, delete_cookies=False):
-        self.ui.authWidget.logout(delete_cookies)
-
-    def successCallback(self, **kwargs):
-        host = kwargs.get("host")
-        if host:
-            self.statusBar().showMessage("Authenticated: %s" % host)
-        self.hide()
-
-    def failureCallback(self, **kwargs):
-        host = kwargs.get("host")
-        message = kwargs.get("message", "Unknown Error")
-        if host:
-            self.statusBar().showMessage(message)
-            msg = QMessageBox()
-            msg.setIcon(QMessageBox.Critical)
-            msg.setWindowTitle("Error authenticating to host: %s" % host)
-            msg.setText(message)
-            msg.setStandardButtons(QMessageBox.Close)
-            msg.exec_()
-        self.hide()
-
-    def changeEvent(self, event):
-        if event.type() == QEvent.WindowStateChange:
-            if self.windowState() & Qt.WindowMinimized:
-                event.ignore()
-                self.hide()
-                return
-
-        super(EmbeddedAuthWindow, self).changeEvent(event)
-
-    def closeEvent(self, event):
-        self.logout()
-
-
-class EmbeddedAuthWindowUI(object):
-
-    def __init__(self,
-                 MainWin,
-                 config,
-                 credential_file,
-                 cookie_persistence,
-                 success_callback,
-                 failure_callback,
-                 log_level):
-
-        # Main Window
-        MainWin.setObjectName("EmbeddedAuthWindow")
-        MainWin.setWindowIcon(QIcon(":/images/keys.png"))
-        MainWin.setWindowTitle(MainWin.tr("DERIVA Authentication Agent %s" % VERSION))
-        MainWin.resize(1024, 745)
-        self.centralWidget = QWidget(MainWin)
-        self.centralWidget.setObjectName("centralWidget")
-        MainWin.setCentralWidget(self.centralWidget)
-        self.verticalLayout = QVBoxLayout(self.centralWidget)
-        self.verticalLayout.setContentsMargins(11, 11, 11, 11)
-        self.verticalLayout.setSpacing(6)
-        self.verticalLayout.setObjectName("verticalLayout")
-        self.authWidget = AuthWidget(MainWin, config, credential_file, cookie_persistence, log_level)
-        self.authWidget.setSuccessCallback(success_callback)
-        self.authWidget.setFailureCallback(failure_callback)
-        self.authWidget.setObjectName("authWidget")
-        self.verticalLayout.addWidget(self.authWidget)
-
-        # Status Bar
-
-        self.statusBar = QStatusBar(MainWin)
-        self.statusBar.setToolTip("")
-        self.statusBar.setStatusTip("")
-        self.statusBar.setObjectName("statusBar")
-        MainWin.setStatusBar(self.statusBar)
-
-        # finalize UI setup
-        QMetaObject.connectSlotsByName(MainWin)
+import logging
+from PyQt5.QtCore import Qt, QEvent, QMetaObject
+from PyQt5.QtGui import QIcon
+from PyQt5.QtWidgets import QWidget, QMainWindow, QStatusBar, QVBoxLayout, QMessageBox
+from deriva.qt import __version__ as VERSION
+from deriva.qt.auth_agent.ui.auth_widget import AuthWidget
+from deriva.qt.auth_agent.resources import resources
+
+
+class EmbeddedAuthWindow(QMainWindow):
+
+    def __init__(self,
+                 parent,
+                 config,
+                 credential_file=None,
+                 cookie_persistence=False,
+                 authentication_success_callback=None,
+                 authentication_failure_callback=None,
+                 log_level=logging.INFO):
+        super(EmbeddedAuthWindow, self).__init__(parent)
+        success_callback = \
+            self.successCallback if not authentication_success_callback else authentication_success_callback
+        failure_callback = \
+            self.failureCallback if not authentication_failure_callback else authentication_failure_callback
+        self.ui = EmbeddedAuthWindowUI(self,
+                                       config,
+                                       credential_file,
+                                       cookie_persistence,
+                                       success_callback,
+                                       failure_callback,
+                                       log_level)
+        self.cookie_persistence = cookie_persistence
+        self.log_level = log_level
+
+    def authenticated(self, get_session=True):
+        return self.ui.authWidget.authenticated(get_session)
+
+    def login(self):
+        self.ui.authWidget.login()
+
+    def logout(self, delete_cookies=False):
+        self.ui.authWidget.logout(delete_cookies)
+
+    def successCallback(self, **kwargs):
+        host = kwargs.get("host")
+        if host:
+            self.statusBar().showMessage("Authenticated: %s" % host)
+        self.hide()
+
+    def failureCallback(self, **kwargs):
+        host = kwargs.get("host")
+        message = kwargs.get("message", "Unknown Error")
+        if host:
+            self.statusBar().showMessage(message)
+            msg = QMessageBox()
+            msg.setIcon(QMessageBox.Critical)
+            msg.setWindowTitle("Error authenticating to host: %s" % host)
+            msg.setText(message)
+            msg.setStandardButtons(QMessageBox.Close)
+            msg.exec_()
+        self.hide()
+
+    def changeEvent(self, event):
+        if event.type() == QEvent.WindowStateChange:
+            if self.windowState() & Qt.WindowMinimized:
+                event.ignore()
+                self.hide()
+                return
+
+        super(EmbeddedAuthWindow, self).changeEvent(event)
+
+    def closeEvent(self, event):
+        self.logout()
+
+
+class EmbeddedAuthWindowUI(object):
+
+    def __init__(self,
+                 MainWin,
+                 config,
+                 credential_file,
+                 cookie_persistence,
+                 success_callback,
+                 failure_callback,
+                 log_level):
+
+        # Main Window
+        MainWin.setObjectName("EmbeddedAuthWindow")
+        MainWin.setWindowIcon(QIcon(":/images/keys.png"))
+        MainWin.setWindowTitle(MainWin.tr("DERIVA Authentication Agent %s" % VERSION))
+        MainWin.resize(1024, 745)
+        self.centralWidget = QWidget(MainWin)
+        self.centralWidget.setObjectName("centralWidget")
+        MainWin.setCentralWidget(self.centralWidget)
+        self.verticalLayout = QVBoxLayout(self.centralWidget)
+        self.verticalLayout.setContentsMargins(11, 11, 11, 11)
+        self.verticalLayout.setSpacing(6)
+        self.verticalLayout.setObjectName("verticalLayout")
+        self.authWidget = AuthWidget(MainWin, config, credential_file, cookie_persistence, log_level)
+        self.authWidget.setSuccessCallback(success_callback)
+        self.authWidget.setFailureCallback(failure_callback)
+        self.authWidget.setObjectName("authWidget")
+        self.verticalLayout.addWidget(self.authWidget)
+
+        # Status Bar
+
+        self.statusBar = QStatusBar(MainWin)
+        self.statusBar.setToolTip("")
+        self.statusBar.setStatusTip("")
+        self.statusBar.setObjectName("statusBar")
+        MainWin.setStatusBar(self.statusBar)
+
+        # finalize UI setup
+        QMetaObject.connectSlotsByName(MainWin)
```

### Comparing `deriva-qt-1.6.1/deriva/qt/common/json_editor.py` & `deriva-qt-1.6.3/deriva/qt/common/json_editor.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,207 +1,207 @@
-import sys
-
-from PyQt5.QtCore import Qt, QRegExp, QSize, QRect
-from PyQt5.QtGui import QSyntaxHighlighter, QTextCharFormat, QFont, QPainter, QColor, QTextFormat
-from PyQt5.QtWidgets import QTextEdit, QApplication, QWidget, QPlainTextEdit, QMessageBox, QDialog, QVBoxLayout
-
-
-class JSONSyntaxHighlighter(QSyntaxHighlighter):
-    def __init__(self, parent=None):
-        super(JSONSyntaxHighlighter, self).__init__(parent)
-
-        self.symbol_format = QTextCharFormat()
-        self.symbol_format.setForeground(Qt.blue)
-        self.symbol_format.setFontWeight(QFont.Bold)
-
-        self.name_format = QTextCharFormat()
-        self.name_format.setForeground(Qt.darkMagenta)
-        self.name_format.setFontWeight(QFont.Bold)
-        self.name_format.setFontItalic(True)
-
-        self.value_format = QTextCharFormat()
-        self.value_format.setForeground(Qt.darkGreen)
-
-    def highlightBlock(self, text):
-        expression = QRegExp("(\\{|\\}|\\[|\\]|\\:|\\,)")
-        index = expression.indexIn(text)
-        while index >= 0:
-            length = expression.matchedLength()
-            self.setFormat(index, length, self.symbol_format)
-            index = expression.indexIn(text, index + length)
-
-        text.replace("\\\"", "  ")
-
-        expression = QRegExp("\".*\" *\\:")
-        expression.setMinimal(True)
-        index = expression.indexIn(text)
-        while index >= 0:
-            length = expression.matchedLength()
-            self.setFormat(index, length - 1, self.name_format)
-            index = expression.indexIn(text, index + length)
-
-        expression = QRegExp("\\: *\".*\"")
-        expression.setMinimal(True)
-        index = expression.indexIn(text)
-        while index >= 0:
-            length = expression.matchedLength()
-            self.setFormat(index, length, self.value_format)
-            index = expression.indexIn(text, index + length)
-
-
-class LineNumberArea(QWidget):
-
-    def __init__(self, editor):
-        super().__init__(editor)
-        self.editor = editor
-
-    def sizeHint(self):
-        return QSize(self.editor.lineNumberAreaWidth(), 0)
-
-    def paintEvent(self, event):
-        self.editor.lineNumberAreaPaintEvent(event)
-
-
-class CodeEditor(QPlainTextEdit):
-    def __init__(self):
-        super().__init__()
-        self.modified = False
-        self.lineNumberArea = LineNumberArea(self)
-
-        self.modificationChanged.connect(self.setModified)
-        self.blockCountChanged.connect(self.updateLineNumberAreaWidth)
-        self.updateRequest.connect(self.updateLineNumberArea)
-        self.cursorPositionChanged.connect(self.highlightCurrentLine)
-
-        self.updateLineNumberAreaWidth(0)
-
-    def setModified(self, modified):
-        self.modified = modified
-
-    def lineNumberAreaWidth(self):
-        digits = 1
-        count = max(1, self.blockCount())
-        while count >= 10:
-            count /= 10
-            digits += 1
-        space = 3 + self.fontMetrics().width('9') * digits
-        return space
-
-    def updateLineNumberAreaWidth(self, _):
-        self.setViewportMargins(self.lineNumberAreaWidth(), 0, 0, 0)
-
-    def updateLineNumberArea(self, rect, dy):
-
-        if dy:
-            self.lineNumberArea.scroll(0, dy)
-        else:
-            self.lineNumberArea.update(0, rect.y(), self.lineNumberArea.width(), rect.height())
-
-        if rect.contains(self.viewport().rect()):
-            self.updateLineNumberAreaWidth(0)
-
-    def resizeEvent(self, event):
-        super().resizeEvent(event)
-
-        cr = self.contentsRect()
-        self.lineNumberArea.setGeometry(QRect(cr.left(), cr.top(), self.lineNumberAreaWidth(), cr.height()))
-
-    def lineNumberAreaPaintEvent(self, event):
-        painter = QPainter(self.lineNumberArea)
-
-        painter.fillRect(event.rect(), Qt.lightGray)
-
-        block = self.firstVisibleBlock()
-        blockNumber = block.blockNumber()
-        top = self.blockBoundingGeometry(block).translated(self.contentOffset()).top()
-        bottom = top + self.blockBoundingRect(block).height()
-
-        height = self.fontMetrics().height()
-        while block.isValid() and (top <= event.rect().bottom()):
-            if block.isVisible() and (bottom >= event.rect().top()):
-                number = str(blockNumber + 1)
-                painter.setPen(Qt.black)
-                painter.drawText(0, top, self.lineNumberArea.width(), height, Qt.AlignRight, number)
-
-            block = block.next()
-            top = bottom
-            bottom = top + self.blockBoundingRect(block).height()
-            blockNumber += 1
-
-    def highlightCurrentLine(self):
-        extraSelections = []
-
-        if not self.isReadOnly():
-            selection = QTextEdit.ExtraSelection()
-            lineColor = QColor(Qt.yellow).lighter(160)
-            selection.format.setBackground(lineColor)
-            selection.format.setProperty(QTextFormat.FullWidthSelection, True)
-            selection.cursor = self.textCursor()
-            selection.cursor.clearSelection()
-            extraSelections.append(selection)
-
-        self.setExtraSelections(extraSelections)
-
-
-class JSONEditor(QDialog):
-    def __init__(self, parent, file_path, title="JSON Editor"):
-        super().__init__(parent)
-        self.setWindowTitle(title)
-        self.file_path = file_path
-        self.editor = CodeEditor()
-        self.highlighter = JSONSyntaxHighlighter(self.editor.document())
-        self.initUI()
-        self.openFile()
-
-    def initUI(self):
-        layout = QVBoxLayout()
-        layout.addWidget(self.editor)
-        self.setLayout(layout)
-        font = QFont()
-        font.setFamily('Courier')
-        font.setFixedPitch(True)
-        font.setPointSize(10)
-        self.setFont(font)
-
-        self.setMinimumSize(800, 600)
-        self.setWindowFlags(self.windowFlags() & ~Qt.WindowContextHelpButtonHint)
-        self.setSizeGripEnabled(True)
-        self.show()
-
-    def saveFile(self):
-        with open(self.file_path, 'w') as f:
-            file_data = self.editor.toPlainText()
-            f.write(file_data)
-
-    def openFile(self):
-        with open(self.file_path, 'r') as f:
-            file_data = f.read()
-            self.editor.setPlainText(file_data)
-
-    def closeEvent(self, event=None):
-        if not self.editor.modified:
-            return
-        msg = QMessageBox()
-        msg.setIcon(QMessageBox.Information)
-        msg.setWindowIcon(self.parent().windowIcon())
-        msg.setWindowTitle("Save Changes?")
-        msg.setText("Do you want to save changes to this file?")
-        msg.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
-        ret = msg.exec_()
-        if ret == QMessageBox.Yes:
-            self.saveFile()
-        if event:
-            event.accept()
-
-    def isModified(self):
-        return self.editor.modified
-
-
-def main():
-    app = QApplication(sys.argv)
-    editor = JSONEditor(sys.argv[1])
-    editor.exec_()
-    sys.exit(app.exec_())
-
-
-if __name__ == "__main__":
-    main()
+import sys
+
+from PyQt5.QtCore import Qt, QRegExp, QSize, QRect
+from PyQt5.QtGui import QSyntaxHighlighter, QTextCharFormat, QFont, QPainter, QColor, QTextFormat
+from PyQt5.QtWidgets import QTextEdit, QApplication, QWidget, QPlainTextEdit, QMessageBox, QDialog, QVBoxLayout
+
+
+class JSONSyntaxHighlighter(QSyntaxHighlighter):
+    def __init__(self, parent=None):
+        super(JSONSyntaxHighlighter, self).__init__(parent)
+
+        self.symbol_format = QTextCharFormat()
+        self.symbol_format.setForeground(Qt.blue)
+        self.symbol_format.setFontWeight(QFont.Bold)
+
+        self.name_format = QTextCharFormat()
+        self.name_format.setForeground(Qt.darkMagenta)
+        self.name_format.setFontWeight(QFont.Bold)
+        self.name_format.setFontItalic(True)
+
+        self.value_format = QTextCharFormat()
+        self.value_format.setForeground(Qt.darkGreen)
+
+    def highlightBlock(self, text):
+        expression = QRegExp("(\\{|\\}|\\[|\\]|\\:|\\,)")
+        index = expression.indexIn(text)
+        while index >= 0:
+            length = expression.matchedLength()
+            self.setFormat(index, length, self.symbol_format)
+            index = expression.indexIn(text, index + length)
+
+        text.replace("\\\"", "  ")
+
+        expression = QRegExp("\".*\" *\\:")
+        expression.setMinimal(True)
+        index = expression.indexIn(text)
+        while index >= 0:
+            length = expression.matchedLength()
+            self.setFormat(index, length - 1, self.name_format)
+            index = expression.indexIn(text, index + length)
+
+        expression = QRegExp("\\: *\".*\"")
+        expression.setMinimal(True)
+        index = expression.indexIn(text)
+        while index >= 0:
+            length = expression.matchedLength()
+            self.setFormat(index, length, self.value_format)
+            index = expression.indexIn(text, index + length)
+
+
+class LineNumberArea(QWidget):
+
+    def __init__(self, editor):
+        super().__init__(editor)
+        self.editor = editor
+
+    def sizeHint(self):
+        return QSize(self.editor.lineNumberAreaWidth(), 0)
+
+    def paintEvent(self, event):
+        self.editor.lineNumberAreaPaintEvent(event)
+
+
+class CodeEditor(QPlainTextEdit):
+    def __init__(self):
+        super().__init__()
+        self.modified = False
+        self.lineNumberArea = LineNumberArea(self)
+
+        self.modificationChanged.connect(self.setModified)
+        self.blockCountChanged.connect(self.updateLineNumberAreaWidth)
+        self.updateRequest.connect(self.updateLineNumberArea)
+        self.cursorPositionChanged.connect(self.highlightCurrentLine)
+
+        self.updateLineNumberAreaWidth(0)
+
+    def setModified(self, modified):
+        self.modified = modified
+
+    def lineNumberAreaWidth(self):
+        digits = 1
+        count = max(1, self.blockCount())
+        while count >= 10:
+            count /= 10
+            digits += 1
+        space = 3 + self.fontMetrics().width('9') * digits
+        return space
+
+    def updateLineNumberAreaWidth(self, _):
+        self.setViewportMargins(self.lineNumberAreaWidth(), 0, 0, 0)
+
+    def updateLineNumberArea(self, rect, dy):
+
+        if dy:
+            self.lineNumberArea.scroll(0, dy)
+        else:
+            self.lineNumberArea.update(0, rect.y(), self.lineNumberArea.width(), rect.height())
+
+        if rect.contains(self.viewport().rect()):
+            self.updateLineNumberAreaWidth(0)
+
+    def resizeEvent(self, event):
+        super().resizeEvent(event)
+
+        cr = self.contentsRect()
+        self.lineNumberArea.setGeometry(QRect(cr.left(), cr.top(), self.lineNumberAreaWidth(), cr.height()))
+
+    def lineNumberAreaPaintEvent(self, event):
+        painter = QPainter(self.lineNumberArea)
+
+        painter.fillRect(event.rect(), Qt.lightGray)
+
+        block = self.firstVisibleBlock()
+        blockNumber = block.blockNumber()
+        top = self.blockBoundingGeometry(block).translated(self.contentOffset()).top()
+        bottom = top + self.blockBoundingRect(block).height()
+
+        height = self.fontMetrics().height()
+        while block.isValid() and (top <= event.rect().bottom()):
+            if block.isVisible() and (bottom >= event.rect().top()):
+                number = str(blockNumber + 1)
+                painter.setPen(Qt.black)
+                painter.drawText(0, top, self.lineNumberArea.width(), height, Qt.AlignRight, number)
+
+            block = block.next()
+            top = bottom
+            bottom = top + self.blockBoundingRect(block).height()
+            blockNumber += 1
+
+    def highlightCurrentLine(self):
+        extraSelections = []
+
+        if not self.isReadOnly():
+            selection = QTextEdit.ExtraSelection()
+            lineColor = QColor(Qt.yellow).lighter(160)
+            selection.format.setBackground(lineColor)
+            selection.format.setProperty(QTextFormat.FullWidthSelection, True)
+            selection.cursor = self.textCursor()
+            selection.cursor.clearSelection()
+            extraSelections.append(selection)
+
+        self.setExtraSelections(extraSelections)
+
+
+class JSONEditor(QDialog):
+    def __init__(self, parent, file_path, title="JSON Editor"):
+        super().__init__(parent)
+        self.setWindowTitle(title)
+        self.file_path = file_path
+        self.editor = CodeEditor()
+        self.highlighter = JSONSyntaxHighlighter(self.editor.document())
+        self.initUI()
+        self.openFile()
+
+    def initUI(self):
+        layout = QVBoxLayout()
+        layout.addWidget(self.editor)
+        self.setLayout(layout)
+        font = QFont()
+        font.setFamily('Courier')
+        font.setFixedPitch(True)
+        font.setPointSize(10)
+        self.setFont(font)
+
+        self.setMinimumSize(800, 600)
+        self.setWindowFlags(self.windowFlags() & ~Qt.WindowContextHelpButtonHint)
+        self.setSizeGripEnabled(True)
+        self.show()
+
+    def saveFile(self):
+        with open(self.file_path, 'w') as f:
+            file_data = self.editor.toPlainText()
+            f.write(file_data)
+
+    def openFile(self):
+        with open(self.file_path, 'r') as f:
+            file_data = f.read()
+            self.editor.setPlainText(file_data)
+
+    def closeEvent(self, event=None):
+        if not self.editor.modified:
+            return
+        msg = QMessageBox()
+        msg.setIcon(QMessageBox.Information)
+        msg.setWindowIcon(self.parent().windowIcon())
+        msg.setWindowTitle("Save Changes?")
+        msg.setText("Do you want to save changes to this file?")
+        msg.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
+        ret = msg.exec_()
+        if ret == QMessageBox.Yes:
+            self.saveFile()
+        if event:
+            event.accept()
+
+    def isModified(self):
+        return self.editor.modified
+
+
+def main():
+    app = QApplication(sys.argv)
+    editor = JSONEditor(sys.argv[1])
+    editor.exec_()
+    sys.exit(app.exec_())
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `deriva-qt-1.6.1/deriva/qt/common/log_widget.py` & `deriva-qt-1.6.3/deriva/qt/common/log_widget.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from PyQt5.Qt import qApp
-from PyQt5.QtCore import pyqtSignal
-from PyQt5.QtWidgets import QPlainTextEdit
-import logging
-
-
-class QPlainTextEditLogger(logging.Handler):
-
-    def __init__(self, parent):
-        logging.Handler.__init__(self)
-        self.widget = QPlainTextEditLog(parent)
-
-    def emit(self, record):
-        msg = self.format(record)
-        self.widget.log_update_signal.emit(msg)
-        qApp.processEvents()
-
-
-class QPlainTextEditLog(QPlainTextEdit):
-    log_update_signal = pyqtSignal(str)
-
-    def __init__(self, parent):
-        super(QPlainTextEdit, self).__init__(parent)
-        self.setReadOnly(True)
-        self.setBackgroundVisible(True)
+from PyQt5.Qt import qApp
+from PyQt5.QtCore import pyqtSignal
+from PyQt5.QtWidgets import QPlainTextEdit
+import logging
+
+
+class QPlainTextEditLogger(logging.Handler):
+
+    def __init__(self, parent):
+        logging.Handler.__init__(self)
+        self.widget = QPlainTextEditLog(parent)
+
+    def emit(self, record):
+        msg = self.format(record)
+        self.widget.log_update_signal.emit(msg)
+        qApp.processEvents()
+
+
+class QPlainTextEditLog(QPlainTextEdit):
+    log_update_signal = pyqtSignal(str)
+
+    def __init__(self, parent):
+        super(QPlainTextEdit, self).__init__(parent)
+        self.setReadOnly(True)
+        self.setBackgroundVisible(True)
```

### Comparing `deriva-qt-1.6.1/deriva/qt/upload_gui/impl/upload_tasks.py` & `deriva-qt-1.6.3/deriva/qt/upload_gui/impl/upload_tasks.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-from PyQt5.QtCore import QObject, pyqtSignal
-from deriva.core import format_exception
-from deriva.transfer import DerivaUpload
-from deriva.qt import async_execute, Task
-
-
-class UploadTask(QObject):
-    status_update_signal = pyqtSignal(bool, str, str, object)
-    progress_update_signal = pyqtSignal(int, int)
-
-    def __init__(self, uploader, parent=None):
-        super(UploadTask, self).__init__(parent)
-        assert (uploader is not None and isinstance(uploader, DerivaUpload))
-        self.uploader = uploader
-        self.task = None
-
-    def start(self):
-        async_execute(self.task)
-
-    def cancel(self):
-        self.task.cancel()
-
-    def set_status(self, success, status, detail, result):
-        self.status_update_signal.emit(success, status, detail, result)
-
-    def result_callback(self, success, result):
-        self.set_status(success, str(status), "", result)
-
-    def progress_callback(self, current, maximum):
-        if self.task.canceled:
-            return False
-
-        self.progress_update_signal.emit(current, maximum)
-        return True
-
-
-class SessionQueryTask(UploadTask):
-    def __init__(self, parent=None):
-        super(SessionQueryTask, self).__init__(parent)
-
-    def result_callback(self, success, result):
-        self.set_status(success,
-                        "Session query success" if success else "Session query failure",
-                        "" if success else format_exception(result),
-                        result.json() if success else None)
-
-    def query(self):
-        self.task = Task(self.uploader.catalog.get_authn_session, [], self.result_callback)
-        self.start()
-
-
-class ConfigUpdateTask(UploadTask):
-    def __init__(self, parent=None):
-        super(ConfigUpdateTask, self).__init__(parent)
-
-    def result_callback(self, success, result):
-        self.set_status(success,
-                        "Configuration update success" if success else "Configuration update failure",
-                        "" if success else format_exception(result),
-                        result if success else None)
-
-    def update_config(self):
-        self.task = Task(self.uploader.getUpdatedConfig, [], self.result_callback)
-        self.start()
-
-
-class ScanDirectoryTask(UploadTask):
-    def __init__(self, parent=None):
-        super(ScanDirectoryTask, self).__init__(parent)
-
-    def result_callback(self, success, result):
-        self.set_status(success,
-                        "Directory scan success" if success else "Directory scan failure.",
-                        "" if success else format_exception(result),
-                        None)
-
-    def scan(self, path):
-        self.task = Task(self.uploader.scanDirectory, [path], self.result_callback)
-        self.start()
-
-
-class UploadFilesTask(UploadTask):
-    def __init__(self, parent=None):
-        super(UploadFilesTask, self).__init__(parent)
-
-    def result_callback(self, success, result):
-        self.set_status(success,
-                        "File upload success" if success else "File upload failure",
-                        "" if success else format_exception(result),
-                        None)
-
-    def upload(self, status_callback=None, file_callback=None):
-        self.task = Task(self.uploader.uploadFiles, [status_callback, file_callback], self.result_callback)
-        self.start()
+from PyQt5.QtCore import QObject, pyqtSignal
+from deriva.core import format_exception
+from deriva.transfer import DerivaUpload
+from deriva.qt import async_execute, Task
+
+
+class UploadTask(QObject):
+    status_update_signal = pyqtSignal(bool, str, str, object)
+    progress_update_signal = pyqtSignal(int, int)
+
+    def __init__(self, uploader, parent=None):
+        super(UploadTask, self).__init__(parent)
+        assert (uploader is not None and isinstance(uploader, DerivaUpload))
+        self.uploader = uploader
+        self.task = None
+
+    def start(self):
+        async_execute(self.task)
+
+    def cancel(self):
+        self.task.cancel()
+
+    def set_status(self, success, status, detail, result):
+        self.status_update_signal.emit(success, status, detail, result)
+
+    def result_callback(self, success, result):
+        self.set_status(success, str(status), "", result)
+
+    def progress_callback(self, current, maximum):
+        if self.task.canceled:
+            return False
+
+        self.progress_update_signal.emit(current, maximum)
+        return True
+
+
+class SessionQueryTask(UploadTask):
+    def __init__(self, parent=None):
+        super(SessionQueryTask, self).__init__(parent)
+
+    def result_callback(self, success, result):
+        self.set_status(success,
+                        "Session query success" if success else "Session query failure",
+                        "" if success else format_exception(result),
+                        result.json() if success else None)
+
+    def query(self):
+        self.task = Task(self.uploader.catalog.get_authn_session, [], self.result_callback)
+        self.start()
+
+
+class ConfigUpdateTask(UploadTask):
+    def __init__(self, parent=None):
+        super(ConfigUpdateTask, self).__init__(parent)
+
+    def result_callback(self, success, result):
+        self.set_status(success,
+                        "Configuration update success" if success else "Configuration update failure",
+                        "" if success else format_exception(result),
+                        result if success else None)
+
+    def update_config(self):
+        self.task = Task(self.uploader.getUpdatedConfig, [], self.result_callback)
+        self.start()
+
+
+class ScanDirectoryTask(UploadTask):
+    def __init__(self, parent=None):
+        super(ScanDirectoryTask, self).__init__(parent)
+
+    def result_callback(self, success, result):
+        self.set_status(success,
+                        "Directory scan success" if success else "Directory scan failure.",
+                        "" if success else format_exception(result),
+                        None)
+
+    def scan(self, path):
+        self.task = Task(self.uploader.scanDirectory, [path], self.result_callback)
+        self.start()
+
+
+class UploadFilesTask(UploadTask):
+    def __init__(self, parent=None):
+        super(UploadFilesTask, self).__init__(parent)
+
+    def result_callback(self, success, result):
+        self.set_status(success,
+                        "File upload success" if success else "File upload failure",
+                        "" if success else format_exception(result),
+                        None)
+
+    def upload(self, status_callback=None, file_callback=None):
+        self.task = Task(self.uploader.uploadFiles, [status_callback, file_callback], self.result_callback)
+        self.start()
```

### Comparing `deriva-qt-1.6.1/deriva/qt/upload_gui/resources/images/upload.icns` & `deriva-qt-1.6.3/deriva/qt/upload_gui/resources/images/upload.icns`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/deriva/qt/upload_gui/resources/images/upload.ico` & `deriva-qt-1.6.3/deriva/qt/upload_gui/resources/images/upload.ico`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/deriva/qt/upload_gui/resources/images/upload.png` & `deriva-qt-1.6.3/deriva/qt/upload_gui/resources/images/upload.png`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/deriva/qt/upload_gui/resources/resources.py` & `deriva-qt-1.6.3/deriva/qt/upload_gui/resources/resources.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,580 +1,580 @@
-# -*- coding: utf-8 -*-
-
-# Resource object code
-#
-# Created by: The Resource Compiler for PyQt5 (Qt v5.7.1)
-#
-# WARNING! All changes made in this file will be lost!
-
-from PyQt5 import QtCore
-
-qt_resource_data = b"\
-\x00\x00\x21\xcf\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x01\x00\x00\x00\x01\x00\x08\x06\x00\x00\x00\x5c\x72\xa8\x66\
-\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\x0b\x13\x00\x00\x0b\x13\
-\x01\x00\x9a\x9c\x18\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\
-\x25\x00\x00\x80\x83\x00\x00\xf9\xff\x00\x00\x80\xe9\x00\x00\x75\
-\x30\x00\x00\xea\x60\x00\x00\x3a\x98\x00\x00\x17\x6f\x92\x5f\xc5\
-\x46\x00\x00\x21\x55\x49\x44\x41\x54\x78\xda\xec\x9d\x79\x7c\x14\
-\x55\xba\xbf\xdf\x53\x4b\x77\xf6\xce\x4a\x42\x76\xb6\x80\x61\x0b\
-\xc4\x18\x30\x84\x80\x2c\xa2\x22\x83\xa8\x70\xd5\xeb\x75\x99\xf1\
-\x5e\xb7\xcb\xa8\x03\xe2\x2e\xb2\x29\x8c\x3a\x8a\x8e\x8e\xfa\x73\
-\xae\x8e\xa3\xfe\xc6\x6d\xbc\xe8\x20\x22\x4c\x64\x10\x30\x84\x48\
-\x88\x2c\x21\x84\x40\x82\x64\x25\x24\xe9\xec\xdd\x55\x75\xee\x1f\
-\x71\x43\x48\xe8\x24\x5d\x9d\xee\xaa\xef\xf3\xd7\x7c\x46\x0d\xe4\
-\x9c\xf3\x3e\xe7\x7d\xdf\x3a\x75\x8a\x71\xce\x09\x00\x60\x4e\x04\
-\x0c\x01\x00\x10\x00\x00\xc0\x84\x48\x18\x02\x83\xe1\x68\xce\xe1\
-\x9a\x53\x22\xd5\x69\xe5\x6d\x35\xd1\xa4\x74\xf8\x11\x63\x7d\xfb\
-\x59\x9c\x13\x0b\x8c\xa9\x22\xd9\xbf\x83\x04\x4b\x27\xb3\xda\x72\
-\x31\xc0\x10\x00\x18\x38\xd2\x78\xf3\x89\x64\xee\x68\x0e\xa6\x8e\
-\xc6\x30\xde\xd1\x10\xca\x5b\xab\xe2\xb5\x53\xfb\xc7\x51\x67\x93\
-\x8d\x3b\xec\x36\x72\xb4\x06\x71\x47\x73\x30\x39\xec\xc4\x3b\xed\
-\x44\x5c\xed\xdf\x9f\x28\x07\x10\xb3\x04\x13\x59\x6c\x0e\x66\x09\
-\x6c\x26\x39\xa8\x99\x59\x43\x1b\x99\xd5\xd6\xc4\xa2\xc6\xed\x65\
-\x81\x83\x6a\x98\x5f\x58\x03\xb3\x84\xd8\x59\x50\x5c\x05\xc9\x01\
-\x3b\x30\x4d\xbe\x03\x43\x13\xd0\x3b\xe1\x8e\xe6\x1c\xea\x38\x1d\
-\xa1\xd5\x1f\x4a\xe5\xf6\xf2\x64\x6e\xff\x2e\x41\x6b\x2a\x1b\xce\
-\x1b\x4a\x86\x92\xb3\x8d\xb8\xd2\x41\xa4\x76\x7a\x41\x11\x29\x11\
-\x89\x56\x62\xa2\x95\x58\x60\x4c\x2b\x0b\x1b\x51\xcc\x6c\xc9\xc7\
-\x58\xd0\xe0\x4a\x21\x72\x6c\x11\x0b\x8c\xa9\x62\xfe\xe1\xf5\x24\
-\xc8\x79\x98\x55\x08\x00\x74\x17\xf0\xed\x75\x73\x78\x63\xd9\x30\
-\xad\xbe\xf8\x02\xad\x6a\xf7\x24\xde\x74\x6c\x38\x6f\x39\x69\xe3\
-\xed\xf5\xbe\xfb\x4b\x89\x16\x62\x81\x31\xc4\x82\x13\x2a\x84\xa8\
-\x71\x85\x42\xf4\x84\x02\x16\x3a\xfc\x88\x10\x3e\xa2\x84\x88\x15\
-\x60\xd6\x21\x00\x13\x07\xfc\xa9\xd9\xdc\x5e\x3e\x44\x3b\xf1\xaf\
-\x1c\xad\xf1\x68\x8a\x56\x57\x34\x81\x37\x7f\x27\x90\xea\x30\xf2\
-\x72\x23\xb2\x04\x91\x10\x99\x5a\x25\x84\xa5\x14\x0b\x83\x2f\xda\
-\x25\x44\x8d\xdf\xcb\x82\x62\x4f\x92\xe4\xb7\x0b\xab\x02\x02\x30\
-\x70\xc4\xab\x19\xbc\xe9\xf8\x10\xad\x7a\x4f\x86\x7a\x72\x67\xb6\
-\x56\x5b\x98\xce\x5b\x2a\x25\x52\xda\xcd\xbd\x00\x03\xa2\x88\x85\
-\x24\xd5\x89\x09\x39\x5b\xd8\xa0\x09\xdf\x08\x91\xa9\xfb\x59\xc0\
-\xa0\x4d\x58\x30\x10\x80\x11\x48\xd3\x4e\x1f\x1e\xad\x95\x6f\x99\
-\xa5\x55\x17\x64\x6a\x55\x5f\x8f\xe2\x9d\x76\x8c\x4a\x4f\x2d\x85\
-\xf0\x14\x87\x10\x93\xb1\x4b\x48\x9a\xb9\x49\x18\x94\x56\xc8\x02\
-\xa2\x20\x03\x08\xc0\xd7\x76\xfa\xf2\x24\xf5\xbb\x6d\x97\x68\xdf\
-\xed\xc8\xd1\xaa\xf3\x53\x7d\xba\x8e\x1f\xc8\xfe\x41\x50\x9c\x26\
-\x26\x5d\xb2\x59\x48\xbc\x64\xab\x30\x68\x7c\x01\xb3\x86\xe2\x31\
-\x24\x04\xe0\xa5\x71\xdf\x56\x37\x47\xab\xda\x7d\x91\x7a\xe4\xa3\
-\x45\x5a\xf5\x1e\x04\xbd\xbb\x33\x83\x88\xd4\x56\x21\x79\xf6\x67\
-\xe2\x90\xd9\x1b\x85\xa8\xb1\x45\x68\x22\x42\x00\x03\x8f\xe6\xcc\
-\xd4\x4e\x97\x8c\x52\xcb\x36\xce\xd5\x8e\x7d\x36\x4f\x6b\x28\xb5\
-\x10\xd7\x30\x2e\x7a\x22\x07\x91\x98\x38\xad\x48\x4c\x9c\xb6\x45\
-\x48\x98\xb6\x95\x05\xc6\x6c\xc4\xa0\x40\x00\x9e\xc5\xd1\x9c\xa3\
-\x56\xfc\x73\xa6\x5a\xfc\xde\xf5\x5a\x6d\xe1\x50\xde\xd9\x84\x31\
-\x19\x88\xc5\x1b\x3a\x4c\x11\x87\x5c\xba\x51\x1c\x31\xff\x03\x21\
-\x22\xf5\x5b\x22\x2a\xc4\xa8\x40\x00\xfa\xa5\xf9\xed\x75\x73\xd4\
-\x63\x9f\x5f\xa6\x1e\xfe\xe0\x3a\xad\x7a\x4f\x14\x46\xc4\x4b\x16\
-\xb1\x35\x94\x84\xa1\x97\x6d\x97\x86\xcf\xfb\x58\x18\x9c\xb9\x83\
-\x44\x0b\x0e\x1d\x41\x00\x6e\x23\x8d\x37\x94\x5c\xa0\x96\x6d\xbc\
-\x52\x39\xfc\xe1\x22\xde\x74\x0c\x2f\x50\x79\x2b\x96\x60\x12\xe3\
-\x2e\x3e\x28\xa6\x5c\xf3\xae\x98\x38\x2d\x97\x24\x7f\x1c\x4b\x86\
-\x00\xfa\x11\xf8\xf6\xf2\xa1\xca\xa1\x77\x6f\x54\x4b\x3f\x99\xcf\
-\xed\xe5\x18\x11\xdf\x59\xd6\x24\xc4\x67\x1f\x97\xc6\xdc\xf4\x9a\
-\x98\x38\x2d\x97\x44\x2b\x0e\x19\x41\x00\xbd\x48\xf5\xed\x15\xf3\
-\xd5\xd2\x0d\x0b\x94\x83\x6f\xdf\xc8\x9b\x4f\x60\x40\x7c\x15\x41\
-\x26\x31\x71\x5a\xb1\x98\xfa\xef\x6f\x8a\x09\x53\x73\xf1\x3e\x02\
-\x04\xd0\x73\xe0\x77\xda\x73\xd4\x23\x1f\x2d\x52\xf6\xbf\xf9\x6b\
-\xde\x70\xc4\x82\x11\x31\x08\x92\x1f\x89\x09\x39\x07\xa5\xf1\xff\
-\xf9\x92\x30\x38\x73\x07\xa1\x59\x08\x01\x9c\x81\xea\xc8\x54\x8f\
-\x7f\x7e\xb9\x52\xf4\xfa\x1d\x68\xee\x19\x18\x39\x90\xa4\x91\xd7\
-\x6e\x95\xc6\xdf\xf6\x12\x0b\x49\x2a\x83\x08\x20\x80\x34\xad\x76\
-\x5f\xba\xf2\xcd\x0b\xf7\xa9\xe5\x5b\x52\x49\x53\x10\x24\x66\x58\
-\xf4\x41\xb1\x24\x8d\xfb\xcd\xeb\x62\xca\x55\x1f\x30\x7f\x73\x1f\
-\x35\x36\xad\x00\x78\xcb\xc9\x79\x4a\xd1\x9f\x6f\x53\x0f\xbd\x33\
-\x97\x3b\x9a\x11\x15\x66\x6c\x11\x44\xa7\xd7\x49\x13\xef\x7e\x56\
-\x4c\x9e\xb5\xc9\xac\xd9\x80\xf9\x04\xc0\xd5\x0c\xb5\x6c\xe3\x5c\
-\x65\xcf\x73\xf7\x6b\xa7\x0f\xfb\x21\x0c\xcc\x6e\x01\x99\xa4\x51\
-\x8b\xb6\x89\x63\x6f\x79\x4d\x08\x1f\x79\xc0\x6c\x22\x30\x95\x00\
-\xb8\xbd\x7c\x81\x73\xcf\x73\x4b\xd4\x92\x0f\x27\xe3\xc8\x2e\x38\
-\x23\x10\x6c\xc9\x24\xa7\xdf\xb3\x4e\x1c\x76\xc5\x06\x33\x9d\x1f\
-\x30\x89\x00\x78\xba\x5a\xfc\xfe\xbf\x39\xbf\x79\xe1\x3e\x1c\xe4\
-\x01\x3d\x21\x0e\x9f\x57\x28\x67\xdc\xf7\x24\x0b\x1d\x5e\x62\x86\
-\x6c\xc0\xf0\x02\xe0\xf6\xf2\x05\xce\xfc\x67\xef\x57\x8f\xfc\x3d\
-\x13\xbb\x3e\x70\x29\x28\x82\x06\x93\x9c\xf1\xbb\x67\xc5\x51\x8b\
-\xde\x31\xfa\x5b\x87\xc6\x15\x00\xd7\xd2\xd5\x8a\xdc\x59\x4a\xde\
-\x53\x8f\x68\xf5\x87\x02\xb1\xac\x41\xef\x22\x43\x24\x71\xe4\xb5\
-\x3b\xe4\x0b\x7f\xfb\x34\x0b\x4e\xf8\x18\x02\xf0\xa5\xd8\x77\x34\
-\xe7\x28\x05\xcf\x2f\x51\xf6\xbf\x31\x97\x94\x0e\x2c\x66\xd0\x67\
-\x84\xc8\x31\xcd\x52\xe6\xb2\x55\x62\xe2\xf4\xcd\x46\x2c\x09\x8c\
-\x26\x80\x34\xad\xa6\x20\xd3\xb9\x6b\xcd\xe3\x5a\x55\xde\x60\x2c\
-\x5f\xe0\x16\xe4\x40\x92\x27\xdc\xf1\xae\x94\x76\xe7\xf3\x46\x7b\
-\xd3\xd0\x48\x02\x48\x53\x8f\x6d\x9a\xeb\xdc\xb9\x72\x25\x5e\xdc\
-\x01\x7a\x20\xa6\x5c\x9d\x27\x4f\x7e\x78\xb9\x91\x2e\x2d\x35\x84\
-\x00\x78\x67\xd3\x74\x75\xff\x1b\xbf\x76\xee\x7d\xf9\x06\x72\xb6\
-\x60\xa5\x02\xfd\x4a\x82\xa8\xb1\x4d\xf2\xc5\xcb\x1f\x16\x62\x8d\
-\xf1\x4e\x81\xcf\x0b\x80\xb7\x56\x5f\xee\xdc\xb9\x72\x85\x5a\xfa\
-\xbf\xe9\x58\x9e\xc0\x23\x41\x13\x34\x98\xe4\x49\x0f\xaf\x11\x47\
-\xcc\x7f\xdf\xd7\x25\xe0\xcb\x02\x48\xd3\xea\x0f\x8d\x75\x6e\x7f\
-\x64\x2d\xea\x7d\xe0\x71\x24\x3f\x92\xd3\xef\x79\x4b\x4a\xbb\xfd\
-\x05\x12\xa4\x7c\x08\xc0\xd3\xc1\x5f\xb9\x6b\xaa\x23\x77\xc9\xf3\
-\xa8\xf7\xc1\x80\x7a\x20\xf5\xfa\xed\x52\xe6\x03\x4f\x30\xbf\xf0\
-\xad\x10\x80\x67\x92\xfe\x74\xf5\xf0\x07\x0b\x9d\x3b\x57\xde\xcf\
-\x3b\x4e\x63\x05\x82\x01\x47\x1c\x7a\xf9\x7e\x39\x6b\xf9\x83\x2c\
-\x28\xf6\x53\x08\x40\xd7\xd8\xd7\xd2\x95\x7d\xaf\xdc\xe5\xdc\xf3\
-\x87\x5b\xc8\xd9\x86\x95\x07\xbc\x06\x21\x3a\xbd\x4e\xce\x59\x7b\
-\xaf\x10\x31\xea\x6d\x08\x40\x0f\x34\x25\xc3\x59\xf0\xfc\x12\xa5\
-\x60\xfd\xc2\x7e\x7f\xf3\x1e\x00\x3d\x82\x29\x74\xb8\x62\x99\xf5\
-\xe2\x6f\x84\xc8\x31\xfb\xc8\x47\x9a\x83\xbe\x21\x00\x4d\xc9\x70\
-\xe6\x3d\xf5\x98\xb2\xef\xd5\xb9\x38\xcf\x0f\xbc\x3a\xa0\x42\x92\
-\xc8\x32\x73\xfd\xed\x42\x74\x7a\x9e\x2f\x48\xc0\xfb\x05\xa0\x76\
-\x4e\x76\x7e\xbd\xe6\x31\xa5\xe8\xf5\x39\x58\x5e\xc0\x27\x24\x10\
-\x14\x4b\x96\x99\x2f\xde\x29\x0c\xbe\x68\x97\xb7\x4b\xc0\xbb\x05\
-\xa0\x76\x4e\x76\xee\x78\x62\xb5\x72\xe0\x2f\xd3\xb1\xac\x80\x4f\
-\x49\xc0\x3f\x92\x2c\x33\x5f\xbc\x57\x88\x9f\xf2\xa5\x37\x4b\xc0\
-\x7b\x05\x80\xe0\x07\x3e\x2f\x81\x08\xb2\xcc\x7e\xe5\x6e\x21\x76\
-\x92\xd7\x9e\x1a\xf4\xce\xcb\x31\x34\x67\xa6\xf3\xeb\x35\x8f\x21\
-\xf8\x81\x2f\xc3\xdb\xeb\xc9\xb1\xe5\xee\x17\xb5\xea\xfc\xc9\x44\
-\x94\x06\x01\xb8\x14\xfc\x4a\x86\x33\x6f\xed\x23\xa8\xf9\xf5\x45\
-\x1c\x79\xed\x2e\x31\x65\x41\x3e\x46\x42\x67\x09\xb4\x56\x93\xe3\
-\x8b\x3b\x5f\xd2\x6a\x0b\xd3\x21\x00\x57\x82\xbf\xe0\xf9\x25\x4a\
-\xe1\x9f\xe6\x62\xe9\xe8\x18\xfc\xc3\xe7\x15\xca\x53\x56\x3c\x68\
-\xc9\x5e\xbd\x54\x1c\x7a\xf9\x7e\x8c\x88\xce\x12\x68\xa9\x22\xc7\
-\xd6\xc5\xaf\x6a\xf5\x07\x6f\x84\x00\xba\x1f\xa6\x74\xa5\xe8\xb5\
-\x3b\x94\x82\xf5\x0b\xb1\x64\x74\x0c\xfe\x11\xf3\x0b\xe4\xec\xd5\
-\x4b\x98\x25\x78\x1b\x59\x82\xb7\xc9\xd3\xd6\x2d\x16\x87\x5d\x51\
-\x84\x91\xd1\x79\x75\x37\x96\x09\xce\xad\x8b\x5f\xe5\x8d\x47\x17\
-\x42\x00\x67\x93\xa6\x1e\xfe\x70\xa1\x73\xcf\x73\xb7\xe0\x90\x8f\
-\x9e\x3b\xff\xaf\x0a\xe4\x29\x2b\x97\x31\xbf\xb0\x1f\xcf\xad\x33\
-\x6b\x68\xae\x9c\xb3\xf6\x1e\x48\xc0\x03\x09\x6e\x7d\xb1\x9f\xe3\
-\xab\xc7\x9e\xe4\x6d\x75\x5e\x53\xde\x8a\xcb\x97\x2f\x1f\xf0\xe0\
-\xd7\x2a\x77\x4d\x75\x7e\xb9\x74\x15\x39\xec\x58\x25\xba\xa6\xfd\
-\x2b\x1f\x64\xfe\xe1\x5b\x7e\xf9\xcf\x98\xe4\x77\x5c\x88\x9b\x72\
-\x84\xdb\xcb\x27\xf2\x86\x23\x83\x30\x5a\x3a\x66\x02\xf6\xf2\x30\
-\xde\x56\x3b\x52\x88\x9d\x5c\xc6\x24\xff\x63\xa6\x17\x80\x76\xfa\
-\xf0\x0c\xc7\x17\x77\xbe\xc6\x5b\xab\xb1\x3a\xf4\xdc\xf9\xb3\x57\
-\xdf\x7f\xae\xe0\xff\x49\x02\xfe\xc7\x84\x84\xa9\xc5\xdc\x5e\x31\
-\x81\x37\x94\x44\x63\xd4\x74\x94\xc0\xe9\xe2\x38\x52\xda\xe3\xc4\
-\xa4\x4b\x8a\x88\xa8\xda\xb4\x02\xe0\xad\xd5\x97\x3b\xff\x79\xef\
-\x4b\xbc\xfe\x50\x10\x96\x85\x8e\x3b\x7f\xf6\xaa\xfb\x5d\x79\x5d\
-\x95\x49\x7e\xc7\x85\xf8\x29\x87\x79\xd3\xf1\x74\x64\x02\x3a\x6f\
-\x7c\xb5\x85\x43\x99\x35\x44\x14\xa2\x27\x9e\x18\x48\x09\x0c\x58\
-\x0f\x80\x77\x36\x4d\x77\xee\x5c\xb1\x5a\xab\xce\xc7\x6e\xa3\x57\
-\xf0\xff\xd0\xf0\xeb\xc5\xbb\xea\xcc\x1a\x9a\x2b\x4f\xfb\xfd\x62\
-\x71\xd8\x95\x85\x18\x41\x7d\x71\xe6\x3f\x73\x9b\x5a\xbe\x65\x0e\
-\x0d\xe0\x19\x81\x81\x12\x40\x9a\xba\xff\x8d\x5f\xab\xa5\x1b\xd2\
-\xb0\x0c\x74\xad\xf9\xcf\x68\xf8\xb9\x2e\x01\x5b\xae\x9c\xf3\xe4\
-\x7d\x68\x0c\xea\x8c\xa3\x99\x9c\x5f\x3d\xf6\xa4\x56\x5f\x3c\xda\
-\x4c\x02\xe8\xba\xbd\x77\xef\x1f\x6f\xc0\x0a\xd0\xb1\xe6\xef\x63\
-\xf0\x9f\x91\x09\xe4\xac\xbd\x07\xe7\x04\x74\xce\x84\xed\x15\xe4\
-\xdc\xb5\x72\x05\x39\x9a\x73\x4c\xd1\x03\xd0\x6a\xbe\xb9\xd2\xb9\
-\x6d\xd9\x1f\xa8\xfd\x14\x66\x5f\xb7\x9a\xbf\xe7\x86\x9f\xcb\x12\
-\x90\xfc\x8e\x0b\x09\xd9\x68\x0c\xea\x2e\x81\xf2\x30\x52\x3b\x63\
-\xc4\xb8\x8b\x4b\x49\x10\x4f\x1a\x57\x00\x8e\xe6\x1c\x07\x9a\x7e\
-\x3a\xa7\xfd\x2b\x96\x31\xff\x88\x2d\xee\xfa\x99\x68\x0c\x7a\x68\
-\x63\xac\xfb\x76\x38\x0b\x18\xd4\x26\x0c\x1a\x5f\x4d\x1e\x6c\x0a\
-\x7a\xae\x04\xe0\x5a\xba\x73\xcf\x73\x4b\xd0\xf4\xd3\x29\xf8\x47\
-\xcc\x2f\x90\xa7\xae\xb9\x8f\xf9\x47\x6e\x76\xf7\xcf\xfe\xa9\x31\
-\x88\x9e\x80\x7e\x06\x70\x92\x92\xff\xec\x62\xad\xae\x68\x82\x21\
-\x7b\x00\xea\x89\x2f\x67\x28\x07\xde\xc4\x19\x7f\x3d\x6b\x7e\x6b\
-\x68\xae\x5e\x7f\x06\xb3\xda\x72\xe5\xa9\x4f\xa1\x31\xa8\xe7\x1e\
-\xd9\x5e\x47\xce\xaf\xd7\x2c\x27\x67\x6b\xb6\xa1\x4a\x00\xde\x58\
-\x76\x8d\xf3\xcb\x25\x2f\xf2\xd6\x1a\x11\xd3\xac\xc3\xce\x9f\xbd\
-\xaa\x5f\x0d\x3f\xd7\xcb\x01\xff\x63\x42\xfc\x54\x94\x03\xba\xf6\
-\x03\x2a\x6c\x4c\xf2\xf3\x13\x06\x5f\x74\x9c\x18\xab\xf2\xfd\x0c\
-\x40\x73\x66\x3a\x77\xaf\x7d\x54\x3b\x5d\x62\xc1\xf4\xea\x12\xfc\
-\x4b\x3d\x11\xfc\x67\x64\x02\x78\x77\x40\x57\x9c\x7b\xff\x74\x9d\
-\xfa\xdd\x76\x8f\xdc\x85\xa1\xb7\x00\xd2\xd4\x92\xbf\x5f\xa3\x1e\
-\xdd\x38\x0e\xd3\xea\xee\xb4\xff\xfb\x86\x9f\x8e\x69\x7f\xb7\x12\
-\xf0\x0b\xdb\x8a\x72\x40\x4f\x03\xb4\x90\xb2\x6b\xd5\x72\xde\xae\
-\xff\x4b\x43\xba\x0a\x80\xdb\xcb\x87\x3a\xf7\xfc\x61\x09\x11\xc7\
-\xa4\xba\xbb\xe6\xef\xe5\x09\x3f\x5d\x24\x90\xf3\xfb\xc5\xe2\xb0\
-\xb9\x90\x80\x1e\x89\x73\xfd\xa1\x40\xa5\xf0\xd5\x3b\x48\xe7\x53\
-\x82\x7a\x0a\x20\xcd\xb9\xe7\x0f\xf7\xf3\xe6\x13\x98\x4d\x77\xef\
-\xfc\xd9\x2b\x97\x79\x32\xed\xef\xbe\x1c\x08\xd9\x26\x4f\xc5\x89\
-\x41\xbd\x50\xf6\xbf\x31\x4f\x3b\xb9\x73\xaa\x4f\x0a\x40\x2d\xdd\
-\x70\xb5\x7a\xe4\xe3\x4c\x4c\xa3\xdb\x6b\xfe\x25\xde\xf4\x1d\xba\
-\xae\x4c\x60\x1d\x7a\x02\xba\x18\xa0\x9d\x9c\xf9\x4f\x3f\x44\xce\
-\x96\x6c\x9f\x12\x00\x6f\xa9\x9a\xeb\xcc\x7f\xe6\x01\xd2\x14\x4c\
-\xa2\x5b\x77\xfe\x55\x4b\xbd\xf1\x23\x94\x78\x44\xa8\x63\x29\x50\
-\xb5\x3b\x5a\x29\xfa\xf3\x7f\x11\xf1\x74\xdf\x10\x80\xa6\x64\x28\
-\x45\xaf\xde\xc1\x1b\x8f\x4a\x98\x3e\x37\xd6\xfc\x3a\x3f\xe7\x77\
-\x4f\x26\xb0\xf6\x1e\xf4\x04\x74\x48\x04\x8a\x5e\xbb\x41\xab\xdb\
-\x3f\xce\x27\x04\xa0\x55\xe7\x4f\x56\x0e\xfd\xff\xcb\x31\x6d\x6e\
-\x0c\xfe\xec\x55\xcb\x98\x7f\xc4\x66\x6f\xff\xbb\x76\xbd\x40\xb4\
-\x0e\x8d\x41\x77\x67\xd4\x1d\x0d\xa4\xec\x7b\xe5\x2e\x3d\xb2\x00\
-\xf7\x0a\x40\x53\x32\x94\xa2\xff\xf7\x5f\xe4\x68\xc6\xac\xb9\x2d\
-\xed\xf7\x8e\x86\x9f\xeb\x12\x40\x63\x50\x0f\xd4\xa3\xff\x48\x57\
-\x8f\x6f\x99\xe5\xd5\x02\x50\x8f\x7d\x36\x57\x3d\xbe\x25\x15\xd3\
-\xe5\x86\xe0\xf7\xc2\x86\x5f\xef\xca\x81\x75\x28\x07\xdc\xba\xb9\
-\x3a\x49\xf9\x66\xfd\x12\xde\x69\xcf\xf1\x4a\x01\xf0\x4e\x7b\x8e\
-\xb2\xf7\xe5\xdf\xe2\x56\x5f\x37\xed\xfc\x53\x56\x2c\xf3\xc5\xe0\
-\xff\x29\x13\xb0\xe5\xca\x53\x9f\xbc\x0f\xf7\x09\xb8\xd1\x01\x35\
-\x85\x11\xea\xe1\xf7\xaf\xf3\x46\x01\xa4\xa9\x07\xfe\xf2\x6b\xad\
-\xae\xc8\x86\x69\x32\xef\xce\x7f\xee\x4c\x00\xc7\x86\xdd\xd8\x0d\
-\x20\x65\xff\x1b\xb7\xf1\xe6\x13\xf3\xbd\x4a\x00\xdc\x5e\x91\xac\
-\x1c\x7a\xf7\x46\x4c\x90\x5b\x82\x7f\xa9\x11\x82\xff\xec\x72\x00\
-\x12\x70\x4b\xac\x35\x1d\x13\xd4\x92\x0f\x17\x92\x9b\x4e\x08\xba\
-\x41\x00\x3c\x5d\x2d\xdd\xb0\x80\xdb\xcb\x31\x3b\xee\x48\xfb\xbd\
-\xf8\x51\x5f\xff\xca\x81\xa7\x50\x0e\xb8\x09\xa5\xf8\xbd\xeb\x78\
-\x4b\x65\xbc\x57\x08\x80\x37\x95\x27\x29\x07\xde\xc2\xee\xdf\xef\
-\x9d\x7f\xf5\x12\x23\xed\xfc\xe7\xcc\x04\xa6\xad\xc3\x6d\xc3\xee\
-\xc9\xb8\x49\x39\xf8\xce\x4d\xee\xc8\x02\xfa\x2b\x80\x34\xe5\xd0\
-\x3b\x37\xf1\x96\x93\x98\x95\x7e\xed\xfc\xbe\xf5\xa8\xaf\xef\x99\
-\x40\x28\x6e\x1b\x76\x13\xea\xa1\x77\xae\xe1\xf6\x8a\xe4\x01\x15\
-\x00\x6f\x28\xb9\x40\x3d\xfa\xe9\x3c\x4c\x47\xbf\x6a\xfe\x25\x66\
-\x08\xfe\x33\x25\x80\xc6\x60\xbf\xb3\x80\xb6\x5a\x52\x0e\xf5\x3f\
-\x0b\xe8\xbb\x00\xb8\x96\xae\x94\x7e\x32\x9f\xdb\x2b\x30\x1b\x7d\
-\xdd\xf9\x0d\xd6\xf0\x83\x04\x3c\x9c\x05\x94\x7c\x34\x9f\x37\x96\
-\x0d\x1f\x10\x01\xf0\xce\xc6\x50\xb5\xe4\x23\x7c\xca\xbb\xcf\x69\
-\xbf\x31\x1b\x7e\x90\x80\x07\xb3\x80\x96\x4a\x52\xcb\xfe\x31\x6f\
-\x40\x04\xa0\x1e\xfd\xf4\x2a\xec\xfe\x7d\x4c\xfb\x75\xba\xbd\xd7\
-\x37\x25\x80\x13\x83\xfd\x41\x29\xf9\x68\x11\x6f\x3f\x35\xdb\xb3\
-\x02\x70\x34\xe7\xa8\xc5\x7f\xbb\x1e\x37\xfd\xf4\x76\xe7\xff\x55\
-\x81\xd9\x77\xfe\xb3\x25\x80\x13\x83\xfd\xca\x02\x1a\x4a\x2d\xea\
-\xd1\x4f\xe7\x7b\x54\x00\x6a\xf9\xd6\xd9\x5a\xed\xbe\x30\x0c\x7f\
-\x2f\x77\xfe\xec\x55\xcb\xcc\x58\xf3\x9f\x57\x02\x7e\x61\x5b\xbb\
-\xbe\x3b\x80\x4c\xa0\x0f\x0a\x20\xf5\xc8\xc7\xd7\x90\xd2\x9e\xe5\
-\x19\x01\x68\xce\x4c\xa5\xf8\x6f\xd7\x63\xe0\x7b\x59\xf3\x7b\xf8\
-\xf6\x5e\x64\x02\xe6\x41\xab\xde\x13\xa5\x9e\xf8\x57\x8e\x47\x04\
-\xa0\x9d\x3e\x3c\x8a\xd7\xed\x4b\xc6\xb0\xf7\x26\xed\x5f\x89\xb4\
-\xdf\xd5\x4c\x00\x8d\xc1\x3e\xa1\x1e\xf9\xfb\x22\xe2\x6a\x86\xee\
-\x02\x50\x8f\xfe\x63\x1e\xef\xb4\x63\xc4\x5d\xdd\xf9\xa7\xae\x59\
-\xea\x0b\x97\x79\x78\x97\x04\xf0\xee\x40\xaf\x37\xe6\xaa\xbc\x71\
-\xbc\xf9\x64\x9c\xae\x02\xe0\xed\x75\x73\xd4\xb2\xcf\x70\xf0\xc7\
-\xd5\xe0\x9f\xb2\x72\x19\xb3\xda\xb0\xf3\xf7\xa9\x1c\x78\xea\x3e\
-\xf4\x04\x7a\x11\x9b\x6d\x75\xa4\x1e\xdb\x34\x57\x57\x01\x68\x95\
-\x5f\x4f\xe6\x8d\xa5\xb8\xeb\xef\x7c\xc1\xff\xc3\xd9\x7e\xec\xfc\
-\xfd\xcd\x04\xd0\x18\xec\x7d\x76\x9e\xa3\x8f\x00\xb8\x96\x8e\x83\
-\x3f\x2e\x04\xff\xb0\x2b\x4d\x73\xb6\x5f\xff\x4c\xe0\xfb\xeb\xc5\
-\xd0\x18\x74\x6d\x83\xae\x2d\x8c\xe2\xa7\xbe\x9d\xa0\x8b\x00\x78\
-\xd3\xf1\x21\x5a\x75\xc1\x28\x0c\xf3\x79\x76\xfe\xa9\xab\x97\x20\
-\xf8\xdd\x9d\x09\x3c\x85\x9e\x80\x4b\x41\xaa\x92\x7a\xe4\xe3\x05\
-\xba\x08\x40\xfd\x6e\xdb\x25\xbc\xe3\x34\x06\xb9\xdb\x9a\xff\xfb\
-\x6e\x3f\x9e\xf3\xeb\x20\x81\x70\x34\x06\x5d\x8d\xd3\xaa\xbc\x2c\
-\xde\xd1\x30\xc3\xbd\x02\xd0\x94\x0c\xad\x62\xdb\x0c\x0c\x6f\x0f\
-\x69\x7f\x36\xd2\x7e\x7d\xcb\x01\x5c\x2a\xe2\x52\x12\xd0\x78\x4c\
-\xd0\x4e\xee\xcc\x72\xab\x00\xb4\x86\xd2\x14\xad\x7a\x77\x0a\x86\
-\xb7\x9b\x9d\x7f\xea\x9a\x25\xd8\xf9\x3d\x54\x0e\x4c\x43\x63\xf0\
-\x3c\x0a\x20\xed\xe4\x57\xd3\x5c\xfd\x86\x80\x6b\x02\x28\xdf\x72\
-\x29\x9e\xfd\x77\x97\xf6\xaf\x78\x08\x3b\xbf\x27\x33\x81\xd0\x5c\
-\x39\xe7\xa9\x7b\x90\x09\xf4\x50\x06\x9c\xd8\x36\x9d\xb7\x9d\x8a\
-\x72\x8f\x00\xd4\xce\xc9\x5a\x55\xde\x64\x0c\xeb\x2f\x82\x7f\xc4\
-\xfc\x02\x39\x7b\xe5\x32\x3c\xea\x1b\x20\x09\x4c\x5b\xb7\x18\x3d\
-\x81\x6e\x72\x80\x96\x4a\xd2\x6a\x0b\xd3\xdc\x22\x00\xed\xf4\xe1\
-\x51\x6a\x55\xde\x70\x0c\xeb\xcf\x77\x7e\xf3\x5e\xe6\xe1\x55\x12\
-\xc0\x07\x49\xbb\x09\x5a\x85\xb4\xf2\x2d\x73\xdc\x22\x00\x5e\x7f\
-\x28\x95\x9c\x6d\x18\xd4\x33\xd2\x7e\x9c\xed\xf7\x9a\x9e\x00\x3e\
-\x48\x7a\x6e\x07\xd4\x15\xa5\xb9\x72\x28\xa8\x67\x01\x70\x35\x43\
-\x3d\xb1\x6d\x26\x86\xf3\x67\xc1\xef\x23\x1f\xea\x34\x5d\x4f\x00\
-\x99\xc0\x99\x02\x38\x75\xd0\xc6\x4f\xed\x1f\xdf\x2f\x01\xf0\x8e\
-\x86\x30\x57\x6b\x09\x73\x04\x3f\x1e\xf5\x79\x77\x39\x80\x4c\xe0\
-\x67\x9b\x37\x69\x75\xfb\xd2\xfa\x27\x80\xa6\xe3\x43\x78\x5b\x2d\
-\x82\xff\x87\x86\x1f\x6a\x7e\x1f\x28\x07\x90\x09\xfc\x80\xfa\xdd\
-\x57\x39\xa4\x39\x33\xfb\x2c\x00\xf5\xc4\xbf\x2e\x21\xa5\xc3\xdc\
-\xc1\xff\xe3\xd9\x7e\x04\xbf\xf7\x67\x02\x38\x2c\x74\xc6\x06\x5e\
-\x7f\x68\x28\x6f\xad\x89\xee\xab\x00\xd2\x78\xc3\x61\x53\x9f\xfd\
-\xff\xe9\x1a\x2f\xa4\xfd\x3e\x95\x09\x4c\x5b\xb7\x18\x12\x20\xe2\
-\xed\xf5\xc4\x9b\x7a\xbe\x36\x5c\xe8\xfe\x3f\xae\x8b\xd1\xea\xbe\
-\x1d\x67\xea\x9d\x3f\x7b\x15\x2e\xf3\xf0\xd5\x9e\x00\x24\xd0\xf5\
-\x72\x50\xe5\xee\xc9\x7d\x13\x40\x63\xd9\x30\xde\x52\x69\xce\xe0\
-\x1f\xfe\xab\xae\xb7\xfa\xf0\xa8\xcf\xf7\x25\x60\xf2\x6f\x11\x7e\
-\x9f\x01\xa4\xf5\x5a\x00\xda\xa9\x03\x63\x49\x53\x4c\x9c\xf6\xa3\
-\xe6\x37\x84\x04\x4c\xde\x18\xd4\x6a\x0b\xd3\x78\x6b\x4d\x6c\xef\
-\x05\x50\xb5\xdb\x74\xc7\x7f\xcd\xf4\xa1\x4e\xf3\x48\x20\x64\x5b\
-\x57\x63\xf0\x32\x53\x96\x03\xbc\xa5\x92\xb8\xbd\x3c\xa9\x57\x02\
-\xe0\x8e\xe6\x1c\xde\x74\x7c\x88\xe9\x76\x7e\x04\xbf\x31\x25\xf0\
-\xe3\x45\xa3\x26\x3c\x27\xa0\x29\xa4\x35\x94\xa6\xf4\x2e\x03\x68\
-\xaf\x8f\xe0\xcd\x27\x82\x4d\xb5\xf3\xa3\xe1\x67\x02\x09\xac\x35\
-\xe5\x5b\x84\xbc\xae\x30\xbd\x57\x02\xd0\xea\x0f\xa5\xf2\xce\x26\
-\x93\x04\x3f\xce\xf6\x9b\xa7\x1c\xb0\x99\xb2\x27\xa0\x35\x1e\x1d\
-\xde\xbb\x12\xa0\xe9\x98\x29\xde\xfe\xfb\xb1\xe1\x87\x9d\x1f\xe5\
-\x80\x91\x33\x80\xd6\xda\xe8\xee\x3e\x20\x7a\x6e\x01\xb4\x9c\x8c\
-\x37\x45\xda\x3f\x65\x05\x6a\x7e\xd3\x66\x02\xe6\xb9\x54\x84\xb7\
-\x56\x09\xbc\xf9\x64\x82\x6b\x02\xd0\x94\x0c\xad\xf1\xe8\x08\xc3\
-\xef\xfc\x38\xde\x6b\x72\x09\xfc\xf0\x88\xd0\x04\x99\x80\xd2\x41\
-\xda\xa9\xfd\x63\x5c\x12\x00\x6f\xad\x8a\xe3\x0d\x47\x12\x0d\x5d\
-\xf3\xa3\xe1\x07\xe8\x67\x57\x8e\x9b\x20\x13\xe0\x2d\x55\xf1\xae\
-\x09\xa0\xd3\x6e\x33\xea\x05\x20\x3f\xde\xe1\x87\x86\x1f\x38\x2b\
-\x13\x30\x76\x63\x90\xb7\x9d\xfb\xa5\xa0\xb3\x4b\x80\x8e\xfa\x08\
-\x6e\xc0\x37\x00\xbb\x3e\xd4\xb9\x1a\x3b\x3f\xe8\x26\x13\x30\xf8\
-\x77\x07\xda\x6a\x5d\x13\x00\xef\x6c\xb2\x91\xe6\x34\xe0\xce\x8f\
-\x47\x7d\xa0\xa7\x4c\xc0\x66\xe8\x9e\x00\x6f\xa9\x8a\x23\x67\x5b\
-\xd6\x79\x05\xa0\x9d\x3a\x30\xce\x70\xc1\x8f\xdb\x7b\x81\xcb\xe5\
-\xc0\x53\x86\x94\x00\x6f\xad\x0e\xe4\x2d\x27\x13\xcf\x9f\x01\xf4\
-\xe1\x1b\xe3\x5e\x9f\xf6\xa3\xdb\x0f\x7a\x2d\x01\x63\x95\x03\x5c\
-\x73\x12\x77\xb6\x05\x9c\xbf\x07\xd0\xd9\x14\x86\xb4\x1f\x40\x02\
-\x06\x6b\x0c\x2a\xed\xc4\x3b\xea\x23\xce\x9f\x01\x38\x9a\x7d\xfe\
-\x1d\x00\x71\xd8\x95\x68\xf8\x01\x48\xe0\x8c\xda\x5e\x21\xea\xb4\
-\xdb\x7a\x14\x00\xef\xb4\xe7\x90\xb3\x25\xc8\xe7\xd3\xfe\xec\x55\
-\xd8\xf9\x81\x7b\x24\x60\xa4\xdb\x86\x95\x76\xbf\x9e\x33\x00\xcd\
-\x61\xe5\x8e\xe6\x40\x9f\x0d\xfe\x11\xf3\x0b\xe4\xec\xd5\x4b\xb0\
-\xf3\x03\xb7\x49\xc0\x40\xb7\x0d\xf3\xce\xc6\xb0\xf3\x08\x40\x95\
-\xc8\xe1\x9b\x1f\x01\xc5\x65\x1e\x40\xbf\x4c\xc0\x66\x88\xcf\x90\
-\x69\xd5\x05\x99\x3d\x97\x00\xad\xd5\x83\xb9\xa3\xc5\x47\x77\xfe\
-\x55\x4b\x10\xfc\x40\xdf\x4c\x60\xdd\x3d\xbe\x7c\xc7\x20\x3f\x47\
-\x79\x7f\x66\x06\xa0\x76\x5a\x88\x6b\x3e\x34\x2b\x02\x49\xa9\xd7\
-\x6f\xb7\xe4\xac\xbd\x17\x8f\xfa\x80\x27\x32\x01\xcb\xf4\x67\xee\
-\x96\x52\xaf\xdf\x4e\x4c\xf4\xbd\x5f\xa0\xd3\x6e\x23\x47\xf3\x19\
-\xdf\x0b\x94\xce\xfc\x0d\x99\xaf\x4d\x08\x11\x93\x14\x67\xde\x53\
-\x8f\x90\xa6\xca\xde\xad\x5f\x4d\x20\x41\x52\xa4\x89\xff\xfd\x2c\
-\x0b\x8c\xde\x88\x70\xfa\xd9\xd0\x34\x1d\xbb\x46\xf9\xf6\x7f\x6e\
-\x23\xd5\x61\x25\x26\x78\xf7\x0e\x24\x88\x4e\x62\x92\xc2\x2c\x81\
-\xc4\x3b\x7d\xab\x5c\xe6\x0e\xbb\x8d\x6b\x8a\xc4\xba\x15\x80\xaf\
-\x2d\x9c\x8e\x06\x52\x0e\xfc\x65\xba\x4f\x95\x2b\x43\x2e\xdd\x08\
-\x01\xfc\x72\x1e\x4f\x47\x28\xdf\xfe\x79\x36\x46\x42\x67\x54\x07\
-\x11\x57\xc5\xee\x4b\x00\xa0\x3f\x7e\x61\xf5\x18\x84\xb3\xb6\x55\
-\x8d\x04\x19\xc3\xa0\x37\x9a\x93\x88\x73\x01\x02\x18\xb8\xa2\x85\
-\x98\x5f\x04\x04\x00\x06\x48\x00\x2a\x11\x71\x82\x00\x06\x76\x16\
-\x30\xe6\x60\x60\x4a\x2d\xcd\xd9\xf5\xa8\x1f\x02\x00\xc0\xa4\x3d\
-\x80\x5f\x6c\x40\x10\x00\x00\xa6\x49\x01\x54\x22\x8e\x12\x00\x00\
-\x00\x01\x00\x60\x32\x44\x0b\xfd\xf2\x9c\x05\x04\x00\x80\x49\x60\
-\x82\x0c\x01\x00\x60\xde\x7c\x1f\x02\x00\xc0\xc4\x02\x90\x20\x00\
-\x00\x4c\x9d\x01\xd0\x99\xef\xfb\x40\x00\x00\x98\x05\xc9\xdf\x41\
-\x82\xe4\xec\x5e\x00\xbf\x78\x46\x08\x00\x30\x0e\xcc\x2f\xb4\x81\
-\x59\x6d\xb9\xdd\x0b\x40\xf2\xeb\xc0\x4b\x19\x00\x18\x54\x00\x72\
-\x60\xf3\x59\x55\xc1\x19\xff\x42\xe0\xe0\x2a\x66\xb5\x61\xa4\x00\
-\x30\x22\x56\x5b\x53\x8f\x02\x20\x41\x72\x92\x25\x58\xc3\x48\x01\
-\x60\x3c\x84\x41\x13\xf6\xf4\x9c\x01\xf8\x85\x6d\x65\x96\xe0\x66\
-\x0c\x15\x00\xc6\xec\x01\xf4\x9c\x01\x10\x11\xc9\x81\x2d\x18\x2a\
-\x00\x0c\x17\xfe\x44\x92\x7f\xfb\x79\x05\x70\x2e\x4b\x00\x00\x7c\
-\x1c\xc9\x4a\xcc\x2f\xbc\xde\x05\x01\x84\x41\x00\x00\x18\x6d\xff\
-\x17\x2d\x44\xd6\x10\xfb\xf9\x05\x10\x39\x76\x2f\x86\x0b\x00\x83\
-\x21\x07\xbb\x98\x01\x04\x46\xd7\x10\xc3\x01\x41\x00\x0c\x95\x01\
-\x84\x24\x54\xb1\xc0\x98\x4a\xd7\x4a\x00\xc9\x0f\x23\x06\x80\x91\
-\x04\xe0\x1f\x51\x47\x44\x85\xe7\x15\x00\x59\x6c\x8d\x4c\xb0\x60\
-\xc4\x00\x30\x92\x00\x02\x07\x57\x9e\xeb\xff\x3f\x47\x09\x10\x53\
-\xc9\x02\x07\x39\x30\x64\x00\x18\x48\x00\x01\x83\x6a\x5c\x13\x80\
-\x35\x64\x1b\x0b\x1b\x79\x10\x43\x06\x80\x61\xc2\x9f\x58\xd8\xf0\
-\x12\x97\x04\xd0\xd5\x30\x48\x3c\x8e\x41\x03\xc0\x28\xf5\x7f\x38\
-\x09\x11\x17\x1c\x74\x5d\x00\x41\xb1\x27\x31\x6c\x00\x18\xa6\xfe\
-\x6f\x26\x4b\x48\x93\xcb\x02\x10\xa2\xc6\xed\xc3\x6b\xc1\x00\x18\
-\xa5\xfe\x8f\xac\xfb\xe5\x3d\x00\xe7\xcd\x00\x58\xc0\x20\x8c\x1c\
-\x00\x46\x10\x40\xf8\x05\xfb\xbb\xfb\x67\xe7\x16\x80\x5f\x68\x03\
-\x0b\x89\xaf\xc2\xd0\x01\xe0\xeb\xd1\x2f\x90\x10\x93\x9e\xdf\x2b\
-\x01\x90\x68\xdd\x25\x44\x8d\xc3\x91\x60\x00\x7c\x1d\x29\x80\x58\
-\x48\xf2\xb1\xde\x09\x80\x88\x84\xe8\xf4\x3d\xbf\xbc\x41\x14\x00\
-\xe0\x5b\x08\x11\xa3\xea\x84\x6e\x1e\x01\xf6\x28\x00\x66\x4b\x2e\
-\xc3\x91\x60\x00\x7c\x5c\x00\xe1\x23\x0f\x92\x20\xe5\xf7\x5e\x00\
-\xc1\xf1\x15\x42\x78\x0a\x5e\x0d\x06\xc0\x97\x5b\x00\x51\xe3\x7b\
-\x2c\xe5\xbb\x17\x80\x35\x34\x57\x88\x1c\x5b\x84\x21\x04\xc0\x47\
-\x91\x03\x48\x88\x4e\xfb\xa6\x4f\x02\x20\x22\x62\xe1\x38\x12\x0c\
-\x80\xcf\xee\xfe\x81\xb1\xca\xb9\x5e\x01\x76\x59\x00\x42\x5c\xd6\
-\x76\xe6\x17\x86\x91\x04\xc0\x07\x11\x63\x27\xed\x60\x7e\xe1\x5b\
-\xfb\x2e\x80\xe0\xf8\x0a\x16\x92\x84\x3e\x00\x00\x3e\x88\x10\x93\
-\x9e\x77\xde\x7f\xe7\x3c\x35\xc4\x0e\x21\x61\x6a\x2e\x86\x12\x00\
-\x1f\x4b\xff\xad\xa1\x24\x44\x4f\x2c\xe8\x9f\x00\x88\x48\x88\x9e\
-\x98\x8f\xe1\x04\xc0\xe7\x76\xff\x12\x66\x1b\x72\xb4\xff\x02\x88\
-\x1c\x53\xc4\x6c\xc9\x18\x51\x00\x7c\x29\x03\x88\x1c\x5b\x44\x4c\
-\xe8\x7f\x06\xc0\x02\x63\x2a\x85\xc1\x93\x76\x60\x48\x01\xf0\x11\
-\xe4\x20\x12\x93\x67\x6d\x72\x29\x53\x70\xe1\xdf\x29\x14\x93\x67\
-\x6e\xc2\xeb\xc1\x00\xf8\x48\xfa\x1f\x9e\x52\x2f\x84\x0e\x2d\x75\
-\x97\x00\x48\x88\x49\xdf\xc3\x82\x06\x63\x64\x01\xf0\x01\xc4\xa4\
-\x19\x9b\xc8\x12\xbc\xcd\x6d\x02\x60\x7e\x11\x75\x62\xe2\x8c\xcd\
-\x18\x5a\x00\xbc\x3f\xfd\x17\x62\x32\x76\xbb\x9c\x2d\xb8\xd6\x51\
-\x10\x0a\x84\xd8\xcc\xaf\xf1\xc1\x10\x00\xbc\x3c\xfd\x8f\xb8\xa0\
-\xa6\xa7\xf7\xff\xfb\x26\x00\x22\x12\x62\x33\x77\xb1\xd0\x61\xb8\
-\x2e\x1c\x00\x6f\x16\x40\xfc\x94\x6d\x24\x5a\x77\xb9\x5d\x00\xcc\
-\x3f\x6a\x93\x18\x37\xe5\x4b\x0c\x31\x00\xde\x09\xb3\x04\x93\x34\
-\xe2\x57\x1f\xf6\x4a\x18\xbd\x6a\x2e\xa4\x2c\xf8\x80\x24\x7f\x8c\
-\x34\x00\xde\xb8\xfb\x27\xcd\xcc\x67\xa1\xc3\x8e\xea\x26\x00\x21\
-\x6a\x6c\xa1\x18\x3f\xa5\x18\x43\x0d\x80\xb7\x45\xbf\x44\xe2\x90\
-\xd9\x9f\x11\xb1\x02\xdd\x04\x40\x82\x94\x2f\x24\xcd\xdc\x84\x66\
-\x20\x00\x5e\x16\xff\xa1\xc3\x3a\x84\xf8\xa9\xbd\x2e\xd1\x7b\x1d\
-\xc9\x62\xe2\xb4\x5c\x16\x1c\x8f\x11\x07\xc0\x8b\x10\x87\x5d\xb1\
-\xa1\xbb\xbb\xff\xdd\x2a\x00\x16\x14\x57\x21\x26\xcd\xc4\x99\x00\
-\x00\xbc\x04\x66\x09\x26\x21\xc9\xb5\xa3\xbf\xfd\x16\x00\x11\x15\
-\x8a\xa3\x16\xbd\x43\x72\x10\x46\x1e\x00\x6f\x48\xff\x87\x5e\xbe\
-\x43\x88\x4c\xdd\xef\x29\x01\x90\x10\x39\x7a\x9f\x38\x64\x36\x5e\
-\x13\x06\x60\xa0\x91\x03\x48\x1a\xb5\xf0\x5d\x62\x62\xbe\xc7\x04\
-\x40\x44\x85\xe2\x88\x05\xef\xe1\x91\x20\x00\x03\x5c\xfb\xc7\x67\
-\x1f\x14\xa2\xd3\x77\xf7\xf5\xbf\x17\xfa\xfe\x07\x67\x6d\x17\x63\
-\x27\x95\x62\x0a\x00\x18\xa8\xe2\x5f\x20\x71\xe4\xc2\xb7\x7b\xba\
-\xf7\x5f\x37\x01\x90\x20\xe7\x89\xa3\x16\xbe\x83\x47\x82\x00\x0c\
-\x50\xed\x3f\x68\x42\x9d\x98\x38\xad\x5f\x57\xf6\xf5\x2b\x7a\xc5\
-\xc4\x4b\xb6\x08\xb1\x93\x4e\x62\x2a\x00\xf0\xf4\xee\x2f\x92\x94\
-\x7a\xdd\x5b\xbd\x39\xf7\xef\x76\x01\x90\x1c\xb8\x5d\x1a\x73\xf3\
-\xab\xc4\x44\x4c\x08\x00\x1e\xdd\xfd\xd3\xea\x84\xa1\x57\x6c\xe8\
-\xf7\xcf\xe9\xef\x0f\x10\x13\x72\x72\x85\xb8\xac\xe3\x98\x12\x00\
-\x3c\x15\xfd\x32\x49\x63\xfe\xe3\x75\xe6\xe2\xa5\x1f\xba\x0a\x80\
-\xe4\xc0\xed\xd2\xb8\x5b\x5f\xc1\x87\x44\x01\xf0\x0c\x62\x7c\x56\
-\x99\x38\xe4\xd2\x8d\x6e\x71\x89\x5b\xfe\x42\x09\xd3\xb6\x8a\xb1\
-\x93\xf1\x44\x00\x00\xfd\x8b\x7f\x12\xc7\xdc\xfc\x1a\xc9\x41\xdb\
-\xbd\x46\x00\x24\x48\xf9\xe2\xb8\xdf\xbc\x42\xa2\x15\xf3\x03\x80\
-\x9e\xbb\xff\x90\xd9\x07\xc5\x78\xf7\x7d\xac\xc7\x6d\xcf\xf0\xc4\
-\xd8\xc9\xdb\xc5\x94\x05\xdb\x31\x45\x00\xe8\x84\x1c\x44\xd2\x84\
-\xbb\x9e\x23\xd1\x92\xe7\x75\x02\x20\xd1\x92\x27\xa7\xdd\xb1\x9e\
-\x05\x46\x63\xa2\x00\xd0\x01\x69\xd4\xb5\x9b\xdd\xfd\xa5\x2e\xb7\
-\x9e\xe2\x61\xa1\x43\x4b\xa5\x31\x37\xbf\x85\xa9\x02\xc0\xcd\x95\
-\x7f\x48\x22\x49\xa3\x6f\x7c\x83\x88\x0a\xbd\x56\x00\x44\x54\x28\
-\x8e\xfa\xb7\x77\x84\xc8\xd1\xcd\x98\x32\x00\xdc\xb8\xfb\x8f\xbb\
-\xed\x65\x16\x96\x72\xc8\xdd\x3f\xd7\xed\xe7\x78\x59\x40\xd4\x26\
-\x69\xdc\x6f\x5e\x26\xd1\x82\x59\x03\xc0\x1d\x41\x3a\xf8\xa2\x1a\
-\x31\xe5\xea\xbf\xb9\x7b\xf7\xd7\x45\x00\x44\x44\xe2\x88\xab\x3e\
-\x10\x87\xcd\xc5\xeb\xc2\x00\xf4\x17\x4b\x30\x49\x13\x17\x3f\xcd\
-\xac\x21\xdb\xf4\xf8\xf1\xfa\xbc\xc9\x23\x48\xf9\xd2\x84\xbb\x9e\
-\x67\x21\x89\x98\x40\x00\xfa\x93\xfa\x8f\xbe\x71\x83\x98\x90\xbd\
-\x4d\xaf\x9f\xaf\xdb\xab\x7c\x42\xf8\xc8\x03\xd2\xc4\xff\x7e\x96\
-\x88\x61\x16\x01\xe8\x4b\x0c\x45\xa4\xb6\x4a\x63\x6f\x7d\xa5\xaf\
-\x97\x7d\x0c\xa8\x00\x88\xa8\x50\x1a\x3e\xef\x63\x71\xc8\xa5\x07\
-\x31\x95\x00\xf4\x3a\x8b\x26\x29\xe3\x77\x6b\x58\x60\xcc\x46\x5d\
-\xff\x18\x5d\x7f\x09\x39\x70\xbb\x9c\x79\xff\x2a\x16\x18\x83\x09\
-\x05\xa0\x37\xa9\xff\xa8\x85\xdb\xc5\x21\xb3\x3f\xd7\xdd\x33\x7a\
-\xff\x01\x2c\x2c\xe5\x90\x74\xe1\x3d\xeb\x51\x0a\x00\xe0\x62\x50\
-\x46\x8e\x6e\x96\x32\x96\xac\xe9\xed\x47\x3e\xbc\x52\x00\x44\x54\
-\x28\x5d\x70\xdd\x5f\xc5\x91\x57\xe7\x61\x6a\x01\x38\xcf\x86\xe9\
-\x17\x46\x52\xe6\x03\xab\x58\xc0\xa0\x4d\x9e\xf8\xf3\x3c\x73\x9f\
-\x17\x13\xf3\xe5\x0b\xef\x5d\x27\x84\xa7\xe0\xeb\xc2\x00\xf4\x94\
-\xfa\x8f\xbd\xf5\x5d\x31\x71\xba\xc7\xbe\xbb\xe1\xb1\x0b\xfd\x58\
-\x48\xd2\x47\xd2\xa4\x87\x1e\xc7\xbd\x01\x00\x9c\x1b\x31\x71\x7a\
-\xa9\x94\x76\xfb\x1f\x49\x87\x03\x3f\x03\x2e\x00\x22\x22\x31\x69\
-\xe6\x26\x29\xed\x8e\xf7\x30\xd5\x00\x9c\xb5\x41\x92\x34\xf9\x91\
-\xe5\x24\xf9\xef\xf0\x68\xbf\xc1\xc3\xbf\x67\xa1\x9c\x76\xc7\x7a\
-\x71\xd8\x95\x85\x98\x72\x00\xbe\x47\x0e\x20\x39\x7b\xe5\x32\x21\
-\x7c\xe4\x01\x4f\xff\xd1\xc2\x00\xfc\xb2\x3b\xe4\xac\xe5\x0f\x0b\
-\x11\xa9\xad\x98\x79\x00\x18\xc9\x13\xee\x7a\x5b\x4c\xbc\x64\xb3\
-\x27\x53\xff\x81\x13\x00\x11\xb1\xc0\xe8\x8d\x72\xd6\xe3\x8f\x30\
-\xff\x48\x33\x4e\xb8\x86\x45\x0f\x7e\x2c\x8b\x53\x16\xe4\x49\xe3\
-\xff\xf3\xe5\x81\x08\xfe\x01\x13\x00\x11\x91\x10\x97\xf5\xa5\x3c\
-\xe9\xc1\xa7\x71\xa5\x38\x20\xc9\xaf\xc3\x8c\xbf\xb6\x10\x35\xb6\
-\x49\x9e\xf4\xd0\x0a\x4f\xd7\xfd\x67\x0c\xfd\x00\xfe\xfe\x85\xe2\
-\xa8\x45\x24\xd9\xcb\x87\x2a\x05\xeb\x17\x98\x63\xca\x39\xa9\x25\
-\x1f\x2d\x64\x21\x89\x99\xc4\x35\x7c\x52\x89\x88\x88\x09\x1a\x6f\
-\x39\x19\x67\xba\x5f\x3b\x24\x91\xe4\x29\x2b\x97\xb1\xc0\xe8\x8d\
-\x03\xfa\xf7\xe0\x9c\x0f\x6c\x48\x74\x36\x4d\x77\xee\x58\xbe\x5a\
-\x3d\xfc\xfe\x64\x44\x03\x30\x45\xf0\xfb\x47\x90\x3c\x63\xfd\x52\
-\x31\x21\x67\xcb\x40\xa5\xfe\x03\x5e\x02\xfc\x38\x18\x56\x5b\xae\
-\x3c\xf9\xa1\x15\x62\xf2\xac\x62\x2c\x0d\x60\xfc\xa2\xdf\x4a\x72\
-\xd6\xf2\x35\xde\x10\xfc\x5e\x21\x80\x2e\x23\x46\x6d\x92\xa7\xac\
-\x5c\x26\x44\x8d\x6b\xc2\x0a\x01\x46\x46\xce\xf8\xdd\x9b\xe2\x88\
-\xab\xde\xf7\x86\xe0\xf7\x1a\x01\x10\x11\xb1\xe0\xf8\x0d\x72\xce\
-\xda\x7b\x99\x2d\x19\xab\x04\x18\x12\x69\xec\x2d\x9b\xa5\xb4\xdb\
-\x5f\xf0\x96\xe0\xf7\x2a\x01\x10\x11\x09\x51\x63\xf7\x5a\x66\xbd\
-\x74\x2b\x0b\x8e\xc7\x6a\x01\xc6\x0a\xfe\xd4\x1b\xb6\x49\x19\x4b\
-\xd7\x10\x13\x0a\xbc\x2a\xe6\xbc\x6c\x9c\x0a\x85\xa8\x71\x7b\x2d\
-\x33\x5f\xb8\x93\xf9\x47\x61\xd5\x00\x63\x94\xfd\x23\xaf\xdd\x25\
-\x65\x2e\x5b\xa9\xd7\xbd\x7e\x46\x12\x40\x97\x04\x62\x32\x76\x59\
-\x66\xbe\x70\x2f\xf3\x0b\xc7\xea\x01\xbe\x1d\xfc\x23\xe6\x17\xc8\
-\x17\x3f\xfa\x28\xf3\x0b\xdf\xea\x8d\x7f\x3f\x6f\x7d\x16\x5d\x28\
-\xc4\x4f\xf9\x52\x9e\xba\x7a\x05\xf3\x0b\xc3\x2a\x02\xbe\x19\xfc\
-\xc3\xae\x28\x92\xb3\x96\x3f\xe4\xad\xc1\x4f\x34\xb0\x07\x81\xce\
-\x2b\x01\x71\xd8\x95\xc4\xac\xb6\x26\xc7\x96\xc5\xcf\xf0\xf6\x53\
-\x58\x51\xc0\xc7\x76\xfe\xc7\x1f\x61\xfe\x91\x9b\xbd\xf9\xef\x39\
-\xe0\x07\x81\x5c\x20\x4d\xab\xca\xcb\x72\x7c\x71\xd7\x8b\xbc\xb5\
-\x1a\x2b\x0b\xf8\x44\xcd\x2f\x5f\xfc\xd8\xa3\xcc\x2f\x6c\xab\xb7\
-\xff\x5d\x7d\x41\x00\x5d\x12\xa8\xde\x93\xe9\xd8\xba\xf8\x4f\xdc\
-\x5e\x81\x15\x06\xbc\x16\x29\xf5\xfa\xed\x52\xe6\x03\x4f\x78\x73\
-\xda\xef\x8b\x02\xe8\x92\x40\x5d\xd1\x04\xc7\xd6\xdf\xfe\x89\x37\
-\x1c\xc1\x77\xc7\x80\xf7\x05\xff\xd8\x5b\x36\x4b\x19\x4b\xd7\x78\
-\x63\xb7\xdf\x08\x02\x20\x22\x22\xed\x74\xc9\x75\xce\xed\x0f\x3e\
-\xa3\x55\xe6\x0d\xc6\x92\x03\xde\x11\xf9\xfe\x24\x67\xdc\xf7\x3f\
-\x52\xda\x1d\xeb\xc9\x8b\x0e\xf9\x18\x52\x00\x44\x44\xbc\xa5\x6a\
-\xae\x73\xe7\x8a\x95\xea\xd1\x4f\xd2\xb0\xfa\xc0\x80\x06\x90\x7f\
-\x24\xc9\x59\x8f\xaf\xf1\xa6\xe3\xbd\x86\x17\x00\x11\x11\xef\x68\
-\x98\xa1\xe4\xad\x7d\x54\x39\xf8\xd7\x1c\x2c\x43\x30\x20\xc1\x13\
-\x92\x48\x72\xf6\x9a\xa5\x62\xe2\xb4\x2d\xbe\x18\xfc\x3e\x2d\x80\
-\xae\x7a\x40\xc9\x50\xf6\xbd\x7a\x97\xb3\xe0\xb9\x9b\xc8\xd9\x86\
-\x15\x09\x3c\x86\x10\x3d\xa1\x5e\xce\x7a\xe2\x41\x21\x7a\x62\xbe\
-\xaf\x06\xbf\xef\x0b\xa0\x8b\x34\xb5\x6c\xe3\x3c\xe7\xae\x55\x4f\
-\xe0\x09\x01\xf0\x04\x62\xca\xd5\x79\xf2\xc5\x8f\x3d\xc6\xfc\x23\
-\x36\xfb\xfa\xef\x62\x04\x01\x10\x7d\xff\x84\xc0\xb9\x73\xe5\x4a\
-\xad\x72\x57\x1c\x96\x28\xd0\x05\x39\x80\xe4\x09\x77\xbe\x2b\x4d\
-\xb8\xeb\x79\x12\x64\x43\x7c\xe9\xca\x28\x02\xe8\xea\x0b\x74\xda\
-\x73\x94\xdd\x6b\x1f\x55\x0e\xbc\x35\x83\x38\xee\xde\x04\x6e\x0c\
-\x14\xdb\x10\x4d\xce\x7a\xfc\x61\x31\x69\xc6\x17\x9e\xf8\x66\x1f\
-\x04\xd0\x9f\xbe\xc0\xfe\x37\x6e\x53\xf6\xfe\xf1\x36\xde\x56\x87\
-\x95\x0b\xfa\x5f\xef\x27\xe4\x94\xc9\x17\x3f\xf6\x98\x10\x3e\xf2\
-\x6d\xc3\x89\xcd\x70\x02\xf8\xa1\x24\xa8\x2d\x4c\x77\x7e\xbd\xe6\
-\x09\xed\xe4\x4e\x94\x04\xa0\x6f\xc1\x61\x09\x26\x69\xfc\x6d\xef\
-\x49\xe3\x6f\x5f\x4f\x72\xc0\x0e\x43\xfe\x8e\x06\x15\x40\x57\x49\
-\xd0\x71\x7a\x86\x52\xf4\xfa\xed\x4a\xd1\x6b\xd7\xe0\x29\x01\xe8\
-\xd5\xae\x3f\x68\x7c\x83\x74\xe1\x7d\xeb\xc4\xa4\x19\x9b\xc8\x87\
-\xbb\xfc\xa6\x16\xc0\x0f\xd9\x80\x7a\xf4\xd3\xab\x9c\xbb\x7f\xff\
-\x10\x6f\x3c\x2a\x61\x69\x83\x9e\x23\x5f\x22\x69\xd4\xc2\xed\x52\
-\xc6\x92\x35\x9e\xfa\x44\x37\x04\xe0\x89\x6c\xa0\xa5\x72\xae\xb2\
-\xef\x95\xbb\x94\x03\x7f\x9d\x43\x6a\x27\x16\x3a\x38\x3b\xf6\x23\
-\xc7\x34\x4b\xe9\x8b\x9f\x16\x93\x67\x7f\x46\x82\x94\x6f\x8a\x32\
-\xc7\x2c\x02\xf8\x31\x1b\xa8\xf8\x72\xa6\xb2\xe7\x99\x07\xb4\x9a\
-\xbd\x11\x58\xf2\x80\x88\x88\xe4\x00\x92\xc6\xdc\xbc\x41\x1a\xfd\
-\x1f\xaf\xb3\xe0\xf8\x0d\x66\xfa\xd5\xcd\x26\x80\xae\x6c\xa0\xb3\
-\x69\xba\xb2\xef\xd5\x3b\xd5\xfd\x6f\x5c\xc3\x3b\x71\x13\xb9\xa9\
-\x77\xfd\xd8\xcc\x2a\x69\xfc\xed\xeb\xc5\xe4\x59\x86\xae\xf5\x21\
-\x80\x73\x64\x03\x5a\xcd\xde\x0c\x65\xdf\x2b\x77\xab\x65\x9f\x8d\
-\x23\xae\x22\x1a\xcc\xb4\xf0\x43\x12\x49\x1a\x7b\xeb\x6b\xe2\xc8\
-\x6b\xdf\x65\x56\x5b\xae\x69\xc7\xc1\xc4\x02\xf8\x3e\x1d\x50\x33\
-\xd4\xb2\x4d\x97\x29\x85\x2f\xdd\xa3\xd5\xee\xc3\x05\x84\x46\x5f\
-\xf0\xd6\x10\x12\x53\xae\xde\x2c\x5e\x70\xc3\x5f\x84\x88\x51\x07\
-\xcc\xb8\xeb\x43\x00\xe7\x2c\x0b\x1a\xa7\xab\xc5\x7f\xbb\x41\x39\
-\xf8\xf6\x2d\xbc\xb1\x0c\x1f\xee\x34\xde\x52\x27\x71\xc8\xa5\x07\
-\xa5\xb4\xdb\xd7\x0b\x31\x17\xe6\x99\x3d\xf0\x21\x80\xee\x44\x60\
-\x2f\x5f\xa0\x1c\xfe\x60\x91\x7a\xf8\xfd\x85\xbc\xf9\x3b\x0c\x88\
-\x11\xea\xfc\x84\x9c\x32\x69\xcc\x4d\xaf\x8b\x49\x33\xbe\x20\x26\
-\xe6\x63\x44\x20\x80\xf3\xf6\x07\xb8\xbd\x22\x59\x39\xf8\xd7\x5b\
-\xd4\xe2\xf7\xe6\xe1\x46\x62\x5f\x5c\xd9\x02\x09\xd1\xe9\x35\x52\
-\xea\x0d\x6f\x8a\x43\xe7\x7c\x4a\x72\xd0\x76\x0c\x0a\x04\xd0\x7b\
-\x11\x34\x96\xa6\x28\x07\xdf\xbe\x49\x2d\xfd\xe4\x72\xdc\x4a\xec\
-\x23\x3b\xfe\xe0\x8b\x6a\xa4\x31\x37\xbf\x26\xc4\x67\x7f\xe9\x0b\
-\x37\xf3\x42\x00\xbe\x20\x82\x86\x92\x0b\xd4\xb2\x8d\x57\x2a\x25\
-\x1f\x2d\x42\x8f\xc0\x0b\x91\x03\x49\x8c\xbb\xb8\x58\x1c\xb9\xf0\
-\x6d\x31\x21\x27\xd7\xa8\x67\xf7\x21\x80\x81\xee\x11\xb4\xd5\xce\
-\x51\x4b\x37\x2c\x50\x4b\x3f\x99\xaf\xd5\x14\xe0\x03\x86\x03\xbd\
-\x80\xad\x21\x24\x0c\x99\xb3\x4b\x1a\xb9\xf0\x6d\x61\x70\xc6\x6e\
-\xd4\xf8\x10\x80\x67\x70\xb6\x65\xa9\x15\x5b\x67\xab\xa5\x1b\x16\
-\x68\x55\x7b\xc6\xf0\x76\xbc\x7a\xec\xd1\xfa\x3e\x7c\x64\xab\x30\
-\xe4\xb2\x7f\x88\x89\xd3\xb7\x08\xd1\x13\x7c\xfa\x5a\x2e\x08\xc0\
-\xa7\x53\x02\x2d\x5d\x3b\xb5\x7f\x9c\x56\xbe\x75\x96\x7a\x7c\xf3\
-\xe5\x5a\xfd\x21\x1b\x69\x0a\xc6\x45\x97\xdd\x3e\x94\x84\xa4\x4b\
-\xf2\xc5\xa4\x99\x9f\x0b\x09\x53\xff\xc9\xac\xa1\xb9\x18\x15\x08\
-\xc0\x7b\x5c\xd0\xd9\x34\x5d\xab\xda\x9d\xa9\x96\x6e\x58\xa0\xd5\
-\x14\x64\xe0\x8e\x42\x77\xd4\xf6\x01\x24\x44\x8d\xad\x12\x62\xb3\
-\xb6\x4b\xc3\xaf\xfc\x98\x85\x8d\x38\x84\xdd\x1e\x02\xf0\x76\xd2\
-\x78\x5b\x6d\x8c\xf6\xdd\x57\x39\x6a\xe5\xae\x2c\xed\xc4\xb6\x6c\
-\xde\x52\x45\x44\x18\x6b\x57\xeb\x7a\x16\x3a\xac\x5e\x4c\x9a\xb1\
-\x59\x48\x9a\xf9\xb9\x10\x3a\xac\x94\x24\x7f\x34\xf5\x20\x00\x1f\
-\x95\x41\x4b\x55\xbc\x56\xb7\x2f\x4d\x3d\xbe\x65\x0e\xaf\x2b\x4c\
-\xd7\xea\x8b\xfd\x30\x2c\xbf\x0c\x7a\x1b\x09\xd1\xe9\xa5\x2c\x6a\
-\x4c\x91\x98\x34\x73\x13\x0b\x1b\x51\xc2\x2c\xc1\xdb\x30\x32\x10\
-\x80\xe1\xca\x04\x5e\xb7\x6f\x82\x56\xb3\x77\xa2\x7a\x72\x67\x36\
-\x6f\x38\x92\xc8\xdb\x6a\x4d\x98\xda\x07\x12\x0b\x1c\xac\x88\xb1\
-\x17\xed\x12\xa2\x27\xe6\x0b\x31\x17\xe6\xb1\x90\xe4\x63\x66\x79\
-\x0f\x1f\x02\x00\x44\x9a\x92\xc1\x9b\x4f\x24\x69\x4d\xc7\x87\x6a\
-\x55\x79\x93\x79\xe3\xd1\xe1\x5a\x6d\xd1\x18\xde\x56\x4b\xa4\x39\
-\x8d\xb4\xcc\xba\x6a\xf9\xb0\x11\x0d\x42\x64\xea\x7e\x16\x35\xbe\
-\x40\x88\x1a\x57\xc4\x82\xe3\x2a\x7c\xe5\x2b\xba\x10\x00\xf0\x50\
-\xb9\x50\x19\xcf\xed\x15\x49\xda\xe9\x43\xa3\xb5\xda\xa2\x34\x6e\
-\x2f\x1f\xca\x5b\xab\xa3\x79\x4b\x25\xf9\xca\xd3\x05\xe6\x17\x46\
-\x2c\x70\x70\x2b\x05\x44\xd5\x08\xe1\x23\x8b\x85\xe8\xf4\x3c\x16\
-\x3a\xe4\x98\x10\x96\x52\x8c\x1d\x1e\x02\x00\xbd\x41\x69\xcf\xe2\
-\x9d\x76\x1b\x6f\xa9\x8c\xd3\x4e\x7d\x3b\x9e\xb7\x54\xc6\xf1\xd6\
-\x9a\x68\x6a\xab\x8d\xe6\xad\xd5\xb1\xbc\xb5\xc6\x8f\x6b\x0a\x91\
-\xd2\x4e\x1e\xbb\xd3\x40\xb4\x10\x93\xfc\x88\x04\x2b\xb1\x90\xf8\
-\x7a\x16\x10\x5d\xc3\x02\x63\xaa\x58\x60\x4c\x25\x0b\x1b\x5e\x22\
-\x84\x8f\x3a\x48\x7e\xa1\x0d\x78\x4c\x07\x01\x00\x3d\x51\x3b\x27\
-\x6b\x4d\xc7\x87\x92\xb3\x35\x80\xb7\xd7\x47\x90\xa3\xd9\xc6\x95\
-\xb6\x00\x5e\x5f\x3c\x9a\x37\x9f\x48\xe0\xce\xd6\x60\xea\xb4\x87\
-\x70\x67\x6b\x60\xd7\xad\xc8\x1a\x11\xd7\x88\x3b\x9a\x7f\x4a\xcd\
-\xbb\x3a\x13\x44\xa2\x95\x98\xe4\x4f\xc4\x35\x22\xc9\x4a\x24\x05\
-\x2a\xcc\x12\xd4\x4c\x56\x5b\x03\xb3\x04\xb7\x08\xd1\x13\xf2\x99\
-\xd5\xd6\x44\x72\x50\x0b\xb3\xda\x9a\xc8\x2f\xbc\x9e\xc9\x01\xad\
-\x2c\x38\xa1\x1c\xbb\x3a\x04\x00\xbc\x14\xee\x68\xce\x21\xcd\x29\
-\x91\xa6\xca\x44\x9c\x88\x73\x81\x34\xe7\xd9\xb7\x23\x33\x41\x23\
-\x41\x52\x7e\xf6\xbf\x9d\xd8\xc1\x21\x00\x00\x80\x81\xc1\x5b\x6d\
-\x00\x40\x00\x00\x00\x33\xf2\x7f\x03\x00\xf8\x9c\x68\x4d\x99\x9a\
-\x06\x90\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
-"
-
-qt_resource_name = b"\
-\x00\x06\
-\x07\x03\x7d\xc3\
-\x00\x69\
-\x00\x6d\x00\x61\x00\x67\x00\x65\x00\x73\
-\x00\x0a\
-\x05\x78\xd9\x27\
-\x00\x75\
-\x00\x70\x00\x6c\x00\x6f\x00\x61\x00\x64\x00\x2e\x00\x70\x00\x6e\x00\x67\
-"
-
-qt_resource_struct = b"\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
-\x00\x00\x00\x12\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-"
-
-def qInitResources():
-    QtCore.qRegisterResourceData(0x01, qt_resource_struct, qt_resource_name, qt_resource_data)
-
-def qCleanupResources():
-    QtCore.qUnregisterResourceData(0x01, qt_resource_struct, qt_resource_name, qt_resource_data)
-
-qInitResources()
+# -*- coding: utf-8 -*-
+
+# Resource object code
+#
+# Created by: The Resource Compiler for PyQt5 (Qt v5.7.1)
+#
+# WARNING! All changes made in this file will be lost!
+
+from PyQt5 import QtCore
+
+qt_resource_data = b"\
+\x00\x00\x21\xcf\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x01\x00\x00\x00\x01\x00\x08\x06\x00\x00\x00\x5c\x72\xa8\x66\
+\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\x0b\x13\x00\x00\x0b\x13\
+\x01\x00\x9a\x9c\x18\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\
+\x25\x00\x00\x80\x83\x00\x00\xf9\xff\x00\x00\x80\xe9\x00\x00\x75\
+\x30\x00\x00\xea\x60\x00\x00\x3a\x98\x00\x00\x17\x6f\x92\x5f\xc5\
+\x46\x00\x00\x21\x55\x49\x44\x41\x54\x78\xda\xec\x9d\x79\x7c\x14\
+\x55\xba\xbf\xdf\x53\x4b\x77\xf6\xce\x4a\x42\x76\xb6\x80\x61\x0b\
+\xc4\x18\x30\x84\x80\x2c\xa2\x22\x83\xa8\x70\xd5\xeb\x75\x99\xf1\
+\x5e\xb7\xcb\xa8\x03\xe2\x2e\xb2\x29\x8c\x3a\x8a\x8e\x8e\xfa\x73\
+\xae\x8e\xa3\xfe\xc6\x6d\xbc\xe8\x20\x22\x4c\x64\x10\x30\x84\x48\
+\x88\x2c\x21\x84\x40\x82\x64\x25\x24\xe9\xec\xdd\x55\x75\xee\x1f\
+\x71\x43\x48\xe8\x24\x5d\x9d\xee\xaa\xef\xf3\xd7\x7c\x46\x0d\xe4\
+\x9c\xf3\x3e\xe7\x7d\xdf\x3a\x75\x8a\x71\xce\x09\x00\x60\x4e\x04\
+\x0c\x01\x00\x10\x00\x00\xc0\x84\x48\x18\x02\x83\xe1\x68\xce\xe1\
+\x9a\x53\x22\xd5\x69\xe5\x6d\x35\xd1\xa4\x74\xf8\x11\x63\x7d\xfb\
+\x59\x9c\x13\x0b\x8c\xa9\x22\xd9\xbf\x83\x04\x4b\x27\xb3\xda\x72\
+\x31\xc0\x10\x00\x18\x38\xd2\x78\xf3\x89\x64\xee\x68\x0e\xa6\x8e\
+\xc6\x30\xde\xd1\x10\xca\x5b\xab\xe2\xb5\x53\xfb\xc7\x51\x67\x93\
+\x8d\x3b\xec\x36\x72\xb4\x06\x71\x47\x73\x30\x39\xec\xc4\x3b\xed\
+\x44\x5c\xed\xdf\x9f\x28\x07\x10\xb3\x04\x13\x59\x6c\x0e\x66\x09\
+\x6c\x26\x39\xa8\x99\x59\x43\x1b\x99\xd5\xd6\xc4\xa2\xc6\xed\x65\
+\x81\x83\x6a\x98\x5f\x58\x03\xb3\x84\xd8\x59\x50\x5c\x05\xc9\x01\
+\x3b\x30\x4d\xbe\x03\x43\x13\xd0\x3b\xe1\x8e\xe6\x1c\xea\x38\x1d\
+\xa1\xd5\x1f\x4a\xe5\xf6\xf2\x64\x6e\xff\x2e\x41\x6b\x2a\x1b\xce\
+\x1b\x4a\x86\x92\xb3\x8d\xb8\xd2\x41\xa4\x76\x7a\x41\x11\x29\x11\
+\x89\x56\x62\xa2\x95\x58\x60\x4c\x2b\x0b\x1b\x51\xcc\x6c\xc9\xc7\
+\x58\xd0\xe0\x4a\x21\x72\x6c\x11\x0b\x8c\xa9\x62\xfe\xe1\xf5\x24\
+\xc8\x79\x98\x55\x08\x00\x74\x17\xf0\xed\x75\x73\x78\x63\xd9\x30\
+\xad\xbe\xf8\x02\xad\x6a\xf7\x24\xde\x74\x6c\x38\x6f\x39\x69\xe3\
+\xed\xf5\xbe\xfb\x4b\x89\x16\x62\x81\x31\xc4\x82\x13\x2a\x84\xa8\
+\x71\x85\x42\xf4\x84\x02\x16\x3a\xfc\x88\x10\x3e\xa2\x84\x88\x15\
+\x60\xd6\x21\x00\x13\x07\xfc\xa9\xd9\xdc\x5e\x3e\x44\x3b\xf1\xaf\
+\x1c\xad\xf1\x68\x8a\x56\x57\x34\x81\x37\x7f\x27\x90\xea\x30\xf2\
+\x72\x23\xb2\x04\x91\x10\x99\x5a\x25\x84\xa5\x14\x0b\x83\x2f\xda\
+\x25\x44\x8d\xdf\xcb\x82\x62\x4f\x92\xe4\xb7\x0b\xab\x02\x02\x30\
+\x70\xc4\xab\x19\xbc\xe9\xf8\x10\xad\x7a\x4f\x86\x7a\x72\x67\xb6\
+\x56\x5b\x98\xce\x5b\x2a\x25\x52\xda\xcd\xbd\x00\x03\xa2\x88\x85\
+\x24\xd5\x89\x09\x39\x5b\xd8\xa0\x09\xdf\x08\x91\xa9\xfb\x59\xc0\
+\xa0\x4d\x58\x30\x10\x80\x11\x48\xd3\x4e\x1f\x1e\xad\x95\x6f\x99\
+\xa5\x55\x17\x64\x6a\x55\x5f\x8f\xe2\x9d\x76\x8c\x4a\x4f\x2d\x85\
+\xf0\x14\x87\x10\x93\xb1\x4b\x48\x9a\xb9\x49\x18\x94\x56\xc8\x02\
+\xa2\x20\x03\x08\xc0\xd7\x76\xfa\xf2\x24\xf5\xbb\x6d\x97\x68\xdf\
+\xed\xc8\xd1\xaa\xf3\x53\x7d\xba\x8e\x1f\xc8\xfe\x41\x50\x9c\x26\
+\x26\x5d\xb2\x59\x48\xbc\x64\xab\x30\x68\x7c\x01\xb3\x86\xe2\x31\
+\x24\x04\xe0\xa5\x71\xdf\x56\x37\x47\xab\xda\x7d\x91\x7a\xe4\xa3\
+\x45\x5a\xf5\x1e\x04\xbd\xbb\x33\x83\x88\xd4\x56\x21\x79\xf6\x67\
+\xe2\x90\xd9\x1b\x85\xa8\xb1\x45\x68\x22\x42\x00\x03\x8f\xe6\xcc\
+\xd4\x4e\x97\x8c\x52\xcb\x36\xce\xd5\x8e\x7d\x36\x4f\x6b\x28\xb5\
+\x10\xd7\x30\x2e\x7a\x22\x07\x91\x98\x38\xad\x48\x4c\x9c\xb6\x45\
+\x48\x98\xb6\x95\x05\xc6\x6c\xc4\xa0\x40\x00\x9e\xc5\xd1\x9c\xa3\
+\x56\xfc\x73\xa6\x5a\xfc\xde\xf5\x5a\x6d\xe1\x50\xde\xd9\x84\x31\
+\x19\x88\xc5\x1b\x3a\x4c\x11\x87\x5c\xba\x51\x1c\x31\xff\x03\x21\
+\x22\xf5\x5b\x22\x2a\xc4\xa8\x40\x00\xfa\xa5\xf9\xed\x75\x73\xd4\
+\x63\x9f\x5f\xa6\x1e\xfe\xe0\x3a\xad\x7a\x4f\x14\x46\xc4\x4b\x16\
+\xb1\x35\x94\x84\xa1\x97\x6d\x97\x86\xcf\xfb\x58\x18\x9c\xb9\x83\
+\x44\x0b\x0e\x1d\x41\x00\x6e\x23\x8d\x37\x94\x5c\xa0\x96\x6d\xbc\
+\x52\x39\xfc\xe1\x22\xde\x74\x0c\x2f\x50\x79\x2b\x96\x60\x12\xe3\
+\x2e\x3e\x28\xa6\x5c\xf3\xae\x98\x38\x2d\x97\x24\x7f\x1c\x4b\x86\
+\x00\xfa\x11\xf8\xf6\xf2\xa1\xca\xa1\x77\x6f\x54\x4b\x3f\x99\xcf\
+\xed\xe5\x18\x11\xdf\x59\xd6\x24\xc4\x67\x1f\x97\xc6\xdc\xf4\x9a\
+\x98\x38\x2d\x97\x44\x2b\x0e\x19\x41\x00\xbd\x48\xf5\xed\x15\xf3\
+\xd5\xd2\x0d\x0b\x94\x83\x6f\xdf\xc8\x9b\x4f\x60\x40\x7c\x15\x41\
+\x26\x31\x71\x5a\xb1\x98\xfa\xef\x6f\x8a\x09\x53\x73\xf1\x3e\x02\
+\x04\xd0\x73\xe0\x77\xda\x73\xd4\x23\x1f\x2d\x52\xf6\xbf\xf9\x6b\
+\xde\x70\xc4\x82\x11\x31\x08\x92\x1f\x89\x09\x39\x07\xa5\xf1\xff\
+\xf9\x92\x30\x38\x73\x07\xa1\x59\x08\x01\x9c\x81\xea\xc8\x54\x8f\
+\x7f\x7e\xb9\x52\xf4\xfa\x1d\x68\xee\x19\x18\x39\x90\xa4\x91\xd7\
+\x6e\x95\xc6\xdf\xf6\x12\x0b\x49\x2a\x83\x08\x20\x80\x34\xad\x76\
+\x5f\xba\xf2\xcd\x0b\xf7\xa9\xe5\x5b\x52\x49\x53\x10\x24\x66\x58\
+\xf4\x41\xb1\x24\x8d\xfb\xcd\xeb\x62\xca\x55\x1f\x30\x7f\x73\x1f\
+\x35\x36\xad\x00\x78\xcb\xc9\x79\x4a\xd1\x9f\x6f\x53\x0f\xbd\x33\
+\x97\x3b\x9a\x11\x15\x66\x6c\x11\x44\xa7\xd7\x49\x13\xef\x7e\x56\
+\x4c\x9e\xb5\xc9\xac\xd9\x80\xf9\x04\xc0\xd5\x0c\xb5\x6c\xe3\x5c\
+\x65\xcf\x73\xf7\x6b\xa7\x0f\xfb\x21\x0c\xcc\x6e\x01\x99\xa4\x51\
+\x8b\xb6\x89\x63\x6f\x79\x4d\x08\x1f\x79\xc0\x6c\x22\x30\x95\x00\
+\xb8\xbd\x7c\x81\x73\xcf\x73\x4b\xd4\x92\x0f\x27\xe3\xc8\x2e\x38\
+\x23\x10\x6c\xc9\x24\xa7\xdf\xb3\x4e\x1c\x76\xc5\x06\x33\x9d\x1f\
+\x30\x89\x00\x78\xba\x5a\xfc\xfe\xbf\x39\xbf\x79\xe1\x3e\x1c\xe4\
+\x01\x3d\x21\x0e\x9f\x57\x28\x67\xdc\xf7\x24\x0b\x1d\x5e\x62\x86\
+\x6c\xc0\xf0\x02\xe0\xf6\xf2\x05\xce\xfc\x67\xef\x57\x8f\xfc\x3d\
+\x13\xbb\x3e\x70\x29\x28\x82\x06\x93\x9c\xf1\xbb\x67\xc5\x51\x8b\
+\xde\x31\xfa\x5b\x87\xc6\x15\x00\xd7\xd2\xd5\x8a\xdc\x59\x4a\xde\
+\x53\x8f\x68\xf5\x87\x02\xb1\xac\x41\xef\x22\x43\x24\x71\xe4\xb5\
+\x3b\xe4\x0b\x7f\xfb\x34\x0b\x4e\xf8\x18\x02\xf0\xa5\xd8\x77\x34\
+\xe7\x28\x05\xcf\x2f\x51\xf6\xbf\x31\x97\x94\x0e\x2c\x66\xd0\x67\
+\x84\xc8\x31\xcd\x52\xe6\xb2\x55\x62\xe2\xf4\xcd\x46\x2c\x09\x8c\
+\x26\x80\x34\xad\xa6\x20\xd3\xb9\x6b\xcd\xe3\x5a\x55\xde\x60\x2c\
+\x5f\xe0\x16\xe4\x40\x92\x27\xdc\xf1\xae\x94\x76\xe7\xf3\x46\x7b\
+\xd3\xd0\x48\x02\x48\x53\x8f\x6d\x9a\xeb\xdc\xb9\x72\x25\x5e\xdc\
+\x01\x7a\x20\xa6\x5c\x9d\x27\x4f\x7e\x78\xb9\x91\x2e\x2d\x35\x84\
+\x00\x78\x67\xd3\x74\x75\xff\x1b\xbf\x76\xee\x7d\xf9\x06\x72\xb6\
+\x60\xa5\x02\xfd\x4a\x82\xa8\xb1\x4d\xf2\xc5\xcb\x1f\x16\x62\x8d\
+\xf1\x4e\x81\xcf\x0b\x80\xb7\x56\x5f\xee\xdc\xb9\x72\x85\x5a\xfa\
+\xbf\xe9\x58\x9e\xc0\x23\x41\x13\x34\x98\xe4\x49\x0f\xaf\x11\x47\
+\xcc\x7f\xdf\xd7\x25\xe0\xcb\x02\x48\xd3\xea\x0f\x8d\x75\x6e\x7f\
+\x64\x2d\xea\x7d\xe0\x71\x24\x3f\x92\xd3\xef\x79\x4b\x4a\xbb\xfd\
+\x05\x12\xa4\x7c\x08\xc0\xd3\xc1\x5f\xb9\x6b\xaa\x23\x77\xc9\xf3\
+\xa8\xf7\xc1\x80\x7a\x20\xf5\xfa\xed\x52\xe6\x03\x4f\x30\xbf\xf0\
+\xad\x10\x80\x67\x92\xfe\x74\xf5\xf0\x07\x0b\x9d\x3b\x57\xde\xcf\
+\x3b\x4e\x63\x05\x82\x01\x47\x1c\x7a\xf9\x7e\x39\x6b\xf9\x83\x2c\
+\x28\xf6\x53\x08\x40\xd7\xd8\xd7\xd2\x95\x7d\xaf\xdc\xe5\xdc\xf3\
+\x87\x5b\xc8\xd9\x86\x95\x07\xbc\x06\x21\x3a\xbd\x4e\xce\x59\x7b\
+\xaf\x10\x31\xea\x6d\x08\x40\x0f\x34\x25\xc3\x59\xf0\xfc\x12\xa5\
+\x60\xfd\xc2\x7e\x7f\xf3\x1e\x00\x3d\x82\x29\x74\xb8\x62\x99\xf5\
+\xe2\x6f\x84\xc8\x31\xfb\xc8\x47\x9a\x83\xbe\x21\x00\x4d\xc9\x70\
+\xe6\x3d\xf5\x98\xb2\xef\xd5\xb9\x38\xcf\x0f\xbc\x3a\xa0\x42\x92\
+\xc8\x32\x73\xfd\xed\x42\x74\x7a\x9e\x2f\x48\xc0\xfb\x05\xa0\x76\
+\x4e\x76\x7e\xbd\xe6\x31\xa5\xe8\xf5\x39\x58\x5e\xc0\x27\x24\x10\
+\x14\x4b\x96\x99\x2f\xde\x29\x0c\xbe\x68\x97\xb7\x4b\xc0\xbb\x05\
+\xa0\x76\x4e\x76\xee\x78\x62\xb5\x72\xe0\x2f\xd3\xb1\xac\x80\x4f\
+\x49\xc0\x3f\x92\x2c\x33\x5f\xbc\x57\x88\x9f\xf2\xa5\x37\x4b\xc0\
+\x7b\x05\x80\xe0\x07\x3e\x2f\x81\x08\xb2\xcc\x7e\xe5\x6e\x21\x76\
+\x92\xd7\x9e\x1a\xf4\xce\xcb\x31\x34\x67\xa6\xf3\xeb\x35\x8f\x21\
+\xf8\x81\x2f\xc3\xdb\xeb\xc9\xb1\xe5\xee\x17\xb5\xea\xfc\xc9\x44\
+\x94\x06\x01\xb8\x14\xfc\x4a\x86\x33\x6f\xed\x23\xa8\xf9\xf5\x45\
+\x1c\x79\xed\x2e\x31\x65\x41\x3e\x46\x42\x67\x09\xb4\x56\x93\xe3\
+\x8b\x3b\x5f\xd2\x6a\x0b\xd3\x21\x00\x57\x82\xbf\xe0\xf9\x25\x4a\
+\xe1\x9f\xe6\x62\xe9\xe8\x18\xfc\xc3\xe7\x15\xca\x53\x56\x3c\x68\
+\xc9\x5e\xbd\x54\x1c\x7a\xf9\x7e\x8c\x88\xce\x12\x68\xa9\x22\xc7\
+\xd6\xc5\xaf\x6a\xf5\x07\x6f\x84\x00\xba\x1f\xa6\x74\xa5\xe8\xb5\
+\x3b\x94\x82\xf5\x0b\xb1\x64\x74\x0c\xfe\x11\xf3\x0b\xe4\xec\xd5\
+\x4b\x98\x25\x78\x1b\x59\x82\xb7\xc9\xd3\xd6\x2d\x16\x87\x5d\x51\
+\x84\x91\xd1\x79\x75\x37\x96\x09\xce\xad\x8b\x5f\xe5\x8d\x47\x17\
+\x42\x00\x67\x93\xa6\x1e\xfe\x70\xa1\x73\xcf\x73\xb7\xe0\x90\x8f\
+\x9e\x3b\xff\xaf\x0a\xe4\x29\x2b\x97\x31\xbf\xb0\x1f\xcf\xad\x33\
+\x6b\x68\xae\x9c\xb3\xf6\x1e\x48\xc0\x03\x09\x6e\x7d\xb1\x9f\xe3\
+\xab\xc7\x9e\xe4\x6d\x75\x5e\x53\xde\x8a\xcb\x97\x2f\x1f\xf0\xe0\
+\xd7\x2a\x77\x4d\x75\x7e\xb9\x74\x15\x39\xec\x58\x25\xba\xa6\xfd\
+\x2b\x1f\x64\xfe\xe1\x5b\x7e\xf9\xcf\x98\xe4\x77\x5c\x88\x9b\x72\
+\x84\xdb\xcb\x27\xf2\x86\x23\x83\x30\x5a\x3a\x66\x02\xf6\xf2\x30\
+\xde\x56\x3b\x52\x88\x9d\x5c\xc6\x24\xff\x63\xa6\x17\x80\x76\xfa\
+\xf0\x0c\xc7\x17\x77\xbe\xc6\x5b\xab\xb1\x3a\xf4\xdc\xf9\xb3\x57\
+\xdf\x7f\xae\xe0\xff\x49\x02\xfe\xc7\x84\x84\xa9\xc5\xdc\x5e\x31\
+\x81\x37\x94\x44\x63\xd4\x74\x94\xc0\xe9\xe2\x38\x52\xda\xe3\xc4\
+\xa4\x4b\x8a\x88\xa8\xda\xb4\x02\xe0\xad\xd5\x97\x3b\xff\x79\xef\
+\x4b\xbc\xfe\x50\x10\x96\x85\x8e\x3b\x7f\xf6\xaa\xfb\x5d\x79\x5d\
+\x95\x49\x7e\xc7\x85\xf8\x29\x87\x79\xd3\xf1\x74\x64\x02\x3a\x6f\
+\x7c\xb5\x85\x43\x99\x35\x44\x14\xa2\x27\x9e\x18\x48\x09\x0c\x58\
+\x0f\x80\x77\x36\x4d\x77\xee\x5c\xb1\x5a\xab\xce\xc7\x6e\xa3\x57\
+\xf0\xff\xd0\xf0\xeb\xc5\xbb\xea\xcc\x1a\x9a\x2b\x4f\xfb\xfd\x62\
+\x71\xd8\x95\x85\x18\x41\x7d\x71\xe6\x3f\x73\x9b\x5a\xbe\x65\x0e\
+\x0d\xe0\x19\x81\x81\x12\x40\x9a\xba\xff\x8d\x5f\xab\xa5\x1b\xd2\
+\xb0\x0c\x74\xad\xf9\xcf\x68\xf8\xb9\x2e\x01\x5b\xae\x9c\xf3\xe4\
+\x7d\x68\x0c\xea\x8c\xa3\x99\x9c\x5f\x3d\xf6\xa4\x56\x5f\x3c\xda\
+\x4c\x02\xe8\xba\xbd\x77\xef\x1f\x6f\xc0\x0a\xd0\xb1\xe6\xef\x63\
+\xf0\x9f\x91\x09\xe4\xac\xbd\x07\xe7\x04\x74\xce\x84\xed\x15\xe4\
+\xdc\xb5\x72\x05\x39\x9a\x73\x4c\xd1\x03\xd0\x6a\xbe\xb9\xd2\xb9\
+\x6d\xd9\x1f\xa8\xfd\x14\x66\x5f\xb7\x9a\xbf\xe7\x86\x9f\xcb\x12\
+\x90\xfc\x8e\x0b\x09\xd9\x68\x0c\xea\x2e\x81\xf2\x30\x52\x3b\x63\
+\xc4\xb8\x8b\x4b\x49\x10\x4f\x1a\x57\x00\x8e\xe6\x1c\x07\x9a\x7e\
+\x3a\xa7\xfd\x2b\x96\x31\xff\x88\x2d\xee\xfa\x99\x68\x0c\x7a\x68\
+\x63\xac\xfb\x76\x38\x0b\x18\xd4\x26\x0c\x1a\x5f\x4d\x1e\x6c\x0a\
+\x7a\xae\x04\xe0\x5a\xba\x73\xcf\x73\x4b\xd0\xf4\xd3\x29\xf8\x47\
+\xcc\x2f\x90\xa7\xae\xb9\x8f\xf9\x47\x6e\x76\xf7\xcf\xfe\xa9\x31\
+\x88\x9e\x80\x7e\x06\x70\x92\x92\xff\xec\x62\xad\xae\x68\x82\x21\
+\x7b\x00\xea\x89\x2f\x67\x28\x07\xde\xc4\x19\x7f\x3d\x6b\x7e\x6b\
+\x68\xae\x5e\x7f\x06\xb3\xda\x72\xe5\xa9\x4f\xa1\x31\xa8\xe7\x1e\
+\xd9\x5e\x47\xce\xaf\xd7\x2c\x27\x67\x6b\xb6\xa1\x4a\x00\xde\x58\
+\x76\x8d\xf3\xcb\x25\x2f\xf2\xd6\x1a\x11\xd3\xac\xc3\xce\x9f\xbd\
+\xaa\x5f\x0d\x3f\xd7\xcb\x01\xff\x63\x42\xfc\x54\x94\x03\xba\xf6\
+\x03\x2a\x6c\x4c\xf2\xf3\x13\x06\x5f\x74\x9c\x18\xab\xf2\xfd\x0c\
+\x40\x73\x66\x3a\x77\xaf\x7d\x54\x3b\x5d\x62\xc1\xf4\xea\x12\xfc\
+\x4b\x3d\x11\xfc\x67\x64\x02\x78\x77\x40\x57\x9c\x7b\xff\x74\x9d\
+\xfa\xdd\x76\x8f\xdc\x85\xa1\xb7\x00\xd2\xd4\x92\xbf\x5f\xa3\x1e\
+\xdd\x38\x0e\xd3\xea\xee\xb4\xff\xfb\x86\x9f\x8e\x69\x7f\xb7\x12\
+\xf0\x0b\xdb\x8a\x72\x40\x4f\x03\xb4\x90\xb2\x6b\xd5\x72\xde\xae\
+\xff\x4b\x43\xba\x0a\x80\xdb\xcb\x87\x3a\xf7\xfc\x61\x09\x11\xc7\
+\xa4\xba\xbb\xe6\xef\xe5\x09\x3f\x5d\x24\x90\xf3\xfb\xc5\xe2\xb0\
+\xb9\x90\x80\x1e\x89\x73\xfd\xa1\x40\xa5\xf0\xd5\x3b\x48\xe7\x53\
+\x82\x7a\x0a\x20\xcd\xb9\xe7\x0f\xf7\xf3\xe6\x13\x98\x4d\x77\xef\
+\xfc\xd9\x2b\x97\x79\x32\xed\xef\xbe\x1c\x08\xd9\x26\x4f\xc5\x89\
+\x41\xbd\x50\xf6\xbf\x31\x4f\x3b\xb9\x73\xaa\x4f\x0a\x40\x2d\xdd\
+\x70\xb5\x7a\xe4\xe3\x4c\x4c\xa3\xdb\x6b\xfe\x25\xde\xf4\x1d\xba\
+\xae\x4c\x60\x1d\x7a\x02\xba\x18\xa0\x9d\x9c\xf9\x4f\x3f\x44\xce\
+\x96\x6c\x9f\x12\x00\x6f\xa9\x9a\xeb\xcc\x7f\xe6\x01\xd2\x14\x4c\
+\xa2\x5b\x77\xfe\x55\x4b\xbd\xf1\x23\x94\x78\x44\xa8\x63\x29\x50\
+\xb5\x3b\x5a\x29\xfa\xf3\x7f\x11\xf1\x74\xdf\x10\x80\xa6\x64\x28\
+\x45\xaf\xde\xc1\x1b\x8f\x4a\x98\x3e\x37\xd6\xfc\x3a\x3f\xe7\x77\
+\x4f\x26\xb0\xf6\x1e\xf4\x04\x74\x48\x04\x8a\x5e\xbb\x41\xab\xdb\
+\x3f\xce\x27\x04\xa0\x55\xe7\x4f\x56\x0e\xfd\xff\xcb\x31\x6d\x6e\
+\x0c\xfe\xec\x55\xcb\x98\x7f\xc4\x66\x6f\xff\xbb\x76\xbd\x40\xb4\
+\x0e\x8d\x41\x77\x67\xd4\x1d\x0d\xa4\xec\x7b\xe5\x2e\x3d\xb2\x00\
+\xf7\x0a\x40\x53\x32\x94\xa2\xff\xf7\x5f\xe4\x68\xc6\xac\xb9\x2d\
+\xed\xf7\x8e\x86\x9f\xeb\x12\x40\x63\x50\x0f\xd4\xa3\xff\x48\x57\
+\x8f\x6f\x99\xe5\xd5\x02\x50\x8f\x7d\x36\x57\x3d\xbe\x25\x15\xd3\
+\xe5\x86\xe0\xf7\xc2\x86\x5f\xef\xca\x81\x75\x28\x07\xdc\xba\xb9\
+\x3a\x49\xf9\x66\xfd\x12\xde\x69\xcf\xf1\x4a\x01\xf0\x4e\x7b\x8e\
+\xb2\xf7\xe5\xdf\xe2\x56\x5f\x37\xed\xfc\x53\x56\x2c\xf3\xc5\xe0\
+\xff\x29\x13\xb0\xe5\xca\x53\x9f\xbc\x0f\xf7\x09\xb8\xd1\x01\x35\
+\x85\x11\xea\xe1\xf7\xaf\xf3\x46\x01\xa4\xa9\x07\xfe\xf2\x6b\xad\
+\xae\xc8\x86\x69\x32\xef\xce\x7f\xee\x4c\x00\xc7\x86\xdd\xd8\x0d\
+\x20\x65\xff\x1b\xb7\xf1\xe6\x13\xf3\xbd\x4a\x00\xdc\x5e\x91\xac\
+\x1c\x7a\xf7\x46\x4c\x90\x5b\x82\x7f\xa9\x11\x82\xff\xec\x72\x00\
+\x12\x70\x4b\xac\x35\x1d\x13\xd4\x92\x0f\x17\x92\x9b\x4e\x08\xba\
+\x41\x00\x3c\x5d\x2d\xdd\xb0\x80\xdb\xcb\x31\x3b\xee\x48\xfb\xbd\
+\xf8\x51\x5f\xff\xca\x81\xa7\x50\x0e\xb8\x09\xa5\xf8\xbd\xeb\x78\
+\x4b\x65\xbc\x57\x08\x80\x37\x95\x27\x29\x07\xde\xc2\xee\xdf\xef\
+\x9d\x7f\xf5\x12\x23\xed\xfc\xe7\xcc\x04\xa6\xad\xc3\x6d\xc3\xee\
+\xc9\xb8\x49\x39\xf8\xce\x4d\xee\xc8\x02\xfa\x2b\x80\x34\xe5\xd0\
+\x3b\x37\xf1\x96\x93\x98\x95\x7e\xed\xfc\xbe\xf5\xa8\xaf\xef\x99\
+\x40\x28\x6e\x1b\x76\x13\xea\xa1\x77\xae\xe1\xf6\x8a\xe4\x01\x15\
+\x00\x6f\x28\xb9\x40\x3d\xfa\xe9\x3c\x4c\x47\xbf\x6a\xfe\x25\x66\
+\x08\xfe\x33\x25\x80\xc6\x60\xbf\xb3\x80\xb6\x5a\x52\x0e\xf5\x3f\
+\x0b\xe8\xbb\x00\xb8\x96\xae\x94\x7e\x32\x9f\xdb\x2b\x30\x1b\x7d\
+\xdd\xf9\x0d\xd6\xf0\x83\x04\x3c\x9c\x05\x94\x7c\x34\x9f\x37\x96\
+\x0d\x1f\x10\x01\xf0\xce\xc6\x50\xb5\xe4\x23\x7c\xca\xbb\xcf\x69\
+\xbf\x31\x1b\x7e\x90\x80\x07\xb3\x80\x96\x4a\x52\xcb\xfe\x31\x6f\
+\x40\x04\xa0\x1e\xfd\xf4\x2a\xec\xfe\x7d\x4c\xfb\x75\xba\xbd\xd7\
+\x37\x25\x80\x13\x83\xfd\x41\x29\xf9\x68\x11\x6f\x3f\x35\xdb\xb3\
+\x02\x70\x34\xe7\xa8\xc5\x7f\xbb\x1e\x37\xfd\xf4\x76\xe7\xff\x55\
+\x81\xd9\x77\xfe\xb3\x25\x80\x13\x83\xfd\xca\x02\x1a\x4a\x2d\xea\
+\xd1\x4f\xe7\x7b\x54\x00\x6a\xf9\xd6\xd9\x5a\xed\xbe\x30\x0c\x7f\
+\x2f\x77\xfe\xec\x55\xcb\xcc\x58\xf3\x9f\x57\x02\x7e\x61\x5b\xbb\
+\xbe\x3b\x80\x4c\xa0\x0f\x0a\x20\xf5\xc8\xc7\xd7\x90\xd2\x9e\xe5\
+\x19\x01\x68\xce\x4c\xa5\xf8\x6f\xd7\x63\xe0\x7b\x59\xf3\x7b\xf8\
+\xf6\x5e\x64\x02\xe6\x41\xab\xde\x13\xa5\x9e\xf8\x57\x8e\x47\x04\
+\xa0\x9d\x3e\x3c\x8a\xd7\xed\x4b\xc6\xb0\xf7\x26\xed\x5f\x89\xb4\
+\xdf\xd5\x4c\x00\x8d\xc1\x3e\xa1\x1e\xf9\xfb\x22\xe2\x6a\x86\xee\
+\x02\x50\x8f\xfe\x63\x1e\xef\xb4\x63\xc4\x5d\xdd\xf9\xa7\xae\x59\
+\xea\x0b\x97\x79\x78\x97\x04\xf0\xee\x40\xaf\x37\xe6\xaa\xbc\x71\
+\xbc\xf9\x64\x9c\xae\x02\xe0\xed\x75\x73\xd4\xb2\xcf\x70\xf0\xc7\
+\xd5\xe0\x9f\xb2\x72\x19\xb3\xda\xb0\xf3\xf7\xa9\x1c\x78\xea\x3e\
+\xf4\x04\x7a\x11\x9b\x6d\x75\xa4\x1e\xdb\x34\x57\x57\x01\x68\x95\
+\x5f\x4f\xe6\x8d\xa5\xb8\xeb\xef\x7c\xc1\xff\xc3\xd9\x7e\xec\xfc\
+\xfd\xcd\x04\xd0\x18\xec\x7d\x76\x9e\xa3\x8f\x00\xb8\x96\x8e\x83\
+\x3f\x2e\x04\xff\xb0\x2b\x4d\x73\xb6\x5f\xff\x4c\xe0\xfb\xeb\xc5\
+\xd0\x18\x74\x6d\x83\xae\x2d\x8c\xe2\xa7\xbe\x9d\xa0\x8b\x00\x78\
+\xd3\xf1\x21\x5a\x75\xc1\x28\x0c\xf3\x79\x76\xfe\xa9\xab\x97\x20\
+\xf8\xdd\x9d\x09\x3c\x85\x9e\x80\x4b\x41\xaa\x92\x7a\xe4\xe3\x05\
+\xba\x08\x40\xfd\x6e\xdb\x25\xbc\xe3\x34\x06\xb9\xdb\x9a\xff\xfb\
+\x6e\x3f\x9e\xf3\xeb\x20\x81\x70\x34\x06\x5d\x8d\xd3\xaa\xbc\x2c\
+\xde\xd1\x30\xc3\xbd\x02\xd0\x94\x0c\xad\x62\xdb\x0c\x0c\x6f\x0f\
+\x69\x7f\x36\xd2\x7e\x7d\xcb\x01\x5c\x2a\xe2\x52\x12\xd0\x78\x4c\
+\xd0\x4e\xee\xcc\x72\xab\x00\xb4\x86\xd2\x14\xad\x7a\x77\x0a\x86\
+\xb7\x9b\x9d\x7f\xea\x9a\x25\xd8\xf9\x3d\x54\x0e\x4c\x43\x63\xf0\
+\x3c\x0a\x20\xed\xe4\x57\xd3\x5c\xfd\x86\x80\x6b\x02\x28\xdf\x72\
+\x29\x9e\xfd\x77\x97\xf6\xaf\x78\x08\x3b\xbf\x27\x33\x81\xd0\x5c\
+\x39\xe7\xa9\x7b\x90\x09\xf4\x50\x06\x9c\xd8\x36\x9d\xb7\x9d\x8a\
+\x72\x8f\x00\xd4\xce\xc9\x5a\x55\xde\x64\x0c\xeb\x2f\x82\x7f\xc4\
+\xfc\x02\x39\x7b\xe5\x32\x3c\xea\x1b\x20\x09\x4c\x5b\xb7\x18\x3d\
+\x81\x6e\x72\x80\x96\x4a\xd2\x6a\x0b\xd3\xdc\x22\x00\xed\xf4\xe1\
+\x51\x6a\x55\xde\x70\x0c\xeb\xcf\x77\x7e\xf3\x5e\xe6\xe1\x55\x12\
+\xc0\x07\x49\xbb\x09\x5a\x85\xb4\xf2\x2d\x73\xdc\x22\x00\x5e\x7f\
+\x28\x95\x9c\x6d\x18\xd4\x33\xd2\x7e\x9c\xed\xf7\x9a\x9e\x00\x3e\
+\x48\x7a\x6e\x07\xd4\x15\xa5\xb9\x72\x28\xa8\x67\x01\x70\x35\x43\
+\x3d\xb1\x6d\x26\x86\xf3\x67\xc1\xef\x23\x1f\xea\x34\x5d\x4f\x00\
+\x99\xc0\x99\x02\x38\x75\xd0\xc6\x4f\xed\x1f\xdf\x2f\x01\xf0\x8e\
+\x86\x30\x57\x6b\x09\x73\x04\x3f\x1e\xf5\x79\x77\x39\x80\x4c\xe0\
+\x67\x9b\x37\x69\x75\xfb\xd2\xfa\x27\x80\xa6\xe3\x43\x78\x5b\x2d\
+\x82\xff\x87\x86\x1f\x6a\x7e\x1f\x28\x07\x90\x09\xfc\x80\xfa\xdd\
+\x57\x39\xa4\x39\x33\xfb\x2c\x00\xf5\xc4\xbf\x2e\x21\xa5\xc3\xdc\
+\xc1\xff\xe3\xd9\x7e\x04\xbf\xf7\x67\x02\x38\x2c\x74\xc6\x06\x5e\
+\x7f\x68\x28\x6f\xad\x89\xee\xab\x00\xd2\x78\xc3\x61\x53\x9f\xfd\
+\xff\xe9\x1a\x2f\xa4\xfd\x3e\x95\x09\x4c\x5b\xb7\x18\x12\x20\xe2\
+\xed\xf5\xc4\x9b\x7a\xbe\x36\x5c\xe8\xfe\x3f\xae\x8b\xd1\xea\xbe\
+\x1d\x67\xea\x9d\x3f\x7b\x15\x2e\xf3\xf0\xd5\x9e\x00\x24\xd0\xf5\
+\x72\x50\xe5\xee\xc9\x7d\x13\x40\x63\xd9\x30\xde\x52\x69\xce\xe0\
+\x1f\xfe\xab\xae\xb7\xfa\xf0\xa8\xcf\xf7\x25\x60\xf2\x6f\x11\x7e\
+\x9f\x01\xa4\xf5\x5a\x00\xda\xa9\x03\x63\x49\x53\x4c\x9c\xf6\xa3\
+\xe6\x37\x84\x04\x4c\xde\x18\xd4\x6a\x0b\xd3\x78\x6b\x4d\x6c\xef\
+\x05\x50\xb5\xdb\x74\xc7\x7f\xcd\xf4\xa1\x4e\xf3\x48\x20\x64\x5b\
+\x57\x63\xf0\x32\x53\x96\x03\xbc\xa5\x92\xb8\xbd\x3c\xa9\x57\x02\
+\xe0\x8e\xe6\x1c\xde\x74\x7c\x88\xe9\x76\x7e\x04\xbf\x31\x25\xf0\
+\xe3\x45\xa3\x26\x3c\x27\xa0\x29\xa4\x35\x94\xa6\xf4\x2e\x03\x68\
+\xaf\x8f\xe0\xcd\x27\x82\x4d\xb5\xf3\xa3\xe1\x67\x02\x09\xac\x35\
+\xe5\x5b\x84\xbc\xae\x30\xbd\x57\x02\xd0\xea\x0f\xa5\xf2\xce\x26\
+\x93\x04\x3f\xce\xf6\x9b\xa7\x1c\xb0\x99\xb2\x27\xa0\x35\x1e\x1d\
+\xde\xbb\x12\xa0\xe9\x98\x29\xde\xfe\xfb\xb1\xe1\x87\x9d\x1f\xe5\
+\x80\x91\x33\x80\xd6\xda\xe8\xee\x3e\x20\x7a\x6e\x01\xb4\x9c\x8c\
+\x37\x45\xda\x3f\x65\x05\x6a\x7e\xd3\x66\x02\xe6\xb9\x54\x84\xb7\
+\x56\x09\xbc\xf9\x64\x82\x6b\x02\xd0\x94\x0c\xad\xf1\xe8\x08\xc3\
+\xef\xfc\x38\xde\x6b\x72\x09\xfc\xf0\x88\xd0\x04\x99\x80\xd2\x41\
+\xda\xa9\xfd\x63\x5c\x12\x00\x6f\xad\x8a\xe3\x0d\x47\x12\x0d\x5d\
+\xf3\xa3\xe1\x07\xe8\x67\x57\x8e\x9b\x20\x13\xe0\x2d\x55\xf1\xae\
+\x09\xa0\xd3\x6e\x33\xea\x05\x20\x3f\xde\xe1\x87\x86\x1f\x38\x2b\
+\x13\x30\x76\x63\x90\xb7\x9d\xfb\xa5\xa0\xb3\x4b\x80\x8e\xfa\x08\
+\x6e\xc0\x37\x00\xbb\x3e\xd4\xb9\x1a\x3b\x3f\xe8\x26\x13\x30\xf8\
+\x77\x07\xda\x6a\x5d\x13\x00\xef\x6c\xb2\x91\xe6\x34\xe0\xce\x8f\
+\x47\x7d\xa0\xa7\x4c\xc0\x66\xe8\x9e\x00\x6f\xa9\x8a\x23\x67\x5b\
+\xd6\x79\x05\xa0\x9d\x3a\x30\xce\x70\xc1\x8f\xdb\x7b\x81\xcb\xe5\
+\xc0\x53\x86\x94\x00\x6f\xad\x0e\xe4\x2d\x27\x13\xcf\x9f\x01\xf4\
+\xe1\x1b\xe3\x5e\x9f\xf6\xa3\xdb\x0f\x7a\x2d\x01\x63\x95\x03\x5c\
+\x73\x12\x77\xb6\x05\x9c\xbf\x07\xd0\xd9\x14\x86\xb4\x1f\x40\x02\
+\x06\x6b\x0c\x2a\xed\xc4\x3b\xea\x23\xce\x9f\x01\x38\x9a\x7d\xfe\
+\x1d\x00\x71\xd8\x95\x68\xf8\x01\x48\xe0\x8c\xda\x5e\x21\xea\xb4\
+\xdb\x7a\x14\x00\xef\xb4\xe7\x90\xb3\x25\xc8\xe7\xd3\xfe\xec\x55\
+\xd8\xf9\x81\x7b\x24\x60\xa4\xdb\x86\x95\x76\xbf\x9e\x33\x00\xcd\
+\x61\xe5\x8e\xe6\x40\x9f\x0d\xfe\x11\xf3\x0b\xe4\xec\xd5\x4b\xb0\
+\xf3\x03\xb7\x49\xc0\x40\xb7\x0d\xf3\xce\xc6\xb0\xf3\x08\x40\x95\
+\xc8\xe1\x9b\x1f\x01\xc5\x65\x1e\x40\xbf\x4c\xc0\x66\x88\xcf\x90\
+\x69\xd5\x05\x99\x3d\x97\x00\xad\xd5\x83\xb9\xa3\xc5\x47\x77\xfe\
+\x55\x4b\x10\xfc\x40\xdf\x4c\x60\xdd\x3d\xbe\x7c\xc7\x20\x3f\x47\
+\x79\x7f\x66\x06\xa0\x76\x5a\x88\x6b\x3e\x34\x2b\x02\x49\xa9\xd7\
+\x6f\xb7\xe4\xac\xbd\x17\x8f\xfa\x80\x27\x32\x01\xcb\xf4\x67\xee\
+\x96\x52\xaf\xdf\x4e\x4c\xf4\xbd\x5f\xa0\xd3\x6e\x23\x47\xf3\x19\
+\xdf\x0b\x94\xce\xfc\x0d\x99\xaf\x4d\x08\x11\x93\x14\x67\xde\x53\
+\x8f\x90\xa6\xca\xde\xad\x5f\x4d\x20\x41\x52\xa4\x89\xff\xfd\x2c\
+\x0b\x8c\xde\x88\x70\xfa\xd9\xd0\x34\x1d\xbb\x46\xf9\xf6\x7f\x6e\
+\x23\xd5\x61\x25\x26\x78\xf7\x0e\x24\x88\x4e\x62\x92\xc2\x2c\x81\
+\xc4\x3b\x7d\xab\x5c\xe6\x0e\xbb\x8d\x6b\x8a\xc4\xba\x15\x80\xaf\
+\x2d\x9c\x8e\x06\x52\x0e\xfc\x65\xba\x4f\x95\x2b\x43\x2e\xdd\x08\
+\x01\xfc\x72\x1e\x4f\x47\x28\xdf\xfe\x79\x36\x46\x42\x67\x54\x07\
+\x11\x57\xc5\xee\x4b\x00\xa0\x3f\x7e\x61\xf5\x18\x84\xb3\xb6\x55\
+\x8d\x04\x19\xc3\xa0\x37\x9a\x93\x88\x73\x01\x02\x18\xb8\xa2\x85\
+\x98\x5f\x04\x04\x00\x06\x48\x00\x2a\x11\x71\x82\x00\x06\x76\x16\
+\x30\xe6\x60\x60\x4a\x2d\xcd\xd9\xf5\xa8\x1f\x02\x00\xc0\xa4\x3d\
+\x80\x5f\x6c\x40\x10\x00\x00\xa6\x49\x01\x54\x22\x8e\x12\x00\x00\
+\x00\x01\x00\x60\x32\x44\x0b\xfd\xf2\x9c\x05\x04\x00\x80\x49\x60\
+\x82\x0c\x01\x00\x60\xde\x7c\x1f\x02\x00\xc0\xc4\x02\x90\x20\x00\
+\x00\x4c\x9d\x01\xd0\x99\xef\xfb\x40\x00\x00\x98\x05\xc9\xdf\x41\
+\x82\xe4\xec\x5e\x00\xbf\x78\x46\x08\x00\x30\x0e\xcc\x2f\xb4\x81\
+\x59\x6d\xb9\xdd\x0b\x40\xf2\xeb\xc0\x4b\x19\x00\x18\x54\x00\x72\
+\x60\xf3\x59\x55\xc1\x19\xff\x42\xe0\xe0\x2a\x66\xb5\x61\xa4\x00\
+\x30\x22\x56\x5b\x53\x8f\x02\x20\x41\x72\x92\x25\x58\xc3\x48\x01\
+\x60\x3c\x84\x41\x13\xf6\xf4\x9c\x01\xf8\x85\x6d\x65\x96\xe0\x66\
+\x0c\x15\x00\xc6\xec\x01\xf4\x9c\x01\x10\x11\xc9\x81\x2d\x18\x2a\
+\x00\x0c\x17\xfe\x44\x92\x7f\xfb\x79\x05\x70\x2e\x4b\x00\x00\x7c\
+\x1c\xc9\x4a\xcc\x2f\xbc\xde\x05\x01\x84\x41\x00\x00\x18\x6d\xff\
+\x17\x2d\x44\xd6\x10\xfb\xf9\x05\x10\x39\x76\x2f\x86\x0b\x00\x83\
+\x21\x07\xbb\x98\x01\x04\x46\xd7\x10\xc3\x01\x41\x00\x0c\x95\x01\
+\x84\x24\x54\xb1\xc0\x98\x4a\xd7\x4a\x00\xc9\x0f\x23\x06\x80\x91\
+\x04\xe0\x1f\x51\x47\x44\x85\xe7\x15\x00\x59\x6c\x8d\x4c\xb0\x60\
+\xc4\x00\x30\x92\x00\x02\x07\x57\x9e\xeb\xff\x3f\x47\x09\x10\x53\
+\xc9\x02\x07\x39\x30\x64\x00\x18\x48\x00\x01\x83\x6a\x5c\x13\x80\
+\x35\x64\x1b\x0b\x1b\x79\x10\x43\x06\x80\x61\xc2\x9f\x58\xd8\xf0\
+\x12\x97\x04\xd0\xd5\x30\x48\x3c\x8e\x41\x03\xc0\x28\xf5\x7f\x38\
+\x09\x11\x17\x1c\x74\x5d\x00\x41\xb1\x27\x31\x6c\x00\x18\xa6\xfe\
+\x6f\x26\x4b\x48\x93\xcb\x02\x10\xa2\xc6\xed\xc3\x6b\xc1\x00\x18\
+\xa5\xfe\x8f\xac\xfb\xe5\x3d\x00\xe7\xcd\x00\x58\xc0\x20\x8c\x1c\
+\x00\x46\x10\x40\xf8\x05\xfb\xbb\xfb\x67\xe7\x16\x80\x5f\x68\x03\
+\x0b\x89\xaf\xc2\xd0\x01\xe0\xeb\xd1\x2f\x90\x10\x93\x9e\xdf\x2b\
+\x01\x90\x68\xdd\x25\x44\x8d\xc3\x91\x60\x00\x7c\x1d\x29\x80\x58\
+\x48\xf2\xb1\xde\x09\x80\x88\x84\xe8\xf4\x3d\xbf\xbc\x41\x14\x00\
+\xe0\x5b\x08\x11\xa3\xea\x84\x6e\x1e\x01\xf6\x28\x00\x66\x4b\x2e\
+\xc3\x91\x60\x00\x7c\x5c\x00\xe1\x23\x0f\x92\x20\xe5\xf7\x5e\x00\
+\xc1\xf1\x15\x42\x78\x0a\x5e\x0d\x06\xc0\x97\x5b\x00\x51\xe3\x7b\
+\x2c\xe5\xbb\x17\x80\x35\x34\x57\x88\x1c\x5b\x84\x21\x04\xc0\x47\
+\x91\x03\x48\x88\x4e\xfb\xa6\x4f\x02\x20\x22\x62\xe1\x38\x12\x0c\
+\x80\xcf\xee\xfe\x81\xb1\xca\xb9\x5e\x01\x76\x59\x00\x42\x5c\xd6\
+\x76\xe6\x17\x86\x91\x04\xc0\x07\x11\x63\x27\xed\x60\x7e\xe1\x5b\
+\xfb\x2e\x80\xe0\xf8\x0a\x16\x92\x84\x3e\x00\x00\x3e\x88\x10\x93\
+\x9e\x77\xde\x7f\xe7\x3c\x35\xc4\x0e\x21\x61\x6a\x2e\x86\x12\x00\
+\x1f\x4b\xff\xad\xa1\x24\x44\x4f\x2c\xe8\x9f\x00\x88\x48\x88\x9e\
+\x98\x8f\xe1\x04\xc0\xe7\x76\xff\x12\x66\x1b\x72\xb4\xff\x02\x88\
+\x1c\x53\xc4\x6c\xc9\x18\x51\x00\x7c\x29\x03\x88\x1c\x5b\x44\x4c\
+\xe8\x7f\x06\xc0\x02\x63\x2a\x85\xc1\x93\x76\x60\x48\x01\xf0\x11\
+\xe4\x20\x12\x93\x67\x6d\x72\x29\x53\x70\xe1\xdf\x29\x14\x93\x67\
+\x6e\xc2\xeb\xc1\x00\xf8\x48\xfa\x1f\x9e\x52\x2f\x84\x0e\x2d\x75\
+\x97\x00\x48\x88\x49\xdf\xc3\x82\x06\x63\x64\x01\xf0\x01\xc4\xa4\
+\x19\x9b\xc8\x12\xbc\xcd\x6d\x02\x60\x7e\x11\x75\x62\xe2\x8c\xcd\
+\x18\x5a\x00\xbc\x3f\xfd\x17\x62\x32\x76\xbb\x9c\x2d\xb8\xd6\x51\
+\x10\x0a\x84\xd8\xcc\xaf\xf1\xc1\x10\x00\xbc\x3c\xfd\x8f\xb8\xa0\
+\xa6\xa7\xf7\xff\xfb\x26\x00\x22\x12\x62\x33\x77\xb1\xd0\x61\xb8\
+\x2e\x1c\x00\x6f\x16\x40\xfc\x94\x6d\x24\x5a\x77\xb9\x5d\x00\xcc\
+\x3f\x6a\x93\x18\x37\xe5\x4b\x0c\x31\x00\xde\x09\xb3\x04\x93\x34\
+\xe2\x57\x1f\xf6\x4a\x18\xbd\x6a\x2e\xa4\x2c\xf8\x80\x24\x7f\x8c\
+\x34\x00\xde\xb8\xfb\x27\xcd\xcc\x67\xa1\xc3\x8e\xea\x26\x00\x21\
+\x6a\x6c\xa1\x18\x3f\xa5\x18\x43\x0d\x80\xb7\x45\xbf\x44\xe2\x90\
+\xd9\x9f\x11\xb1\x02\xdd\x04\x40\x82\x94\x2f\x24\xcd\xdc\x84\x66\
+\x20\x00\x5e\x16\xff\xa1\xc3\x3a\x84\xf8\xa9\xbd\x2e\xd1\x7b\x1d\
+\xc9\x62\xe2\xb4\x5c\x16\x1c\x8f\x11\x07\xc0\x8b\x10\x87\x5d\xb1\
+\xa1\xbb\xbb\xff\xdd\x2a\x00\x16\x14\x57\x21\x26\xcd\xc4\x99\x00\
+\x00\xbc\x04\x66\x09\x26\x21\xc9\xb5\xa3\xbf\xfd\x16\x00\x11\x15\
+\x8a\xa3\x16\xbd\x43\x72\x10\x46\x1e\x00\x6f\x48\xff\x87\x5e\xbe\
+\x43\x88\x4c\xdd\xef\x29\x01\x90\x10\x39\x7a\x9f\x38\x64\x36\x5e\
+\x13\x06\x60\xa0\x91\x03\x48\x1a\xb5\xf0\x5d\x62\x62\xbe\xc7\x04\
+\x40\x44\x85\xe2\x88\x05\xef\xe1\x91\x20\x00\x03\x5c\xfb\xc7\x67\
+\x1f\x14\xa2\xd3\x77\xf7\xf5\xbf\x17\xfa\xfe\x07\x67\x6d\x17\x63\
+\x27\x95\x62\x0a\x00\x18\xa8\xe2\x5f\x20\x71\xe4\xc2\xb7\x7b\xba\
+\xf7\x5f\x37\x01\x90\x20\xe7\x89\xa3\x16\xbe\x83\x47\x82\x00\x0c\
+\x50\xed\x3f\x68\x42\x9d\x98\x38\xad\x5f\x57\xf6\xf5\x2b\x7a\xc5\
+\xc4\x4b\xb6\x08\xb1\x93\x4e\x62\x2a\x00\xf0\xf4\xee\x2f\x92\x94\
+\x7a\xdd\x5b\xbd\x39\xf7\xef\x76\x01\x90\x1c\xb8\x5d\x1a\x73\xf3\
+\xab\xc4\x44\x4c\x08\x00\x1e\xdd\xfd\xd3\xea\x84\xa1\x57\x6c\xe8\
+\xf7\xcf\xe9\xef\x0f\x10\x13\x72\x72\x85\xb8\xac\xe3\x98\x12\x00\
+\x3c\x15\xfd\x32\x49\x63\xfe\xe3\x75\xe6\xe2\xa5\x1f\xba\x0a\x80\
+\xe4\xc0\xed\xd2\xb8\x5b\x5f\xc1\x87\x44\x01\xf0\x0c\x62\x7c\x56\
+\x99\x38\xe4\xd2\x8d\x6e\x71\x89\x5b\xfe\x42\x09\xd3\xb6\x8a\xb1\
+\x93\xf1\x44\x00\x00\xfd\x8b\x7f\x12\xc7\xdc\xfc\x1a\xc9\x41\xdb\
+\xbd\x46\x00\x24\x48\xf9\xe2\xb8\xdf\xbc\x42\xa2\x15\xf3\x03\x80\
+\x9e\xbb\xff\x90\xd9\x07\xc5\x78\xf7\x7d\xac\xc7\x6d\xcf\xf0\xc4\
+\xd8\xc9\xdb\xc5\x94\x05\xdb\x31\x45\x00\xe8\x84\x1c\x44\xd2\x84\
+\xbb\x9e\x23\xd1\x92\xe7\x75\x02\x20\xd1\x92\x27\xa7\xdd\xb1\x9e\
+\x05\x46\x63\xa2\x00\xd0\x01\x69\xd4\xb5\x9b\xdd\xfd\xa5\x2e\xb7\
+\x9e\xe2\x61\xa1\x43\x4b\xa5\x31\x37\xbf\x85\xa9\x02\xc0\xcd\x95\
+\x7f\x48\x22\x49\xa3\x6f\x7c\x83\x88\x0a\xbd\x56\x00\x44\x54\x28\
+\x8e\xfa\xb7\x77\x84\xc8\xd1\xcd\x98\x32\x00\xdc\xb8\xfb\x8f\xbb\
+\xed\x65\x16\x96\x72\xc8\xdd\x3f\xd7\xed\xe7\x78\x59\x40\xd4\x26\
+\x69\xdc\x6f\x5e\x26\xd1\x82\x59\x03\xc0\x1d\x41\x3a\xf8\xa2\x1a\
+\x31\xe5\xea\xbf\xb9\x7b\xf7\xd7\x45\x00\x44\x44\xe2\x88\xab\x3e\
+\x10\x87\xcd\xc5\xeb\xc2\x00\xf4\x17\x4b\x30\x49\x13\x17\x3f\xcd\
+\xac\x21\xdb\xf4\xf8\xf1\xfa\xbc\xc9\x23\x48\xf9\xd2\x84\xbb\x9e\
+\x67\x21\x89\x98\x40\x00\xfa\x93\xfa\x8f\xbe\x71\x83\x98\x90\xbd\
+\x4d\xaf\x9f\xaf\xdb\xab\x7c\x42\xf8\xc8\x03\xd2\xc4\xff\x7e\x96\
+\x88\x61\x16\x01\xe8\x4b\x0c\x45\xa4\xb6\x4a\x63\x6f\x7d\xa5\xaf\
+\x97\x7d\x0c\xa8\x00\x88\xa8\x50\x1a\x3e\xef\x63\x71\xc8\xa5\x07\
+\x31\x95\x00\xf4\x3a\x8b\x26\x29\xe3\x77\x6b\x58\x60\xcc\x46\x5d\
+\xff\x18\x5d\x7f\x09\x39\x70\xbb\x9c\x79\xff\x2a\x16\x18\x83\x09\
+\x05\xa0\x37\xa9\xff\xa8\x85\xdb\xc5\x21\xb3\x3f\xd7\xdd\x33\x7a\
+\xff\x01\x2c\x2c\xe5\x90\x74\xe1\x3d\xeb\x51\x0a\x00\xe0\x62\x50\
+\x46\x8e\x6e\x96\x32\x96\xac\xe9\xed\x47\x3e\xbc\x52\x00\x44\x54\
+\x28\x5d\x70\xdd\x5f\xc5\x91\x57\xe7\x61\x6a\x01\x38\xcf\x86\xe9\
+\x17\x46\x52\xe6\x03\xab\x58\xc0\xa0\x4d\x9e\xf8\xf3\x3c\x73\x9f\
+\x17\x13\xf3\xe5\x0b\xef\x5d\x27\x84\xa7\xe0\xeb\xc2\x00\xf4\x94\
+\xfa\x8f\xbd\xf5\x5d\x31\x71\xba\xc7\xbe\xbb\xe1\xb1\x0b\xfd\x58\
+\x48\xd2\x47\xd2\xa4\x87\x1e\xc7\xbd\x01\x00\x9c\x1b\x31\x71\x7a\
+\xa9\x94\x76\xfb\x1f\x49\x87\x03\x3f\x03\x2e\x00\x22\x22\x31\x69\
+\xe6\x26\x29\xed\x8e\xf7\x30\xd5\x00\x9c\xb5\x41\x92\x34\xf9\x91\
+\xe5\x24\xf9\xef\xf0\x68\xbf\xc1\xc3\xbf\x67\xa1\x9c\x76\xc7\x7a\
+\x71\xd8\x95\x85\x98\x72\x00\xbe\x47\x0e\x20\x39\x7b\xe5\x32\x21\
+\x7c\xe4\x01\x4f\xff\xd1\xc2\x00\xfc\xb2\x3b\xe4\xac\xe5\x0f\x0b\
+\x11\xa9\xad\x98\x79\x00\x18\xc9\x13\xee\x7a\x5b\x4c\xbc\x64\xb3\
+\x27\x53\xff\x81\x13\x00\x11\xb1\xc0\xe8\x8d\x72\xd6\xe3\x8f\x30\
+\xff\x48\x33\x4e\xb8\x86\x45\x0f\x7e\x2c\x8b\x53\x16\xe4\x49\xe3\
+\xff\xf3\xe5\x81\x08\xfe\x01\x13\x00\x11\x91\x10\x97\xf5\xa5\x3c\
+\xe9\xc1\xa7\x71\xa5\x38\x20\xc9\xaf\xc3\x8c\xbf\xb6\x10\x35\xb6\
+\x49\x9e\xf4\xd0\x0a\x4f\xd7\xfd\x67\x0c\xfd\x00\xfe\xfe\x85\xe2\
+\xa8\x45\x24\xd9\xcb\x87\x2a\x05\xeb\x17\x98\x63\xca\x39\xa9\x25\
+\x1f\x2d\x64\x21\x89\x99\xc4\x35\x7c\x52\x89\x88\x88\x09\x1a\x6f\
+\x39\x19\x67\xba\x5f\x3b\x24\x91\xe4\x29\x2b\x97\xb1\xc0\xe8\x8d\
+\x03\xfa\xf7\xe0\x9c\x0f\x6c\x48\x74\x36\x4d\x77\xee\x58\xbe\x5a\
+\x3d\xfc\xfe\x64\x44\x03\x30\x45\xf0\xfb\x47\x90\x3c\x63\xfd\x52\
+\x31\x21\x67\xcb\x40\xa5\xfe\x03\x5e\x02\xfc\x38\x18\x56\x5b\xae\
+\x3c\xf9\xa1\x15\x62\xf2\xac\x62\x2c\x0d\x60\xfc\xa2\xdf\x4a\x72\
+\xd6\xf2\x35\xde\x10\xfc\x5e\x21\x80\x2e\x23\x46\x6d\x92\xa7\xac\
+\x5c\x26\x44\x8d\x6b\xc2\x0a\x01\x46\x46\xce\xf8\xdd\x9b\xe2\x88\
+\xab\xde\xf7\x86\xe0\xf7\x1a\x01\x10\x11\xb1\xe0\xf8\x0d\x72\xce\
+\xda\x7b\x99\x2d\x19\xab\x04\x18\x12\x69\xec\x2d\x9b\xa5\xb4\xdb\
+\x5f\xf0\x96\xe0\xf7\x2a\x01\x10\x11\x09\x51\x63\xf7\x5a\x66\xbd\
+\x74\x2b\x0b\x8e\xc7\x6a\x01\xc6\x0a\xfe\xd4\x1b\xb6\x49\x19\x4b\
+\xd7\x10\x13\x0a\xbc\x2a\xe6\xbc\x6c\x9c\x0a\x85\xa8\x71\x7b\x2d\
+\x33\x5f\xb8\x93\xf9\x47\x61\xd5\x00\x63\x94\xfd\x23\xaf\xdd\x25\
+\x65\x2e\x5b\xa9\xd7\xbd\x7e\x46\x12\x40\x97\x04\x62\x32\x76\x59\
+\x66\xbe\x70\x2f\xf3\x0b\xc7\xea\x01\xbe\x1d\xfc\x23\xe6\x17\xc8\
+\x17\x3f\xfa\x28\xf3\x0b\xdf\xea\x8d\x7f\x3f\x6f\x7d\x16\x5d\x28\
+\xc4\x4f\xf9\x52\x9e\xba\x7a\x05\xf3\x0b\xc3\x2a\x02\xbe\x19\xfc\
+\xc3\xae\x28\x92\xb3\x96\x3f\xe4\xad\xc1\x4f\x34\xb0\x07\x81\xce\
+\x2b\x01\x71\xd8\x95\xc4\xac\xb6\x26\xc7\x96\xc5\xcf\xf0\xf6\x53\
+\x58\x51\xc0\xc7\x76\xfe\xc7\x1f\x61\xfe\x91\x9b\xbd\xf9\xef\x39\
+\xe0\x07\x81\x5c\x20\x4d\xab\xca\xcb\x72\x7c\x71\xd7\x8b\xbc\xb5\
+\x1a\x2b\x0b\xf8\x44\xcd\x2f\x5f\xfc\xd8\xa3\xcc\x2f\x6c\xab\xb7\
+\xff\x5d\x7d\x41\x00\x5d\x12\xa8\xde\x93\xe9\xd8\xba\xf8\x4f\xdc\
+\x5e\x81\x15\x06\xbc\x16\x29\xf5\xfa\xed\x52\xe6\x03\x4f\x78\x73\
+\xda\xef\x8b\x02\xe8\x92\x40\x5d\xd1\x04\xc7\xd6\xdf\xfe\x89\x37\
+\x1c\xc1\x77\xc7\x80\xf7\x05\xff\xd8\x5b\x36\x4b\x19\x4b\xd7\x78\
+\x63\xb7\xdf\x08\x02\x20\x22\x22\xed\x74\xc9\x75\xce\xed\x0f\x3e\
+\xa3\x55\xe6\x0d\xc6\x92\x03\xde\x11\xf9\xfe\x24\x67\xdc\xf7\x3f\
+\x52\xda\x1d\xeb\xc9\x8b\x0e\xf9\x18\x52\x00\x44\x44\xbc\xa5\x6a\
+\xae\x73\xe7\x8a\x95\xea\xd1\x4f\xd2\xb0\xfa\xc0\x80\x06\x90\x7f\
+\x24\xc9\x59\x8f\xaf\xf1\xa6\xe3\xbd\x86\x17\x00\x11\x11\xef\x68\
+\x98\xa1\xe4\xad\x7d\x54\x39\xf8\xd7\x1c\x2c\x43\x30\x20\xc1\x13\
+\x92\x48\x72\xf6\x9a\xa5\x62\xe2\xb4\x2d\xbe\x18\xfc\x3e\x2d\x80\
+\xae\x7a\x40\xc9\x50\xf6\xbd\x7a\x97\xb3\xe0\xb9\x9b\xc8\xd9\x86\
+\x15\x09\x3c\x86\x10\x3d\xa1\x5e\xce\x7a\xe2\x41\x21\x7a\x62\xbe\
+\xaf\x06\xbf\xef\x0b\xa0\x8b\x34\xb5\x6c\xe3\x3c\xe7\xae\x55\x4f\
+\xe0\x09\x01\xf0\x04\x62\xca\xd5\x79\xf2\xc5\x8f\x3d\xc6\xfc\x23\
+\x36\xfb\xfa\xef\x62\x04\x01\x10\x7d\xff\x84\xc0\xb9\x73\xe5\x4a\
+\xad\x72\x57\x1c\x96\x28\xd0\x05\x39\x80\xe4\x09\x77\xbe\x2b\x4d\
+\xb8\xeb\x79\x12\x64\x43\x7c\xe9\xca\x28\x02\xe8\xea\x0b\x74\xda\
+\x73\x94\xdd\x6b\x1f\x55\x0e\xbc\x35\x83\x38\xee\xde\x04\x6e\x0c\
+\x14\xdb\x10\x4d\xce\x7a\xfc\x61\x31\x69\xc6\x17\x9e\xf8\x66\x1f\
+\x04\xd0\x9f\xbe\xc0\xfe\x37\x6e\x53\xf6\xfe\xf1\x36\xde\x56\x87\
+\x95\x0b\xfa\x5f\xef\x27\xe4\x94\xc9\x17\x3f\xf6\x98\x10\x3e\xf2\
+\x6d\xc3\x89\xcd\x70\x02\xf8\xa1\x24\xa8\x2d\x4c\x77\x7e\xbd\xe6\
+\x09\xed\xe4\x4e\x94\x04\xa0\x6f\xc1\x61\x09\x26\x69\xfc\x6d\xef\
+\x49\xe3\x6f\x5f\x4f\x72\xc0\x0e\x43\xfe\x8e\x06\x15\x40\x57\x49\
+\xd0\x71\x7a\x86\x52\xf4\xfa\xed\x4a\xd1\x6b\xd7\xe0\x29\x01\xe8\
+\xd5\xae\x3f\x68\x7c\x83\x74\xe1\x7d\xeb\xc4\xa4\x19\x9b\xc8\x87\
+\xbb\xfc\xa6\x16\xc0\x0f\xd9\x80\x7a\xf4\xd3\xab\x9c\xbb\x7f\xff\
+\x10\x6f\x3c\x2a\x61\x69\x83\x9e\x23\x5f\x22\x69\xd4\xc2\xed\x52\
+\xc6\x92\x35\x9e\xfa\x44\x37\x04\xe0\x89\x6c\xa0\xa5\x72\xae\xb2\
+\xef\x95\xbb\x94\x03\x7f\x9d\x43\x6a\x27\x16\x3a\x38\x3b\xf6\x23\
+\xc7\x34\x4b\xe9\x8b\x9f\x16\x93\x67\x7f\x46\x82\x94\x6f\x8a\x32\
+\xc7\x2c\x02\xf8\x31\x1b\xa8\xf8\x72\xa6\xb2\xe7\x99\x07\xb4\x9a\
+\xbd\x11\x58\xf2\x80\x88\x88\xe4\x00\x92\xc6\xdc\xbc\x41\x1a\xfd\
+\x1f\xaf\xb3\xe0\xf8\x0d\x66\xfa\xd5\xcd\x26\x80\xae\x6c\xa0\xb3\
+\x69\xba\xb2\xef\xd5\x3b\xd5\xfd\x6f\x5c\xc3\x3b\x71\x13\xb9\xa9\
+\x77\xfd\xd8\xcc\x2a\x69\xfc\xed\xeb\xc5\xe4\x59\x86\xae\xf5\x21\
+\x80\x73\x64\x03\x5a\xcd\xde\x0c\x65\xdf\x2b\x77\xab\x65\x9f\x8d\
+\x23\xae\x22\x1a\xcc\xb4\xf0\x43\x12\x49\x1a\x7b\xeb\x6b\xe2\xc8\
+\x6b\xdf\x65\x56\x5b\xae\x69\xc7\xc1\xc4\x02\xf8\x3e\x1d\x50\x33\
+\xd4\xb2\x4d\x97\x29\x85\x2f\xdd\xa3\xd5\xee\xc3\x05\x84\x46\x5f\
+\xf0\xd6\x10\x12\x53\xae\xde\x2c\x5e\x70\xc3\x5f\x84\x88\x51\x07\
+\xcc\xb8\xeb\x43\x00\xe7\x2c\x0b\x1a\xa7\xab\xc5\x7f\xbb\x41\x39\
+\xf8\xf6\x2d\xbc\xb1\x0c\x1f\xee\x34\xde\x52\x27\x71\xc8\xa5\x07\
+\xa5\xb4\xdb\xd7\x0b\x31\x17\xe6\x99\x3d\xf0\x21\x80\xee\x44\x60\
+\x2f\x5f\xa0\x1c\xfe\x60\x91\x7a\xf8\xfd\x85\xbc\xf9\x3b\x0c\x88\
+\x11\xea\xfc\x84\x9c\x32\x69\xcc\x4d\xaf\x8b\x49\x33\xbe\x20\x26\
+\xe6\x63\x44\x20\x80\xf3\xf6\x07\xb8\xbd\x22\x59\x39\xf8\xd7\x5b\
+\xd4\xe2\xf7\xe6\xe1\x46\x62\x5f\x5c\xd9\x02\x09\xd1\xe9\x35\x52\
+\xea\x0d\x6f\x8a\x43\xe7\x7c\x4a\x72\xd0\x76\x0c\x0a\x04\xd0\x7b\
+\x11\x34\x96\xa6\x28\x07\xdf\xbe\x49\x2d\xfd\xe4\x72\xdc\x4a\xec\
+\x23\x3b\xfe\xe0\x8b\x6a\xa4\x31\x37\xbf\x26\xc4\x67\x7f\xe9\x0b\
+\x37\xf3\x42\x00\xbe\x20\x82\x86\x92\x0b\xd4\xb2\x8d\x57\x2a\x25\
+\x1f\x2d\x42\x8f\xc0\x0b\x91\x03\x49\x8c\xbb\xb8\x58\x1c\xb9\xf0\
+\x6d\x31\x21\x27\xd7\xa8\x67\xf7\x21\x80\x81\xee\x11\xb4\xd5\xce\
+\x51\x4b\x37\x2c\x50\x4b\x3f\x99\xaf\xd5\x14\xe0\x03\x86\x03\xbd\
+\x80\xad\x21\x24\x0c\x99\xb3\x4b\x1a\xb9\xf0\x6d\x61\x70\xc6\x6e\
+\xd4\xf8\x10\x80\x67\x70\xb6\x65\xa9\x15\x5b\x67\xab\xa5\x1b\x16\
+\x68\x55\x7b\xc6\xf0\x76\xbc\x7a\xec\xd1\xfa\x3e\x7c\x64\xab\x30\
+\xe4\xb2\x7f\x88\x89\xd3\xb7\x08\xd1\x13\x7c\xfa\x5a\x2e\x08\xc0\
+\xa7\x53\x02\x2d\x5d\x3b\xb5\x7f\x9c\x56\xbe\x75\x96\x7a\x7c\xf3\
+\xe5\x5a\xfd\x21\x1b\x69\x0a\xc6\x45\x97\xdd\x3e\x94\x84\xa4\x4b\
+\xf2\xc5\xa4\x99\x9f\x0b\x09\x53\xff\xc9\xac\xa1\xb9\x18\x15\x08\
+\xc0\x7b\x5c\xd0\xd9\x34\x5d\xab\xda\x9d\xa9\x96\x6e\x58\xa0\xd5\
+\x14\x64\xe0\x8e\x42\x77\xd4\xf6\x01\x24\x44\x8d\xad\x12\x62\xb3\
+\xb6\x4b\xc3\xaf\xfc\x98\x85\x8d\x38\x84\xdd\x1e\x02\xf0\x76\xd2\
+\x78\x5b\x6d\x8c\xf6\xdd\x57\x39\x6a\xe5\xae\x2c\xed\xc4\xb6\x6c\
+\xde\x52\x45\x44\x18\x6b\x57\xeb\x7a\x16\x3a\xac\x5e\x4c\x9a\xb1\
+\x59\x48\x9a\xf9\xb9\x10\x3a\xac\x94\x24\x7f\x34\xf5\x20\x00\x1f\
+\x95\x41\x4b\x55\xbc\x56\xb7\x2f\x4d\x3d\xbe\x65\x0e\xaf\x2b\x4c\
+\xd7\xea\x8b\xfd\x30\x2c\xbf\x0c\x7a\x1b\x09\xd1\xe9\xa5\x2c\x6a\
+\x4c\x91\x98\x34\x73\x13\x0b\x1b\x51\xc2\x2c\xc1\xdb\x30\x32\x10\
+\x80\xe1\xca\x04\x5e\xb7\x6f\x82\x56\xb3\x77\xa2\x7a\x72\x67\x36\
+\x6f\x38\x92\xc8\xdb\x6a\x4d\x98\xda\x07\x12\x0b\x1c\xac\x88\xb1\
+\x17\xed\x12\xa2\x27\xe6\x0b\x31\x17\xe6\xb1\x90\xe4\x63\x66\x79\
+\x0f\x1f\x02\x00\x44\x9a\x92\xc1\x9b\x4f\x24\x69\x4d\xc7\x87\x6a\
+\x55\x79\x93\x79\xe3\xd1\xe1\x5a\x6d\xd1\x18\xde\x56\x4b\xa4\x39\
+\x8d\xb4\xcc\xba\x6a\xf9\xb0\x11\x0d\x42\x64\xea\x7e\x16\x35\xbe\
+\x40\x88\x1a\x57\xc4\x82\xe3\x2a\x7c\xe5\x2b\xba\x10\x00\xf0\x50\
+\xb9\x50\x19\xcf\xed\x15\x49\xda\xe9\x43\xa3\xb5\xda\xa2\x34\x6e\
+\x2f\x1f\xca\x5b\xab\xa3\x79\x4b\x25\xf9\xca\xd3\x05\xe6\x17\x46\
+\x2c\x70\x70\x2b\x05\x44\xd5\x08\xe1\x23\x8b\x85\xe8\xf4\x3c\x16\
+\x3a\xe4\x98\x10\x96\x52\x8c\x1d\x1e\x02\x00\xbd\x41\x69\xcf\xe2\
+\x9d\x76\x1b\x6f\xa9\x8c\xd3\x4e\x7d\x3b\x9e\xb7\x54\xc6\xf1\xd6\
+\x9a\x68\x6a\xab\x8d\xe6\xad\xd5\xb1\xbc\xb5\xc6\x8f\x6b\x0a\x91\
+\xd2\x4e\x1e\xbb\xd3\x40\xb4\x10\x93\xfc\x88\x04\x2b\xb1\x90\xf8\
+\x7a\x16\x10\x5d\xc3\x02\x63\xaa\x58\x60\x4c\x25\x0b\x1b\x5e\x22\
+\x84\x8f\x3a\x48\x7e\xa1\x0d\x78\x4c\x07\x01\x00\x3d\x51\x3b\x27\
+\x6b\x4d\xc7\x87\x92\xb3\x35\x80\xb7\xd7\x47\x90\xa3\xd9\xc6\x95\
+\xb6\x00\x5e\x5f\x3c\x9a\x37\x9f\x48\xe0\xce\xd6\x60\xea\xb4\x87\
+\x70\x67\x6b\x60\xd7\xad\xc8\x1a\x11\xd7\x88\x3b\x9a\x7f\x4a\xcd\
+\xbb\x3a\x13\x44\xa2\x95\x98\xe4\x4f\xc4\x35\x22\xc9\x4a\x24\x05\
+\x2a\xcc\x12\xd4\x4c\x56\x5b\x03\xb3\x04\xb7\x08\xd1\x13\xf2\x99\
+\xd5\xd6\x44\x72\x50\x0b\xb3\xda\x9a\xc8\x2f\xbc\x9e\xc9\x01\xad\
+\x2c\x38\xa1\x1c\xbb\x3a\x04\x00\xbc\x14\xee\x68\xce\x21\xcd\x29\
+\x91\xa6\xca\x44\x9c\x88\x73\x81\x34\xe7\xd9\xb7\x23\x33\x41\x23\
+\x41\x52\x7e\xf6\xbf\x9d\xd8\xc1\x21\x00\x00\x80\x81\xc1\x5b\x6d\
+\x00\x40\x00\x00\x00\x33\xf2\x7f\x03\x00\xf8\x9c\x68\x4d\x99\x9a\
+\x06\x90\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
+"
+
+qt_resource_name = b"\
+\x00\x06\
+\x07\x03\x7d\xc3\
+\x00\x69\
+\x00\x6d\x00\x61\x00\x67\x00\x65\x00\x73\
+\x00\x0a\
+\x05\x78\xd9\x27\
+\x00\x75\
+\x00\x70\x00\x6c\x00\x6f\x00\x61\x00\x64\x00\x2e\x00\x70\x00\x6e\x00\x67\
+"
+
+qt_resource_struct = b"\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
+\x00\x00\x00\x12\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+"
+
+def qInitResources():
+    QtCore.qRegisterResourceData(0x01, qt_resource_struct, qt_resource_name, qt_resource_data)
+
+def qCleanupResources():
+    QtCore.qUnregisterResourceData(0x01, qt_resource_struct, qt_resource_name, qt_resource_data)
+
+qInitResources()
```

### Comparing `deriva-qt-1.6.1/deriva/qt/upload_gui/ui/options_window.py` & `deriva-qt-1.6.3/deriva/qt/upload_gui/ui/options_window.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,412 +1,412 @@
-import os
-import re
-import logging
-from PyQt5.QtCore import Qt, pyqtSlot
-from PyQt5.QtWidgets import QDialog, QVBoxLayout, QHBoxLayout, QLabel, QLineEdit, QPushButton, QFileDialog, \
-    QGroupBox, QRadioButton, QComboBox, QCheckBox, QMessageBox, QDialogButtonBox, QSpinBox, qApp
-from deriva.core import stob, DEFAULT_SESSION_CONFIG
-from deriva.transfer import GenericUploader
-from deriva.qt import JSONEditor
-
-
-def warningMessageBox(parent, text, detail):
-    msg = QMessageBox(parent)
-    msg.setIcon(QMessageBox.Warning)
-    msg.setWindowTitle("Attention Required")
-    msg.setText(text)
-    msg.setInformativeText(detail)
-    msg.exec_()
-
-
-def getServerDisplayName(server):
-    host = server.get("host", "")
-    desc = server.get("desc", "")
-    display_name = ("%s" % "https://" + host) if not desc else ("%s: %s" % (desc, "https://" + host))
-    return display_name
-
-
-class OptionsDialog(QDialog):
-    def __init__(self, parent):
-        super(OptionsDialog, self).__init__(parent)
-        self.reconfigure = False
-        self.setWindowTitle("Options")
-        self.setWindowFlags(self.windowFlags() & ~Qt.WindowContextHelpButtonHint)
-        self.setMinimumWidth(600)
-        layout = QVBoxLayout(self)
-        layout.addStretch(1)
-
-        # Servers
-        setServers = getattr(parent.uploader, "setServers", None)
-        self.serversConfigurable = True if callable(setServers) else False
-        self.serversGroupBox = QGroupBox("Servers:", self)
-        self.serverLayout = QHBoxLayout()
-        self.serverLabel = QLabel("Server:")
-        self.serverLayout.addWidget(self.serverLabel)
-        self.serverComboBox = QComboBox()
-        self.serverComboBox.setEditable(False)
-        self.serverComboBox.setMinimumContentsLength(50)
-        self.serverComboBox.currentIndexChanged.connect(self.onServerChanged)
-        self.serverLayout.addWidget(self.serverComboBox)
-        self.serverLayout.addStretch(1)
-        self.addServerButton = QPushButton("Add", parent)
-        self.addServerButton.clicked.connect(self.onServerAdd)
-        self.addServerButton.setEnabled(self.serversConfigurable)
-        self.serverLayout.addWidget(self.addServerButton)
-        self.editServerButton = QPushButton("Edit", parent)
-        self.editServerButton.clicked.connect(self.onServerEdit)
-        self.editServerButton.setEnabled(self.serversConfigurable)
-        self.serverLayout.addWidget(self.editServerButton)
-        self.removeServerButton = QPushButton("Remove", parent)
-        self.removeServerButton.clicked.connect(self.onServerRemove)
-        self.removeServerButton.setEnabled(self.serversConfigurable)
-        self.serverLayout.addWidget(self.removeServerButton)
-        self.serversGroupBox.setLayout(self.serverLayout)
-        layout.addWidget(self.serversGroupBox)
-
-        # Configuration
-        self.configurable = isinstance(parent.uploader, GenericUploader)
-        self.configGroupBox = QGroupBox("Configuration:", self)
-        self.configLayout = QHBoxLayout()
-        self.configPathLabel = QLabel("File:")
-        self.configLayout.addWidget(self.configPathLabel)
-        self.configPathTextBox = QLineEdit()
-        self.configPathTextBox.setReadOnly(True)
-        self.configPathTextBox.setText(os.path.normpath(parent.uploader.getCurrentConfigFilePath()))
-        self.configLayout.addWidget(self.configPathTextBox)
-        self.configBrowseButton = QPushButton("Change", parent)
-        self.configBrowseButton.clicked.connect(self.onConfigChange)
-        self.configBrowseButton.setEnabled(self.configurable)
-        self.configLayout.addWidget(self.configBrowseButton)
-        self.configEditButton = QPushButton("Edit", parent)
-        self.configEditButton.clicked.connect(self.onConfigEdit)
-        self.configEditButton.setEnabled(self.configurable)
-        self.configLayout.addWidget(self.configEditButton)
-        self.configGroupBox.setLayout(self.configLayout)
-        layout.addWidget(self.configGroupBox)
-
-        # Upload
-        # self.uploadGroupBox = QGroupBox("Upload:", self)
-        # self.uploadLayout = QHBoxLayout()
-        # self.uploadAllButton = QRadioButton("Files and Data")
-        # self.uploadAllButton.setChecked(True)
-        # self.uploadLayout.addWidget(self.uploadAllButton)
-        # self.uploadFilesButton = QRadioButton("Files only")
-        # self.uploadLayout.addWidget(self.uploadFilesButton)
-        # self.uploadDataButton = QRadioButton("Data only")
-        # self.uploadLayout.addWidget(self.uploadDataButton)
-        # self.uploadGroupBox.setLayout(self.uploadLayout)
-        # layout.addWidget(self.uploadGroupBox)
-
-        # Miscellaneous
-        self.miscGroupBox = QGroupBox("Miscellaneous:", self)
-        self.miscLayout = QHBoxLayout()
-        self.debugCheckBox = QCheckBox("Debug logging")
-        self.debugCheckBox.setChecked(True if logging.getLogger().getEffectiveLevel() == logging.DEBUG else False)
-        self.miscLayout.addWidget(self.debugCheckBox)
-        self.miscGroupBox.setLayout(self.miscLayout)
-        layout.addWidget(self.miscGroupBox)
-
-        # Button Box
-        self.buttonBox = QDialogButtonBox(parent)
-        self.buttonBox.setObjectName("buttonBox")
-        self.buttonBox.setOrientation(Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel|QDialogButtonBox.Ok)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        layout.addWidget(self.buttonBox)
-
-        self.populateServers()
-
-    @pyqtSlot()
-    def onConfigChange(self):
-        uploader = self.parent().uploader
-        current_path = os.path.normpath(self.configPathTextBox.text())
-        new_path = QFileDialog.getOpenFileName(self,
-                                               "Select Configuration File",
-                                               current_path,
-                                               "Configuration Files (*.json)")
-        if new_path[0]:
-            new_path = os.path.normpath(new_path[0])
-            if new_path != current_path:
-                self.configPathTextBox.setText(new_path)
-                if new_path != uploader.getDefaultConfigFilePath():
-                    uploader.override_config_file = new_path
-                else:
-                    uploader.override_config_file = None
-                self.reconfigure = True
-            else:
-                self.reconfigure = False
-
-    @pyqtSlot()
-    def onConfigEdit(self):
-        uploader = self.parent().uploader
-        configEditor = JSONEditor(self, self.configPathTextBox.text(), "Configuration Editor")
-        configEditor.exec_()
-        if configEditor.isModified():
-            path = self.configPathTextBox.text()
-            uploader.override_config_file = path
-            self.reconfigure = True
-        del configEditor
-
-    @pyqtSlot()
-    def onServerAdd(self):
-        server = ServerDialog.configureServer(self.parent(), {})
-        if not server:
-            return
-        hostname = server.get("host")
-        index = self.serverComboBox.findText(hostname, Qt.MatchExactly)
-        if index > -1:
-            warningMessageBox(self.parent(), "Server already exists!",
-                              "A server configuration for this hostname already exists. "
-                              "Please edit that configuration directly if you wish to make changes to it.")
-            return
-        else:
-            index = self.serverComboBox.count()
-            self.serverComboBox.insertItem(index, getServerDisplayName(server), server)
-
-        self.updateDefaultServer(index)
-        self.editServerButton.setEnabled(self.serversConfigurable)
-
-    @pyqtSlot()
-    def onServerEdit(self):
-        index = self.serverComboBox.currentIndex()
-        server = self.serverComboBox.itemData(index, Qt.UserRole)
-        server = ServerDialog.configureServer(self.parent(), server if server else {})
-        if not server:
-            return
-        self.serverComboBox.setItemData(index, server, Qt.UserRole)
-        self.updateDefaultServer(index)
-
-    @pyqtSlot()
-    def onServerRemove(self):
-        index = self.serverComboBox.currentIndex()
-        self.serverComboBox.removeItem(index)
-        for x in range(self.serverComboBox.count()):
-            current = self.serverComboBox.itemData(x, Qt.UserRole)
-            if current["default"] is True:
-                self.serverComboBox.setCurrentIndex(x)
-
-    @pyqtSlot()
-    def onServerChanged(self):
-        uploader = self.parent().uploader
-        if not uploader.override_config_file:
-            server = self.serverComboBox.currentData(Qt.UserRole)
-            if not server:
-                return
-            config_file = os.path.normpath(os.path.join(
-                uploader.getDeployedConfigPath(), server.get('host', ''), uploader.DefaultConfigFileName))
-            self.configPathTextBox.setText(config_file)
-            if not (os.path.exists(config_file) and os.path.isfile(config_file)):
-                self.configEditButton.setEnabled(False)
-            elif self.configurable:
-                self.configEditButton.setEnabled(True)
-
-    def updateDefaultServer(self, index):
-        new = self.serverComboBox.itemData(index, Qt.UserRole)
-        if not new.get("default", False):
-            return
-        else:
-            self.serverComboBox.removeItem(index)
-            self.serverComboBox.insertItem(0, getServerDisplayName(new), new)
-            self.serverComboBox.setCurrentIndex(0)
-
-        for x in range(self.serverComboBox.count()):
-            current = self.serverComboBox.itemData(x, Qt.UserRole)
-            if new.get("host") != current.get("host"):
-                current["default"] = False
-
-    def populateServers(self):
-        uploader = self.parent().uploader
-        servers = uploader.getServers()
-        if not servers:
-            self.editServerButton.setEnabled(False)
-            return
-        else:
-            index = 0
-            for server in servers:
-                self.serverComboBox.insertItem(index, getServerDisplayName(server), server)
-                if server == uploader.server:
-                    self.serverComboBox.setCurrentIndex(index)
-                elif not uploader.server and server.get("default", False):
-                    self.serverComboBox.setCurrentIndex(index)
-                index += 1
-            self.editServerButton.setEnabled(self.serversConfigurable)
-
-    def getServers(self):
-        servers = list()
-        for x in range(self.serverComboBox.count()):
-            servers.append(self.serverComboBox.itemData(x, Qt.UserRole))
-        return servers
-
-    @staticmethod
-    def getOptions(parent):
-        uploader = parent.uploader
-        dialog = OptionsDialog(parent)
-        ret = dialog.exec_()
-        if QDialog.Accepted == ret:
-            debug = dialog.debugCheckBox.isChecked()
-            logging.getLogger().setLevel(logging.DEBUG if debug else logging.INFO)
-            setServers = getattr(uploader, "setServers", None)
-            if callable(setServers):
-                setServers(dialog.getServers())
-            current_server = dialog.serverComboBox.currentData(Qt.UserRole)
-            if current_server != uploader.server:
-                parent.onServerChanged(current_server)
-                return
-            if dialog.reconfigure:
-                qApp.setOverrideCursor(Qt.WaitCursor)
-                uploader.initialize(cleanup=False)
-                qApp.restoreOverrideCursor()
-                parent.checkVersion()
-        del dialog
-
-
-class ServerDialog(QDialog):
-    def __init__(self, parent, server):
-        super(ServerDialog, self).__init__(parent)
-        self.server = server
-        self.session_config = self.server.get('session', DEFAULT_SESSION_CONFIG.copy())
-        self.setWindowTitle("Server Configuration")
-        self.setWindowFlags(self.windowFlags() & ~Qt.WindowContextHelpButtonHint)
-        self.setMinimumWidth(400)
-        layout = QVBoxLayout(self)
-
-        self.serverLayout = QVBoxLayout(self)
-        self.serverGroupBox = QGroupBox("Server:", self)
-        self.hostnameLayout = QHBoxLayout()
-        self.hostnameLabel = QLabel("Host:")
-        self.hostnameLayout.addWidget(self.hostnameLabel)
-        self.hostnameTextBox = QLineEdit()
-        self.hostnameTextBox.setText(server.get("host", ""))
-        self.hostnameLayout.addWidget(self.hostnameTextBox)
-        self.serverLayout.addLayout(self.hostnameLayout)
-
-        self.descriptionLayout = QHBoxLayout()
-        self.descriptionLabel = QLabel("Description:")
-        self.descriptionLayout.addWidget(self.descriptionLabel)
-        self.descriptionTextBox = QLineEdit()
-        self.descriptionTextBox.setText(server.get("desc", ""))
-        self.descriptionLayout.addWidget(self.descriptionTextBox)
-        self.serverLayout.addLayout(self.descriptionLayout)
-
-        self.catalogIDLayout = QHBoxLayout()
-        self.catalogIDLabel = QLabel("Catalog ID:")
-        self.catalogIDLayout.addWidget(self.catalogIDLabel)
-        self.catalogIDTextBox = QLineEdit()
-        self.catalogIDTextBox.setText(str(server.get("catalog_id", 1)))
-        self.catalogIDLayout.addWidget(self.catalogIDTextBox)
-        self.serverLayout.addLayout(self.catalogIDLayout)
-        self.serverGroupBox.setLayout(self.serverLayout)
-        layout.addWidget(self.serverGroupBox)
-
-        # connect timeout/retry settings
-        self.serverConnectTimeoutsGroupBox = QGroupBox("Connection Timeout and Retries:", self)
-        self.connectLayout = QHBoxLayout()
-        # connect timeout
-        self.connectTimeoutLabel = QLabel("Connect timeout (secs):")
-        self.connectLayout.addWidget(self.connectTimeoutLabel)
-        self.connectTimeoutSpinBox = QSpinBox(parent)
-        self.connectTimeoutSpinBox.setRange(1, 60)
-        self.connectTimeoutSpinBox.setValue(self.session_config.get("timeout")[0] or 6)
-        self.connectLayout.addWidget(self.connectTimeoutSpinBox)
-        # connect retry
-        self.connectRetryLabel = QLabel("Connect retries:")
-        self.connectLayout.addWidget(self.connectRetryLabel)
-        self.connectRetrySpinBox = QSpinBox(parent)
-        self.connectRetrySpinBox.setRange(1, 60)
-        self.connectRetrySpinBox.setValue(self.session_config.get("retry_connect", 10))
-        self.connectLayout.addWidget(self.connectRetrySpinBox)
-        self.serverConnectTimeoutsGroupBox.setLayout(self.connectLayout)
-        layout.addWidget(self.serverConnectTimeoutsGroupBox)
-
-        # io timeout/retry settings
-        self.serverIOTimeoutsGroupBox = QGroupBox("I/O Timeout and Retries:", self)
-        self.ioLayout = QHBoxLayout()
-        # io timeout
-        self.ioTimeoutLabel = QLabel("I/O timeout (secs):")
-        self.ioLayout.addWidget(self.ioTimeoutLabel)
-        self.ioTimeoutSpinBox = QSpinBox(parent)
-        self.ioTimeoutSpinBox.setRange(1, 600)
-        self.ioTimeoutSpinBox.setValue(self.session_config.get("timeout")[1] or 60)
-        self.ioLayout.addWidget(self.ioTimeoutSpinBox)
-        # io retry
-        self.ioRetryLabel = QLabel("I/O retries:")
-        self.ioLayout.addWidget(self.ioRetryLabel)
-        self.ioRetrySpinBox = QSpinBox(parent)
-        self.ioRetrySpinBox.setRange(1, 60)
-        self.ioRetrySpinBox.setValue(self.session_config.get("retry_read", 10))
-        self.ioLayout.addWidget(self.ioRetrySpinBox)
-        self.serverIOTimeoutsGroupBox.setLayout(self.ioLayout)
-        layout.addWidget(self.serverIOTimeoutsGroupBox)
-
-        setServers = getattr(parent.uploader, "setServers", None)
-        self.serversConfigurable = True if callable(setServers) else False
-        self.serverOptionsGroupBox = QGroupBox("Options:", self)
-        self.checkboxLayout = QHBoxLayout()
-        self.defaultServer = QCheckBox("Set as &Default", parent)
-        self.defaultServer.setChecked(stob(server.get("default", False)))
-        self.defaultServer.setEnabled(self.serversConfigurable)
-        self.checkboxLayout.addWidget(self.defaultServer)
-        self.confirm_updates = QCheckBox("&Confirm configuration updates", parent)
-        self.confirm_updates.setChecked(stob(server.get("confirm_updates", False)))
-        self.confirm_updates.setEnabled(self.serversConfigurable)
-        self.checkboxLayout.addWidget(self.confirm_updates)
-
-        self.cookie_persistence = QCheckBox("&Stay logged in", parent)
-        allow_session_caching = True
-        if parent.uploader.config:
-            client_settings = parent.uploader.config.get("client_settings")
-            if client_settings:
-                allow_session_caching = stob(client_settings.get("allow_session_caching", True))
-                if not allow_session_caching:
-                    server["cookie_persistence"] = False
-        self.cookie_persistence.setChecked(stob(server.get("cookie_persistence", False)))
-        self.cookie_persistence.setEnabled(self.serversConfigurable and allow_session_caching)
-        self.checkboxLayout.addWidget(self.cookie_persistence)
-        self.serverOptionsGroupBox.setLayout(self.checkboxLayout)
-        layout.addWidget(self.serverOptionsGroupBox)
-
-        # Button Box
-        self.buttonBox = QDialogButtonBox(parent)
-        self.buttonBox.setObjectName("buttonBox")
-        self.buttonBox.setOrientation(Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel | QDialogButtonBox.Ok)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        layout.addWidget(self.buttonBox)
-
-    def validate(self):
-        host = self.hostnameTextBox.text()
-        hostname = re.sub("(?i)^.*https?://", '', host)
-        if not hostname:
-            warningMessageBox(self.parent(), "Please enter a valid hostname:",
-                              "For example: \'www.host.com\' or \'localhost\', etc.")
-            return False
-        else:
-            self.server["host"] = hostname
-
-        self.server["default"] = self.defaultServer.isChecked()
-        self.server["confirm_updates"] = self.confirm_updates.isChecked()
-        self.server["cookie_persistence"] = self.cookie_persistence.isChecked()
-
-        desc = self.descriptionTextBox.text()
-        self.server["desc"] = desc if desc else ""
-
-        catalog_id = int(self.catalogIDTextBox.text())
-        self.server["catalog_id"] = catalog_id if catalog_id else 1
-
-        self.session_config["timeout"] = (self.connectTimeoutSpinBox.value(), self.ioTimeoutSpinBox.value())
-        self.session_config["retry_connect"] = self.connectRetrySpinBox.value()
-        self.session_config["retry_read"] = self.ioRetrySpinBox.value()
-        self.server["session"] = self.session_config
-
-        return True
-
-    @staticmethod
-    def configureServer(parent, server):
-        dialog = ServerDialog(parent, server)
-        ret = dialog.exec_()
-        if QDialog.Accepted == ret:
-            if dialog.validate():
-                return dialog.server.copy()
-        return None
+import os
+import re
+import logging
+from PyQt5.QtCore import Qt, pyqtSlot
+from PyQt5.QtWidgets import QDialog, QVBoxLayout, QHBoxLayout, QLabel, QLineEdit, QPushButton, QFileDialog, \
+    QGroupBox, QRadioButton, QComboBox, QCheckBox, QMessageBox, QDialogButtonBox, QSpinBox, qApp
+from deriva.core import stob, DEFAULT_SESSION_CONFIG
+from deriva.transfer import GenericUploader
+from deriva.qt import JSONEditor
+
+
+def warningMessageBox(parent, text, detail):
+    msg = QMessageBox(parent)
+    msg.setIcon(QMessageBox.Warning)
+    msg.setWindowTitle("Attention Required")
+    msg.setText(text)
+    msg.setInformativeText(detail)
+    msg.exec_()
+
+
+def getServerDisplayName(server):
+    host = server.get("host", "")
+    desc = server.get("desc", "")
+    display_name = ("%s" % "https://" + host) if not desc else ("%s: %s" % (desc, "https://" + host))
+    return display_name
+
+
+class OptionsDialog(QDialog):
+    def __init__(self, parent):
+        super(OptionsDialog, self).__init__(parent)
+        self.reconfigure = False
+        self.setWindowTitle("Options")
+        self.setWindowFlags(self.windowFlags() & ~Qt.WindowContextHelpButtonHint)
+        self.setMinimumWidth(600)
+        layout = QVBoxLayout(self)
+        layout.addStretch(1)
+
+        # Servers
+        setServers = getattr(parent.uploader, "setServers", None)
+        self.serversConfigurable = True if callable(setServers) else False
+        self.serversGroupBox = QGroupBox("Servers:", self)
+        self.serverLayout = QHBoxLayout()
+        self.serverLabel = QLabel("Server:")
+        self.serverLayout.addWidget(self.serverLabel)
+        self.serverComboBox = QComboBox()
+        self.serverComboBox.setEditable(False)
+        self.serverComboBox.setMinimumContentsLength(50)
+        self.serverComboBox.currentIndexChanged.connect(self.onServerChanged)
+        self.serverLayout.addWidget(self.serverComboBox)
+        self.serverLayout.addStretch(1)
+        self.addServerButton = QPushButton("Add", parent)
+        self.addServerButton.clicked.connect(self.onServerAdd)
+        self.addServerButton.setEnabled(self.serversConfigurable)
+        self.serverLayout.addWidget(self.addServerButton)
+        self.editServerButton = QPushButton("Edit", parent)
+        self.editServerButton.clicked.connect(self.onServerEdit)
+        self.editServerButton.setEnabled(self.serversConfigurable)
+        self.serverLayout.addWidget(self.editServerButton)
+        self.removeServerButton = QPushButton("Remove", parent)
+        self.removeServerButton.clicked.connect(self.onServerRemove)
+        self.removeServerButton.setEnabled(self.serversConfigurable)
+        self.serverLayout.addWidget(self.removeServerButton)
+        self.serversGroupBox.setLayout(self.serverLayout)
+        layout.addWidget(self.serversGroupBox)
+
+        # Configuration
+        self.configurable = isinstance(parent.uploader, GenericUploader)
+        self.configGroupBox = QGroupBox("Configuration:", self)
+        self.configLayout = QHBoxLayout()
+        self.configPathLabel = QLabel("File:")
+        self.configLayout.addWidget(self.configPathLabel)
+        self.configPathTextBox = QLineEdit()
+        self.configPathTextBox.setReadOnly(True)
+        self.configPathTextBox.setText(os.path.normpath(parent.uploader.getCurrentConfigFilePath()))
+        self.configLayout.addWidget(self.configPathTextBox)
+        self.configBrowseButton = QPushButton("Change", parent)
+        self.configBrowseButton.clicked.connect(self.onConfigChange)
+        self.configBrowseButton.setEnabled(self.configurable)
+        self.configLayout.addWidget(self.configBrowseButton)
+        self.configEditButton = QPushButton("Edit", parent)
+        self.configEditButton.clicked.connect(self.onConfigEdit)
+        self.configEditButton.setEnabled(self.configurable)
+        self.configLayout.addWidget(self.configEditButton)
+        self.configGroupBox.setLayout(self.configLayout)
+        layout.addWidget(self.configGroupBox)
+
+        # Upload
+        # self.uploadGroupBox = QGroupBox("Upload:", self)
+        # self.uploadLayout = QHBoxLayout()
+        # self.uploadAllButton = QRadioButton("Files and Data")
+        # self.uploadAllButton.setChecked(True)
+        # self.uploadLayout.addWidget(self.uploadAllButton)
+        # self.uploadFilesButton = QRadioButton("Files only")
+        # self.uploadLayout.addWidget(self.uploadFilesButton)
+        # self.uploadDataButton = QRadioButton("Data only")
+        # self.uploadLayout.addWidget(self.uploadDataButton)
+        # self.uploadGroupBox.setLayout(self.uploadLayout)
+        # layout.addWidget(self.uploadGroupBox)
+
+        # Miscellaneous
+        self.miscGroupBox = QGroupBox("Miscellaneous:", self)
+        self.miscLayout = QHBoxLayout()
+        self.debugCheckBox = QCheckBox("Debug logging")
+        self.debugCheckBox.setChecked(True if logging.getLogger().getEffectiveLevel() == logging.DEBUG else False)
+        self.miscLayout.addWidget(self.debugCheckBox)
+        self.miscGroupBox.setLayout(self.miscLayout)
+        layout.addWidget(self.miscGroupBox)
+
+        # Button Box
+        self.buttonBox = QDialogButtonBox(parent)
+        self.buttonBox.setObjectName("buttonBox")
+        self.buttonBox.setOrientation(Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel|QDialogButtonBox.Ok)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        layout.addWidget(self.buttonBox)
+
+        self.populateServers()
+
+    @pyqtSlot()
+    def onConfigChange(self):
+        uploader = self.parent().uploader
+        current_path = os.path.normpath(self.configPathTextBox.text())
+        new_path = QFileDialog.getOpenFileName(self,
+                                               "Select Configuration File",
+                                               current_path,
+                                               "Configuration Files (*.json)")
+        if new_path[0]:
+            new_path = os.path.normpath(new_path[0])
+            if new_path != current_path:
+                self.configPathTextBox.setText(new_path)
+                if new_path != uploader.getDefaultConfigFilePath():
+                    uploader.override_config_file = new_path
+                else:
+                    uploader.override_config_file = None
+                self.reconfigure = True
+            else:
+                self.reconfigure = False
+
+    @pyqtSlot()
+    def onConfigEdit(self):
+        uploader = self.parent().uploader
+        configEditor = JSONEditor(self, self.configPathTextBox.text(), "Configuration Editor")
+        configEditor.exec_()
+        if configEditor.isModified():
+            path = self.configPathTextBox.text()
+            uploader.override_config_file = path
+            self.reconfigure = True
+        del configEditor
+
+    @pyqtSlot()
+    def onServerAdd(self):
+        server = ServerDialog.configureServer(self.parent(), {})
+        if not server:
+            return
+        hostname = server.get("host")
+        index = self.serverComboBox.findText(hostname, Qt.MatchExactly)
+        if index > -1:
+            warningMessageBox(self.parent(), "Server already exists!",
+                              "A server configuration for this hostname already exists. "
+                              "Please edit that configuration directly if you wish to make changes to it.")
+            return
+        else:
+            index = self.serverComboBox.count()
+            self.serverComboBox.insertItem(index, getServerDisplayName(server), server)
+
+        self.updateDefaultServer(index)
+        self.editServerButton.setEnabled(self.serversConfigurable)
+
+    @pyqtSlot()
+    def onServerEdit(self):
+        index = self.serverComboBox.currentIndex()
+        server = self.serverComboBox.itemData(index, Qt.UserRole)
+        server = ServerDialog.configureServer(self.parent(), server if server else {})
+        if not server:
+            return
+        self.serverComboBox.setItemData(index, server, Qt.UserRole)
+        self.updateDefaultServer(index)
+
+    @pyqtSlot()
+    def onServerRemove(self):
+        index = self.serverComboBox.currentIndex()
+        self.serverComboBox.removeItem(index)
+        for x in range(self.serverComboBox.count()):
+            current = self.serverComboBox.itemData(x, Qt.UserRole)
+            if current["default"] is True:
+                self.serverComboBox.setCurrentIndex(x)
+
+    @pyqtSlot()
+    def onServerChanged(self):
+        uploader = self.parent().uploader
+        if not uploader.override_config_file:
+            server = self.serverComboBox.currentData(Qt.UserRole)
+            if not server:
+                return
+            config_file = os.path.normpath(os.path.join(
+                uploader.getDeployedConfigPath(), server.get('host', ''), uploader.DefaultConfigFileName))
+            self.configPathTextBox.setText(config_file)
+            if not (os.path.exists(config_file) and os.path.isfile(config_file)):
+                self.configEditButton.setEnabled(False)
+            elif self.configurable:
+                self.configEditButton.setEnabled(True)
+
+    def updateDefaultServer(self, index):
+        new = self.serverComboBox.itemData(index, Qt.UserRole)
+        if not new.get("default", False):
+            return
+        else:
+            self.serverComboBox.removeItem(index)
+            self.serverComboBox.insertItem(0, getServerDisplayName(new), new)
+            self.serverComboBox.setCurrentIndex(0)
+
+        for x in range(self.serverComboBox.count()):
+            current = self.serverComboBox.itemData(x, Qt.UserRole)
+            if new.get("host") != current.get("host"):
+                current["default"] = False
+
+    def populateServers(self):
+        uploader = self.parent().uploader
+        servers = uploader.getServers()
+        if not servers:
+            self.editServerButton.setEnabled(False)
+            return
+        else:
+            index = 0
+            for server in servers:
+                self.serverComboBox.insertItem(index, getServerDisplayName(server), server)
+                if server == uploader.server:
+                    self.serverComboBox.setCurrentIndex(index)
+                elif not uploader.server and server.get("default", False):
+                    self.serverComboBox.setCurrentIndex(index)
+                index += 1
+            self.editServerButton.setEnabled(self.serversConfigurable)
+
+    def getServers(self):
+        servers = list()
+        for x in range(self.serverComboBox.count()):
+            servers.append(self.serverComboBox.itemData(x, Qt.UserRole))
+        return servers
+
+    @staticmethod
+    def getOptions(parent):
+        uploader = parent.uploader
+        dialog = OptionsDialog(parent)
+        ret = dialog.exec_()
+        if QDialog.Accepted == ret:
+            debug = dialog.debugCheckBox.isChecked()
+            logging.getLogger().setLevel(logging.DEBUG if debug else logging.INFO)
+            setServers = getattr(uploader, "setServers", None)
+            if callable(setServers):
+                setServers(dialog.getServers())
+            current_server = dialog.serverComboBox.currentData(Qt.UserRole)
+            if current_server != uploader.server:
+                parent.onServerChanged(current_server)
+                return
+            if dialog.reconfigure:
+                qApp.setOverrideCursor(Qt.WaitCursor)
+                uploader.initialize(cleanup=False)
+                qApp.restoreOverrideCursor()
+                parent.checkVersion()
+        del dialog
+
+
+class ServerDialog(QDialog):
+    def __init__(self, parent, server):
+        super(ServerDialog, self).__init__(parent)
+        self.server = server
+        self.session_config = self.server.get('session', DEFAULT_SESSION_CONFIG.copy())
+        self.setWindowTitle("Server Configuration")
+        self.setWindowFlags(self.windowFlags() & ~Qt.WindowContextHelpButtonHint)
+        self.setMinimumWidth(400)
+        layout = QVBoxLayout(self)
+
+        self.serverLayout = QVBoxLayout(self)
+        self.serverGroupBox = QGroupBox("Server:", self)
+        self.hostnameLayout = QHBoxLayout()
+        self.hostnameLabel = QLabel("Host:")
+        self.hostnameLayout.addWidget(self.hostnameLabel)
+        self.hostnameTextBox = QLineEdit()
+        self.hostnameTextBox.setText(server.get("host", ""))
+        self.hostnameLayout.addWidget(self.hostnameTextBox)
+        self.serverLayout.addLayout(self.hostnameLayout)
+
+        self.descriptionLayout = QHBoxLayout()
+        self.descriptionLabel = QLabel("Description:")
+        self.descriptionLayout.addWidget(self.descriptionLabel)
+        self.descriptionTextBox = QLineEdit()
+        self.descriptionTextBox.setText(server.get("desc", ""))
+        self.descriptionLayout.addWidget(self.descriptionTextBox)
+        self.serverLayout.addLayout(self.descriptionLayout)
+
+        self.catalogIDLayout = QHBoxLayout()
+        self.catalogIDLabel = QLabel("Catalog ID:")
+        self.catalogIDLayout.addWidget(self.catalogIDLabel)
+        self.catalogIDTextBox = QLineEdit()
+        self.catalogIDTextBox.setText(str(server.get("catalog_id", "1")))
+        self.catalogIDLayout.addWidget(self.catalogIDTextBox)
+        self.serverLayout.addLayout(self.catalogIDLayout)
+        self.serverGroupBox.setLayout(self.serverLayout)
+        layout.addWidget(self.serverGroupBox)
+
+        # connect timeout/retry settings
+        self.serverConnectTimeoutsGroupBox = QGroupBox("Connection Timeout and Retries:", self)
+        self.connectLayout = QHBoxLayout()
+        # connect timeout
+        self.connectTimeoutLabel = QLabel("Connect timeout (secs):")
+        self.connectLayout.addWidget(self.connectTimeoutLabel)
+        self.connectTimeoutSpinBox = QSpinBox(parent)
+        self.connectTimeoutSpinBox.setRange(1, 60)
+        self.connectTimeoutSpinBox.setValue(self.session_config.get("timeout")[0] or 6)
+        self.connectLayout.addWidget(self.connectTimeoutSpinBox)
+        # connect retry
+        self.connectRetryLabel = QLabel("Connect retries:")
+        self.connectLayout.addWidget(self.connectRetryLabel)
+        self.connectRetrySpinBox = QSpinBox(parent)
+        self.connectRetrySpinBox.setRange(1, 60)
+        self.connectRetrySpinBox.setValue(self.session_config.get("retry_connect", 10))
+        self.connectLayout.addWidget(self.connectRetrySpinBox)
+        self.serverConnectTimeoutsGroupBox.setLayout(self.connectLayout)
+        layout.addWidget(self.serverConnectTimeoutsGroupBox)
+
+        # io timeout/retry settings
+        self.serverIOTimeoutsGroupBox = QGroupBox("I/O Timeout and Retries:", self)
+        self.ioLayout = QHBoxLayout()
+        # io timeout
+        self.ioTimeoutLabel = QLabel("I/O timeout (secs):")
+        self.ioLayout.addWidget(self.ioTimeoutLabel)
+        self.ioTimeoutSpinBox = QSpinBox(parent)
+        self.ioTimeoutSpinBox.setRange(1, 600)
+        self.ioTimeoutSpinBox.setValue(self.session_config.get("timeout")[1] or 60)
+        self.ioLayout.addWidget(self.ioTimeoutSpinBox)
+        # io retry
+        self.ioRetryLabel = QLabel("I/O retries:")
+        self.ioLayout.addWidget(self.ioRetryLabel)
+        self.ioRetrySpinBox = QSpinBox(parent)
+        self.ioRetrySpinBox.setRange(1, 60)
+        self.ioRetrySpinBox.setValue(self.session_config.get("retry_read", 10))
+        self.ioLayout.addWidget(self.ioRetrySpinBox)
+        self.serverIOTimeoutsGroupBox.setLayout(self.ioLayout)
+        layout.addWidget(self.serverIOTimeoutsGroupBox)
+
+        setServers = getattr(parent.uploader, "setServers", None)
+        self.serversConfigurable = True if callable(setServers) else False
+        self.serverOptionsGroupBox = QGroupBox("Options:", self)
+        self.checkboxLayout = QHBoxLayout()
+        self.defaultServer = QCheckBox("Set as &Default", parent)
+        self.defaultServer.setChecked(stob(server.get("default", False)))
+        self.defaultServer.setEnabled(self.serversConfigurable)
+        self.checkboxLayout.addWidget(self.defaultServer)
+        self.confirm_updates = QCheckBox("&Confirm configuration updates", parent)
+        self.confirm_updates.setChecked(stob(server.get("confirm_updates", False)))
+        self.confirm_updates.setEnabled(self.serversConfigurable)
+        self.checkboxLayout.addWidget(self.confirm_updates)
+
+        self.cookie_persistence = QCheckBox("&Stay logged in", parent)
+        allow_session_caching = True
+        if parent.uploader.config:
+            client_settings = parent.uploader.config.get("client_settings")
+            if client_settings:
+                allow_session_caching = stob(client_settings.get("allow_session_caching", True))
+                if not allow_session_caching:
+                    server["cookie_persistence"] = False
+        self.cookie_persistence.setChecked(stob(server.get("cookie_persistence", False)))
+        self.cookie_persistence.setEnabled(self.serversConfigurable and allow_session_caching)
+        self.checkboxLayout.addWidget(self.cookie_persistence)
+        self.serverOptionsGroupBox.setLayout(self.checkboxLayout)
+        layout.addWidget(self.serverOptionsGroupBox)
+
+        # Button Box
+        self.buttonBox = QDialogButtonBox(parent)
+        self.buttonBox.setObjectName("buttonBox")
+        self.buttonBox.setOrientation(Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel | QDialogButtonBox.Ok)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        layout.addWidget(self.buttonBox)
+
+    def validate(self):
+        host = self.hostnameTextBox.text()
+        hostname = re.sub("(?i)^.*https?://", '', host)
+        if not hostname:
+            warningMessageBox(self.parent(), "Please enter a valid hostname:",
+                              "For example: \'www.host.com\' or \'localhost\', etc.")
+            return False
+        else:
+            self.server["host"] = hostname
+
+        self.server["default"] = self.defaultServer.isChecked()
+        self.server["confirm_updates"] = self.confirm_updates.isChecked()
+        self.server["cookie_persistence"] = self.cookie_persistence.isChecked()
+
+        desc = self.descriptionTextBox.text()
+        self.server["desc"] = desc if desc else ""
+
+        catalog_id = self.catalogIDTextBox.text()
+        self.server["catalog_id"] = catalog_id if catalog_id else "1"
+
+        self.session_config["timeout"] = (self.connectTimeoutSpinBox.value(), self.ioTimeoutSpinBox.value())
+        self.session_config["retry_connect"] = self.connectRetrySpinBox.value()
+        self.session_config["retry_read"] = self.ioRetrySpinBox.value()
+        self.server["session"] = self.session_config
+
+        return True
+
+    @staticmethod
+    def configureServer(parent, server):
+        dialog = ServerDialog(parent, server)
+        ret = dialog.exec_()
+        if QDialog.Accepted == ret:
+            if dialog.validate():
+                return dialog.server.copy()
+        return None
```

### Comparing `deriva-qt-1.6.1/deriva/qt/upload_gui/ui/upload_window.py` & `deriva-qt-1.6.3/deriva/qt/upload_gui/ui/upload_window.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,724 +1,727 @@
-import logging
-import os
-import urllib.parse
-import webbrowser
-
-from PyQt5.QtCore import Qt, QMetaObject, QThreadPool, pyqtSlot, pyqtSignal
-from PyQt5.QtWidgets import qApp, QMainWindow, QWidget, QAction, QSizePolicy, QPushButton, QStyle, QSplitter, QLabel, \
-    QToolBar, QStatusBar, QVBoxLayout, QHBoxLayout, QTableWidgetItem, QAbstractItemView, QLineEdit, QFileDialog, \
-    QMessageBox
-from deriva.core import write_config, stob
-from deriva.qt import EmbeddedAuthWindow, QPlainTextEditLogger, Task, TableWidget, __version__
-from deriva.qt.upload_gui.impl.upload_tasks import *
-from deriva.qt.upload_gui.ui.options_window import OptionsDialog
-from deriva.qt.upload_gui.resources import resources
-
-
-class UploadWindow(QMainWindow):
-    progress_update_signal = pyqtSignal(str)
-
-    def __init__(self,
-                 uploader,
-                 config_file=None,
-                 credential_file=None,
-                 hostname=None,
-                 window_title=None,
-                 cookie_persistence=True):
-        super(UploadWindow, self).__init__()
-        qApp.aboutToQuit.connect(self.quitEvent)
-
-        assert uploader is not None
-        self.uploader = None
-        self.auth_window = None
-        self.identity = None
-        self.current_path = None
-        self.uploading = False
-        self.save_progress_on_cancel = False
-
-        self.ui = UploadWindowUI(self)
-        self.ui.title = window_title if window_title else "Deriva Upload Utility %s" % __version__
-        self.setWindowTitle(self.ui.title)
-
-        self.config_file = config_file
-        self.credential_file = credential_file
-        self.cookie_persistence = cookie_persistence
-
-        self.show()
-        self.configure(uploader, hostname)
-
-    def configure(self, uploader, hostname):
-        # if a hostname has been provided, it overrides whatever default host a given uploader is configured for
-        server = None
-        if hostname:
-            server = dict()
-            if hostname.startswith("http"):
-                url = urllib.parse.urlparse(hostname)
-                server["protocol"] = url.scheme
-                server["host"] = url.netloc
-            else:
-                server["protocol"] = "https"
-                server["host"] = hostname
-
-        # instantiate the uploader...
-        # if an uploader instance does not have a default host configured, prompt the user to configure one
-        if self.uploader:
-            del self.uploader
-        self.uploader = uploader(self.config_file, self.credential_file, server, dcctx_cid="gui/DerivaUploadGUI")
-        if not self.uploader.server:
-            if not self.checkValidServer():
-                return
-            else:
-                self.uploader.setServer(server)
-
-        self.setWindowTitle("%s (%s)" % (self.ui.title, self.uploader.server["host"]))
-
-        self.getNewAuthWindow()
-        if not self.checkVersion():
-            return
-        self.getSession()
-
-    def getNewAuthWindow(self):
-        if self.auth_window:
-            if self.auth_window.authenticated():
-                self.on_actionLogout_triggered()
-            self.auth_window.deleteLater()
-
-        self.auth_window = \
-            EmbeddedAuthWindow(self,
-                               config=self.uploader.server,
-                               cookie_persistence=
-                               self.uploader.server.get("cookie_persistence", self.cookie_persistence),
-                               authentication_success_callback=self.onLoginSuccess,
-                               log_level=logging.getLogger().getEffectiveLevel())
-        self.ui.actionLogin.setEnabled(True)
-
-    def getSession(self):
-        qApp.setOverrideCursor(Qt.WaitCursor)
-        logging.debug("Validating session: %s" % self.uploader.server["host"])
-        queryTask = SessionQueryTask(self.uploader)
-        queryTask.status_update_signal.connect(self.onSessionResult)
-        queryTask.query()
-
-    def onLoginSuccess(self, **kwargs):
-        self.auth_window.hide()
-        self.uploader.setCredentials(kwargs["credential"])
-        self.getSession()
-
-    def enableControls(self):
-        self.ui.actionUpload.setEnabled(self.canUpload())
-        self.ui.actionRescan.setEnabled(self.current_path is not None and self.auth_window.authenticated())
-        self.ui.actionCancel.setEnabled(False)
-        self.ui.actionOptions.setEnabled(True)
-        self.ui.actionLogin.setEnabled(not self.auth_window.authenticated())
-        self.ui.actionLogout.setEnabled(self.auth_window.authenticated())
-        self.ui.actionExit.setEnabled(True)
-        self.ui.browseButton.setEnabled(True)
-
-    def disableControls(self):
-        self.ui.actionUpload.setEnabled(False)
-        self.ui.actionRescan.setEnabled(False)
-        self.ui.actionOptions.setEnabled(False)
-        self.ui.actionLogin.setEnabled(False)
-        self.ui.actionLogout.setEnabled(False)
-        self.ui.actionExit.setEnabled(False)
-        self.ui.browseButton.setEnabled(False)
-
-    def closeEvent(self, event=None):
-        self.disableControls()
-        if self.uploading:
-            self.cancelTasks(self.cancelConfirmation())
-        if event:
-            event.accept()
-
-    def checkValidServer(self):
-        self.restoreCursor()
-        if self.uploader.server and self.uploader.server.get("host"):
-            return True
-        msg = QMessageBox()
-        msg.setIcon(QMessageBox.Warning)
-        msg.setWindowTitle("No Server Configured")
-        msg.setText("Add server configuration now?")
-        msg.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
-        ret = msg.exec_()
-        if ret == QMessageBox.Yes:
-            self.on_actionOptions_triggered()
-        else:
-            return False
-
-    def checkAllowSessionCaching(self):
-        client_settings = self.uploader.config.get("client_settings")
-        if not client_settings:
-            return
-        allow_session_caching = stob(client_settings.get("allow_session_caching", True))
-        cookie_persistence = self.uploader.server.get("cookie_persistence", False)
-        if cookie_persistence != allow_session_caching:
-            if not allow_session_caching:
-                self.uploader.server["cookie_persistence"] = False
-                servers = list()
-                for server in self.uploader.getServers():
-                    if server.get("host", "") != self.uploader.server.get("host"):
-                        servers.append(server)
-                servers.append(self.uploader.server)
-                setServers = getattr(self.uploader, "setServers", None)
-                if callable(setServers):
-                    setServers(servers)
-
-    def onServerChanged(self, server):
-        if server is None or server == self.uploader.server:
-            return
-
-        qApp.setOverrideCursor(Qt.WaitCursor)
-        self.uploader.setServer(server)
-        self.restoreCursor()
-        if not self.checkValidServer():
-            return
-        self.setWindowTitle("%s (%s)" % (self.ui.title, self.uploader.server["host"]))
-        self.getNewAuthWindow()
-        self.getSession()
-
-    def cancelTasks(self, save_progress):
-        qApp.setOverrideCursor(Qt.WaitCursor)
-        self.save_progress_on_cancel = save_progress
-        self.uploader.cancel()
-        Task.shutdown_all()
-        self.statusBar().showMessage("Waiting for background tasks to terminate...")
-
-        while True:
-            qApp.processEvents()
-            if QThreadPool.globalInstance().waitForDone(10):
-                break
-
-        self.uploading = False
-        self.statusBar().showMessage("All background tasks terminated successfully")
-        self.restoreCursor()
-
-    def uploadCallback(self, **kwargs):
-        completed = kwargs.get("completed")
-        total = kwargs.get("total")
-        file_path = kwargs.get("file_path")
-        file_name = os.path.basename(file_path) if file_path else ""
-        job_info = kwargs.get("job_info", {})
-        job_info.update()
-        if completed and total:
-            file_name = " [%s]" % file_name
-            job_info.update({"completed": completed, "total": total, "host": kwargs.get("host")})
-            status = "Uploading file%s: %d%% complete" % (file_name, round(((completed / total) % 100) * 100))
-            self.uploader.setTransferState(file_path, job_info)
-        else:
-            summary = kwargs.get("summary", "")
-            file_name = "Uploaded file: [%s] " % file_name
-            status = file_name  # + summary
-        if status:
-            self.progress_update_signal.emit(status)
-
-        if self.uploader.cancelled:
-            if self.save_progress_on_cancel:
-                return -1
-            else:
-                return False
-
-        return True
-
-    def restoreCursor(self):
-        qApp.restoreOverrideCursor()
-        qApp.processEvents()
-
-    def statusCallback(self, **kwargs):
-        status = kwargs.get("status")
-        self.progress_update_signal.emit(status)
-
-    def displayUploads(self, upload_list):
-        keys = ["State",
-                "Status",
-                "File"]
-        hidden = ["State"]
-        self.ui.uploadList.setRowCount(len(upload_list))
-        self.ui.uploadList.setColumnCount(len(keys))
-
-        rows = 0
-        for row in upload_list:
-            cols = 0
-            for key in keys:
-                item = QTableWidgetItem()
-                value = row.get(key)
-                text = str(value) or ""
-                item.setText(text)
-                item.setToolTip("<span>" + text + "</span>")
-                self.ui.uploadList.setItem(rows, cols, item)
-                if key in hidden:
-                    self.ui.uploadList.hideColumn(cols)
-                cols += 1
-            rows += 1
-
-        self.ui.uploadList.setHorizontalHeaderLabels(keys)  # add header names
-        self.ui.uploadList.horizontalHeader().setDefaultAlignment(Qt.AlignLeft)  # set alignment
-        self.ui.uploadList.resizeColumnToContents(0)
-
-    def canUpload(self):
-        return (self.ui.uploadList.rowCount() > 0) and self.auth_window.authenticated()
-
-    def checkVersion(self):
-        if not self.uploader.isVersionCompatible():
-            self.updateStatus("Version incompatibility detected", "Current version: %s, required version: %s" % (
-                self.uploader.getVersion(), self.uploader.getVersionCompatibility()))
-            self.disableControls()
-            self.ui.actionExit.setEnabled(True)
-            self.ui.actionOptions.setEnabled(True)
-            self.updateConfirmation()
-            return False
-
-        self.checkAllowSessionCaching()
-        self.resetUI("Ready...")
-        return True
-
-    def updateConfirmation(self):
-        url = self.uploader.config.get("version_update_url")
-        if not url:
-            return
-        self.restoreCursor()
-        msg = QMessageBox()
-        msg.setIcon(QMessageBox.Warning)
-        msg.setWindowTitle("Version incompatibility detected!")
-        msg.setText("Current version: %s\nRequired version: %s\n\nLaunch browser and download required version?"
-                    % (self.uploader.getVersion(), self.uploader.getVersionCompatibility()))
-        msg.setInformativeText(
-            "Selecting \"Yes\" will close the application and launch an external web browser which will take you to a "
-            "download page where you can get the required version of this software.")
-        msg.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
-        ret = msg.exec_()
-        if ret == QMessageBox.Yes:
-            webbrowser.open_new(url)
-            self.deleteLater()
-
-    def updateConfig(self):
-        qApp.setOverrideCursor(Qt.WaitCursor)
-        configUpdateTask = ConfigUpdateTask(self.uploader)
-        configUpdateTask.status_update_signal.connect(self.onUpdateConfigResult)
-        configUpdateTask.update_config()
-
-    def scanDirectory(self, reset=False):
-        self.uploader.reset()
-        scanTask = ScanDirectoryTask(self.uploader)
-        scanTask.status_update_signal.connect(self.onScanResult)
-        scanTask.scan(self.current_path)
-
-    @pyqtSlot(str)
-    def updateProgress(self, status):
-        if status:
-            self.statusBar().showMessage(status)
-        else:
-            self.displayUploads(self.uploader.getFileStatusAsArray())
-
-    @pyqtSlot(str, str)
-    def updateStatus(self, status, detail=None, success=True):
-        msg = status + ((": %s" % detail) if detail else "")
-        logging.info(msg) if success else logging.error(msg)
-        self.statusBar().showMessage(status)
-
-    @pyqtSlot(str, str)
-    def resetUI(self, status, detail=None, success=True):
-        self.updateStatus(status, detail, success)
-        self.enableControls()
-
-    @pyqtSlot(str)
-    def updateLog(self, text):
-        self.ui.logTextBrowser.widget.appendPlainText(text)
-
-    @pyqtSlot(bool, str, str, object)
-    def onSessionResult(self, success, status, detail, result):
-        self.restoreCursor()
-        if success:
-            self.identity = result["client"]["id"]
-            display_name = result["client"]["full_name"]
-            self.setWindowTitle("%s (%s - %s)" % (self.ui.title, self.uploader.server["host"], display_name))
-            self.ui.actionLogout.setEnabled(True)
-            self.ui.actionLogin.setEnabled(False)
-            if self.current_path:
-                self.ui.actionRescan.setEnabled(True)
-                self.ui.actionUpload.setEnabled(True)
-            self.updateStatus("Logged in.")
-            self.updateConfig()
-        else:
-            self.updateStatus("Login required.")
-
-    @pyqtSlot(bool, str, str, object)
-    def onUpdateConfigResult(self, success, status, detail, result):
-        self.restoreCursor()
-        if not success:
-            self.resetUI(status, detail)
-            return
-        if not result:
-            return
-        confirm_updates = stob(self.uploader.server.get("confirm_updates", False))
-        if confirm_updates:
-            msg = QMessageBox()
-            msg.setIcon(QMessageBox.Information)
-            msg.setWindowTitle("Updated Configuration Available")
-            msg.setText("Apply updated configuration?")
-            msg.setInformativeText(
-                "Selecting \"Yes\" will apply the latest configuration from the server and overwrite the existing "
-                "default configuration file.\n\nSelecting \"No\" will ignore these updates and continue to use the "
-                "existing configuration.\n\nYou should always apply the latest configuration changes from the server "
-                "unless you understand the risk involved with using a potentially out-of-date configuration.")
-
-            msg.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
-            ret = msg.exec_()
-            if ret == QMessageBox.No:
-                return
-
-        write_config(self.uploader.getDeployedConfigFilePath(), result)
-        self.uploader.initialize(cleanup=False)
-        if not self.checkVersion():
-            return
-        self.on_actionRescan_triggered()
-
-    @pyqtSlot()
-    def on_actionBrowse_triggered(self):
-        dialog = QFileDialog()
-        path = dialog.getExistingDirectory(self,
-                                           "Select Directory",
-                                           self.current_path,
-                                           QFileDialog.ShowDirsOnly)
-        if not path:
-            return
-        self.current_path = path
-        self.ui.pathTextBox.setText(os.path.normpath(self.current_path))
-        self.scanDirectory()
-
-    @pyqtSlot()
-    def on_actionRescan_triggered(self):
-        if not self.current_path:
-            return
-
-        self.scanDirectory()
-
-    @pyqtSlot(bool, str, str, object)
-    def onScanResult(self, success, status, detail, result):
-        self.restoreCursor()
-        if success:
-            self.displayUploads(self.uploader.getFileStatusAsArray())
-            self.ui.actionUpload.setEnabled(self.canUpload())
-            self.resetUI("Ready...")
-            if self.uploading:
-                self.on_actionUpload_triggered()
-        else:
-            self.resetUI(status, detail, success)
-
-    @pyqtSlot()
-    def on_actionUpload_triggered(self):
-        if not self.uploading:
-            if self.uploader.cancelled:
-                self.uploading = True
-                self.on_actionRescan_triggered()
-                return
-
-        self.disableControls()
-        self.ui.actionCancel.setEnabled(True)
-        self.save_progress_on_cancel = False
-        qApp.setOverrideCursor(Qt.WaitCursor)
-        self.uploading = True
-        self.updateStatus("Uploading...")
-        self.progress_update_signal.connect(self.updateProgress)
-        uploadTask = UploadFilesTask(self.uploader)
-        uploadTask.status_update_signal.connect(self.onUploadResult)
-        uploadTask.upload(status_callback=self.statusCallback, file_callback=self.uploadCallback)
-
-    @pyqtSlot(bool, str, str, object)
-    def onUploadResult(self, success, status, detail, result):
-        self.restoreCursor()
-        self.uploading = False
-        self.displayUploads(self.uploader.getFileStatusAsArray())
-        if success:
-            self.resetUI("Ready.")
-        else:
-            self.resetUI(status, detail, success)
-
-    @pyqtSlot()
-    def on_actionCancel_triggered(self):
-        self.cancelTasks(self.cancelConfirmation())
-        self.restoreCursor()
-        self.displayUploads(self.uploader.getFileStatusAsArray())
-        self.resetUI("Ready.")
-
-    @pyqtSlot()
-    def on_actionLogin_triggered(self):
-        if not self.auth_window:
-            if self.checkValidServer():
-                self.getNewAuthWindow()
-            else:
-                return
-        self.auth_window.show()
-        self.auth_window.login()
-
-    @pyqtSlot()
-    def on_actionLogout_triggered(self):
-        self.setWindowTitle("%s (%s)" % (self.ui.title, self.uploader.server["host"]))
-        self.auth_window.logout()
-        self.identity = None
-        self.ui.actionUpload.setEnabled(False)
-        self.ui.actionRescan.setEnabled(False)
-        self.ui.actionLogout.setEnabled(False)
-        self.ui.actionLogin.setEnabled(True)
-        self.updateStatus("Logged out.")
-
-    @pyqtSlot()
-    def on_actionOptions_triggered(self):
-        OptionsDialog.getOptions(self)
-
-    @pyqtSlot()
-    def on_actionHelp_triggered(self):
-        pass
-
-    @pyqtSlot()
-    def on_actionExit_triggered(self):
-        self.closeEvent()
-        qApp.quit()
-
-    def quitEvent(self):
-        if self.auth_window:
-            self.auth_window.logout(self.logoutConfirmation())
-        qApp.closeAllWindows()
-        self.deleteLater()
-
-    def logoutConfirmation(self):
-        if self.auth_window and (not self.auth_window.authenticated() or not self.auth_window.cookie_persistence):
-            return
-        msg = QMessageBox()
-        msg.setIcon(QMessageBox.Warning)
-        msg.setWindowTitle("Confirm Action")
-        msg.setText("Do you wish to completely logout of the system?")
-        msg.setInformativeText("Selecting \"Yes\" will clear the login state and invalidate the current user identity."
-                               "\n\nSelecting \"No\" will keep your current identity cached, which will allow you to "
-                               "log back in without authenticating until your session expires.\n\nNOTE: Select \"Yes\" "
-                               "if this is a shared system using a single user account.")
-        msg.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
-        ret = msg.exec_()
-        if ret == QMessageBox.Yes:
-            return True
-        return False
-
-    def cancelConfirmation(self):
-        self.restoreCursor()
-        msg = QMessageBox()
-        msg.setIcon(QMessageBox.Warning)
-        msg.setWindowTitle("Confirm Action")
-        msg.setText("Save progress for the current upload?")
-        msg.setInformativeText("Selecting \"Yes\" will attempt to resume this transfer from the point where it was "
-                               "cancelled.\n\nSelecting \"No\" will require the transfer to be started over from the "
-                               "beginning of file.")
-        msg.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
-        ret = msg.exec_()
-        if ret == QMessageBox.Yes:
-            return True
-        return False
-
-
-# noinspection PyArgumentList
-class UploadWindowUI(object):
-
-    title = "DERIVA File Uploader"
-
-    def __init__(self, MainWin):
-
-        # Main Window
-        MainWin.setObjectName("UploadWindow")
-        MainWin.setWindowTitle(MainWin.tr(self.title))
-        MainWin.resize(1024, 768)
-        self.centralWidget = QWidget(MainWin)
-        self.centralWidget.setObjectName("centralWidget")
-        MainWin.setCentralWidget(self.centralWidget)
-        self.verticalLayout = QVBoxLayout(self.centralWidget)
-        self.verticalLayout.setContentsMargins(11, 11, 11, 11)
-        self.verticalLayout.setSpacing(6)
-        self.verticalLayout.setObjectName("verticalLayout")
-
-        self.horizontalLayout = QHBoxLayout()
-        self.pathLabel = QLabel("Directory:")
-        self.horizontalLayout.addWidget(self.pathLabel)
-        self.pathTextBox = QLineEdit()
-        self.pathTextBox.setReadOnly(True)
-        self.horizontalLayout.addWidget(self.pathTextBox)
-        self.browseButton = QPushButton("Browse", self.centralWidget)
-        self.browseButton.clicked.connect(MainWin.on_actionBrowse_triggered)
-        self.horizontalLayout.addWidget(self.browseButton)
-        self.verticalLayout.addLayout(self.horizontalLayout)
-
-        # Splitter for Upload list/Log
-        self.splitter = QSplitter(Qt.Vertical)
-
-        # Table View (Upload list)
-        self.uploadList = TableWidget(self.centralWidget)
-        self.uploadList.setObjectName("uploadList")
-        self.uploadList.setStyleSheet(
-            """
-            QTableWidget {
-                    border: 2px solid grey;
-                    border-radius: 5px;
-            }
-            """)
-        self.uploadList.setEditTriggers(QAbstractItemView.NoEditTriggers)  # use NoEditTriggers to disable editing
-        self.uploadList.setAlternatingRowColors(True)
-        self.uploadList.setSelectionBehavior(QAbstractItemView.SelectRows)
-        self.uploadList.setSelectionMode(QAbstractItemView.NoSelection)
-        self.uploadList.verticalHeader().setDefaultSectionSize(18)  # tighten up the row size
-        self.uploadList.horizontalHeader().setStretchLastSection(True)
-        self.uploadList.setSortingEnabled(True)  # allow sorting
-        self.splitter.addWidget(self.uploadList)
-
-        # Log Widget
-        self.logTextBrowser = QPlainTextEditLogger(self.centralWidget)
-        self.logTextBrowser.widget.setObjectName("logTextBrowser")
-        self.logTextBrowser.widget.setStyleSheet(
-            """
-            QPlainTextEdit {
-                    border: 2px solid grey;
-                    border-radius: 5px;
-                    background-color: lightgray;
-            }
-            """)
-        self.splitter.addWidget(self.logTextBrowser.widget)
-
-        # add splitter
-        self.splitter.setSizes([400, 200])
-        self.verticalLayout.addWidget(self.splitter)
-
-    # Actions
-
-        # Browse
-        self.actionBrowse = QAction(MainWin)
-        self.actionBrowse.setObjectName("actionBrowse")
-        self.actionBrowse.setText(MainWin.tr("Browse"))
-        self.actionBrowse.setToolTip(MainWin.tr("Set the upload directory"))
-        self.actionBrowse.setShortcut(MainWin.tr("Ctrl+B"))
-
-        # Upload
-        self.actionUpload = QAction(MainWin)
-        self.actionUpload.setObjectName("actionUpload")
-        self.actionUpload.setText(MainWin.tr("Upload"))
-        self.actionUpload.setToolTip(MainWin.tr("Upload files"))
-        self.actionUpload.setShortcut(MainWin.tr("Ctrl+L"))
-        self.actionUpload.setEnabled(False)
-
-        # Rescan
-        self.actionRescan = QAction(MainWin)
-        self.actionRescan.setObjectName("actionRescan")
-        self.actionRescan.setText(MainWin.tr("Rescan"))
-        self.actionRescan.setToolTip(MainWin.tr("Rescan the upload directory"))
-        self.actionRescan.setShortcut(MainWin.tr("Ctrl+R"))
-        self.actionRescan.setEnabled(False)
-
-        # Cancel
-        self.actionCancel = QAction(MainWin)
-        self.actionCancel.setObjectName("actionCancel")
-        self.actionCancel.setText(MainWin.tr("Cancel"))
-        self.actionCancel.setToolTip(MainWin.tr("Cancel any upload(s) in-progress"))
-        self.actionCancel.setShortcut(MainWin.tr("Ctrl+C"))
-
-        # Options
-        self.actionOptions = QAction(MainWin)
-        self.actionOptions.setObjectName("actionOptions")
-        self.actionOptions.setText(MainWin.tr("Options"))
-        self.actionOptions.setToolTip(MainWin.tr("Configuration Options"))
-        self.actionOptions.setShortcut(MainWin.tr("Ctrl+P"))
-
-        # Login
-        self.actionLogin = QAction(MainWin)
-        self.actionLogin.setObjectName("actionLogin")
-        self.actionLogin.setText(MainWin.tr("Login"))
-        self.actionLogin.setToolTip(MainWin.tr("Login to the server"))
-        self.actionLogin.setShortcut(MainWin.tr("Ctrl+G"))
-        self.actionLogin.setEnabled(False)
-
-        # Logout
-        self.actionLogout = QAction(MainWin)
-        self.actionLogout.setObjectName("actionLogout")
-        self.actionLogout.setText(MainWin.tr("Logout"))
-        self.actionLogout.setToolTip(MainWin.tr("Logout of the server"))
-        self.actionLogout.setShortcut(MainWin.tr("Ctrl+O"))
-        self.actionLogout.setEnabled(False)
-
-        # Exit
-        self.actionExit = QAction(MainWin)
-        self.actionExit.setObjectName("actionExit")
-        self.actionExit.setText(MainWin.tr("Exit"))
-        self.actionExit.setToolTip(MainWin.tr("Exit the application"))
-        self.actionExit.setShortcut(MainWin.tr("Ctrl+Z"))
-
-        # Help
-        self.actionHelp = QAction(MainWin)
-        self.actionHelp.setObjectName("actionHelp")
-        self.actionHelp.setText(MainWin.tr("Help"))
-        self.actionHelp.setToolTip(MainWin.tr("Help"))
-        self.actionHelp.setShortcut(MainWin.tr("Ctrl+H"))
-
-    # Menu Bar
-
-        """
-        self.menuBar = QMenuBar(MainWin)
-        self.menuBar.setObjectName("menuBar")
-        MainWin.setMenuBar(self.menuBar)
-        self.menuBar.setStyleSheet(
-            "QMenuBar{font-family: Arial;font-style: normal;font-size: 10pt;font-weight: bold;};")
-        """
-
-    # Tool Bar
-
-        self.mainToolBar = QToolBar(MainWin)
-        self.mainToolBar.setObjectName("mainToolBar")
-        self.mainToolBar.setToolButtonStyle(Qt.ToolButtonTextUnderIcon)
-        self.mainToolBar.setContextMenuPolicy(Qt.PreventContextMenu)
-        MainWin.addToolBar(Qt.TopToolBarArea, self.mainToolBar)
-
-        # Upload
-        self.mainToolBar.addAction(self.actionUpload)
-        self.actionUpload.setIcon(qApp.style().standardIcon(QStyle.SP_FileDialogToParent))
-
-        # Rescan
-        self.mainToolBar.addAction(self.actionRescan)
-        self.actionRescan.setIcon(qApp.style().standardIcon(QStyle.SP_BrowserReload))
-
-        # Cancel
-        self.mainToolBar.addAction(self.actionCancel)
-        self.actionCancel.setIcon(qApp.style().standardIcon(QStyle.SP_BrowserStop))
-        self.actionCancel.setEnabled(False)
-
-        # Options
-        self.mainToolBar.addAction(self.actionOptions)
-        self.actionOptions.setIcon(qApp.style().standardIcon(QStyle.SP_FileDialogDetailedView))
-
-        # this spacer right justifies everything that comes after it
-        spacer = QWidget()
-        spacer.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
-        self.mainToolBar.addWidget(spacer)
-
-        # Login
-        self.mainToolBar.addAction(self.actionLogin)
-        self.actionLogin.setIcon(qApp.style().standardIcon(QStyle.SP_DialogApplyButton))
-
-        # Logout
-        self.mainToolBar.addAction(self.actionLogout)
-        self.actionLogout.setIcon(qApp.style().standardIcon(QStyle.SP_DialogOkButton))
-
-        # Help
-        #self.mainToolBar.addAction(self.actionHelp)
-        self.actionHelp.setIcon(qApp.style().standardIcon(QStyle.SP_MessageBoxQuestion))
-
-        # Exit
-        self.mainToolBar.addAction(self.actionExit)
-        self.actionExit.setIcon(qApp.style().standardIcon(QStyle.SP_DialogCancelButton))
-
-    # Status Bar
-
-        self.statusBar = QStatusBar(MainWin)
-        self.statusBar.setToolTip("")
-        self.statusBar.setStatusTip("")
-        self.statusBar.setObjectName("statusBar")
-        MainWin.setStatusBar(self.statusBar)
-
-    # configure logging
-        self.logTextBrowser.widget.log_update_signal.connect(MainWin.updateLog)
-        self.logTextBrowser.setFormatter(logging.Formatter("%(asctime)s - %(levelname)s - %(message)s"))
-        logging.getLogger().addHandler(self.logTextBrowser)
-
-    # finalize UI setup
-        QMetaObject.connectSlotsByName(MainWin)
+import logging
+import os
+import urllib.parse
+import webbrowser
+
+from PyQt5.QtCore import Qt, QMetaObject, QThreadPool, pyqtSlot, pyqtSignal
+from PyQt5.QtWidgets import qApp, QMainWindow, QWidget, QAction, QSizePolicy, QPushButton, QStyle, QSplitter, QLabel, \
+    QToolBar, QStatusBar, QVBoxLayout, QHBoxLayout, QTableWidgetItem, QAbstractItemView, QLineEdit, QFileDialog, \
+    QMessageBox
+from deriva.core import write_config, stob
+from deriva.qt import EmbeddedAuthWindow, QPlainTextEditLogger, Task, TableWidget, __version__
+from deriva.qt.upload_gui.impl.upload_tasks import *
+from deriva.qt.upload_gui.ui.options_window import OptionsDialog
+from deriva.qt.upload_gui.resources import resources
+
+
+class UploadWindow(QMainWindow):
+    progress_update_signal = pyqtSignal(str)
+
+    def __init__(self,
+                 uploader,
+                 config_file=None,
+                 credential_file=None,
+                 hostname=None,
+                 window_title=None,
+                 cookie_persistence=True):
+        super(UploadWindow, self).__init__()
+        qApp.aboutToQuit.connect(self.quitEvent)
+
+        assert uploader is not None
+        self.uploader = None
+        self.auth_window = None
+        self.identity = None
+        self.current_path = None
+        self.uploading = False
+        self.save_progress_on_cancel = False
+
+        self.ui = UploadWindowUI(self)
+        self.ui.title = window_title if window_title else "Deriva Upload Utility %s" % __version__
+        self.setWindowTitle(self.ui.title)
+
+        self.config_file = config_file
+        self.credential_file = credential_file
+        self.cookie_persistence = cookie_persistence
+
+        self.show()
+        self.configure(uploader, hostname)
+
+    def configure(self, uploader, hostname):
+        # if a hostname has been provided, it overrides whatever default host a given uploader is configured for
+        server = None
+        if hostname:
+            server = dict()
+            if hostname.startswith("http"):
+                url = urllib.parse.urlparse(hostname)
+                server["protocol"] = url.scheme
+                server["host"] = url.netloc
+            else:
+                server["protocol"] = "https"
+                server["host"] = hostname
+
+        # instantiate the uploader...
+        # if an uploader instance does not have a default host configured, prompt the user to configure one
+        if self.uploader:
+            del self.uploader
+        self.uploader = uploader(self.config_file, self.credential_file, server, dcctx_cid="gui/DerivaUploadGUI")
+        if not self.uploader.server:
+            if not self.checkValidServer():
+                return
+            else:
+                self.uploader.setServer(server)
+
+        self.setWindowTitle("%s (%s)" % (self.ui.title, self.uploader.server["host"]))
+
+        self.getNewAuthWindow()
+        if not self.checkVersion():
+            return
+
+    def getNewAuthWindow(self):
+        if self.auth_window:
+            if self.auth_window.authenticated():
+                self.on_actionLogout_triggered()
+            self.auth_window.deleteLater()
+
+        self.auth_window = \
+            EmbeddedAuthWindow(self,
+                               config=self.uploader.server,
+                               cookie_persistence=
+                               self.uploader.server.get("cookie_persistence", self.cookie_persistence),
+                               authentication_success_callback=self.onLoginSuccess,
+                               log_level=logging.getLogger().getEffectiveLevel())
+        self.ui.actionLogin.setEnabled(True)
+
+    def getSession(self):
+        qApp.setOverrideCursor(Qt.WaitCursor)
+        logging.debug("Validating session: %s" % self.uploader.server["host"])
+        queryTask = SessionQueryTask(self.uploader)
+        queryTask.status_update_signal.connect(self.onSessionResult)
+        queryTask.query()
+
+    def onLoginSuccess(self, **kwargs):
+        self.auth_window.hide()
+        self.uploader.setCredentials(kwargs["credential"])
+        self.getSession()
+
+    def enableControls(self):
+        self.ui.actionUpload.setEnabled(self.canUpload())
+        self.ui.actionRescan.setEnabled(self.current_path is not None and self.auth_window.authenticated())
+        self.ui.actionCancel.setEnabled(False)
+        self.ui.actionOptions.setEnabled(True)
+        self.ui.actionLogin.setEnabled(not self.auth_window.authenticated())
+        self.ui.actionLogout.setEnabled(self.auth_window.authenticated())
+        self.ui.actionExit.setEnabled(True)
+        self.ui.browseButton.setEnabled(True)
+
+    def disableControls(self):
+        self.ui.actionUpload.setEnabled(False)
+        self.ui.actionRescan.setEnabled(False)
+        self.ui.actionOptions.setEnabled(False)
+        self.ui.actionLogin.setEnabled(False)
+        self.ui.actionLogout.setEnabled(False)
+        self.ui.actionExit.setEnabled(False)
+        self.ui.browseButton.setEnabled(False)
+
+    def closeEvent(self, event=None):
+        self.disableControls()
+        if self.uploading:
+            self.cancelTasks(self.cancelConfirmation())
+        if event:
+            event.accept()
+
+    def checkValidServer(self):
+        self.restoreCursor()
+        if self.uploader.server and self.uploader.server.get("host"):
+            return True
+        msg = QMessageBox()
+        msg.setIcon(QMessageBox.Warning)
+        msg.setWindowTitle("No Server Configured")
+        msg.setText("Add server configuration now?")
+        msg.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
+        ret = msg.exec_()
+        if ret == QMessageBox.Yes:
+            self.on_actionOptions_triggered()
+        else:
+            return False
+
+    def checkAllowSessionCaching(self):
+        client_settings = self.uploader.config.get("client_settings")
+        if not client_settings:
+            return
+        allow_session_caching = stob(client_settings.get("allow_session_caching", True))
+        cookie_persistence = self.uploader.server.get("cookie_persistence", False)
+        if cookie_persistence != allow_session_caching:
+            if not allow_session_caching:
+                self.uploader.server["cookie_persistence"] = False
+                servers = list()
+                for server in self.uploader.getServers():
+                    if server.get("host", "") != self.uploader.server.get("host"):
+                        servers.append(server)
+                servers.append(self.uploader.server)
+                setServers = getattr(self.uploader, "setServers", None)
+                if callable(setServers):
+                    setServers(servers)
+
+    def onServerChanged(self, server):
+        if server is None or server == self.uploader.server:
+            return
+
+        qApp.setOverrideCursor(Qt.WaitCursor)
+        self.uploader.setServer(server)
+        self.restoreCursor()
+        if not self.checkValidServer():
+            return
+        self.setWindowTitle("%s (%s)" % (self.ui.title, self.uploader.server["host"]))
+        self.getNewAuthWindow()
+        self.getSession()
+
+    def cancelTasks(self, save_progress):
+        qApp.setOverrideCursor(Qt.WaitCursor)
+        self.save_progress_on_cancel = save_progress
+        self.uploader.cancel()
+        Task.shutdown_all()
+        self.statusBar().showMessage("Waiting for background tasks to terminate...")
+
+        while True:
+            qApp.processEvents()
+            if QThreadPool.globalInstance().waitForDone(10):
+                break
+
+        self.uploading = False
+        self.statusBar().showMessage("All background tasks terminated successfully")
+        self.restoreCursor()
+
+    def uploadCallback(self, **kwargs):
+        completed = kwargs.get("completed")
+        total = kwargs.get("total")
+        file_path = kwargs.get("file_path")
+        file_name = os.path.basename(file_path) if file_path else ""
+        job_info = kwargs.get("job_info", {})
+        job_info.update()
+        if completed and total:
+            file_name = " [%s]" % file_name
+            job_info.update({"completed": completed, "total": total, "host": kwargs.get("host")})
+            status = "Uploading file%s: %d%% complete" % (file_name, round(((completed / total) % 100) * 100))
+            self.uploader.setTransferState(file_path, job_info)
+        else:
+            summary = kwargs.get("summary", "")
+            file_name = "Uploaded file: [%s] " % file_name
+            status = file_name  # + summary
+        if status:
+            self.progress_update_signal.emit(status)
+
+        qApp.processEvents()
+        if self.uploader.cancelled:
+            if self.save_progress_on_cancel:
+                return -1
+            else:
+                return False
+
+        return True
+
+    def restoreCursor(self):
+        qApp.restoreOverrideCursor()
+        qApp.processEvents()
+
+    def statusCallback(self, **kwargs):
+        status = kwargs.get("status")
+        self.progress_update_signal.emit(status)
+        qApp.processEvents()
+
+    def displayUploads(self, upload_list):
+        keys = ["State",
+                "Status",
+                "File"]
+        hidden = ["State"]
+        self.ui.uploadList.setRowCount(len(upload_list))
+        self.ui.uploadList.setColumnCount(len(keys))
+
+        rows = 0
+        for row in upload_list:
+            cols = 0
+            for key in keys:
+                item = QTableWidgetItem()
+                value = row.get(key)
+                text = str(value) or ""
+                item.setText(text)
+                item.setToolTip("<span>" + text + "</span>")
+                self.ui.uploadList.setItem(rows, cols, item)
+                if key in hidden:
+                    self.ui.uploadList.hideColumn(cols)
+                cols += 1
+            rows += 1
+
+        self.ui.uploadList.setHorizontalHeaderLabels(keys)  # add header names
+        self.ui.uploadList.horizontalHeader().setDefaultAlignment(Qt.AlignLeft)  # set alignment
+        self.ui.uploadList.resizeColumnToContents(0)
+
+    def canUpload(self):
+        return (self.ui.uploadList.rowCount() > 0) and self.auth_window.authenticated()
+
+    def checkVersion(self):
+        if not self.uploader.isVersionCompatible():
+            self.updateStatus("Version incompatibility detected", "Current version: %s, required version: %s" % (
+                self.uploader.getVersion(), self.uploader.getVersionCompatibility()))
+            self.disableControls()
+            self.ui.actionExit.setEnabled(True)
+            self.ui.actionOptions.setEnabled(True)
+            self.updateConfirmation()
+            return False
+
+        self.checkAllowSessionCaching()
+        self.resetUI("Ready...")
+        return True
+
+    def updateConfirmation(self):
+        url = self.uploader.config.get("version_update_url")
+        if not url:
+            return
+        self.restoreCursor()
+        msg = QMessageBox()
+        msg.setIcon(QMessageBox.Warning)
+        msg.setWindowTitle("Version incompatibility detected!")
+        msg.setText("Current version: %s\nRequired version: %s\n\nLaunch browser and download required version?"
+                    % (self.uploader.getVersion(), self.uploader.getVersionCompatibility()))
+        msg.setInformativeText(
+            "Selecting \"Yes\" will close the application and launch an external web browser which will take you to a "
+            "download page where you can get the required version of this software.")
+        msg.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
+        ret = msg.exec_()
+        if ret == QMessageBox.Yes:
+            webbrowser.open_new(url)
+            self.deleteLater()
+
+    def updateConfig(self):
+        qApp.setOverrideCursor(Qt.WaitCursor)
+        configUpdateTask = ConfigUpdateTask(self.uploader)
+        configUpdateTask.status_update_signal.connect(self.onUpdateConfigResult)
+        configUpdateTask.update_config()
+
+    def scanDirectory(self, reset=False):
+        self.uploader.reset()
+        scanTask = ScanDirectoryTask(self.uploader)
+        scanTask.status_update_signal.connect(self.onScanResult)
+        scanTask.scan(self.current_path)
+
+    @pyqtSlot(str)
+    def updateProgress(self, status):
+        if status:
+            self.statusBar().showMessage(status)
+        else:
+            self.displayUploads(self.uploader.getFileStatusAsArray())
+
+    @pyqtSlot(str, str)
+    def updateStatus(self, status, detail=None, success=True):
+        msg = status + ((": %s" % detail) if detail else "")
+        logging.info(msg) if success else logging.error(msg)
+        self.statusBar().showMessage(status)
+
+    @pyqtSlot(str, str)
+    def resetUI(self, status, detail=None, success=True):
+        self.updateStatus(status, detail, success)
+        self.enableControls()
+
+    @pyqtSlot(str)
+    def updateLog(self, text):
+        self.ui.logTextBrowser.widget.appendPlainText(text)
+
+    @pyqtSlot(bool, str, str, object)
+    def onSessionResult(self, success, status, detail, result):
+        self.restoreCursor()
+        if success:
+            self.identity = result["client"]["id"]
+            display_name = result["client"]["full_name"]
+            self.setWindowTitle("%s (%s - %s)" % (self.ui.title, self.uploader.server["host"], display_name))
+            self.ui.actionLogout.setEnabled(True)
+            self.ui.actionLogin.setEnabled(False)
+            if self.current_path:
+                self.ui.actionRescan.setEnabled(True)
+                self.ui.actionUpload.setEnabled(True)
+            self.updateStatus("Logged in.")
+            self.updateConfig()
+        else:
+            self.updateStatus("Login required.")
+
+    @pyqtSlot(bool, str, str, object)
+    def onUpdateConfigResult(self, success, status, detail, result):
+        self.restoreCursor()
+        if not success:
+            self.resetUI(status, detail)
+            return
+        if not result:
+            return
+        confirm_updates = stob(self.uploader.server.get("confirm_updates", False))
+        if confirm_updates:
+            msg = QMessageBox()
+            msg.setIcon(QMessageBox.Information)
+            msg.setWindowTitle("Updated Configuration Available")
+            msg.setText("Apply updated configuration?")
+            msg.setInformativeText(
+                "Selecting \"Yes\" will apply the latest configuration from the server and overwrite the existing "
+                "default configuration file.\n\nSelecting \"No\" will ignore these updates and continue to use the "
+                "existing configuration.\n\nYou should always apply the latest configuration changes from the server "
+                "unless you understand the risk involved with using a potentially out-of-date configuration.")
+
+            msg.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
+            ret = msg.exec_()
+            if ret == QMessageBox.No:
+                return
+
+        write_config(self.uploader.getDeployedConfigFilePath(), result)
+        self.uploader.initialize(cleanup=False)
+        if not self.checkVersion():
+            return
+        self.on_actionRescan_triggered()
+
+    @pyqtSlot()
+    def on_actionBrowse_triggered(self):
+        dialog = QFileDialog()
+        path = dialog.getExistingDirectory(self,
+                                           "Select Directory",
+                                           self.current_path,
+                                           QFileDialog.ShowDirsOnly)
+        if not path:
+            return
+        self.current_path = path
+        self.ui.pathTextBox.setText(os.path.normpath(self.current_path))
+        self.scanDirectory()
+
+    @pyqtSlot()
+    def on_actionRescan_triggered(self):
+        if not self.current_path:
+            return
+
+        self.scanDirectory()
+
+    @pyqtSlot(bool, str, str, object)
+    def onScanResult(self, success, status, detail, result):
+        self.restoreCursor()
+        if success:
+            self.displayUploads(self.uploader.getFileStatusAsArray())
+            self.ui.actionUpload.setEnabled(self.canUpload())
+            self.resetUI("Ready...")
+            if self.uploading:
+                self.on_actionUpload_triggered()
+        else:
+            self.resetUI(status, detail, success)
+
+    @pyqtSlot()
+    def on_actionUpload_triggered(self):
+        if not self.uploading:
+            if self.uploader.cancelled:
+                self.uploading = True
+                self.on_actionRescan_triggered()
+                return
+
+        self.disableControls()
+        self.ui.actionCancel.setEnabled(True)
+        self.save_progress_on_cancel = False
+        qApp.setOverrideCursor(Qt.WaitCursor)
+        self.uploading = True
+        self.updateStatus("Uploading...")
+        self.progress_update_signal.connect(self.updateProgress)
+        uploadTask = UploadFilesTask(self.uploader)
+        uploadTask.status_update_signal.connect(self.onUploadResult)
+        uploadTask.upload(status_callback=self.statusCallback, file_callback=self.uploadCallback)
+
+    @pyqtSlot(bool, str, str, object)
+    def onUploadResult(self, success, status, detail, result):
+        self.restoreCursor()
+        self.uploading = False
+        self.displayUploads(self.uploader.getFileStatusAsArray())
+        if success:
+            self.resetUI("Ready.")
+        else:
+            self.resetUI(status, detail, success)
+
+    @pyqtSlot()
+    def on_actionCancel_triggered(self):
+        self.cancelTasks(self.cancelConfirmation())
+        self.restoreCursor()
+        self.displayUploads(self.uploader.getFileStatusAsArray())
+        self.resetUI("Ready.")
+
+    @pyqtSlot()
+    def on_actionLogin_triggered(self):
+        if not self.auth_window:
+            if self.checkValidServer():
+                self.getNewAuthWindow()
+            else:
+                return
+        if self.auth_window.authenticated():
+            return
+        self.auth_window.show()
+        self.auth_window.login()
+
+    @pyqtSlot()
+    def on_actionLogout_triggered(self):
+        self.setWindowTitle("%s (%s)" % (self.ui.title, self.uploader.server["host"]))
+        self.auth_window.logout()
+        self.identity = None
+        self.ui.actionUpload.setEnabled(False)
+        self.ui.actionRescan.setEnabled(False)
+        self.ui.actionLogout.setEnabled(False)
+        self.ui.actionLogin.setEnabled(True)
+        self.updateStatus("Logged out.")
+
+    @pyqtSlot()
+    def on_actionOptions_triggered(self):
+        OptionsDialog.getOptions(self)
+
+    @pyqtSlot()
+    def on_actionHelp_triggered(self):
+        pass
+
+    @pyqtSlot()
+    def on_actionExit_triggered(self):
+        self.closeEvent()
+        qApp.quit()
+
+    def quitEvent(self):
+        if self.auth_window:
+            self.auth_window.logout(self.logoutConfirmation())
+        qApp.closeAllWindows()
+        self.deleteLater()
+
+    def logoutConfirmation(self):
+        if self.auth_window and (not self.auth_window.authenticated(False) or not self.auth_window.cookie_persistence):
+            return
+        msg = QMessageBox()
+        msg.setIcon(QMessageBox.Warning)
+        msg.setWindowTitle("Confirm Action")
+        msg.setText("Do you wish to completely logout of the system?")
+        msg.setInformativeText("Selecting \"Yes\" will clear the login state and invalidate the current user identity."
+                               "\n\nSelecting \"No\" will keep your current identity cached, which will allow you to "
+                               "log back in without authenticating until your session expires.\n\nNOTE: Select \"Yes\" "
+                               "if this is a shared system using a single user account.")
+        msg.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
+        ret = msg.exec_()
+        if ret == QMessageBox.Yes:
+            return True
+        return False
+
+    def cancelConfirmation(self):
+        self.restoreCursor()
+        msg = QMessageBox()
+        msg.setIcon(QMessageBox.Warning)
+        msg.setWindowTitle("Confirm Action")
+        msg.setText("Save progress for the current upload?")
+        msg.setInformativeText("Selecting \"Yes\" will attempt to resume this transfer from the point where it was "
+                               "cancelled.\n\nSelecting \"No\" will require the transfer to be started over from the "
+                               "beginning of file.")
+        msg.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
+        ret = msg.exec_()
+        if ret == QMessageBox.Yes:
+            return True
+        return False
+
+
+# noinspection PyArgumentList
+class UploadWindowUI(object):
+
+    title = "DERIVA File Uploader"
+
+    def __init__(self, MainWin):
+
+        # Main Window
+        MainWin.setObjectName("UploadWindow")
+        MainWin.setWindowTitle(MainWin.tr(self.title))
+        MainWin.resize(1024, 768)
+        self.centralWidget = QWidget(MainWin)
+        self.centralWidget.setObjectName("centralWidget")
+        MainWin.setCentralWidget(self.centralWidget)
+        self.verticalLayout = QVBoxLayout(self.centralWidget)
+        self.verticalLayout.setContentsMargins(11, 11, 11, 11)
+        self.verticalLayout.setSpacing(6)
+        self.verticalLayout.setObjectName("verticalLayout")
+
+        self.horizontalLayout = QHBoxLayout()
+        self.pathLabel = QLabel("Directory:")
+        self.horizontalLayout.addWidget(self.pathLabel)
+        self.pathTextBox = QLineEdit()
+        self.pathTextBox.setReadOnly(True)
+        self.horizontalLayout.addWidget(self.pathTextBox)
+        self.browseButton = QPushButton("Browse", self.centralWidget)
+        self.browseButton.clicked.connect(MainWin.on_actionBrowse_triggered)
+        self.horizontalLayout.addWidget(self.browseButton)
+        self.verticalLayout.addLayout(self.horizontalLayout)
+
+        # Splitter for Upload list/Log
+        self.splitter = QSplitter(Qt.Vertical)
+
+        # Table View (Upload list)
+        self.uploadList = TableWidget(self.centralWidget)
+        self.uploadList.setObjectName("uploadList")
+        self.uploadList.setStyleSheet(
+            """
+            QTableWidget {
+                    border: 2px solid grey;
+                    border-radius: 5px;
+            }
+            """)
+        self.uploadList.setEditTriggers(QAbstractItemView.NoEditTriggers)  # use NoEditTriggers to disable editing
+        self.uploadList.setAlternatingRowColors(True)
+        self.uploadList.setSelectionBehavior(QAbstractItemView.SelectRows)
+        self.uploadList.setSelectionMode(QAbstractItemView.NoSelection)
+        self.uploadList.verticalHeader().setDefaultSectionSize(18)  # tighten up the row size
+        self.uploadList.horizontalHeader().setStretchLastSection(True)
+        self.uploadList.setSortingEnabled(True)  # allow sorting
+        self.splitter.addWidget(self.uploadList)
+
+        # Log Widget
+        self.logTextBrowser = QPlainTextEditLogger(self.centralWidget)
+        self.logTextBrowser.widget.setObjectName("logTextBrowser")
+        self.logTextBrowser.widget.setStyleSheet(
+            """
+            QPlainTextEdit {
+                    border: 2px solid grey;
+                    border-radius: 5px;
+                    background-color: lightgray;
+            }
+            """)
+        self.splitter.addWidget(self.logTextBrowser.widget)
+
+        # add splitter
+        self.splitter.setSizes([400, 200])
+        self.verticalLayout.addWidget(self.splitter)
+
+    # Actions
+
+        # Browse
+        self.actionBrowse = QAction(MainWin)
+        self.actionBrowse.setObjectName("actionBrowse")
+        self.actionBrowse.setText(MainWin.tr("Browse"))
+        self.actionBrowse.setToolTip(MainWin.tr("Set the upload directory"))
+        self.actionBrowse.setShortcut(MainWin.tr("Ctrl+B"))
+
+        # Upload
+        self.actionUpload = QAction(MainWin)
+        self.actionUpload.setObjectName("actionUpload")
+        self.actionUpload.setText(MainWin.tr("Upload"))
+        self.actionUpload.setToolTip(MainWin.tr("Upload files"))
+        self.actionUpload.setShortcut(MainWin.tr("Ctrl+L"))
+        self.actionUpload.setEnabled(False)
+
+        # Rescan
+        self.actionRescan = QAction(MainWin)
+        self.actionRescan.setObjectName("actionRescan")
+        self.actionRescan.setText(MainWin.tr("Rescan"))
+        self.actionRescan.setToolTip(MainWin.tr("Rescan the upload directory"))
+        self.actionRescan.setShortcut(MainWin.tr("Ctrl+R"))
+        self.actionRescan.setEnabled(False)
+
+        # Cancel
+        self.actionCancel = QAction(MainWin)
+        self.actionCancel.setObjectName("actionCancel")
+        self.actionCancel.setText(MainWin.tr("Cancel"))
+        self.actionCancel.setToolTip(MainWin.tr("Cancel any upload(s) in-progress"))
+        self.actionCancel.setShortcut(MainWin.tr("Ctrl+C"))
+
+        # Options
+        self.actionOptions = QAction(MainWin)
+        self.actionOptions.setObjectName("actionOptions")
+        self.actionOptions.setText(MainWin.tr("Options"))
+        self.actionOptions.setToolTip(MainWin.tr("Configuration Options"))
+        self.actionOptions.setShortcut(MainWin.tr("Ctrl+P"))
+
+        # Login
+        self.actionLogin = QAction(MainWin)
+        self.actionLogin.setObjectName("actionLogin")
+        self.actionLogin.setText(MainWin.tr("Login"))
+        self.actionLogin.setToolTip(MainWin.tr("Login to the server"))
+        self.actionLogin.setShortcut(MainWin.tr("Ctrl+G"))
+        self.actionLogin.setEnabled(False)
+
+        # Logout
+        self.actionLogout = QAction(MainWin)
+        self.actionLogout.setObjectName("actionLogout")
+        self.actionLogout.setText(MainWin.tr("Logout"))
+        self.actionLogout.setToolTip(MainWin.tr("Logout of the server"))
+        self.actionLogout.setShortcut(MainWin.tr("Ctrl+O"))
+        self.actionLogout.setEnabled(False)
+
+        # Exit
+        self.actionExit = QAction(MainWin)
+        self.actionExit.setObjectName("actionExit")
+        self.actionExit.setText(MainWin.tr("Exit"))
+        self.actionExit.setToolTip(MainWin.tr("Exit the application"))
+        self.actionExit.setShortcut(MainWin.tr("Ctrl+Z"))
+
+        # Help
+        self.actionHelp = QAction(MainWin)
+        self.actionHelp.setObjectName("actionHelp")
+        self.actionHelp.setText(MainWin.tr("Help"))
+        self.actionHelp.setToolTip(MainWin.tr("Help"))
+        self.actionHelp.setShortcut(MainWin.tr("Ctrl+H"))
+
+    # Menu Bar
+
+        """
+        self.menuBar = QMenuBar(MainWin)
+        self.menuBar.setObjectName("menuBar")
+        MainWin.setMenuBar(self.menuBar)
+        self.menuBar.setStyleSheet(
+            "QMenuBar{font-family: Arial;font-style: normal;font-size: 10pt;font-weight: bold;};")
+        """
+
+    # Tool Bar
+
+        self.mainToolBar = QToolBar(MainWin)
+        self.mainToolBar.setObjectName("mainToolBar")
+        self.mainToolBar.setToolButtonStyle(Qt.ToolButtonTextUnderIcon)
+        self.mainToolBar.setContextMenuPolicy(Qt.PreventContextMenu)
+        MainWin.addToolBar(Qt.TopToolBarArea, self.mainToolBar)
+
+        # Upload
+        self.mainToolBar.addAction(self.actionUpload)
+        self.actionUpload.setIcon(qApp.style().standardIcon(QStyle.SP_FileDialogToParent))
+
+        # Rescan
+        self.mainToolBar.addAction(self.actionRescan)
+        self.actionRescan.setIcon(qApp.style().standardIcon(QStyle.SP_BrowserReload))
+
+        # Cancel
+        self.mainToolBar.addAction(self.actionCancel)
+        self.actionCancel.setIcon(qApp.style().standardIcon(QStyle.SP_BrowserStop))
+        self.actionCancel.setEnabled(False)
+
+        # Options
+        self.mainToolBar.addAction(self.actionOptions)
+        self.actionOptions.setIcon(qApp.style().standardIcon(QStyle.SP_FileDialogDetailedView))
+
+        # this spacer right justifies everything that comes after it
+        spacer = QWidget()
+        spacer.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
+        self.mainToolBar.addWidget(spacer)
+
+        # Login
+        self.mainToolBar.addAction(self.actionLogin)
+        self.actionLogin.setIcon(qApp.style().standardIcon(QStyle.SP_DialogApplyButton))
+
+        # Logout
+        self.mainToolBar.addAction(self.actionLogout)
+        self.actionLogout.setIcon(qApp.style().standardIcon(QStyle.SP_DialogOkButton))
+
+        # Help
+        #self.mainToolBar.addAction(self.actionHelp)
+        self.actionHelp.setIcon(qApp.style().standardIcon(QStyle.SP_MessageBoxQuestion))
+
+        # Exit
+        self.mainToolBar.addAction(self.actionExit)
+        self.actionExit.setIcon(qApp.style().standardIcon(QStyle.SP_DialogCancelButton))
+
+    # Status Bar
+
+        self.statusBar = QStatusBar(MainWin)
+        self.statusBar.setToolTip("")
+        self.statusBar.setStatusTip("")
+        self.statusBar.setObjectName("statusBar")
+        MainWin.setStatusBar(self.statusBar)
+
+    # configure logging
+        self.logTextBrowser.widget.log_update_signal.connect(MainWin.updateLog)
+        self.logTextBrowser.setFormatter(logging.Formatter("%(asctime)s - %(levelname)s - %(message)s"))
+        logging.getLogger().addHandler(self.logTextBrowser)
+
+    # finalize UI setup
+        QMetaObject.connectSlotsByName(MainWin)
```

### Comparing `deriva-qt-1.6.1/deriva_qt.egg-info/PKG-INFO` & `deriva-qt-1.6.3/deriva_qt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: deriva-qt
-Version: 1.6.1
+Version: 1.6.3
 Summary: Graphical User Interface tools for DERIVA built on PyQt5
 Home-page: https://github.com/informatics-isi-edu/deriva-qt
 Author: USC Information Sciences Institute, Informatics Systems Research Division
 Author-email: isrd-support@isi.edu
 Maintainer: USC Information Sciences Institute, Informatics Systems Research Division
 Maintainer-email: isrd-support@isi.edu
 License: GNU GPL 3.0
-Description: For further information, visit the project [homepage](https://github.com/informatics-isi-edu/deriva-qt).
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
@@ -21,7 +19,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: PyQt5
 Provides-Extra: PyQtWebEngine
+License-File: LICENSE
+
+For further information, visit the project [homepage](https://github.com/informatics-isi-edu/deriva-qt).
```

### Comparing `deriva-qt-1.6.1/deriva_qt.egg-info/SOURCES.txt` & `deriva-qt-1.6.3/deriva_qt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,18 +20,14 @@
 deriva/qt/auth_agent/ui/auth_window.py
 deriva/qt/auth_agent/ui/embedded_auth_window.py
 deriva/qt/common/__init__.py
 deriva/qt/common/async_task.py
 deriva/qt/common/json_editor.py
 deriva/qt/common/log_widget.py
 deriva/qt/common/table_widget.py
-deriva/qt/common/resources/__init__.py
-deriva/qt/common/resources/images/deriva-star.icns
-deriva/qt/common/resources/images/deriva-star.ico
-deriva/qt/common/resources/images/deriva-star.png
 deriva/qt/upload_gui/__init__.py
 deriva/qt/upload_gui/__main__.py
 deriva/qt/upload_gui/deriva-upload-mac.spec
 deriva/qt/upload_gui/deriva-upload-win.spec
 deriva/qt/upload_gui/deriva_upload_gui.py
 deriva/qt/upload_gui/conf/config.json
 deriva/qt/upload_gui/impl/__init__.py
```

### Comparing `deriva-qt-1.6.1/docs/images/deriva-auth-empty.png` & `deriva-qt-1.6.3/docs/images/deriva-auth-empty.png`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/docs/images/deriva-auth-globus.png` & `deriva-qt-1.6.3/docs/images/deriva-auth-globus.png`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/docs/images/pending.png` & `deriva-qt-1.6.3/docs/images/pending.png`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/docs/images/server-config.blank.png` & `deriva-qt-1.6.3/docs/images/server-config.blank.png`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/docs/images/server-config.gudmap.png` & `deriva-qt-1.6.3/docs/images/server-config.gudmap.png`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/docs/images/show-details.png` & `deriva-qt-1.6.3/docs/images/show-details.png`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/docs/images/update-config.png` & `deriva-qt-1.6.3/docs/images/update-config.png`

 * *Files identical despite different names*

### Comparing `deriva-qt-1.6.1/docs/uploading.md` & `deriva-qt-1.6.3/docs/uploading.md`

 * *Files 16% similar despite different names*

```diff
@@ -54,41 +54,54 @@
 On the remote server, install the latest version of deriva-py:
 ```
 pip3 install --upgrade git+https://github.com/informatics-isi-edu/deriva-py.git
 ```
 
 ### 2. Getting an authentication token
 
-The uploader requires an authentication token to communicate with the server. Running the DERIVA-Auth tool on your desktop (through the applications menu on Windows or Mac, or with `deriva-auth` on Linux) will bring up an authentication window similar to the one used in the data browser. The first time you log in, you'll see a mostly-empty window:
-![Initial DERIVA-Auth run](images/deriva-auth-empty.png)
+Upload requests are authorized using OAuth2; to obtain an OAuth token, run the `deriva-globus-auth-util` utility on the host from which you'll be uploading files:
 
-In the "Server:" area, type in the server provided by the DERIVA administrator. You should now see something that looks similar to the data browser login screen
-![Login window](https://github.com/informatics-isi-edu/gudmap-rbk/blob/master/wiki_images/submitting-data/sequencing_uploader/deriva-auth-globus.png)
+`deriva-globus-auth-utils login --host` _host_
 
-Note: in subsequent runs, DERIVA-Auth might take you directly to this window (skipping the blank screen at the beginning). It's always a good idea to look at the hostname before you log in.
+You can add the `--refresh` option if you want the token to last beyond the default timeout. This will generate a URL for a OAuth consent page and ask you to paste the resulting authorization code:
 
-After logging in, you'll see an "Authentication Successful" message. Click the "Show Token" button; this will bring up another dialog box to verify that you really want to view the token. Click on "Show Details" to display the token.
-!["Show Details" window](images/show-details.png)
+```
+Please paste the following URL in a browser:
+https://auth.globus.org/v2/oauth2/authorize?client_id=[long url redacted]
+Please Paste your Auth Code Below:
+```
+Paste the URL into a browser, follow the directions there, and then paste the authorization code back into the `deriva-globus-auth-utils` session. This will create and store your OAuth token.
+
+```
+Please paste the following URL in a browser:
+https://auth.globus.org/v2/oauth2/authorize?client_id=[long url redacted]
+Please Paste your Auth Code Below: 
+[code redacted]
+Login Successful
+```
+
+To end the session, you can allow the token to expire or run:
+
+`deriva-globus-auth-utils logout`
 
 ### 3. Uploading files
 
 On the server, run the command:
 
-`deriva-upload-cli` --catalog _n_ --token _token_ --catalog _n_ _host_ _/path/to/_/deriva
+`deriva-upload-cli` --catalog _n_ _host_ _/path/to/_/deriva
 
 where:
 
-* _n_ is the catalog number specified by your DERIVA administrator,
-* _token_ is the token cut-and-pasted from your DERIVA-Auth session, 
+* _n_ is the catalog number (if specified by your DERIVA administrator; otherwise this option can be omitted),
 * _host_ is the hostname provided by your DERIVA admin, and 
 * _/path/to/_/deriva is the path to the `deriva` directory you created above. 
 
 For example:
 ```
-deriva-upload-cli --catalog 2 --token xXXxxxxXXxxxxXxXXXxXxxxX www.gudmap.org $HOME/deriva
+deriva-upload-cli --catalog 2 www.atlas-d2k.org $HOME/deriva
 ```
 
 ### 4. Logging out
 
 Authentication tokens expire after 30 minutes of activity; you can log out explicitly by clicking on the "Logout" button at the top of the DERIVA-Auth window.
```

### Comparing `deriva-qt-1.6.1/setup.py` & `deriva-qt-1.6.3/setup.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-#
-# Copyright 2017 University of Southern California
-# Distributed under the GNU GPL 3.0 license. See LICENSE for more info.
-#
-
-""" Installation script for deriva.qt
-"""
-
-from setuptools import setup, find_packages
-import re
-import io
-
-__version__ = re.search(
-    r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
-    io.open('deriva/qt/__init__.py', encoding='utf_8_sig').read()
-    ).group(1)
-
-
-def get_readme_contents():
-    with io.open('README.md') as readme_file:
-        return readme_file.read()
-
-
-url = 'https://github.com/informatics-isi-edu/deriva-qt'
-author = 'USC Information Sciences Institute, Informatics Systems Research Division'
-author_email = 'isrd-support@isi.edu'
-
-
-setup(
-    name='deriva-qt',
-    description='Graphical User Interface tools for DERIVA built on PyQt5',
-    long_description="For further information, visit the project [homepage](%s)." % url,
-    long_description_content_type='text/markdown',
-    url=url,
-    author=author,
-    author_email=author_email,
-    maintainer=author,
-    maintainer_email=author_email,
-    version=__version__,
-    python_requires='>=3.6',
-    packages=find_packages(),
-    package_data={'deriva.qt': ['upload_gui/conf/config.json', '*/resources/images/*']},
-    entry_points={
-        'console_scripts': [
-            'deriva-auth = deriva.qt.auth_agent.__main__:main',
-            'deriva-upload = deriva.qt.upload_gui.__main__:main'
-        ]
-    },
-    install_requires=[
-        'deriva>=1.5.0'
-    ],
-    extras_require={
-        'PyQt5': ["PyQt5==5.11.3"],
-        'PyQtWebEngine': ["PyQtWebEngine>=5.15.4"]
-    },
-    license='GNU GPL 3.0',
-    classifiers=[
-        'Intended Audience :: Science/Research',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Operating System :: POSIX',
-        'Operating System :: MacOS :: MacOS X',
-        'Operating System :: Microsoft :: Windows',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
-    ]
-)
-
+#
+# Copyright 2017 University of Southern California
+# Distributed under the GNU GPL 3.0 license. See LICENSE for more info.
+#
+
+""" Installation script for deriva.qt
+"""
+
+from setuptools import setup, find_packages
+import re
+import io
+
+__version__ = re.search(
+    r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
+    io.open('deriva/qt/__init__.py', encoding='utf_8_sig').read()
+    ).group(1)
+
+
+def get_readme_contents():
+    with io.open('README.md') as readme_file:
+        return readme_file.read()
+
+
+url = 'https://github.com/informatics-isi-edu/deriva-qt'
+author = 'USC Information Sciences Institute, Informatics Systems Research Division'
+author_email = 'isrd-support@isi.edu'
+
+
+setup(
+    name='deriva-qt',
+    description='Graphical User Interface tools for DERIVA built on PyQt5',
+    long_description="For further information, visit the project [homepage](%s)." % url,
+    long_description_content_type='text/markdown',
+    url=url,
+    author=author,
+    author_email=author_email,
+    maintainer=author,
+    maintainer_email=author_email,
+    version=__version__,
+    python_requires='>=3.6',
+    packages=find_packages(),
+    package_data={'deriva.qt': ['upload_gui/conf/config.json', '*/resources/images/*']},
+    entry_points={
+        'console_scripts': [
+            'deriva-auth = deriva.qt.auth_agent.__main__:main',
+            'deriva-upload = deriva.qt.upload_gui.__main__:main'
+        ]
+    },
+    install_requires=[
+        'deriva>=1.5.0'
+    ],
+    extras_require={
+        'PyQt5': ["PyQt5==5.11.3"],
+        'PyQtWebEngine': ["PyQtWebEngine>=5.15.4"]
+    },
+    license='GNU GPL 3.0',
+    classifiers=[
+        'Intended Audience :: Science/Research',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+        'Operating System :: POSIX',
+        'Operating System :: MacOS :: MacOS X',
+        'Operating System :: Microsoft :: Windows',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9'
+    ]
+)
+
```

