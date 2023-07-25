# Comparing `tmp/rcon-2.4.0.tar.gz` & `tmp/rcon-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcon-2.4.0.tar", last modified: Mon Jul 24 16:26:02 2023, max compression
+gzip compressed data, was "rcon-2.4.1.tar", last modified: Tue Jul 25 09:16:12 2023, max compression
```

## Comparing `rcon-2.4.0.tar` & `rcon-2.4.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.555612 rcon-2.4.0/
--rw-r--r--   0 rne       (1000) rne       (1000)     1806 2022-02-17 09:30:26.000000 rcon-2.4.0/.gitignore
--rw-r--r--   0 rne       (1000) rne       (1000)       35 2020-12-22 14:06:00.000000 rcon-2.4.0/.readthedocs.yml
--rw-r--r--   0 rne       (1000) rne       (1000)      720 2021-01-11 21:30:07.000000 rcon-2.4.0/Jenkinsfile
--rw-r--r--   0 rne       (1000) rne       (1000)    35147 2018-08-10 22:34:58.000000 rcon-2.4.0/LICENSE.txt
--rw-r--r--   0 rne       (1000) rne       (1000)      443 2022-02-17 09:30:26.000000 rcon-2.4.0/Makefile
--rw-r--r--   0 rne       (1000) rne       (1000)     2632 2023-07-24 16:26:02.555612 rcon-2.4.0/PKG-INFO
--rw-r--r--   0 rne       (1000) rne       (1000)     2293 2022-08-25 20:42:40.000000 rcon-2.4.0/README.md
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.548945 rcon-2.4.0/docs/
--rw-r--r--   0 rne       (1000) rne       (1000)      638 2020-12-04 16:56:37.000000 rcon-2.4.0/docs/Makefile
--rw-r--r--   0 rne       (1000) rne       (1000)      804 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/make.bat
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.552279 rcon-2.4.0/docs/source/
--rw-r--r--   0 rne       (1000) rne       (1000)      193 2020-12-19 22:39:46.000000 rcon-2.4.0/docs/source/bugs.rst
--rw-r--r--   0 rne       (1000) rne       (1000)      950 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/source/conf.py
--rw-r--r--   0 rne       (1000) rne       (1000)      457 2020-12-19 22:36:25.000000 rcon-2.4.0/docs/source/index.rst
--rw-r--r--   0 rne       (1000) rne       (1000)      321 2020-12-19 22:27:44.000000 rcon-2.4.0/docs/source/installation.rst
--rw-r--r--   0 rne       (1000) rne       (1000)    35493 2020-12-04 16:56:37.000000 rcon-2.4.0/docs/source/license.rst
--rw-r--r--   0 rne       (1000) rne       (1000)       49 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/source/modules.rst
--rw-r--r--   0 rne       (1000) rne       (1000)      480 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/source/rcon.battleye.rst
--rw-r--r--   0 rne       (1000) rne       (1000)     1386 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/source/rcon.rst
--rw-r--r--   0 rne       (1000) rne       (1000)      619 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/source/rcon.source.rst
--rw-r--r--   0 rne       (1000) rne       (1000)     2764 2023-05-17 01:25:27.000000 rcon-2.4.0/docs/source/usage.rst
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.552279 rcon-2.4.0/rcon/
--rw-r--r--   0 rne       (1000) rne       (1000)      986 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/__init__.py
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.552279 rcon-2.4.0/rcon/battleye/
--rw-r--r--   0 rne       (1000) rne       (1000)      163 2023-05-17 01:25:27.000000 rcon-2.4.0/rcon/battleye/__init__.py
--rw-r--r--   0 rne       (1000) rne       (1000)     3022 2023-07-24 16:18:40.000000 rcon-2.4.0/rcon/battleye/client.py
--rw-r--r--   0 rne       (1000) rne       (1000)     4821 2023-07-24 12:26:16.000000 rcon-2.4.0/rcon/battleye/proto.py
--rw-r--r--   0 rne       (1000) rne       (1000)     1884 2023-05-17 01:25:27.000000 rcon-2.4.0/rcon/client.py
--rw-r--r--   0 rne       (1000) rne       (1000)     2892 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/config.py
--rw-r--r--   0 rne       (1000) rne       (1000)     3447 2023-05-17 01:25:27.000000 rcon-2.4.0/rcon/console.py
--rw-r--r--   0 rne       (1000) rne       (1000)     1264 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/errorhandler.py
--rw-r--r--   0 rne       (1000) rne       (1000)      588 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/exceptions.py
--rw-r--r--   0 rne       (1000) rne       (1000)     7243 2023-05-17 01:25:27.000000 rcon-2.4.0/rcon/gui.py
--rw-r--r--   0 rne       (1000) rne       (1000)     1933 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/rconclt.py
--rw-r--r--   0 rne       (1000) rne       (1000)     1905 2023-05-17 01:25:27.000000 rcon-2.4.0/rcon/rconshell.py
--rw-r--r--   0 rne       (1000) rne       (1000)     1254 2023-05-17 01:25:27.000000 rcon-2.4.0/rcon/readline.py
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.552279 rcon-2.4.0/rcon/source/
--rw-r--r--   0 rne       (1000) rne       (1000)      144 2022-02-17 09:30:26.000000 rcon-2.4.0/rcon/source/__init__.py
--rw-r--r--   0 rne       (1000) rne       (1000)     2097 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/source/async_rcon.py
--rw-r--r--   0 rne       (1000) rne       (1000)     2389 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/source/client.py
--rw-r--r--   0 rne       (1000) rne       (1000)     6162 2022-08-25 20:42:40.000000 rcon-2.4.0/rcon/source/proto.py
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.552279 rcon-2.4.0/rcon.egg-info/
--rw-r--r--   0 rne       (1000) rne       (1000)     2632 2023-07-24 16:26:02.000000 rcon-2.4.0/rcon.egg-info/PKG-INFO
--rw-r--r--   0 rne       (1000) rne       (1000)      962 2023-07-24 16:26:02.000000 rcon-2.4.0/rcon.egg-info/SOURCES.txt
--rw-r--r--   0 rne       (1000) rne       (1000)        1 2023-07-24 16:26:02.000000 rcon-2.4.0/rcon.egg-info/dependency_links.txt
--rw-r--r--   0 rne       (1000) rne       (1000)      102 2023-07-24 16:26:02.000000 rcon-2.4.0/rcon.egg-info/entry_points.txt
--rw-r--r--   0 rne       (1000) rne       (1000)       23 2023-07-24 16:26:02.000000 rcon-2.4.0/rcon.egg-info/requires.txt
--rw-r--r--   0 rne       (1000) rne       (1000)        5 2023-07-24 16:26:02.000000 rcon-2.4.0/rcon.egg-info/top_level.txt
--rw-r--r--   0 rne       (1000) rne       (1000)        0 2021-01-07 21:40:17.000000 rcon-2.4.0/requirements.txt
--rw-r--r--   0 rne       (1000) rne       (1000)       38 2023-07-24 16:26:02.555612 rcon-2.4.0/setup.cfg
--rwxr-xr-x   0 rne       (1000) rne       (1000)      846 2022-08-25 20:42:40.000000 rcon-2.4.0/setup.py
-drwxr-xr-x   0 rne       (1000) rne       (1000)        0 2023-07-24 16:26:02.555612 rcon-2.4.0/tests/
--rw-r--r--   0 rne       (1000) rne       (1000)       18 2022-02-17 09:30:26.000000 rcon-2.4.0/tests/__init__.py
--rw-r--r--   0 rne       (1000) rne       (1000)      500 2022-02-17 09:30:26.000000 rcon-2.4.0/tests/test_battleye_proto.py
--rw-r--r--   0 rne       (1000) rne       (1000)     1789 2022-02-17 09:30:26.000000 rcon-2.4.0/tests/test_config.py
--rw-r--r--   0 rne       (1000) rne       (1000)     5638 2022-02-17 09:30:26.000000 rcon-2.4.0/tests/test_source_proto.py
+drwxr-xr-x   0 neumann   (1000) neumann   (1000)        0 2023-07-25 09:16:12.387290 rcon-2.4.1/
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     1806 2022-02-10 10:07:53.000000 rcon-2.4.1/.gitignore
+-rw-r--r--   0 neumann   (1000) neumann   (1000)       35 2022-02-10 09:17:26.000000 rcon-2.4.1/.readthedocs.yml
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      720 2022-02-10 09:17:26.000000 rcon-2.4.1/Jenkinsfile
+-rw-r--r--   0 neumann   (1000) neumann   (1000)    35147 2022-02-10 09:17:26.000000 rcon-2.4.1/LICENSE.txt
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      443 2022-02-10 10:07:30.000000 rcon-2.4.1/Makefile
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     2632 2023-07-25 09:16:12.387290 rcon-2.4.1/PKG-INFO
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     2293 2022-08-31 14:27:09.000000 rcon-2.4.1/README.md
+drwxr-xr-x   0 neumann   (1000) neumann   (1000)        0 2023-07-25 09:16:12.383957 rcon-2.4.1/docs/
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      638 2022-02-10 09:17:26.000000 rcon-2.4.1/docs/Makefile
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      804 2022-11-08 12:43:01.000000 rcon-2.4.1/docs/make.bat
+drwxr-xr-x   0 neumann   (1000) neumann   (1000)        0 2023-07-25 09:16:12.383957 rcon-2.4.1/docs/source/
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      193 2022-02-10 09:17:26.000000 rcon-2.4.1/docs/source/bugs.rst
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      950 2022-11-08 13:03:29.000000 rcon-2.4.1/docs/source/conf.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      457 2022-11-08 12:44:54.000000 rcon-2.4.1/docs/source/index.rst
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      321 2022-02-10 09:17:26.000000 rcon-2.4.1/docs/source/installation.rst
+-rw-r--r--   0 neumann   (1000) neumann   (1000)    35493 2022-02-10 09:17:26.000000 rcon-2.4.1/docs/source/license.rst
+-rw-r--r--   0 neumann   (1000) neumann   (1000)       49 2022-11-08 12:45:48.000000 rcon-2.4.1/docs/source/modules.rst
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      480 2022-11-08 12:45:48.000000 rcon-2.4.1/docs/source/rcon.battleye.rst
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     1386 2022-11-08 12:45:48.000000 rcon-2.4.1/docs/source/rcon.rst
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      619 2022-11-08 12:45:48.000000 rcon-2.4.1/docs/source/rcon.source.rst
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     2764 2022-11-08 13:03:23.000000 rcon-2.4.1/docs/source/usage.rst
+drwxr-xr-x   0 neumann   (1000) neumann   (1000)        0 2023-07-25 09:16:12.383957 rcon-2.4.1/rcon/
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      986 2022-08-31 14:27:09.000000 rcon-2.4.1/rcon/__init__.py
+drwxr-xr-x   0 neumann   (1000) neumann   (1000)        0 2023-07-25 09:16:12.383957 rcon-2.4.1/rcon/battleye/
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      163 2022-11-08 13:03:04.000000 rcon-2.4.1/rcon/battleye/__init__.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     3278 2023-07-25 09:13:24.000000 rcon-2.4.1/rcon/battleye/client.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     4821 2023-07-25 09:07:19.000000 rcon-2.4.1/rcon/battleye/proto.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     1884 2022-11-08 12:37:23.000000 rcon-2.4.1/rcon/client.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     2892 2022-08-10 12:23:07.000000 rcon-2.4.1/rcon/config.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     3447 2023-07-10 12:17:52.000000 rcon-2.4.1/rcon/console.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     1264 2022-08-10 12:25:04.000000 rcon-2.4.1/rcon/errorhandler.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      588 2022-08-31 14:27:09.000000 rcon-2.4.1/rcon/exceptions.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     7243 2023-07-10 12:17:52.000000 rcon-2.4.1/rcon/gui.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     1933 2022-08-10 12:26:15.000000 rcon-2.4.1/rcon/rconclt.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     1905 2023-07-10 12:17:52.000000 rcon-2.4.1/rcon/rconshell.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     1254 2023-07-10 12:17:52.000000 rcon-2.4.1/rcon/readline.py
+drwxr-xr-x   0 neumann   (1000) neumann   (1000)        0 2023-07-25 09:16:12.387290 rcon-2.4.1/rcon/source/
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      144 2022-02-13 16:37:46.000000 rcon-2.4.1/rcon/source/__init__.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     2097 2022-08-31 14:27:09.000000 rcon-2.4.1/rcon/source/async_rcon.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     2389 2022-08-31 14:27:09.000000 rcon-2.4.1/rcon/source/client.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     6162 2022-08-31 14:27:09.000000 rcon-2.4.1/rcon/source/proto.py
+drwxr-xr-x   0 neumann   (1000) neumann   (1000)        0 2023-07-25 09:16:12.383957 rcon-2.4.1/rcon.egg-info/
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     2632 2023-07-25 09:16:12.000000 rcon-2.4.1/rcon.egg-info/PKG-INFO
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      962 2023-07-25 09:16:12.000000 rcon-2.4.1/rcon.egg-info/SOURCES.txt
+-rw-r--r--   0 neumann   (1000) neumann   (1000)        1 2023-07-25 09:16:12.000000 rcon-2.4.1/rcon.egg-info/dependency_links.txt
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      102 2023-07-25 09:16:12.000000 rcon-2.4.1/rcon.egg-info/entry_points.txt
+-rw-r--r--   0 neumann   (1000) neumann   (1000)       23 2023-07-25 09:16:12.000000 rcon-2.4.1/rcon.egg-info/requires.txt
+-rw-r--r--   0 neumann   (1000) neumann   (1000)        5 2023-07-25 09:16:12.000000 rcon-2.4.1/rcon.egg-info/top_level.txt
+-rw-r--r--   0 neumann   (1000) neumann   (1000)        0 2022-02-10 09:17:26.000000 rcon-2.4.1/requirements.txt
+-rw-r--r--   0 neumann   (1000) neumann   (1000)       38 2023-07-25 09:16:12.387290 rcon-2.4.1/setup.cfg
+-rwxr-xr-x   0 neumann   (1000) neumann   (1000)      846 2022-02-19 17:04:51.000000 rcon-2.4.1/setup.py
+drwxr-xr-x   0 neumann   (1000) neumann   (1000)        0 2023-07-25 09:16:12.387290 rcon-2.4.1/tests/
+-rw-r--r--   0 neumann   (1000) neumann   (1000)       18 2022-02-14 10:45:31.000000 rcon-2.4.1/tests/__init__.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)      500 2022-02-14 10:48:26.000000 rcon-2.4.1/tests/test_battleye_proto.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     1789 2022-02-14 08:57:03.000000 rcon-2.4.1/tests/test_config.py
+-rw-r--r--   0 neumann   (1000) neumann   (1000)     5638 2022-02-14 08:55:05.000000 rcon-2.4.1/tests/test_source_proto.py
```

### Comparing `rcon-2.4.0/.gitignore` & `rcon-2.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/Jenkinsfile` & `rcon-2.4.1/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/LICENSE.txt` & `rcon-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/PKG-INFO` & `rcon-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcon
-Version: 2.4.0
+Version: 2.4.1
 Summary: An RCON client library.
 Home-page: https://github.com/conqp/rcon
 Author: Richard Neumann
 Author-email: mail@richard-neumann.de
 License: GPLv3
 Keywords: python rcon client
 Requires-Python: >=3.10
```

### Comparing `rcon-2.4.0/README.md` & `rcon-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/docs/Makefile` & `rcon-2.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/docs/make.bat` & `rcon-2.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/docs/source/conf.py` & `rcon-2.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/docs/source/license.rst` & `rcon-2.4.1/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/docs/source/rcon.rst` & `rcon-2.4.1/docs/source/rcon.rst`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/docs/source/rcon.source.rst` & `rcon-2.4.1/docs/source/rcon.source.rst`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/docs/source/usage.rst` & `rcon-2.4.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/__init__.py` & `rcon-2.4.1/rcon/__init__.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/battleye/client.py` & `rcon-2.4.1/rcon/battleye/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from collections import defaultdict
 from logging import getLogger
 from socket import SOCK_DGRAM
 from typing import Callable
 
 from rcon.battleye.proto import RESPONSE_TYPES
 from rcon.battleye.proto import CommandRequest
+from rcon.battleye.proto import CommandResponse
 from rcon.battleye.proto import Header
 from rcon.battleye.proto import LoginRequest
 from rcon.battleye.proto import Request
 from rcon.battleye.proto import Response
 from rcon.battleye.proto import ServerMessage
 from rcon.battleye.proto import ServerMessageAck
 from rcon.client import BaseClient
@@ -31,15 +32,15 @@
 
 class Client(BaseClient, socket_type=SOCK_DGRAM):
     """BattlEye RCon client."""
 
     def __init__(
             self,
             *args,
-            max_length: int = 4096,
+            max_length: int = 6096,
             message_handler: MessageHandler = log_message,
             **kwargs
     ):
         super().__init__(*args, **kwargs)
         self.max_length = max_length
         self.message_handler = message_handler
 
@@ -57,39 +58,42 @@
                 (data := self._socket.recv(self.max_length))[:8]
             )).type
         ].from_bytes(header, data[8:])
 
     def communicate(self, request: Request) -> Response | str:
         """Send a request and receive a response."""
         acknowledged = defaultdict(set)
-        messages = []
+        command_responses = []
 
-        while True:
-            with self._socket.makefile('wb') as file:
-                file.write(bytes(request))
+        with self._socket.makefile('wb') as file:
+            file.write(bytes(request))
 
+        while True:
             response = self.receive()
 
             try:
                 seq = response.seq
             except AttributeError:
                 return response
 
-            if seq in acknowledged[msg_type := type(response)]:
-                break
+            if isinstance(response, CommandResponse):
+                # Collect fragmented command responses with the same seq
+                command_responses.append(response)
             else:
-                acknowledged[msg_type].add(seq)
+                if seq in acknowledged[response_type := type(response)]:
+                    break
+                else:
+                    acknowledged[response_type].add(seq)
 
             if isinstance(response, ServerMessage):
                 self.handle_server_message(response)
-            else:
-                messages.append(response)
 
         return ''.join(
-            msg.message for msg in sorted(messages, key=lambda msg: msg.seq)
+            command_response.message for command_response in
+            sorted(command_responses, key=lambda cr: cr.seq)
         )
 
     def login(self, passwd: str) -> bool:
         """Log-in the user."""
         if not self.communicate(LoginRequest(passwd)).success:
             raise WrongPassword()
```

### Comparing `rcon-2.4.0/rcon/battleye/proto.py` & `rcon-2.4.1/rcon/battleye/proto.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/client.py` & `rcon-2.4.1/rcon/client.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/config.py` & `rcon-2.4.1/rcon/config.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/console.py` & `rcon-2.4.1/rcon/console.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/errorhandler.py` & `rcon-2.4.1/rcon/errorhandler.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/exceptions.py` & `rcon-2.4.1/rcon/exceptions.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/gui.py` & `rcon-2.4.1/rcon/gui.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/rconclt.py` & `rcon-2.4.1/rcon/rconclt.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/rconshell.py` & `rcon-2.4.1/rcon/rconshell.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/readline.py` & `rcon-2.4.1/rcon/readline.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/source/async_rcon.py` & `rcon-2.4.1/rcon/source/async_rcon.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/source/client.py` & `rcon-2.4.1/rcon/source/client.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon/source/proto.py` & `rcon-2.4.1/rcon/source/proto.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/rcon.egg-info/PKG-INFO` & `rcon-2.4.1/rcon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcon
-Version: 2.4.0
+Version: 2.4.1
 Summary: An RCON client library.
 Home-page: https://github.com/conqp/rcon
 Author: Richard Neumann
 Author-email: mail@richard-neumann.de
 License: GPLv3
 Keywords: python rcon client
 Requires-Python: >=3.10
```

### Comparing `rcon-2.4.0/rcon.egg-info/SOURCES.txt` & `rcon-2.4.1/rcon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/setup.py` & `rcon-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/tests/test_config.py` & `rcon-2.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rcon-2.4.0/tests/test_source_proto.py` & `rcon-2.4.1/tests/test_source_proto.py`

 * *Files identical despite different names*

