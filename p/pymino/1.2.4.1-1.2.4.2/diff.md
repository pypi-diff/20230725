# Comparing `tmp/pymino-1.2.4.1.tar.gz` & `tmp/pymino-1.2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\sss\pymino-1.2.3.8\dist\.tmp-sru2qhdd\pymino-1.2.4.1.tar", last modified: Sat Jul 22 04:22:41 2023, max compression
+gzip compressed data, was "pymino-1.2.4.2.tar", last modified: Tue Jul 25 19:30:35 2023, max compression
```

## Comparing `pymino-1.2.4.1.tar` & `pymino-1.2.4.2.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 04:22:41.638357 pymino-1.2.4.1/
--rw-rw-rw-   0        0        0     1085 2023-07-14 23:58:40.000000 pymino-1.2.4.1/LICENSE
--rw-rw-rw-   0        0        0     7373 2023-07-22 04:22:41.638357 pymino-1.2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-07-20 02:36:23.000000 pymino-1.2.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 04:22:41.566436 pymino-1.2.4.1/pymino/
--rw-rw-rw-   0        0        0      952 2023-07-22 04:20:37.000000 pymino-1.2.4.1/pymino/__init__.py
--rw-rw-rw-   0        0        0    12297 2023-07-22 04:05:59.000000 pymino-1.2.4.1/pymino/async_bot.py
--rw-rw-rw-   0        0        0    38219 2023-07-22 04:02:40.000000 pymino-1.2.4.1/pymino/async_client.py
--rw-rw-rw-   0        0        0    32248 2023-07-22 03:46:10.000000 pymino-1.2.4.1/pymino/bot.py
--rw-rw-rw-   0        0        0    37736 2023-07-22 04:05:43.000000 pymino-1.2.4.1/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-07-22 04:22:41.597187 pymino-1.2.4.1/pymino/ext/
--rw-rw-rw-   0        0        0      638 2023-07-22 03:26:20.000000 pymino-1.2.4.1/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    11300 2023-07-22 04:04:33.000000 pymino-1.2.4.1/pymino/ext/account.py
--rw-rw-rw-   0        0        0    11529 2023-07-22 04:02:21.000000 pymino-1.2.4.1/pymino/ext/async_account.py
--rw-rw-rw-   0        0        0   345197 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    21402 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    25878 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0    72111 2023-07-20 02:29:35.000000 pymino-1.2.4.1/pymino/ext/async_global_client.py
--rw-rw-rw-   0        0        0     7203 2023-07-22 02:16:09.000000 pymino-1.2.4.1/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   344131 2023-07-22 03:45:27.000000 pymino-1.2.4.1/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/console.py
--rw-rw-rw-   0        0        0    45520 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/context.py
--rw-rw-rw-   0        0        0     2052 2023-07-21 19:38:46.000000 pymino-1.2.4.1/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-07-22 04:22:41.624963 pymino-1.2.4.1/pymino/ext/entities/
--rw-rw-rw-   0        0        0      428 2023-07-22 03:26:32.000000 pymino-1.2.4.1/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     9014 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/admin_log.py
--rw-rw-rw-   0        0        0     1670 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    16021 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43827 2023-07-20 01:14:10.000000 pymino-1.2.4.1/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     5516 2023-07-21 20:49:34.000000 pymino-1.2.4.1/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1839 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    32492 2023-07-22 04:20:07.000000 pymino-1.2.4.1/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0    74405 2023-07-20 01:25:38.000000 pymino-1.2.4.1/pymino/ext/global_client.py
--rw-rw-rw-   0        0        0      543 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6609 2023-07-21 21:24:55.000000 pymino-1.2.4.1/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-07-22 04:22:41.636868 pymino-1.2.4.1/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11719 2023-07-22 02:49:03.000000 pymino-1.2.4.1/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6280 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1514 2023-07-22 04:06:11.000000 pymino-1.2.4.1/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-07-14 23:58:40.000000 pymino-1.2.4.1/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10853 2023-07-22 03:21:49.000000 pymino-1.2.4.1/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-22 04:22:41.576356 pymino-1.2.4.1/pymino.egg-info/
--rw-rw-rw-   0        0        0     7373 2023-07-22 04:22:41.000000 pymino-1.2.4.1/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-07-22 04:22:41.000000 pymino-1.2.4.1/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 04:22:41.000000 pymino-1.2.4.1/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-07-22 04:22:41.000000 pymino-1.2.4.1/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-22 04:22:41.000000 pymino-1.2.4.1/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      833 2023-07-22 04:22:41.644307 pymino-1.2.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-07-22 02:34:26.000000 pymino-1.2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:35.486045 pymino-1.2.4.2/
+-rw-rw-rw-   0        0        0     1085 2023-07-14 23:58:40.000000 pymino-1.2.4.2/LICENSE
+-rw-rw-rw-   0        0        0     7373 2023-07-25 19:30:35.486045 pymino-1.2.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-07-25 19:30:17.000000 pymino-1.2.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:35.414048 pymino-1.2.4.2/pymino/
+-rw-rw-rw-   0        0        0      952 2023-07-25 19:16:15.000000 pymino-1.2.4.2/pymino/__init__.py
+-rw-rw-rw-   0        0        0    12297 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    38219 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/async_client.py
+-rw-rw-rw-   0        0        0    32248 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/bot.py
+-rw-rw-rw-   0        0        0    37736 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:35.439179 pymino-1.2.4.2/pymino/ext/
+-rw-rw-rw-   0        0        0      638 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    11300 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/account.py
+-rw-rw-rw-   0        0        0    11529 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/async_account.py
+-rw-rw-rw-   0        0        0   345197 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    21402 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    25878 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0    72111 2023-07-20 02:29:35.000000 pymino-1.2.4.2/pymino/ext/async_global_client.py
+-rw-rw-rw-   0        0        0     7203 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   344131 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    45520 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     2052 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:35.470455 pymino-1.2.4.2/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      428 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     9014 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/admin_log.py
+-rw-rw-rw-   0        0        0     1670 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    16021 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43827 2023-07-20 01:14:10.000000 pymino-1.2.4.2/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     5516 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1839 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    32492 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0    75199 2023-07-25 19:15:48.000000 pymino-1.2.4.2/pymino/ext/global_client.py
+-rw-rw-rw-   0        0        0      543 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6609 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:35.470455 pymino-1.2.4.2/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11719 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6280 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1514 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10853 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:35.423555 pymino-1.2.4.2/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7373 2023-07-25 19:30:35.000000 pymino-1.2.4.2/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1640 2023-07-25 19:30:35.000000 pymino-1.2.4.2/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 19:30:35.000000 pymino-1.2.4.2/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-07-25 19:30:35.000000 pymino-1.2.4.2/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 19:30:35.000000 pymino-1.2.4.2/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      833 2023-07-25 19:30:35.486045 pymino-1.2.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-07-25 18:46:41.000000 pymino-1.2.4.2/setup.py
```

### Comparing `pymino-1.2.4.1/LICENSE` & `pymino-1.2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/PKG-INFO` & `pymino-1.2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.4.1
+Version: 1.2.4.2
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.4.1 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.4.2 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `pymino-1.2.4.1/README.md` & `pymino-1.2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/__init__.py` & `pymino-1.2.4.2/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from requests import get
 from colorama import Fore, Style
 
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.4.1'
+__version__ = '1.2.4.2'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot
 from .async_bot import AsyncBot
 from .client import Client
 from .async_client import AsyncClient
```

### Comparing `pymino-1.2.4.1/pymino/async_bot.py` & `pymino-1.2.4.2/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/async_client.py` & `pymino-1.2.4.2/pymino/async_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/bot.py` & `pymino-1.2.4.2/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/client.py` & `pymino-1.2.4.2/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/__init__.py` & `pymino-1.2.4.2/pymino/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/account.py` & `pymino-1.2.4.2/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/async_account.py` & `pymino-1.2.4.2/pymino/ext/async_account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/async_community.py` & `pymino-1.2.4.2/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/async_context.py` & `pymino-1.2.4.2/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/async_event_handler.py` & `pymino-1.2.4.2/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/async_global_client.py` & `pymino-1.2.4.2/pymino/ext/async_global_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/async_socket.py` & `pymino-1.2.4.2/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/community.py` & `pymino-1.2.4.2/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/console.py` & `pymino-1.2.4.2/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/context.py` & `pymino-1.2.4.2/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/dispatcher.py` & `pymino-1.2.4.2/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/acm.py` & `pymino-1.2.4.2/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/admin_log.py` & `pymino-1.2.4.2/pymino/ext/entities/admin_log.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/api_response.py` & `pymino-1.2.4.2/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/bubble.py` & `pymino-1.2.4.2/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/chat_threads.py` & `pymino-1.2.4.2/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/comments.py` & `pymino-1.2.4.2/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/enums.py` & `pymino-1.2.4.2/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/exceptions.py` & `pymino-1.2.4.2/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/general.py` & `pymino-1.2.4.2/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/handlers.py` & `pymino-1.2.4.2/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/link_info.py` & `pymino-1.2.4.2/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/member.py` & `pymino-1.2.4.2/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/messages.py` & `pymino-1.2.4.2/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/notification.py` & `pymino-1.2.4.2/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/sticker.py` & `pymino-1.2.4.2/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/threads.py` & `pymino-1.2.4.2/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/userprofile.py` & `pymino-1.2.4.2/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/entities/wsevents.py` & `pymino-1.2.4.2/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/global_client.py` & `pymino-1.2.4.2/pymino/ext/global_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1922,8 +1922,30 @@
         >>> community_list = client.community.fetch_available_communities(start=0, size=10, language="en")
         >>> for name, comId in zip(community_list.name, community_list.comId):
         >>>     print(name, comId])
         """
         return CCommunityList(self.make_request(
             method = "GET",
             url = f"/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&start={start}&size={size}&pagingType=t"
+        ))
+    
+    def unfollow(self, userId: str) -> ApiResponse:
+        """
+        Unfollows a user.
+
+        :param userId: The ID of the user to unfollow.
+        :type userId: str
+        :return: An ApiResponse object containing the response data from the API.
+        :rtype: ApiResponse
+
+        This function allows the logged-in user to unfollow another user specified by their ID.
+        After successful execution, the user will no longer be following the specified user.
+
+        **Example usage:**
+
+        >>> response = client.unfollow(userId="user123")
+        >>> print(response.status_code)
+        """
+        return ApiResponse(self.make_request(
+            method = "DELETE",
+            url = f"/g/s/user-profile/{userId}/member/{self.userId}"
         ))
```

### Comparing `pymino-1.2.4.1/pymino/ext/handle_queue.py` & `pymino-1.2.4.2/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/socket.py` & `pymino-1.2.4.2/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.4.2/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/utilities/chat_console.py` & `pymino-1.2.4.2/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/utilities/commands.py` & `pymino-1.2.4.2/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/utilities/community_console.py` & `pymino-1.2.4.2/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/utilities/generate.py` & `pymino-1.2.4.2/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/utilities/menu.py` & `pymino-1.2.4.2/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/utilities/profile_console.py` & `pymino-1.2.4.2/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino/ext/utilities/request_handler.py` & `pymino-1.2.4.2/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.1/pymino.egg-info/PKG-INFO` & `pymino-1.2.4.2/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.4.1
+Version: 1.2.4.2
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.4.1 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.4.2 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `pymino-1.2.4.1/pymino.egg-info/SOURCES.txt` & `pymino-1.2.4.2/pymino.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pymino/client.py
 pymino.egg-info/PKG-INFO
 pymino.egg-info/SOURCES.txt
 pymino.egg-info/dependency_links.txt
 pymino.egg-info/requires.txt
 pymino.egg-info/top_level.txt
 pymino/ext/__init__.py
+pymino/ext/_global.py
 pymino/ext/account.py
 pymino/ext/async_account.py
 pymino/ext/async_community.py
 pymino/ext/async_context.py
 pymino/ext/async_event_handler.py
 pymino/ext/async_global_client.py
 pymino/ext/async_socket.py
```

### Comparing `pymino-1.2.4.1/setup.cfg` & `pymino-1.2.4.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e34 2e31 0d0a 6175  on = 1.2.4.1..au
+00000020: 6f6e 203d 2031 2e32 2e34 2e32 0d0a 6175  on = 1.2.4.2..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.4.1/setup.py` & `pymino-1.2.4.2/setup.py`

 * *Files identical despite different names*

